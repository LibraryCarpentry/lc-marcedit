---
title: "Introduction to MarcEdit"
teaching: 0
exercises: 0
questions:
- "What is MarcEdit?"
- "What can MarcEdit do?"
objectives:
- "Explain what the MarcEdit software does"
- "Explain how the MarcEdit software can help work with metadata files"
keypoints:
- "MarcEdit is a tool for working with bibliographic metadata, specifically in the MARC format"
- "MarcEdit can be used to open and edit MARC files"
- "MarcEdit can be used to convert between several different metadata formats, including different expressions of MARC such as MARCXML and Mnemonic MARC"
---
## What is MarcEdit?

MarcEdit is a suite of tools created and maintained by Terry Reese. The tools together form the MarcEdit software. These tools provide numerous features which can be used to create, edit, and work with library metadata, particularly (though not limited to) records in a variety of MARC formats and standards. In this way, the MarcEdit software is MARC agnostic and can work with Unimarc or MARC21. MarcEdit can be used to

* make small, single, edits to individual MARC records
* make edits across many MARC records at a single time
* automate common edits/processes
* validate your data against MARC rules
* convert data between different formats
* enhance your data
* pull data from external sources

The features offered by the suite of MarcEdit tools continue to evolve, with new features added as the software is updated by Terry Reese. [A list of features](https://marcedit.reeset.net/features) is available on the MarcEdit website.

Although the ability to create, view and edit MARC records is built into many pieces of library and bibliographic management software, MarcEdit is particularly flexible and powerful for editing MARC data as well as offering integration with other software and services. With MarcEdit's wide-ranging functionality and integration into other library services it is a very powerful toolkit for anyone working with bibliographic data.

## MarcEdit's Primary Features

### Profiling MARC Data
Before working with any data, it is advantageous to understand that data. Does the file contain MARC data that describes only books and are those books print and/or electronic? Do the records follow national metadata standards and best practices needed for your local systems? How many records are in the file?

Getting a profile of the MARC data in your file can help you make a plan on what changes need to be made to the file. Further, it can help you automate some of the changes if this type of file is one that you work with often.

### Manipulating MARC Data
The MarcEditor is like the Swiss army knife of MARC data. You can perform single or global edits such as adding or deleting MARC fields, subfields, indicator values. Other edit functions are building fields using MARC data from other fields, or changing the case of data in a field. Other operations include running operations to help update your MARC data to the content standard Resource Description and Access (RDA) or to assign OCLC's FAST headings to records in the file.

### Tasks and Automation
Edits can be performed on one record by editing directly on the record in the MarcEditor. Edits can be global and done one at a time to the entire file. If you have a list of changes to make, these can be set up in what is called a MARC task. These tasks make automating manipulating your MARC data easier and quicker.

### Integrations
The MarcEditor can integrate with OCLC's WorldCat and Ex Libris' Alma library system platform. Using the MarcEditor, you can retrieve records through these integrations, manipulate the records, and the push those changes back to the integration of your choice.

Though not necessarily an integration, harvested records can also be manipulated in the MarcEditor. MarcEdit allows to harvest Duplin Core or MARC records.

### Regular Expressions
The MarcEditor allows for the use of regular expressions in many of its MARC data manipulation features. Regular expressions are a sequence of text to identify a search pattern. This is a powerful tool that allows greater flexibility when manipulating MARC data.
## Getting help

If you encounter problems installing or running MarcEdit, a good source of support is the [MarcEdit mailing list]( http://listserv.gmu.edu/cgi-bin/wa?A0=marcedit-l). [The MarcEdit website has a list of places where you can get help using the software](https://marcedit.reeset.net/help) including:

* [The MarcEdit Knowledgebase](https://marcedit.reeset.net/archives/category/knowledge_base)
* [The MarcEdit 101 Webinar](https://marcedit.reeset.net/marcedit-101-workshop)
* [A set of video tutorials on YouTube](https://www.youtube.com/playlist?list=PLrHRsJ91nVFScJLS91SWR5awtFfpewMWg)

{% include links.md %}
