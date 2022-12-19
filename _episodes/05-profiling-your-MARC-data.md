---
title: "Profiling Your MARC data"
teaching: 10
exercises: 5
questions:
- "How do I use different reports to get an overview of my MARC file?"
- "How do I locate errors in my records?"
- "How do I use the Edit Shortcuts tool to identify and fix common errors?"

objectives:
- "Access reports for getting an overview of your MARC data"
- "Find tools to locate errors in your MARC records by using the MARCedit Edit toolbar"

keypoints:
- "MarcEditor provides many different tools and reports to profile and edit your MARC records"
---

{% include links.md %}


## Profiling your MARC data
The MarcEditor provides multiple reporting options and tools to help you profile your MARC data and understand the contents of your file. Reports are located under the Reports tab.

### Overview reports
The `Material Type Report` can be used to identify the types of resources described in your MARC file. This report is helpful when you're uncertain of what resources are represented in your file, or to locate potential errors.

To run the Material Type Report
* Click Reports
* Select Material Type Report
* Click Generate Report

If we expect our MARC file to contain only book records, we can easily locate and review records with other material types by using the `Find Records by Type` Report.

To run the Find Records by Type Reports
* Click Reports
* Select Material Type Report
* Select material type of records you want to review from the drop-down list. For this exercise select Continuing Resources.
A window will open displaying the Leader of each record. Double click on a result to be brought to that record in the MarcEditor.
* Click Close to exit the results window

The `Field Count` Report can also be used to profile your data. The Field Count Report lists each field found in your records, the number of times each field occurs in the record set, and the total number of records each field occurs in. While high level, the results can tell you about the cataloguing standards used (260 vs. 264) and identify potential errors (repeating non-repeatable fields), missing fields, local fields, etc.

To run the Field Count Reports
* Click Reports
* Select Field Count

> ## Locate errors using the Field Count Report
>
> 1. What do the field count results tell us about our records?
> 2. Looking at fields 100-300 do any of the results indicate errors in our records?
>
> > ## Solution
> > 1. Field count outlines each field found in our records, the number of times it occurs, and how many records it occurs in. Field count can also tell us the number of records in our file (536).
> > 2. Non-repeatable field 245 occurs more times than the number of records it's found in. At least one record contains multiple 245 fields. Field 245 appears in one less record than other required fields.
> {: .solution}
{: .challenge}

### Edit functions
Other useful tools for profiling your data can be found under the Edit tab.

Like many applications, the MarcEditor provides a `Find` function. Find is particularly useful for locating and reviewing all instances of a MARC field within your data, or locating a particular text string within your data.

We can use Find to locate and review the 245 field. To run the Find Report
* Click Edit
* Select Find
* In the "Find what:" dialogue box enter =245
* Click Find All

The results list is organized by record number, displaying the matched field content on the left, and the record number the field belongs to on the right. We can see from our results that Record # 8 appears twice, signaling that this record contains two 245 fields.  By double clicking on  "Jump to record #: 8" we could go directly to the record in our file to edit it. However, next we will show you a set of tools that can be used to locate and fix common errors like duplicate fields.

The `Find Records With Duplicate Tags` function allows us to easily locate records with a duplicated field. To run this function
* Click Edit
* Select Edit Shortcuts
* Select Field Edits
* Click Find Records With Duplicate Tags
* In the dialogue box enter 245 and click OK
The results list includes two records with duplicate 245 fields, # 8 and # 28. Click on Jump to Record # to be taken to the record in the MarcEditor. Once on the record you can manually delete the incorrect 245 field.

The `Find Records Missing Field` function allows us to easily locate records with a missing field. To run this function
* Click Edit
* Select Edit Shortcuts
* Select Field Edits
* Click Find Records Missing Field
* In the dialogue box enter 245 and click OK
The results list will show one record missing a 245 field. Click on Jump to Record # to be taken to the record in the MarcEditor.

> ## Correct the missing 245 field
>
> 1. What’s the issue with this record? Is the 245 formatted correctly?
>
> > ## Solution
> > 1. The 245 field number is formatted incorrectly. The MarcEditor relies on a standard format to identify and take actions on fields. Remove the rouge space and update the field number to correct this record.
> {: .solution}
{: .challenge}
