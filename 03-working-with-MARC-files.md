---
title: Working with MARC files
teaching: 17
exercises: 2
---

::::::::::::::::::::::::::::::::::::::: objectives

- Explain the difference between mrc and mrk MARC file formats
- Successfully break and open a file of MARC records in the MarcEditor
- Explain character encoding and its importance
- Understand how to read a MARC record in the MarcEditor

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What is a MARC binary file?
- What does it mean to break and make a MARC file and how do I open a file of MARC records in MARCedit?
- Why is encoding important?
- How does the MarcEditor display MARC records?

::::::::::::::::::::::::::::::::::::::::::::::::::
## Understanding MARC 21 in MarcEdit
:::::::::::::::::::::::::::::::::::::::::  callout
### MARC file types
MarcEdit recognizes the following MARC file types:

<table>
 <tr>
  <td><strong>File type</strong>
  </td>
  <td><strong>File extension</strong>
  </td>
  <td><strong>Usage</strong>
  </td>
 </tr>
 <tr>
  <td>Binary MARC file
  </td>
  <td>mrc
  </td>
  <td>File format typically used in an ILS or LSP. Other file extensions provided by vendors (ex. marc, dat, bin) are equivalent. Binary is a format consisting of a series of sequential bytes, each of which is eight bits in length.
  </td>
 </tr>
 <tr>
  <td>Mnemonic MARC Text File
  </td>
  <td>mrk
  </td>
  <td>File format used by MarcEdit that is a human readable version of the binary file.
  </td>
 </tr>
  <tr>
  <td>OCLC DAT binary file
  </td>
  <td>dat
  </td>
  <td>File format used by OCLC, especially on export to a local computer. The export .dat file is a binary MARC21 UTF-8 file.
  </td>
 </tr>
 <tr>
  <td>MARC UTF-8 Text File
  </td>
  <td>mrk8
  </td>
  <td>Legacy file format for MARC mnemonic files saved with UTF8 encoding.
  </td>
 </tr>
 <tr>
  <td>MARCXML file
  </td>
  <td>xml
  </td>
  <td>A MARC file expressed in the eXtensible Markup format or a text-based format for representing structured information.
  </td>
 </tr>
 </table>
To work with a MARC file in the MARCEditor your file needs to be in MARC mnemonic format. If you only have a binary file, then that file needs to be converted to the mnemonic format.

::::::::::::::::::::::::::::::::::::::::::::::::::

### MARC Tools

To work with MARC data files or convert between metadata formats for library bibliographic data recognized by MarcEdit, click on the MARC Tools icon that has the crossed hammer and spanner in the upper left hand corner of the main menu. The available features are:

- MarcBreaker: This "breaks" the MARC binary file into a readable (mnemonic) format that can be edited in the MarcEditor.
- MarcMaker: This takes the readable (mnemonic) format MARC data file and creates the MARC binary file.
- MARC21 to MARC21XML: This converts a MARC21 file to MARC21XML.
- MARC21XML to MARC21: This converts a MARC21XML file to a MARC21 binary file.
- MARC to JSON: This converts a MARC21 file to a JSON file.
- JSON to MARC: This converts a JSON file to a MARC21 file.
- JSON to XML: This converts a JSON file to XML.
- XML to JSON: This converts an XML file to JSON.

The conversions from one encoding standard to another, as in MARC21 to MARC21XML, rely on eXtensible stylesheets. MarcEdit comes with several default stylesheets which come from those maintained by the Library of Congress. If you are familiar with stylesheets, you can also create your own.

:::::::::::::::::::::::::::::::::::::::::  callout

### Character Encoding

To ensure the integrity of your data you need to select the correct character encoding for your dataset. MarcEdit does not automatically detect character encoding, however, UTF8 is set as the default encoding scheme. You can update the encoding scheme when using the MarcBreaker, or you can update the default in Preferences → MarEditor → Default Encoding. For more information on character encoding and translating from one encoding to another, see [The MarcEdit Field Guide](https://marcedit.reeset.net/learning_marcedit/9-2/dealing-with-character-encodings-in-marcedit/)


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::  checklist

### Break a MARC Binary File

To transform our binary MARC file (.mrc) into MARC mnemonic human readable format (.mrk), you use the MarcBreaker.

#### Break a MARC (.mrc) file to use in the MarcEditor

1. Launch MarcEdit and from the main window click on the MARC Tools Icon.
2. In the MARC Tools window, Select Operation → MARCBreaker.
3. In the field, Select Data to Process, click the file folder image to the right of the Open box to browse for the sample MARC data file (.mrc). Double click the found file to select it.
4. Next, you will need save your file in the MARC mnemonic format (.mrk) by clicking the file folder to the right of the Save As box. Select the location and name you would like to give your new file.
5. Under Character encoding select UTF8 as default character encoding.
6. Click execute.
7. Once you click execute the newly created .mrk file will be available to open in the MarcEditor. Under Results at the bottom of the window you will see a count of the records in your file. Click Edit Records to open the .mrk file in the MarcEditor.

**Note:** When you break a .mrc file and create a new .mrk file for editing in the MarcEditor, you are making a copy of your data in a new file format. As a result, any edits you make to the .mrk file in the MarcEditor will not automatically be reflected in the original .mrc file. We will cover saving and compiling (using the MarcMaker) to create an updated .mrc file in an upcoming lesson.

::::::::::::::::::::::::::::::::::::::::::::::::::

### MARC Record layout in the MarcEditor
You should now see the MARC records from the file displaying in the MarcEditor:

![](fig/marc_sample_data.png){alt='MarcEditor screen with file open'}

The MarcEditor displays the records in what is called the 'Mnemonic MARC Text File' format (file extension \*.mrk). Each line in the file represents a field in a MARC record:

```
=245  14$aThe Lord of the Rings /$c J.R.R. Tolkien.
```

This example breaks down as follows:

<table>
  <tr>   <td><code>=</code>   </td>   <td>Each line/field starts with the '=' sign.
   </td>
  </tr>
  <tr>   <td><code>245</code>   </td>   <td>The '=' is followed immediately by the three character MARC field code.
   </td>
  </tr>
  <tr>   <td><code>[two spaces]</code>   </td>   <td>The MARC field is always followed by two spaces.
   </td>
  </tr>
  <tr>   <td><code>14</code>   </td>   <td>The field indicators follow the spaces if the field has indicators. When an indicator is not coded a <code>\\</code> is used. For the control or fixed fields where no indicators are used, the field content starts directly after the spaces.
   </td>
  </tr>
  <tr>   <td><code>\$aThe Lord of the Rings /\$c J.R.R. Tolkien.</code>   </td>   <td>The field content contains the subfields (indicated using the <code>\$</code> symbol) and the text. Because the subfields use the <code>\$</code> symbol, any real occurrences of the dollar symbol (e.g. for currency) is shown as <code>[dollar]</code> instead. Unlike in some cataloguing applications, there are no spaces between subfield codes and the subfield text.
   </td>
  </tr>
</table>

Records in the MarcEditor display are separated by a blank line.

:::::::::::::::::::::::::::::::::::::::::  callout

### MARC syntax in the MarcEditor

Understanding the layout of MARC data in the MarcEditor is key to using the program's tools successfully. For instance, in some tools it is important to specify a field's indicators directly preceeding the first subfield. Throughout this workshop we will highlight how different tools rely on this syntax to apply edits. 


::::::::::::::::::::::::::::::::::::::::::::::::::

The MarcEditor divides a file of MARC records into 'pages' of 100 records. You can scroll up and down the page of MARC records using the scroll bar as usual, but to see the next 100 records you need to use the Next/Previous page controls which are at the bottom left of the screen. The MarcEditor can handle very large files of MARC records, because it never tries to load all the records at the same time.

### Setting MarcEditor Preferences

You can adjust the number of records displayed per 'page' through the MarcEditor preferences which can be accessed through the Edit → Preferences menu option from the MarcEditor, or through the 'Settings' icon on the opening screen of MarcEdit.

Within the MarcEditor preferences, you can adjust the font and font size within the MarcEditor. You can also set your character encoding defaults. If you navigate to File Associations within the Preferences window, you can select Associate (`*.mrc`) files with the MarcBreaker and Associate (`*.mrk`) files with the MarcEditor. Setting these file associations will make it easy to break `.mrc` files and edit `.mrk` files.

If you change your preferences for the MarcEditor, the tool used to work with MARC data, you can always go back to the default settings.

:::::::::::::::::::::::::::::::::::::::  checklist

### Reset settings for the MarcEditor in Preferences

1. Click Edit → Preferences
2. Select "MarcEditor" in the Preferences window in the left-hand pane
3. In the right-hand pane, under Set MarcEditor Font Properties, select Set Defaults
4. Click Ok
  

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::  callout

### Behavior when you reset your preferences and other popup windows

When you click Ok to reset preferences, there is a chance that the popup window for Preferences and/or even MarcEdit main menu will close. If the MarcEdit main menu closes, sometimes it will reopen. If it does not, then click on MarcEdit again on your desktop to reopen the application. 

It should be noted that not all MarcEdit popup windows will close automatically such as Find, Replace, or the MarcValidator. However, the Select Records for Edit temporary editor will close if you click Save. These idiosyncracies for each will be covered in their upcoming episodes.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::: instructor

Note: Some preference updates will force MarcEdit to restart and others will not. Also note that in order for some preference changes to display (such as updating the MarcEditor font settings), you will need to close and reopen the MarcEditor, which would require saving your file if you haven't done so. Emphasize popup window inconsistencies for learners, especially the need to close windows after use for actions such as Find and Replace. If learners do not close popup windows as they move through exercises, they are more likely to lose their place or get confused.

:::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: keypoints

- MarcEdit can work with a variety of file formats
- The MARC Tools Icon allow you to convert data from one file format to another
- The MarcEditor works with a MarcEdit specific mnemonic format of MARC records (.mrk)
- It is necessary to break a MARC binary file to work with that MARC data in the MarcEditor. The extension of these easily readable MARC files are .mrk rather than the binary extension of .mrc
- Understanding the layout (syntax) of MARC records in the MarcEditor is key to working with the records.

::::::::::::::::::::::::::::::::::::::::::::::::::


