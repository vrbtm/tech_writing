# PDFsam Basic. Extracting pages from .pdf files

The guide explains how to install PDFsam Basic application (hereinafter called PDFsam) on desktop computer and extract pages from .pdf files.  
The guide is intended for Windows PC users. The application's interface language is English.


## 1. Downloading PDFsam
Open the following address in your browser: [https://pdfsam.org/download-pdfsam-basic/](https://pdfsam.org/download-pdfsam-basic/).
To download the Windows application installer, click _Windows downloader (.exe)_. The _PDFsam_ will begin downloading to your downloads folder. 

## 2. Installation PDFsam
When the download is finished, go to your downloads folder and double-click on _PDFsamBasicInstaller.exe_ (the file name may slightly vary).
The _PDFsam_ application installer will be launched.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_inst1.png" width="60%">

Select English as your preferred language. Click _Next_.  
Application's installation will begin:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_inst2.png" width="60%">

While PDFsam is being installed you can minimize the installer's window by clicking _Minimize_ and switch to other applications.  
When the installation finishes, a "Thank you" page of the PDFsam website will open in your browser. It contains links to frequently asked questions, documentation and contacts. You can follow these links if you wish, or close this page.

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_inst3.png" width="60%">


## 3. Extracting pages
PDFsam Basic icon was created on your Windows desktop. Double-click on it.

<img src="https://github.com/vrbtm/tech_writing/blob/36db6a09d966a23fd9a9aef4a1cfa362aba29eed/img/pdfsam_ext1.png" width="300">

The application's main windows will open.  
To begin extracting pages from a file, click on _Extract_ button in the left menu or in the main area (marked on screenshot):

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext2.png">

The page extraction section will open.  
Click on _Add_ button located above the area with caption _Drag and drop PDF files here_:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext3.png">

The browsing window will open.  
Mark the file from which the pages should be extracted (hereinafter called *input file*) and click on _Open_ button:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext4.png" width="60%">

The file will be added to the list for processing:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext5.png" width="60%">

To extract pages:

  1) Highlight the file in the list.
  2) In item _Extract settings_, type the required pages separated with comma and/or page intervals (an example is shown on the screenshot above).  

> **Note**  
> If you check the item _Separate file for each set of pages_, a separate file will be created for each comma-separated group of pages.  
> In the case above, separate files will be generated for page 1, page 6 and pages 16-18. If you don't check this item, all extracted pages will be placed in one file.

  3) In _Output settings_ item, click Browse button and select the folder to save the file with extracted pages (hereinafter called *output file*).

> **Note**  
> If you check the item _Overwrite if already exists_, the input file will be replaced with the output file.

  4) In item _File names settings_, specify the beginning (prefix) for output files' names. The default prefix is _PDFsam_.
  5) Click _Run_ button.

If the folder specified in item 3) is not empty, dialogue window _Directory not empty_ will be shown.  
Select _Rename_ option:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext6.png" width="60%">

## 4. Extraction result
When the task is accomplished, _Open_ button will appear beside the _Run_ button. Click this button to open the folder where the output files were saved:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_en_ext7.png" width="60%">

A _Completed_ caption and a color-filled progress bar will also appear.  
In the folder you had selected in item 3), a file with extracted pages was created. Its name consists of the first page number of the selected page intervals (in this case, 1), _PDFsam_ prefix and the input file's name:

<img src="https://github.com/vrbtm/tech_writing/blob/b54df565432fb649449220e66c80151fdc663c34/img/pdfsam_ext8.png" width="60%">