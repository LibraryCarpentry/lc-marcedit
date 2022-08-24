---
title: "Top Level Menu Features"
teaching: 20
exercises: 3
questions:
- "What are the top level features?"
- "Where are the top level features located?"
objectives:
- "Locate top level menu features"
- "Explain the top level menu features"
keypoints:
- "MarcEdit offers the ability to add shortcuts to the main window"
- "MarcEdit allows you to set preferences for features and tools such as the main window or the MarcEditor"
- "Preferences can be accessed using the gearbox icon, going to Tools -> Preferences or using the keyboard shortcut of Ctrl+Shift+P"
---

# Top Level Menu Features

## Where are the top level menu features?
When you launch MarcEdit, the main window opens. From here, you can access the suite of MarcEdit tools, features, plug-ins, quick links, or help. One thing you'll notice is that there are both shortcuts, linked icons, and menu options that lead to the same features or tools. For example, to update your preferences, you can go to Tools -> Preferences, use the keyboard shortcut of Ctrl+Shift+P, or click on the gearbox in the upper left hand corner of the main window. 

### MarcEdit Main Menu: Preferences
In MarcEdit, Preferences allow you to change the main window and various tools, such as the MarcEditor (the tool used to manipulate MARC data). For example, for the main window you can change the font and font size and select your most frequently used tools to display as shortcuts. For the MarcEditor, you can update the default character encoding for records that are opened in this tool (such as MARC8 or UTF-8).

>## Let's add a shortcut to our main window
>1. Click on the gearbox in the top left corner or go to Tools -> Preferences
>2. Make sure you select "Main Window" in the Preferences popup window in the left hand pane
>3. In the right hand pane, select MARCSplit
>3. Click Ok
{: .checklist}

>## How many shortcuts can be added to the main window?
>
> > ## Solution
> > 1. Click on the gear icon in the main window or go to Tools -> Preferences
> > 2. In the new window, make sure you select Main Window in the left hand pane
> > 3. In the right pane, select any tool that hasn't been selected
> > 5. You will see a popup message that says "Only four items can be select. Unselect on one of the options and then reselect."
> > 6. A user can only select 4 options or tools as shortcuts to appear in the main window.
> {: .solution}
{: .challenge}

If you change your preferences for the MarcEditor, the tool used to work with MARC data, you can always go back to the default settings. 
>## Reset settings for the MarcEditor in Preferences
>1. Click on the gearbox in the top left corner or go to Tools -> Preferences
>2. Make sure you select "MarcEditor" in the Preferences window in the left hand pane
>3. In the right hand pane, select Set Defaults for either font or font size
>3. Click Ok
{: .checklist}

>## Name three other tools or features that can be changed in Preferences.
>
> > ## Solution
> > 1. Click on the gear icon in the main window or go to Tools -> Preferences
> > 2. In the left hand pane, look at the names there
> > 3. Tools or features that can be changed in Preferences: Main Window, Bibframe, MarcEditor, MARCEngine, Ease of Use, File Associations, Language, Locations, Other, Updates, Configure Watcher, ILS Integration, OCLC API Integration.
> {: .solution}
{: .challenge}

### MarcEdit Main Window: Top Level Menu
In the main window top level menu, there are three options: Tools, Plug-ins, and Help. 

#### Plug-Ins
There are a number of useful plugins that can be added to MarcEdit to extend its functionality. An example is the MARC to [KBART or Knowledge bases and related tools](https://www.niso.org/standards-committees/kbart/kbart-frequently-asked-questions) converter. You can find more information on plugins on the [MarcEdit Plugin page](https://marcedit.reeset.net/managing-plugins-in-marcedit).

#### Help
This top level menu Help allows you to find information on updates, about your current MarcEdit installation, and links out to video tutorials or online help for instance. 

#### Tools
The Tools menu allows you to access a number of different features such as Prefernces which we saw above. Other features to highlight are:
* The MarcEdit regular expression store
* OAI Harvester
* Export either MARC records or records reformatted as a text delimited csv (comma separated value) or tsv (tab separated value) file
* MARC Processing Tools: MARCsplit, MARCcompare, MARCjoin, MARCmerge, find duplicate records, RDA Helper, or MARCValidator for instance
* Delimited Text Translator
* Preferences
* Utilities that include a verify URL tool

#### MARCTools or the tools icon
If you want to work with MARC data files or converting between metadata formats for library bibliographic data, click on the MARCTools icon that has the crossed hammer and spanner in the upper left hand corner. The available features are:
* MarcBreaker: This "breaks" the MARC binary file into a readable format that can be edited in the MarcEditor.
* MarcMaker: This takes the readable format MARC data file and creates the MARC binary file.
* MARC21 to MARC21XML: This converts a MARC21 file to MARC21XML.
* MARC21XML to MARC21: This converts a MARC21XML file to a MARC21 binary file.
* MARC to JSON: This converts a MARC21 file to a JSON file.
* JSON to MARC: This converts a JSON file to a MARC21 file.
* JSON to XML: This converts a JSON file to XML.
* XML to JSON: This converts an XML file to JSON.

The conversions from one encoding standard to another, as in MARC21 to MARC21XML, rely on eXtensible stylesheets. MarcEdit comes with several default stylesheets which come from those maintained by the Library of Congress. If you are familiar with stylesheets, you can also create your own.

>## Where is the feature to export MARC records as a text delimited file?
>
> > ## Solution
> > 1. go to Tools -> Preferences
> > 2. Click on Export
> > 3. Select Export Tab Delimited Records
> {: .solution}
{: .challenge}

>## Difference between Tools menu and MARCTools icon
>The functionality in Tools menu is related to working with one or more MARC data files at a time such as exporting, harvesting, spliting, comparing, or joining. Other features that we've seen above are accessing Preferences or using utilities such as checking URLs.
>The MARCTools icon allows you to work with a specific MARC data file in terms of converting MARC files from one format into another such as a binary MARC file into a human readable mnenomic format, or a MARC21 file into a MARCXML file.
{: .callout}

### MarcEdit Main Window: History
MarcEdit remembers what you did last. You can see this history in the Quick Links section which is a drop down of features and tools you frequently use. Although not related to a history of what you did last in MarcEdit, the "What would you like to do?" box in the upper right hand corner is convenient for quickly finding tools and features in MarcEdit.


