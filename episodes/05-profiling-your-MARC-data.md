---
title: Profiling Your MARC data
teaching: 10
exercises: 5
---

::::::::::::::::::::::::::::::::::::::: objectives

- Access reports for getting an overview of your MARC data
- Find tools to locate errors in your MARC records by using the MARCedit Edit toolbar

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How do I use different reports to get an overview of my MARC file?
- How do I locate errors in my records?
- How do I use the Edit Shortcuts tool to identify and fix common errors?

::::::::::::::::::::::::::::::::::::::::::::::::::



## Profiling your MARC data

The MarcEditor provides multiple reporting options and tools to help you profile your MARC data and understand the contents of your file. Reports are located under the Reports tab.

### Overview reports

The `Material Type Report` can be used to identify the types of resources described in your MARC file. This report is helpful when you're uncertain of what resources are represented in your file, or to locate potential errors.

:::::::::::::::::::::::::::::::::::::: instructor

Note: The type of material is generated by the LEADER or LDR field position 6 (type of record), position 7 (bibliographic level), and 008 position 23 or 29 depending on the type of record.
  
:::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::  checklist

## Run Material Type Report

To run the Material Type Report

1. Click Reports
2. Select Material Type Report
3. Click Generate Report


::::::::::::::::::::::::::::::::::::::::::::::::::

If we expect our MARC file to contain only book records, we can easily locate and review records with other material types by using the `Find Records by Type` Report.

:::::::::::::::::::::::::::::::::::::::  checklist

## Run Find Records by Type Report

To run the Find Records by Type Reports

1. Click Reports
2. Select Material Type Report
3. Select material type of records you want to review from the drop-down list. For this exercise select Continuing Resources.
  A window will open displaying the Leader of each record. Double click on a result to be brought to that record in the MarcEditor.
4. Click Close to exit the results window


::::::::::::::::::::::::::::::::::::::::::::::::::

The `Field Count` Report can also be used to profile your data. The Field Count Report lists each field found in your records, the number of times each field occurs in the record set, and the total number of records each field occurs in. While high level, the results can tell you about the cataloguing standards used (260 vs. 264) and identify potential errors (repeating non-repeatable fields), missing fields, local fields, etc.

:::::::::::::::::::::::::::::::::::::::  checklist

## Run Field Count Report

To run the Field Count Reports

1. Click Reports
2. Select Field Count


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::  challenge

## Locate errors using the Field Count Report

1. What do the field count results tell us about our records?
2. Looking at fields 100-300 do any of the results indicate errors in our records?

:::::::::::::::  solution

## Solution

1. Field count outlines each field found in our records, the number of times it occurs, and how many records it occurs in. Field count can also tell us the number of records in our file (536).
2. Non-repeatable field 245 occurs more times than the number of records it's found in. At least one record contains multiple 245 fields. Field 245 appears in one less record than other required fields.
  
  

:::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

### Edit functions

Other useful tools for profiling your data can be found under the Edit tab.

Like many applications, the MarcEditor provides a `Find` function. Find is particularly useful for locating and reviewing all instances of a MARC field within your data, or locating a particular text string within your data.

We can use Find to locate and review the 245 field. 

:::::::::::::::::::::::::::::::::::::::  checklist

## Run Find Function

To use the Find function

1. Click Edit
2. Select Find (*Ctrl+f will also launch the `Find` function)
3. In the "Find what:" dialogue box enter =245
4. Click Find All

**Note:**  When using `Find` to locate instances of a specific field, make sure to include the preceding = before the field number. Including the = ensures only matches on field number will be returned.


::::::::::::::::::::::::::::::::::::::::::::::::::

The Find results list is organized by record number, displaying the matched field content on the left, and the record number the field belongs to on the right. We can see from our results that Record # 8 appears twice, signaling that this record contains two 245 fields.  By double clicking on  "Jump to record #: 8" we could go directly to the record in our file to edit it. However, next we will show you a set of tools that can be used to locate and fix common errors like duplicate fields.

The `Find Records With Duplicate Tags` function allows us to easily locate records with a duplicated field. 

:::::::::::::::::::::::::::::::::::::::  checklist

## Run Find Records With Duplicate Tags Function

1. Click Edit
2. Select Edit Shortcuts
3. Select Field Edits
4. Click Find Records With Duplicate Tags
5. In the dialogue box enter 245 and click OK

The results list includes two records with duplicate 245 fields, # 8 and # 28. Click on Jump to Record # to be taken to the record in the MarcEditor. Once on the record you can manually delete the incorrect 245 field.


::::::::::::::::::::::::::::::::::::::::::::::::::

The `Find Records Missing Field` function allows us to easily locate records with a missing field. To run this function

:::::::::::::::::::::::::::::::::::::::  checklist

## Run Find Records Missing Field Function
1. Click Edit
2. Select Edit Shortcuts
3. Select Field Edits
4. Click Find Records Missing Field
5. In the dialogue box enter 245 and click OK

The results list will show one record missing a 245 field. Click on Jump to Record # to be taken to the record in the MarcEditor.


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::  challenge

## Correct the missing 245 field

1. What's the issue with this record? Is the 245 formatted correctly?

:::::::::::::::  solution

## Solution

1. The 245 field number is formatted incorrectly. The MarcEditor relies on a standard format to identify and take actions on fields. Remove the rogue space and update the field number to correct this record.
  
  

:::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

## Validation and Log Reports

- Validate ISBNs: When you select this report, a popup window will appear. Enter the MARC field where the ISBNs are. The report will see if these are correct. For example, if an ISBN is followed by text such ebook without a space, then the report will highlight this. However, if there is a space between the ISBN and any text, this is considered valid as in this example, 9780190856939 (ebook). You will need to close the popup windows.
- Validate ISSNs: When you select this report, a popup window will appear. Enter the MARC field where the ISSNs are. The behavior is similar to the ISBN report. The report will provide a result of errors or a message that no invalid ISSNs were found.
- Validate Headings: Unlike in Connexion or OCLC's WorldShare, validating headings does not create hyperlinks. This report will compare headings to several online services. These online services are listed in the Service Status when you click on Validate Headings and select Service Status. Results will appear in a popup window. 
- Manage log files: There is no version control such as Git in MarcEdit. However, if you click on Manage Log Files -> View Current Log, you will see the entire list of actions that you have done on your file.

## MarcValidator Report
The MarcValidator report has a couple of options of which 2 are highlighted here. Note that if you are working with a large file, it will take longer to prep the file. Once it is prepped, there is a message that says "MarcEditor file has been prepped and is awaiting validation". You can view results grouped by errors or remove invalid records automatically from your file.

- Check MARC Usings Rules File: The Rules file, called marcrules.txt, includes all the valid MARC fields, their valid indicators, and whether that field can be repeated. The Rules file can be modified. Once you open the MarcValidator, in the popup window, you will see the option to "Edit the Rules File". You will need to respect spaces and entry conventions by following what is already present in that text file.
- Validate Record Structure: This report checks if the MARC syntax is valid and includes a check for HTML, tabs, and smart characters.

:::::::::::::::::::::::::::::::::::::::: keypoints

- MarcEditor provides many different tools and reports to profile and edit your MARC records

::::::::::::::::::::::::::::::::::::::::::::::::::


