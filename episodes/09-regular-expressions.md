---
title: "Regular Expressions"
teaching: 15
exercises: 20
questions:
- "What are regular expressions?"
- "Where and how can you use regular expressions in the MarcEditor?"
- "What types of edits can you accomplish with regular expressions?"
objectives:
- "Understand what regular expressions are and how they can support advanced editing in the MarcEditor"


keypoints:
- "Regular expressions are a powerful tool for selecting and editing your data in the MarcEditor"
- "Regular expressions can be used in many functions and tools in MarcEdit and the MarcEditor"
- "Knowing your data is essential to ensuring your regular expressions are working as intended"
---
{% include links.md %}


# Regular Expressions
Regular expressions, often referred to as regex, are a tool you can use to match, capture and manipulate data across your MARC record file. Regular expressions are comprised of a sequence of literal characters and metacharacters which are formulated to match a particular pattern found in your data that you want to manipulate. A detailed introduction to working with regular expressions can be found in the [Library Carpentry lesson Introduction to Working with Data (Regular Expressions)](https://librarycarpentry.org/lc-data-intro/index.html). In this lesson we will focus on the application of regex in the MarcEditor.

## Regular Expressions in MarcEdit
MarcEdit uses the .NET regular expression syntax. Visit the .Net [Regular Expression Language - Quick Reference](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference) for a breakdown of the syntax used for regex metacharacters in MarcEdit. You can also download the [.Net Regex metacharacter reference sheet](https://download.microsoft.com/download/D/2/4/D240EBF6-A9BA-4E4F-A63F-AEB6DA0B921C/Regular%20expressions%20quick%20reference.pdf) to support the creation of your own regular expressions in MarcEdit.

Many MarcEdit functions support the use of regular expressions for data selection and manipulation. They include: Find and Replace, Edit Field, Copy Field, Swap Field, Build New Field, Delete Field, Record Validation, and both the Extract and Delete Selected Records tool. The intent of this lesson is to demonstrate where and how you can leverage regular expressions to work with your MARC data.

## Edit Field Data


With regular expressions you can easily locate variations in your data and replace them with a single value. In our file the OCLC identifier in the 035 field uses the prefixes on, ocn, and ocm, but our library formats the OCLC with the (OCoLC) prefix. Instead of running three Edit Field Data functions to update these prefixes we can use a regular expression in the Edit Field Data tool to replace these prefixes with the (OCoLC) prefix in a single edit.

>## Update 035 OCLC prefixes
>1. Select Tools --> Edit Field Data
>2. Enter the following values:
>Field: 035    Find: on|ocn|ocm    Replace: (OCoLC)
>3. Check Use Regular Expressions box
>4. Click drop down menu --> Preview Results
>5. Verify your results look as expected, close preview tab and then click Process
>
>In this regular expression we use the pipe (|) metacharacter to specify that we are looking for the string on OR ocn OR ocm. We then replace the captured string with (OCoLC).
{: .checklist}

>## Knowing your dataset
>Regular expressions are a powerful tool, but using them can sometimes lead to unexpected and undesirable results if you do not know your dataset. In the Edit Field Data exercise above, any 035 field containing the string on, ocn, or ocm would have had these values replaced with (OCoLC).
>For example: =035  //$a(SFUonline)638023 would have become =035  //$a(SFU(OCoLC)line)638023
>Reviewing your dataset before employing regular expressions is a good best practice. The MarcEditor Preview Results feature also supports trial and error.
{: .callout}


## Find and Replace

The Find and Replace tool is another useful way to identify and manipulate data in the MarcEditor with the support of regular expressions. In our file the local call numbers in the 090 field are formatted without a space between the class and subclass (ex. LD1780 and not LD 1780). To update the call number to follow our local policy we need to isolate the components of the call number so we can add a space between them. We can do this with a regular expression by employing groups.

>## Add a space between 090 class and subclass
>1. Select Edit --> Find
>2. Enter =090 in the Find box and click Find All
>Review the list of 090 fields, what observations can you make about the call numbers in this field?
>Review shows us that not all call numbers begin with letters. We do not want to add a space to these call numbers and need to account for this in our regular expression.
>3. In the Find window, click Replace to bring up the Replace Text functions
>4. In the Find box enter the regular expression (=090  \\\\\$a[A-Z]+)(\d.*)
>This regular expression uses two sets of () to capture groups and then manipulate them.
>- Broken down, the first group (=090  \\\\\$a[A-Z]+) will match the literal string "=090  \\$a" (the additional backslashes are used to escape the regex metacharacters \ and $ so that they will be read as literals) followed by any single capital letter in the range A to Z ([A-Z]) one or more times (+). By specifying that the regular expression must locate a capital letter at the start of the call number, the regular expression will not edit the call numbers that begin with a digit.
>- The second group (\d.*) will match any digit (/d) followed by any character (.) zero or more times (*)
>5. In the Replace box enter $1 $2
>This regular expression refers back to the groups we defined and captured in the Find box. $1 refers to the group defined in the first set of brackets, and $2 refers to the group defined in the second set of brackets. If we had defined additional groups they would be referred to chronologically as $3, $4 etc. The regular expression $1 $2 will output the contents of the two captured groups with a space between them.
>6. Check the Use regular expressions box
>7. Click drop down menu --> Preview Results
>8. Verify your results look as expected, close preview tab and then click Process
{: .checklist}
