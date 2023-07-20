
# Облачное хранилище NextCloud. Работа с файлами

Руководство предназначено для пользователей NextCloud — облачного хранилища на основе открытого ПО.  
В нём объясняется, как работать с облачным хранилищем — в том числе загружать в него файлы и папки, удалять их и восстанавливать, предоставлять доступ к объектам в хранилище другим пользователям.

## Оглавление
[1. Вход в облачное хранилище](#1-%D0%B2%D1%85%D0%BE%D0%B4-%D0%B2-%D0%BE%D0%B1%D0%BB%D0%B0%D1%87%D0%BD%D0%BE%D0%B5-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B5)  
[2. Загрузка файла или папки в хранилище](#2-%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0-%D1%84%D0%B0%D0%B9%D0%BB%D0%B0-%D0%B8%D0%BB%D0%B8-%D0%BF%D0%B0%D0%BF%D0%BA%D0%B8-%D0%B2-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B5)  
[3. Удаление файла или папки](#3-%D1%83%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%B0-%D0%B8%D0%BB%D0%B8-%D0%BF%D0%B0%D0%BF%D0%BA%D0%B8)  
[4. Восстановление файла или папки](#4-%D0%B2%D0%BE%D1%81%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%B0-%D0%B8%D0%BB%D0%B8-%D0%BF%D0%B0%D0%BF%D0%BA%D0%B8)  
[5. Скачивание файла или папки](#5-%D1%81%D0%BA%D0%B0%D1%87%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%B0-%D0%B8%D0%BB%D0%B8-%D0%BF%D0%B0%D0%BF%D0%BA%D0%B8)  
[6. Предоставление общего доступа к файлу или папке](#6-%D0%BF%D1%80%D0%B5%D0%B4%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%BE%D0%B1%D1%89%D0%B5%D0%B3%D0%BE-%D0%B4%D0%BE%D1%81%D1%82%D1%83%D0%BF%D0%B0-%D0%BA-%D1%84%D0%B0%D0%B9%D0%BB%D1%83-%D0%B8%D0%BB%D0%B8-%D0%BF%D0%B0%D0%BF%D0%BA%D0%B5)

## 1. Вход в облачное хранилище
1.1. Откройте в браузере страницу [https://example.cloud.ru](www.example.com).  
Откроется страница ввода логина и пароля.

<div align="left">
<img src="https://github.com/vrbtm/tech_writing/blob/b06711c36e53a3b06018422f2ed0d4fd9433bf2f/img/nextcloud_1.jpg"></div>
<div align="left"><i>Страница ввода логина и пароля</i></div>
&nbsp;
&nbsp;

1.2. В верхнем поле введите свой адрес электронной почты (например, ivanov.gi@[почтовый домен]).  
В нижнем поле введите свой пароль от электронной почты.  
Нажмите на кнопку **Войти**.  
Отобразится страница со списком ваших папок и файлов.

1.3. Внешний вид хранилища
На следующем рисунке обведены и пронумерованы рабочие области.

<div align="left">
<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_2.png"></div>
<div align="left"><i>Внешний вид хранилища</i></div>
&nbsp;
&nbsp;

В области (1) находится меню со ссылками на файлы, отсортированными по типу:

 - недавно изменённые файлы;
 - файлы и папки, помеченные вами как избранные;
 - опубликованные файлы или папки — те, которыми вы поделились с другими, либо которыми поделились с вами;
 - метки (ключевые слова, которыми можно помечать файлы для упрощения их поиска).  

<p>В области (2) находятся кнопки <b>Домой</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_home_button.png"> (домашняя папка со списком файлов) и <b>Добавить</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_add_button.png">.</p>
В области (3) отображаются последние изменённые файлы.  
В области (4) — список объектов в домашней папке.  
В области (5) находятся:

 - cсылка на **Корзину**;
 - объём доступного пространства для хранения файлов;
 - ссылка на меню настроек.  

## 2. Загрузка файла или папки в хранилище
<p>2.1. Нажмите кнопку <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_add_button.png"> над списком ваших файлов.  
Отобразится меню добавления файла или папки.</p>

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_4.jpg"></div>
<div align="left"><i>Кнопка <b>Добавить</b></i> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_add_button.png"></div>
&nbsp;
&nbsp;

2.2. Выберите пункт **Загрузить файл**:

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_5.jpg"></div>
<div align="left"><i>Пункт <b>Загрузить файл</b></i></div>
&nbsp;
&nbsp;

Отобразится окно выбора файла для загрузки.  
Выберите файл, который требуется загрузить в хранилище:

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_7.png"></div>
<div align="left"><i>Окно выбора файла для загрузки</i></div>
&nbsp;
&nbsp;

2.3. Нажмите кнопку **Открыть**:

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_9.png"></div>
<div align="left"><i>Выбор файла для загрузки</i></div>
&nbsp;
&nbsp;

2.4. Теперь в списке отображается загруженный файл:
<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_8.jpg"></div>
<div align="left"><i>Файл загружен</i></div>
&nbsp;
&nbsp;

Папки загружаются так же, как файлы, но на шаге 2.2 вместо файла выберите нужную папку.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_10.png"></div>
<div align="left"><i>Папка загружена</i></div>
&nbsp;
&nbsp;
 

## 3. Удаление файла или папки
3.1. Щёлкните мышью на файле или папке, которые требуется удалить. При этом слева от названия файла или папки появится галочка.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_12.png"></div>
<div align="left"><i>Файл выделен</i></div>
&nbsp;
&nbsp;

<p>3.2. Нажмите на кнопку <b>Меню</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_prop_button.png"> в конце строки с названием удаляемого файла.
<br>Отобразится меню действий с файлом.</p>

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_13.png"></div>
<div align="left"><i>Переход к меню действий с файлом</i></div>
&nbsp;
&nbsp;

3.3. Выберите пункт **Удалить**.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_14.png"></div>
<div align="left"><i>Удаление файла</i></div>
&nbsp;
&nbsp;

Теперь файл не отображается в списке.


## 4. Восстановление файла или папки
4.1. Чтобы восстановить удалённый файл (отменить удаление), перейдите в папку **Корзина**.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_15.png"></div>
<div align="left"><i>Переход в папку <b>Корзина</b></i></div>
&nbsp;
&nbsp;

4.2. Выделите нужный файл и нажмите кнопку **Восстановить**.
 
<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_16.png"></div>
<div align="left"><i>Восстановление файла</i></div>
&nbsp;
&nbsp;

Теперь файл снова отображается в списке.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_8.jpg"></div>
<div align="left"><i>Файл восстановлен</i></div>
&nbsp;
&nbsp;


## 5. Скачивание файла или папки
5.1. Выделите нужный файл в списке.  

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_12.png"></div>
<div align="left"><i>Файл выделен</i></div>
&nbsp;
&nbsp;

<p>5.2. Нажмите на кнопку <b>Меню</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_prop_button.png"> в конце строки с названием удаляемого файла.
<br>Отобразится меню действий с файлом.</p>

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_13.png"></div>
<div align="left"><i>Переход к меню действий с файлом</i></div>
&nbsp;
&nbsp;

5.3. Выберите пункт **Скачать**.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_18.png"></div>
<div align="left"><i>Загрузка файла</i></div>
&nbsp;
&nbsp;

Требуемый файл или папка будут загружены на ваш компьютер.


## 6. Предоставление общего доступа к файлу или папке

6.1. Выделите нужный файл в списке.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_12.png"></div>
<div align="left"><i>Файл выделен</i></div>
&nbsp;
&nbsp;
 
<p>6.2. Нажмите на кнопку <b>Поделиться</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_share_button.png">, отмеченную на рисунке.
<br>Отобразится меню выбора получателя.</p>

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_17.png"></div>
<div align="left"><i>Переход к меню выбора получателя</i></div>
&nbsp;
&nbsp;
<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_19.png"></div>
<div align="left"><i>Меню выбора получателя</i></div>
&nbsp;
&nbsp;

6.3. Укажите в поле **Имя или адрес e-mail** служебный адрес электронной почты пользователя, которому хотели бы предоставить доступ к файлу.
Во всплывающем меню отобразится адрес пользователя.

6.4. Щёлкните левой клавишей мыши по этому адресу.
<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_20.jpg"></div>
<div align="left"><i>Получатель файла добавлен</i></div>
&nbsp;
&nbsp;

Теперь этот адрес отображается ниже поля ввода.

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_21.jpg"></div>
<div align="left"><i>Получатель файла выбран</i></div>
&nbsp;
&nbsp;

Это означает, что получатель ссылки сможет открыть файл.

6.5. При необходимости вы можете отметить поле **Разрешить редактировать**: пользователь с доступом к файлу (далее "получатель") сможет редактировать файл.  
<p>Если нажать на кнопку <b>Меню</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_prop_button.png"> в конце строки, раскрывается меню со следующими пунктами:</p>  
 
 | Пункт                     	| Действие                                                                                                                                              |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| Разрешить делиться        	| Если поставить галочку, получатель сможет предоставлять доступ к этому файлу (давать ссылку на него) другим пользователям. |
| Установить срок действия  	| Если поставить галочку, можно будет указать дату, до которой файл будет доступен по ссылке.                                                          |
| Примечание для получателя 	| Написать комментарий для получателя.                                                                                                                  |
| Удалить ссылку            	| Закрыть доступ к файлу.                                                                                                                               |
&nbsp;
&nbsp;

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_22.png"></div>
<div align="left"><i>Меню общего доступа к файлу</i></div>
&nbsp;
&nbsp;

<p>6.6. Нажмите на кнопку <b>Меню</b><img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_prop_button.png"> в конце пункта <b>Общий доступ по ссылке</b>.</p>

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/nextcloud_23.jpg"></div>
<div align="left"><i>Переход к меню добавления получателя</i></div>
&nbsp;
&nbsp;

<p>Вместо кнопки <b>Добавить</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_add_button.png"> отобразится кнопка <b>Копия</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_copy_button.png"> (отмечена на рисунке) и кнопка <b>Меню</b> <img src= https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_prop_button.png">.</p>

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/f6e60bbbac891f884ca4c686010b474021af4393/img/nextcloud_24.png"></div>
<div align="left"><i>Копирование ссылки на файл</i></div>
&nbsp;
&nbsp;

<p>Чтобы отправить ссылку на файл по электронной почте или в мессенджере, нажмите кнопку <b>Копия</b> <img src="https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_copy_button.png"> (выделена на рисунке) &mdash; ссылка на файл будет скопирована. Чтобы вставить ссылку в письмо, щёлкните правой кнопкой мыши в поле создания письма. Чтобы вставить ссылку в сообщение мессенджера &mdash; в поле набора сообщения и выберите пункт <b>Вставить</b>.</p>

<p>6.7. Если нажать кнопку <b>Меню</b> <img src= https://github.com/vrbtm/tech_writing/blob/9055776f974666a4754511bb1cb336ab76234ddb/img/nextcloud_prop_button.png">, откроется меню со следующими пунктами:</p>

| Пункт                     		| Действие                                                                                                                                              	|
|---------------------------		|-------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Разрешить редактирование  		| Если поставить галочку, получатель сможет редактировать файл.                                                                                         	|
| Скрыть загрузку           		| Если поставить галочку, у получателя при открытии файла будет скрыта кнопка **Загрузить**. Таким образом, скачивание будет затруднено.                 		|
| Защитить паролем          		| Если поставить галочку, можно защитить файл паролем.                                                                                              	|
| Установить срок действия  		| Если поставить галочку, можно указать дату, до которой файл будет доступен по ссылке.                                                           	|
| Примечание для получателя 		| Написать комментарий для получателя.                                                                                                                  		|
| Удалить ссылку            		| Закрыть доступ к файлу.                                                                                                                               		|
| Добавить другую ссылку    		| Создать ещё одну ссылку для доступа к этому файлу, чтобы установить для неё другие опции доступа (возможность редактирования, защиту паролем и т.д.). 		|

\ 
\ 

<div align="left"><img src="https://github.com/vrbtm/tech_writing/blob/f6e60bbbac891f884ca4c686010b474021af4393/img/nextcloud_25.png"></div>
<div align="left"><i>Меню выбора параметров доступа к файлу</i></div>
\ 
\ 

6.8. После выбора нужных свойств доступа отправьте ссылку получателю.  
