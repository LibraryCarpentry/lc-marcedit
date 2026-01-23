---
title: Setup
---

## Getting Ready

You need to install the latest version of MarcEdit and download a data file to follow this lesson. If you are using an older version of MarcEdit, it is recommended you upgrade to the latest version.

## Downloading MarcEdit

MarcEdit is a free, open-source application. You can download MarcEdit from
[https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads).
This lesson has been tested with the following versions: MarcEdit 7 (specifically 7.6.3 and 7.7.10) for Windows and MarcEdit 3 for MacOS. It should be highlighted that MarcEdit is frequently updated with minor changes. It is recommended that the latest version is used, but note that this may mean there are minor differences between the current version and the versions used to test this lesson. 

#### Plug-Ins and Packages

Packages, along with associated system requirements, are available on [https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads) for Windows and MacOS.

### Windows

#### System Requirements for Windows

System requirements for MarcEdit 7/MarcEdit Windows [https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads):

- RAM: 8MB minimum; 32 MB+ is recommended
- Disc space for Windows: 34 MB (setup); 15 MB (application)
- For Windows, Windows .NET 4.7.2+ is required.

#### Determining if your system is 32 or 64-bit
Windows: In the Start menu, type in About to get About Your PC. In Device Specifications, the system type will tell you if it's a 32 or 64-bit CPU.

### Installing MarcEdit On Windows - [Video](https://www.youtube.com/watch?v=FX0r7jIxeN4)

From the Downloads page, click on [Windows Build Options](https://marcedit.reeset.net/downloads). A pop-up window will appear with two choices: the Windows User Only Installation and the Consolidated Installation. The Windows User Only Installation should work for the majority of participants. If you will be using a communal computer, and expect MarcEdit to be used by a number of users on that machine, read through the "Windows Build Options" pop-up to decide the best installation option for you. You can also view this [video tutorial](https://youtu.be/7wYo7VoOwMI) for this type of advanced installation called the consolidated option.

#### Notes for Windows users

- The Consolidated Installation for MarcEdit 7.5 for Windows is the only one installation option that currently supports 32-bit systems.
- If the installation is being done via distributed software or via a distribution client like Microsoft's SCCM, refer to the packaging tool available on GitHub [https://github.com/reeset/marcedit\_package\_builder](https://github.com/reeset/marcedit_package_builder).
- Instructions for system administrators have been provided. Also, information on managing MarcEdit installations is available [https://marcedit.reeset.net/managing-marcedit-installations](https://marcedit.reeset.net/managing-marcedit-installations).

### MAC

#### System Requirements for Mac

System requirements for MarcEdit 7/MarcEdit MacOS 3 [https://marcedit.reeset.net/downloads](https://marcedit.reeset.net/downloads):

- Operating system: Vista (32 \& 64-bit), MacOS 10.10+
- RAM: 8MB minimum; 32 MB+ is recommended
- Disc space for MacOS: 60 MB (setup); 150 MB (installed)
- For MacOS, Installer, where all dependencies are packaged and installed, is required.

#### Determining if your system is 32 or 64-bit

MacOS: Select the About This Mac option in the Apple menu. On the About This Mac window, click the Systems Report below the information in the Overview. Click on Hardware. In the Hardware Overview in the top left column, you will see the processor name to determine if it's a 32-bit or 64-bit CPU.

### Installing MarcEdit on Mac - [Video](https://www.youtube.com/watch?v=m8TQsNhpw8I)

For MacOS, select ["MacOs"](https://marcedit.reeset.net/software/marcedit75/MarcEdit3_5.pkg.zip). Unzip the package and follow the MacOS instructions.

#### Notes for MAC users
- The functionality between MAC and Windows is not the same. The Windows version offers more functionality.
- Appearance and where menu features are placed is not the same between the MAC and Windows versions.

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
  - XML Processing Engine: Select Choose for me

## Downloading the data

-  Click on [this link](https://github.com/LibraryCarpentry/lc-marcedit/blob/main/episodes/data/marc_sample_data.mrc)
-  Click on download button ![](fig/downloadButton.png){alt='GitHub Download Button icon'}
-  The marc sample file will be saved to your local computer

For this lesson, you need to download our sample file from the Library Carpentries MarcEdit GitHub repository. This MARC file follows the MARC21 standard and is encoded in UTF-8. The sample file comes from MARC 21 records downloaded from the Open Textbook Library and the University of Florida's original catalog data. "Open Textbook Library records are in the public domain and available under a Creative Commons CC0 license." [Open Textbook Library](https://open.umn.edu/opentextbooks/discovery). The book catalog in MARC 21 format from the University of Florida has been released in the public domain under a CC0 license. [Creative Commons](https://wiki.creativecommons.org/wiki/CC0_use_for_data#University_of_Florida_Library)


## Seeing file extensions
For this lesson, it will be helpful to be able to see file extensions.

### Enabling file extensions on a PC

- Open File Explorer (open any folder)
- Click on the caret next to View
- Click Show
- Select File name extensions

### Enabling file extensions on a MAC

- Open Finder
- Select the Preferences
- Click on the Advanced tab
- Check the box "Show all filename extensions"

## Getting help

Installation video demonstrations are available for all users [https://youtu.be/FX0r7jIxeN4](https://youtu.be/FX0r7jIxeN4).

If you encounter problems installing or running MarcEdit, a good source of support is the [MarcEdit mailing list and user forum](https://listserv.gmu.edu/cgi-bin/wa?A0=marcedit-l). You can also fill out the [Help Form](https://marcedit.reeset.net/contact-me).
Include your operating system when searching to find the most relevant answers for your issue.

You may also want to check the [Videos](https://www.youtube.com/playlist?list=PLrHRsJ91nVFScJLS91SWR5awtFfpewMWg) or the [MarcEdit Knowledge Base](https://marcedit.reeset.net/archives/category/knowledge_base).

## Updating MarcEdit

MarcEdit is continually being improved. Fixes and sometimes new functionality are released several times per year. There is no set schedule as to when an update is available. However, it is recommended to subscribe to the MarcEdit mailing list and user forum where information is posted on new updates and/or versions.

:::::::::::::::::::::::::::::::::::::: instructor

Note: Typically updates will not remove funtionality. However, some updates will re-arrange tools and functions slightly differently from time to time. For example, from 7.6 to 7.7, the Edit Shortcuts menu went from one level to choose from to a mix of 2 and one. 
  
:::::::::::::::::::::::::::::::::::::::::::::::::
