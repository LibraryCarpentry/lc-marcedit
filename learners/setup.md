---
title: Setup
---

## Getting Ready

You need to install the latest version of MarcEdit and download a data file to follow this lesson. If you are using an older version of MarcEdit, it is recommended you upgrade to the latest version which may be beyond what was tested for this lesson.

## Downloading MarcEdit

MarcEdit is a free, open-source application. You can download MarcEdit from
[https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads).
This lesson has been tested with the following versions: MarcEdit 7 (specifically 7.6.3) for Windows and MarcEdit 3 for MacOS. It should be highlighted that MarcEdit is frequently updated and these instructions might have been tested on a slightly earlier version. 

#### Plug-Ins and Packages

Packages, along with associated system requirements, are available on [https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads) for Windows and MacOS.

#### System Requirements for Mac and Windows

System requirements for MarcEdit 7/MarcEdit MacOS 3 [https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads):

- Operating system: Vista (32 \& 64-bit), MacOS 10.10+
- RAM: 8MB minimum; 32 MB+ is recommended
- Disc space for Windows: 34 MB (setup); 15 MB (application)
- Disc space for MacOS: 60 MB (setup); 150 MB (installed)
- For Windows, Windows .NET 4.7.2+ is required.
- For MacOS, Installer, where all dependencies are packaged and installed, is required.

#### Determining if your system is 32 or 64-bit

- MacOS: Select the About This Mac option in the Apple menu. On the About This Mac window, click the Systems Report below the information in the Overview. Click on Hardware. In the Hardware Overview in the top left column, you will see the processor name to determine if it's a 32-bit or 64-bit CPU.
- Windows: In the Start menu, type in About to get About Your PC. In Device Specifications, the system type will tell you if it's a 32 or 64-bit CPU.

### Installing MarcEdit On Windows - [Video](https://www.youtube.com/watch?v=FX0r7jIxeN4)

For Windows, select [Windows Build Options -> Download MarcEdit 7.5 (All Users)](https://marcedit.reeset.net/software/marcedit75/MarcEdit_7_5_User_Install.exe). The Windows User Only Installation should work for the majority of participants. If you will be using a communal computer, and expect MarcEdit to be used by a number of users on that machine, read through the "Windows Build Options" pop-up to decide the best installation option for you. You can also view this [video tutorial](https://youtu.be/7wYo7VoOwMI) for this type of advanced installation called the consolidated option.

#### Notes for Windows users

- The Consolidated Installation for MarcEdit 7.5 for Windows is the only one installation option that currently supports 32-bit systems.
- If the installation is being done via distributed software or via a distribution client like Microsoft's SCCM, refer to the packaging tool available on GitHub [https://github.com/reeset/marcedit\_package\_builder](https://github.com/reeset/marcedit_package_builder).
- Instructions for system administrators has been provided. Also information on managing MarcEdit installations are available [https://marcedit.reeset.net/managing-marcedit-installations](https://marcedit.reeset.net/managing-marcedit-installations).


### Installing MarcEdit on Mac - [Video](https://www.youtube.com/watch?v=m8TQsNhpw8I)

For MacOS, select ["MacOs"](https://marcedit.reeset.net/software/marcedit75/MarcEdit3_5.pkg.zip). Unzip the package and follow the MacOS instructions.

### Running MarcEdit for the First Time: The Setup Wizard - [Video](https://www.youtube.com/watch?v=iHEimALeojU)

After downloading MarcEdit and once you launch the installation the first time, you will be asked to go through the setup wizard. This wizard will ask you to configure the default font, font size, and recommended theme. The wizard will then ask you to configure the MARC standard and file standard being used.

- Click on "Let's get started"
- MarcEdit Appearance
  - Default font: Select your preferred font
  - Application font size: Select your preferred font size
  - Recommended Theme: Select default
- MarcEdit Data Settings
  - My MARC Format is: Select MARC21
  - Default Recording Encoding: Select MARC21/UTF8
  - Make sure "Enforce Unicode Normalization" is checked
  - XML Processing Enging: Select Choose for me

## Downloading the data

For this lesson, you need to download our sample file from the Library Carpentries MarcEdit GitHub repository. Go to the GitHub [page for that marc\_sample\_data.mrc](https://github.com/LibraryCarpentry/lc-marcedit/blob/main/episodes/data/marc_sample_data.mrc). Then, click the download button on the right hand side. This MARC file follows the MARC21 standard and is encoded in UTF-8.

-  Click on [this link](https://github.com/LibraryCarpentry/lc-marcedit/blob/main/episodes/data/marc_sample_data.mrc)
-  Click on download button ![](fig/downloadButton.png){alt='GitHub Download Button icon'}
-  The marc sample file will be saved to your local computer

## Getting help

Installation video demostrations are available for all users [https://youtu.be/FX0r7jIxeN4](https://youtu.be/FX0r7jIxeN4).

If you encounter problems installing or running MarcEdit, a good source of support is the [MarcEdit mailing list and user forum](https://listserv.gmu.edu/cgi-bin/wa?A0=marcedit-l). You can also fill out the [Help Form](https://marcedit.reeset.net/contact-me).
Include your operating system when searching to find the most relevant answers for your issue.

You may also want to check the [Videos](https://www.youtube.com/playlist?list=PLrHRsJ91nVFScJLS91SWR5awtFfpewMWg) or the [MarcEdit Knowledge Base](https://marcedit.reeset.net/archives/category/knowledge_base).
