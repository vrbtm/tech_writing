
# Копирование образа диска при помощи утилиты dd

**Для кого:** опытные пользователи компьютера, умеющие работать с командной строкой Linux, физически подключать и отключать жёсткий диск компьютера.

**Оборудование:**

 - настольный компьютер или ноутбук;
 - исходный жёсткий диск — диск, с которого будет скопированы данные. Копирование данных с диска также называется **снятием образа**;
 - целевой жёсткий диск — диск, на который будет скопированы данные;
 - загрузочный USB-накопитель [Live USB](https://ru.wikipedia.org/wiki/Live_CD) с любым дистрибутивом Linux.
 
<table>
<tbody>
<tr>
<td>:information_source: Например, при составлении этой инструкции использовался LiveUSB с <a href="https://linuxmint.com/edition.php?id=258">Linux Mint 19.1 XFCE</a>.
</td>
</tr>
</tbody>
</table>

## 1. Узнайте параметры исходного диска
1.1. Убедитесь, что из жёстких дисков и других накопителей к компьютеру физически подключён только исходный диск.  
1.2. Включите компьютер.  
1.3. Запустите `lsblk` — утилиту для отображения блочных устройств. 
```
$ lsblk -o name,size,vendor,model
    NAME     SIZE    VENDOR       MODEL     
    sda      500G    Samsung      HD502IJ 
    └─sda1  
```
**Пояснение**  
`-o` — краткая запись ключа `--output`. После этого ключа перечисляются выводимые параметры.

| Параметр	| Пояснение 		|
|--------	|------------	|
| `name`	| Имя в системе  	|
| `size`  	| Ёмкость в Гбайт  	|
| `vendor` 	| Производитель  	|
| `model` 	| Модель			|

1.4. Чтобы не перепутать исходный диск с целевым, составьте таблицу, как показано ниже, и запишите в неё информацию об исходном диске. В следующем разделе объясняется, как узнать информацию о целевом диске.

| Назначение 	| Имя в системе | Производитель | Модель     | Ёмкость  |
|------------	|---------------|---------------|------------|----------|
| Исходный   	| sda           | Samsung       | HD502IJ    | 500 Гбайт|

1.5. Выключите компьютер.  
1.6. Подпишите диск, который записали в таблицу, как исходный — например, простым карандашом на этикетке.

## 2. Узнайте параметры целевого диска
2.1. Подключите к компьютеру целевой диск — тот, на который будут скопированы данные. Он должен быть такой же ёмкости, как исходный, или больше. 

2.2. Включите компьютер.  
<!-- Добавить в таблицы отступ слева -->

<!--table>
<tbody>
<tr>
<td>:information_source: <i>Если целевой диск больше исходного, то после копирования образа нужно:</i>
<br> - <i>либо добавить на неразмеченное пространство целевого диска дополнительный раздел,</i>
<br> - <i>либо увеличить последний раздел скопированного образа до конца диска.</i>
<br>
<br><i>Если этого не сделать, то после копирования образа на целевом диске, который больше исходного, будет доступен для хранения тот же объём пространства, что и на исходном.,</i>
<br><i>Пример: исходный диск — 500 Гбайт, целевой диск — 2 Тбайта.,</i>
<br><i>После копирования образа на целевом диске будет доступно 500 Гбайт, пока вы не добавите новые разделы или не увеличите последний раздел.,</i>
</td>
</tr>
</tbody>
</table>
<p></p-->
<table>
<tbody>
<tr>
<td>:information_source: <b>Примечание</b>
<br>
<br>Если целевой диск больше исходного, то после копирования образа нужно:
<br> - либо добавить на неразмеченное пространство целевого диска дополнительный раздел,
<br> - либо увеличить последний раздел скопированного образа до конца диска.
<br>
<br>Если этого не сделать, то после копирования образа на целевом диске, который больше исходного, будет доступен для хранения тот же объём пространства, что и на исходном.
<br>Пример: исходный диск — 500 Гбайт, целевой диск — 2 Тбайта.
<br>После копирования образа на целевом диске будет доступно 500 Гбайт, пока вы не добавите новые разделы или не увеличите последний раздел.
</td>
</tr>
</tbody>
</table>

2.3. Запустите утилиту `lsblk`.  
```
$ lsblk -o name,size,vendor,model
```

Теперь в выводе утилиты отображаются два диска: исходный и целевой — например, WDC WD5000AZRZ (500 Гбайт). 

```
$ lsblk -o name,size,vendor,model
	NAME 	SIZE   VENDOR   	MODEL	 
	sda  	500G   Samsung  	HD502IJ
	├─sda1                                   	 
	sdb  	500G   WDC      	WD5000AZRZ
	└─sdb1 
```

2.4. Запишите эти данные в таблицу. 

| Назначение 	|Системное имя | Производитель | Модель     | Ёмкость   |
|------------	|--------------|---------------|------------|-----------|
| Исходный   	|sda           | Samsung       | HD502IJ    | 500 Гбайт |
| Целевой    	|sdb           | WDC           | WD5000AZRZ | 500 Гбайт |

2.5. Выключите компьютер.


## 3. Загрузите компьютер с USB-накопителя
3.1. Подключите загрузочный USB-накопитель с Linux.  
3.2. Включите компьютер.  
3.3. Перейдите в меню BIOS и выберите вариант загрузки с USB-накопителя.  
3.4. После загрузки операционной системы запустите утилиту `lsblk`, добавив параметр `mountpoint` — «точка монтирования». Он показывает, какие диски примонтированы к системе. 
```
$ lsblk -o name,size,mountpoint,vendor,model
```

Убедитесь, что оба жёстких диска — исходный и целевой — отмонтированы: значение `MOUNTPOINT` у этих дисков — в этом случае Samsung и WDC — должно быть пустым. 

```
$ lsblk -o name,size,mountpoint,vendor,model
    NAME     SIZE   MOUNTPOINT   VENDOR       MODEL     
    sda      500G                Samsung      HD502IJ 
    ├─sda1                                        
    sdb      500G                WDC          WD5000AZRZ
    └─sdb1                                        
    sdc      30G                 SanDisk      Cruzer Blade
    ├─sdc1          /boot/efi                              
    └─sdc2          /mnt/usbstick                        
```

## 4. Скопируйте образ диска
4.1. Утилита `dd` побайтово копирует полный образ исходного диска на целевой диск. Образ замещает все данные на целевом диске. Поэтому убедитесь, что `sda` — исходный диск, а на `sdb` нет данных или нужные данные скопированы на резервный носитель.  

`$ sudo dd if=/dev/sda of=/dev/sdb bs=1M status=progress conv=sync,noerror`

**Пояснения к параметрам копирования**  
| Ключ            	| Пояснение                                                                                                                                                                                                                   	|
|-----------------	|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| `if`             	| Файл исходного диска                                                                                                                                                                                                        	|
| `of`             	| Файл целевого диска                                                                                                                                                                                                         	|
| `bs`             	| Размер одного копируемого блока. Чем больше это значение, тем меньше времени займёт копирование.                                                                                             	|
| `status=progress`	| Будет отображаться ход записи.                                                                                                                                                                                              	|
| `conv`           	| Дополнительные параметры копирования:  
|                 	| - значение `sync` записывает вместо проблемных блоков нули, чтобы на целевом диске не возникло смещений; 
|                 	| - значение `noerror` препятствует остановке копирования при обнаружении на диске ошибок. |

Во время выполнения задачи будет отображаться ход копирования:  
```
6089080832 bytes (6.1 GB) copied, 59.287173 s, 102 MB/s
```
Когда копирование завершится, отобразятся сведения об объёме скопированных данных, времени и средней скорости копирования:  
```
122096646+0 records in
122096646+0 records out
50010782016 bytes (500GB) copied, 10975.5 s, 45.6 MB/s
```
4.2. Выключите компьютер. 

## 5. Проверьте, как загружается целевой диск
5.1. Отключите USB-накопитель.  
5.2. Если модель и ёмкость у исходного и целевого дисков одинаковые, перед включением физически отключите исходный жёсткий диск.  
5.3. Включите компьютер. Операционная система должна загрузиться точно так же, как на исходном диске.

