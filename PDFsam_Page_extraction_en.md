# PDFsam Basic. Extracting pages from .pdf files

The guide explains how to install PDFsam Basic application on desktop computer and extract pages from .pdf files.  
The guide is intended for Windows 10 and 11 users. The application's interface language is English.

## Table of Contents  
[1. Downloading PDFsam](#1-downloading-pdfsam)  
[2. Installing PDFsam](#2-installing-pdfsam)  
[3. Extracting pages](#3-extracting-pages)  
[4. Checking the extraction result](#4-checking-the-extraction-result)  

## 1. Downloading PDFsam
Go to the [PDFsam Basic site](https://pdfsam.org/download-pdfsam-basic/).
To download the Windows application installer, select **Windows downloader.exe**. The PDFsam begins downloading to your downloads folder. 

## 2. Installing PDFsam
When the download is finished, go to your downloads folder and double-click on **PDFsamBasicInstaller.exe**. The file name may slightly vary. The PDFsam application installer is launched.

Select English as your preferred language. Select **Next**. The installation begins.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_inst1.png" width="60%">

While PDFsam is being installed, you can minimize the installer's window by clicking **Minimize** and switch to other applications. 

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_inst2.png" width="60%">

When the installation finishes, a _Thank you_ page on the PDFsam website opens in your browser. It contains links to frequently asked questions, documentation and contacts. You can follow these links if you wish, or close this page.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_inst3.png" width="60%">


## 3. Extracting pages
3.1. Launch PDFsam Basic. The application's main window opens. 

3.2. Click **Extract** button in the left menu or in the main area. Both buttons are marked on the screenshot. The page extraction section opens. 

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext2.png">

3.3a. Open File Explorer in Windows. Drag and drop the file from which the pages should be extracted (hereinafter called **input file**) into the area with caption **Drag and drop PDF files here**. 


3.3b. Alternatively, click on **Add** button marked on screenshot below. The browsing window opens. 

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext3.png">

Highlight the input file and select **Open**.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext4.png" width="70%">

The file is added to the list for processing.

<img src="https://github.com/vrbtm/tech_writing/blob/3d065e0a996e17e24ee1d7f448c7af57895eb61d/img/pdfsam_en_ext41.png" width="70%">

3.4. To extract pages:

  1) Highlight the file in the list.
  2) In item **Extract settings**, type the reuqired page numbers separated with comma, or page intervals. An example is shown on the screenshot below.  

>  :information_source: **Note**  
> If you check the item **Separate file for each set of pages**, a separate file is created for each comma-separated group of pages.  
> In the case below, a separate file is generated for:
> - page 1,
> - page 6,
> - and pages 16-18. 

> If you don't check this item, all extracted pages are placed in one file.

  3) In **Output settings** item, select **Browse** and select the folder where the file with extracted pages (hereinafter called **output file**) should be saved.

>  :information_source: **Note**  
> If you check the item **Overwrite if already exists**, the input file is replaced with the output file.

  4) In item **File names settings**, specify the prefix for output files' names. The default prefix is _PDFsam_.
  5) Click **Run**.

<img src="https://github.com/vrbtm/tech_writing/blob/89019990772bd46d119833c9b1e67609906e2250/img/pdfsam_en_ext5.png" width="70%">

If the folder specified in item 3) is not empty, dialogue window **Directory not empty** is shown. Select **Rename**.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext6.png" width="50%">

## 4. Checking the extraction result
When the task is accomplished, the **Open** button, _Completed_ caption and a color-filled progress bar appear beside the **Run** button.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext7.png" width="70%">

Select **Open** to open the folder where the output files were saved.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext8.png" width="70%">

The created file's name consists of the first page number of the selected page intervals, _PDFsam_ prefix, and the input file's name.
