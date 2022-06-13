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

<img src="../assets/img/topLevelFeatures_marcEditor.PNG" width="650">

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

OCLC WorldCat: Requires OCLC Integration Setup
* Search WorldCat
* Add/Delete/Update OCLC Bibliographic Data
* Create/Update Bibliographic Data
* Update Holdings
