---
title: "Working in the MarcEditor"
teaching: 10
exercises: 0
questions:
- "What is the MarcEditor?"
- "How are MARC files organized in the MarcEditor"
objectives:
- "Explain what the MarcEditor does"
- "Explain how the MarcEditor features can help work with MARC files"
keypoints:
- "MarcEditor is a tool to work with MARC data in an easily readable format"
- "The MarcEditor can be used to perform a number of different functions such as adding, deleting MARC fields or subfields, building MARC fields, running reports, or checking the validity of MARC data"
- "The MarcEditor can be used to perform one task at a time or automate a set of tasks for particular types of MARC files"
- "It is necessary to break a MARC binary file to work with that MARC data in the MarcEditor. The extension of these easily readble MARC files are .mrk rather than the binary extension of .mrc"
---
# MarcEditor Top Level Menu
The MarcEditor has a robust set of features available via the top level menu. Features can be accessed through the menu or through shortcut keys. The shortcut key for a feature appears next to it in the menu.

![MarcEditor Top Level Menu](../assets/img/topLevelFeatures_marcEditor.png)

## MarcEditor Top Level Menu Features
Each top level menu features so many gems. Let's highlight some of those.

File
* Save, Save As, Open, Recent: This is where you'll find those important functions of saving, saving as, opening up a recent file, or opening a new file.
* Select Records for Edit: This is where you can work on a subset of the data.
* Compile File: This is the same function as MarcMaker meaning that the readable version of your MARC data in the MarcEditor will be converted to a MARC binary file.

Edit
* Find and Replace: You can find or find and replace just on the current page or in the entire file.
* Edit Shortcuts: This is where you can change the case, find records that have a missing MARC field or duplicate MARC field, or find fields with a missing word.
* Jump To: You can use this to jump to record in the file.
* Insert/Edit 006 or 008: This will open a form to easily insert or edit these fixed fields.
* Delete Record: You can delete one or more records in a range or based on invalid encoding characters.

Fonts
If you need to change the font and size for the current MARC data you are working on in the MarcEditor, this is the place to do that.

Reports
* Create a custom report
* Get a count of all the MARC Fields in the MARC Data
* Get a count of the records based on type (book, serials, videorecordings, etc.)
* MARCValidator

Tools
* Add/Delete Marc Fields
* Edit subfields
* Edit Indicators
* Build a new MARC field
* RDA Helper
* Sort By

OCLC WorldCat
MarcEdit offers a number of integrations one of which is to OCLC. You can use the Z39.50 tool or OCLC's APIs for metadata and searching to bring in records from WorldCat, update/delete holdings, or work on local bibliographic data.

>## Where is the feature "Select Records for Edit"
>
>1. Find Select Records for Edit
>
> > ## Solution
> > 1. In the MarcEditor, click on File
> > 2. Scroll down to Select Records to Edit
> {: .solution}
{: .challenge

>## Where is the feature to edit one or both indicators for a MARC field
>
>1. Find Edit Indicators
>
> > ## Solution
> > 1. In the MarcEditor, click on Tools
> > 2. Scroll down to Edit Indicator Data
> {: .solution}
{: .challenge}

>## Where is the feature to find a missing MARC field
>
>1. Find out if you file has any missing 856 MARC fields
>
> > ## Solution
> > 1. In the MarcEditor, click on Edit
> > 2. Scroll down to Edit Shortcuts
> > 3. Select Field Edits
> > 4. Select Find Records Missing Fields
> > 5. In the pop up winder, type in 856
> > 6. Click OK
> {: .solution}
{: .challenge}

# Working in the MarcEditor
MarcEditor works slightly differently than other text editors. To work with MARC data in the MarcEditor, it is first necessary to "break" the MARC binary file using MarcBreaker. To do this you can use the MarcBreaker tools. Another way is to simply click on the MARC finary file (often this file has the extension .mrc). This will prompt the MarcBreaker tool window to open. Selecting execute will start the process. Here MarcEdit reads the entire MARC file. It then creates the virtual pages of the MARC records in the file. This is called the Paging style of opening a file.

# MarcEditor features
There are five features to highlight that will be covered in the next lessons:
* Profiling MARC data
* Manipulating MARC data
* Tasks and automation
* Integrations
* Use of regular expressions

## Profiling MARC Data
Before working with any data, it is advantagous to understand that data. Does the file contain MARC data that describes only books and are those books print and/or electronic? Do the records follow national metadata standards and best practices needed for your local systems? How many records are in the file?

Getting a profile of the MARC data in your file can help you make a plan on what changes need to be made to the file. Further, it can help you automate some of the changes if this type of file is one that you work with often.

## Manipulating MARC Data
The MarcEditor is like the Swiss army knife of MARC data. You can perform single or global edits such as adding or deleting MARC fields, subfields, indicator values. Other edit functions are building fields using MARC data from other fields, or changing the case of data in a field. Other operations include running operations to help update your MARC data to the content standard Resource Description and Access (RDA) or to assign OCLC's FAST headings to records in the file.

## Tasks and Automation
Edits can be performed on one record by editing directly on the record in the MarcEditor. Edits can be global and done one at a time to the entire file. If you have a list of changes to make, these can be set up in what is called a MARC task. These tasks make automating manipulating your MARC data easier and quicker.

## Integrations
The MarcEditor can integrate with OCLC's WorldCat and Ex Libis' Alma library system platform. Using the MarcEditor, you can retrive records through these integrations, manipulate the records, and the push those changes back to the integration of your choice.

Though not necessarily an integration, harvested records can also be manipulated in the MarcEdtor. MarcEdit allows to harvest Duplin Core or MARC records.

## Regular Expressions
The MarcEditor allows for the use of regular expressions in many of its MARC data manipulation features. Regular expressions are a sequence of text to identify a search pattern. This is a powerful tool that allows greater flexibility when manipulating MARC data.
