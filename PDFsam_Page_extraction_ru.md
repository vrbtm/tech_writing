# PDFsam Basic. Извлечение страниц из pdf-файлов 

Руководство объясняет, как работать с одной из функций приложения PDFsam Basic (далее PDFsam) – извлекать определённые страницы из pdf-файлов.  
Руководство предназначено для пользователей компьютеров с операционной системой Windows. Интерфейс устанавливаемого приложения — русскоязычный.

## Оглавление
[1. Загрузите PDFsam](#1-%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%B8%D1%82%D0%B5-pdfsam)  
[2. Установите PDFsam](#2-%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D1%82%D0%B5-pdfsam)  
[3. Как извлекать страницы из pdf-документов](#3-%D0%BA%D0%B0%D0%BA-%D0%B8%D0%B7%D0%B2%D0%BB%D0%B5%D0%BA%D0%B0%D1%82%D1%8C-%D1%81%D1%82%D1%80%D0%B0%D0%BD%D0%B8%D1%86%D1%8B-%D0%B8%D0%B7-pdf-%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2)  
[4. Проверьте результат извлечения](#4-%D0%BF%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D1%8C%D1%82%D0%B5-%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82-%D0%B8%D0%B7%D0%B2%D0%BB%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D1%8F)

## 1. Загрузите PDFsam
Перейдите на [страницу PDFsam Basic](https://pdfsam.org/download-pdfsam-basic/).
Чтобы загрузить приложение для Windows, выберите **Windows downloader.exe**. Установщик **PDFsam** начнет загружаться в папку загрузок. 

## 2. Установите PDFsam
После окончания загрузки откройте файл **PDFsamBasicInstaller.exe**. Имя файла может немного отличаться. Откроется окно установки приложения **PDFsam**.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_inst1.png" width="60%">

По умолчанию в качестве языка приложения выбран русский. Нажмите кнопку **Далее**. Начнётся установка приложения.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_inst2.png" width="60%">

На время установки вы можете свернуть это окно нажатием кнопки **Свернуть** и переключиться на другие окна.  
Когда установка завершится, в браузере откроется страница компании-производителя приложения со ссылками на часто задаваемые вопросы — _FAQ_, документацию — _Documentation_ и контакты — _Contact us_. Вы можете перейти по ссылкам, если вас интересуют эти разделы, либо закрыть эту страницу.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_inst3.png" width="60%">

## 3. Как извлекать страницы из pdf-документов
3.1. Запустите **PDFsam Basic**. Откроется основное окно приложения.

3.2. Нажмите на ссылку **Извлечь** в левом меню либо на основном поле. Оба пункта меню выделены на рисунке. Откроется окно раздела извлечения страниц.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext2.png">

3.3a Откройте Проводник Windows. Перетащите мышью файл, из которого требуется извлечь страницы (далее — исходный файл), в область с надписью **Перетащите PDF-файлы сюда**. Файл будет добавлен в список для обработки. 


3.3b Либо нажмите кнопку **Добавить**, выделенную на рисунке. Откроется окно выбора файла.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext3.png">

Выделите исходный файл и нажмите кнопку **Открыть**.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext4.png" width="60%">

Файл будет добавлен в список для обработки.

<img src="https://github.com/vrbtm/tech_writing/blob/3d065e0a996e17e24ee1d7f448c7af57895eb61d/img/pdfsam_ext41.png" width="70%">

3.4. Настройте параметры файла с извлечёнными страницами (далее — создаваемого файла):

  1) Выделите файл.
  2) В пункте **Настройки извлечения** укажите страницы через запятую или интервалы страниц. На рисунке показан пример перечисления.
  
>  :information_source: **Примечание**  
> Если поставить галочку в пункте **Отдельный файл для каждого набора страниц**, то появится отдельный файл для каждой группы страниц, разделённых запятыми. Для диапазона, указанного на рисунке, будут созданы:
> - файл со страницей 1,
> - файл со страницей 6,
> - файл со страницами 16-18. 

> Если не отмечать этот пункт, то все извлечённые страницы будут помещены в один файл.

  3) В пункте **Настройки вывода** нажмите кнопку **Обзор** и выберите папку для сохранения создаваемого файла.  

>  :information_source: **Примечание**  
> Если поставить галочку в пункте **Заменить, если уже существует**, то исходный файл будет заменён создаваемым файлом.

  4) В пункте **Настройка имён файлов** укажите префикс названий создаваемых файлов. Префикс по умолчанию — слово _PDFsam_.
  5) Нажмите кнопку **Выполнить**.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext5.png" width="60%">

Если папка, которую вы указали в пункте 3), не пустая, отобразится диалоговое окно **Каталог не пуст**. Выберите вариант **Переименовать**.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext7.png" width="420">

## 4. Проверьте результат извлечения
После завершения извлечения рядом с кнопкой **Выполнить** отобразятся кнопка **Открыть**, надпись _Выполнено_ и полностью закрашенная полоса индикатора выполнения. 

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext6.png" width="60%">

Если нажать кнопку **Открыть**, откроется папка, в которой были сохранены созданные файлы. Название созданного файла состоит из номера первой страницы указанного вами диапазона, префикса _PDFsam_ и названия исходного файла.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext8.png" width="70%">
