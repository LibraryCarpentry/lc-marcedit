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
# Working in the MarcEditor
MarcEditor works slightly differently than other text editors. To work with MARC data in the MarcEditor, it is first necessary to "break" the MARC binary file using MarcBreaker. To do this you can use the MarcBreaker tools. Another way is to simply click on the MARC finary file (often this file has the extension .mrc). This will prompt the MarcBreaker tool window to open. Selecting execute will start the process. Here MarcEdit reads the entire MARC file. It then creates the virtual pages of the MARC records in the file. This is called the Paging style of opening a file.

## Paging versus Preview
Preview mode is particularly useful for large MARC files. In Preview mode, you can use the edit functions on the file. However, the disadvantage is that you can not edit the file itself because Preview mode opens the file as read only.

Paging mode is the default set when opening up a file in the MarcEditor. Here, the entire MARC file is read to retrieve the total number of records in the MARC file that are then split into a number of virtually created pages. Here, you can use any of the MarcEdtor tools and make edits to any record on any of the virtual pages. When this file is saved in Paging mode, the number of pages is recalculated, or the file is re-paged.

> ## Paging Version 7 Updates
>
> In version 7, the technology behind saving and re-paging saved to address the issue of the time it took to do this on large files. For previous versions, and in particular version 6, it is recommended to use the preview mode for data over approximately 150 MB. In other words, the paging mode works better for data under approximately 150 MBs.
>
{: .callout}

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
