---
title: "Top Level Menu Features"
teaching: 20
exercises: 6
questions:
- "What are top level features?"
- "Where are the top level features located?"
- "What can it do?"
objectives:
- "Locate top level menu features"
- "Explain the top level menu features"
keypoints:
- "MarcEdit offers a customizable interface with a suite of tools including the MarcEditor"
- "Users can customize their preferences in the Settings module"
---

# Top Level Menu Features

**1. Getting Started**

## Where are the top level menu features?
MarcEdit has two sections with top level menus. There is the Main Menu and the top level menu in the MarcEditor. This lesson will cover because each offers different and important options for working with MARC data.

### MarcEdit Main Menu
The main menu of MarcEdit is the first window to open when you click to open this application. From here, you can access MarcTools, Settings, Plug-ins, and Help.
![MarcEdit Main Menu](../assets/img/topLevelFeatures_mainMenu.png)

MarcEdit remembers what you did last. In Quick Links, you can easily access your most used tools in MarcEdit.
![MarcEdit Main Menu Quick Links](../assets/img/quickLinks_mainMenu.png)

Settings is where you can set your preferences for MarcEdit. Preferences include the font and size used in the MarcEditor, the default character encoding such as MARC8 or UTF-8, the tools that appear in the MarcEdit Main Menu, or languages for instance.
![MarcEdit Main Menu Settings](../assets/img/settings_mainMenu.png)

#### MarcEdit Main Menu
When you click on MARCEdit Tools Icon from the Main Menu, the available features are:
* MarcBreaker: This "breaks" the MARC binary file into a readable format that can be edited in the MarcEditor.
* MarcMaker: This takes the readable format MARC data file and creates the MARC binary file.
* MARC21 to MARC21XML: This converts a MARC21 file to MARC21XML.
* MARC21XML to MARC21: This converts a MARC21XML file to a MARC21 binary file.
* MARC to JSON: This converts a MARC21 file to a JSON file.
* JSON to MARC: This converts a JSON file to a MARC21 file.
* JSON to XML: This converts a JSON file to XML.
* XML to JSON: This converts an XML file to JSON.
Options include changing the default character encoding only for the tool that you select, translating the MARC data to MARC-8 or UTF8. To change the default character encoding, you will need to go to Settings.

The conversions from one encoding standard to another, as in MARC21 to MARC21XML, rely on eXtensible stylesheets. MarcEdit comes with several default stylesheets which come from those maintained by the Library of Congress. If you are familiar with stylesheets, you can also create your own.

There are more features available with the tope level menu option called Tools. There are so many options here. Some will be covered in Integrations in Lesson 8. Let's highlight some tools from this menu.
* Preferences: This will take you to Settings. Often in MarcEdit, there is more than one place to get to a feature or setting.
* Delimited Text Translator: If you have a spreadsheet of data, this tool will take that data and create MARC data.
* Export: You can export a MARC record. More importantly, you can export a Tab Delimited file from MARC data. This tool will take a MARC binary file and create a spreadsheet (either tab or comma separated based on your selection) of all the MARC data.
* MARC Processing Tools: Features include MARCSplit, MARCJoin, Merge, MARCCompare, MARCValidator, or finding duplicate records.

The MARC Processing Tools can be added to the Main Menu Window in Preferences or Settings. For example, if you use MARCJOIN frequently, then you can add this to the Main Menu Window.
![MarcEdit Main Menu Tools](../assets/img/tools_mainMenu.png)

>## Update the default character encoding setting
>
>1. Change or verify the default character encoding setting to UTF8
>
> > ## Solution
> > 1. Click on the gear icon in the Main Menu window or go to Tools and then Preferences
> > 2. Click on MarcEditor
> > 3. In the Default Encoding down down menu, select UTF8
> > 4. Click OK
> {: .solution}
{: .challenge}

>## Change the font and size used in the MarcEditor
>
>1. Change the font to Arial and size 14
>
> > ## Solution
> > 1. Click on the gear icon in the Main Menu window or go to Tools and then Preferences
> > 2. Click on MarcEditor
> > 3. In the Set MarcEditor Font Properties window, click on Set Font
> > 4. Scroll down to Ariel and select font size 14
> > 5. Click OK
> {: .solution}
{: .challenge}

> ## Go back to the defaults
>
> If you don't like the font and size, you can go back to the defaults.
> Go back to Settings by clicking on the gear icon or Tools and Preferences
> Go to MarcEditor
> In the Set MarcEditor Font Properties, click on Set Defaults.
>
{: .callout}

>## Add a MARC Processing Tool to the Main Menu Window
>
>1. Add MARCJoin to the Main Menu Window
>
> > ## Solution
> > 1. Click on the gear icon in the Main Menu window or go to Tools and then Preferences
> > 2. The top option Main Window should already be highlighted. If not, click on Main Window
> > 3. Check off MARCJoin
> > 5. Click OK
> {: .solution}
{: .challenge}

> ## Main Window and Updating Settings/Preferences
>
> Only 4 programs can be added to the Main Window.
> When you update some settings like the font and size, you might have to close and reopen MarcEdit.
>
{: .callout}
