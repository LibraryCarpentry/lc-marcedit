---
title: "Working with MARC files"
teaching: 20
exercises: 1
questions:
- "What is a MARC binary file?"
- "What does it mean to break and make a MARC file and how do I open a file of MARC records in MARCedit?"
- "Why is encoding important?"

objectives:
- "Explain the difference between mrc and mrk MARC file formats"
- "Successfully break and open a file of MARC records"
- "Explain encoding and its importance"

keypoints:
- "MarcEdit can work with a variety of file formats"
- "MARC ToolsIcon allow you to convert data from one file format to another"
- "The MarcEditor works with a MarcEdit specific mnemonic format of MARC records (.mrk)"
- "It is necessary to break a MARC binary file to work with that MARC data in the MarcEditor. The extension of these easily readable MARC files are .mrk rather than the binary extension of .mrc"
---


>## Working with MARC files
>MarcEdit recognizes the following MARC file types:
>
><table>
>  <tr>
>   <td><strong>File type</strong>
>   </td>
>   <td><strong>File extension</strong>
>   </td>
>   <td><strong>Usage</strong>
>   </td>
>  </tr>
>  <tr>
>   <td>Binary MARC file
>   </td>
>   <td>mrc
>   </td>
>   <td>File format typically used in an  ILS or LSP. Other file extensions provided by vendors (ex. marc, dat, bin) are equivalent. Binary is format consisting of a series of sequential bytes, each of which is eight bits in length.
>   </td>
>  </tr>
>  <tr>
>   <td>Mnemonic MARC Text File
>   </td>
>   <td>mrk
>   </td>
>   <td>File format used by MarcEdit that is a human readable version of the binary file.
>   </td>
>  </tr>
>  <tr>
>   <td>MARC UTF-8 Text File
>   </td>
>   <td>mrk8
>   </td>
>   <td>Legacy file format for MARC mnemonic files saved with UTF8 encoding.
>   </td>
>  </tr>
>  <tr>
>   <td>MARCXML file
>   </td>
>   <td>xml
>   </td>
>   <td>A MARC file expressed in the eXtensible Markup format or a text-based format for representing structured information.
>   </td>
>  </tr>
>  ></table>
>To work with a MARC file in the MARCEditor your file needs to be in MARC mnemonic format. If you only have a binary file, then that file needs to be converted to the mnemonic format.
{: .callout}

>## MARC Tools
>MarcEdit’s MARC Tools allows you to convert between different data formats recognized by MarcEdit.  To transform our binary MARC file into MARC mnemonic human readable format, you use the MarcBreaker.
>
>### Break a MARC (.mrc) file to use in the MarcEditor
>
>1. Launch MarcEdit and from the main window click on the ToolsIcon.
>2. In the MARC Tools window, Select Operation -> MARCBreaker.
>3. In the field, Select Data to Process, click the file folder image to the right of the Open box to browse for the sample MARC data file (.mrc). Double click the found file to select it.
>4. Next, you will need save your file in the MARC mnemonic format by clicking the file folder to the right of the Save As box. Select the location and name you would like to give you new file.
>5. Under Character encoding select UTF8 as default character encoding.
>6. Click execute.
>7. Once you click execute the newly created .mrk file will available to open in the MarcEditor. Under Results at the bottom of the window you will see a count of the records in your file. Click Edit Records to open the .mrk file in the MarcEditor.
>
{: .checklist}

>## Character Encoding
>To ensure the integrity of your data you need to select the correct character encoding for your dataset. MarcEdit does not automatically detect character encoding, however, UTF8 is set as the default encoding scheme. You can update the encoding scheme when using the MarcBreaker, or you can update the default in Preferences → MarEditor → Default Encoding. For more information on character encoding and translating from one encoding to another, see [The MarcEdit Field Guide](https://marcedit.reeset.net/learning_marcedit/9-2/dealing-with-character-encodings-in-marcedit/)
{: .callout}
