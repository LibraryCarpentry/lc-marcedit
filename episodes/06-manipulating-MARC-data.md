---
title: "Manipulating MARC data"
teaching: 20
exercises: 5
questions:
- "How can MARC data be manipulated?"
- "How can fields, subfields, and/or indicators be added, changed, or removed?"
- "How can the RDA Helper be used?"
- "How can fixed fields be manipulated?"
- "How can Select Records for Edit be used to manipulate a subset of your MARC file?"
- "What is the difference between save and compile?"
objectives:
- "Explain how to add, update, and remove fields, subfields, indicators, and fixed fields"
- "Explain the functions RDA Helper and Select Records for Edit"
- "Explain the difference between save and compile"
- "Successfully manipulate MARC data"
- "Successfully save your MARC data"
- "Successfully compile your MARC data"
keypoints:
- "MarcEdit can be used to edit any part of the MARC data including the Leader, fixed fields, fields, indicators, subfields and the content in those fields."
- "MarcEdit comes with an array of tools to manipulate data and validate MARC."
---

## Manipulating MARC data
MarcEdit provides a number of ways to manipulate MARC data. Fields, subfields, indicators can be added, removed, or changed. Fixed fields can be corrected. Fields and subfields specific to RDA can be added while AACR2 conventions are removed. It is possible to work with a subset of MARC data and then incorporate those changes into the original whole MARC data set. The variations sometime seem endless and give more weight to the nickname of MarcEdit, the swiss army knife of MARC data.

To manipulate MARC data, that MARC data needs to be open as .mrk in the MarcEditor. This is often referred to "breaking" a MARC file, and hence the feature of MarcBreaker to create a .mrk file from a .mrc one. In the MarcEditor, "Tools" in the menu is where you will find those functions to manipulate data.

### Add/Delete a MARC field
To add or delete a MARC field, go to Tools in the upper menu in the MarcEditor and scroll down to Add/Delete. This will open a new window. The Add/Delete functions are on the same menu level and you will need to select the action of either add or delete using the buttons on the right hand side.

In the top middle section of the window, there are two data entry fields: Field and Field Data. Enter the MARC field number in Field. Enter the indicators, subfields, and data in Field Data. Remember to include the dollar sign to indicate a subfield.
  <img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/addDeleteField.png" width="650">
  <img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/example_addDelete.png" width="650">

To add the field, click on the Add button and to delete, the Delete button.

There are a number of options for adding a MARC field to your data. If the field you are adding already exists, it can be inserted first in the list of those MARC fields or last. MARC fields can be added only if that MARC field is not present in that record or based on the presence of other criteria based on other MARC fields. For example, a MARC field 655  \4$aElectronic books can be added to only those records that are eBooks based on the data in the LDR or 008.

The options to delete a MARC field include removing duplicates, removing MARC fields based on field position, removing MARC fields that do not match what is entered in the Field Data, or removing invalid UTF-8 MARC fields. For example, to ensure that only the field 655  \4$aElectronic books. is present in the MARC data, the option to remove the MARC fields that don't match can be selected.

>## Add and then Delete a MARC field to your MARC data
>
>1. Add a 655 for electronic books with the indicators of blank and 4 to the MARC data.
>2. Delete that 655 that you just added.
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select Add/Delete Field (F7)
> > 3. Add 655 in the Field box and \4$aElectronic books. in the Field Data box
> > 4. Click on the Add button. You can also preview this change by clicking on the arrow on the right side and selecting Preview in the 7.5 version of MarcEdit
> > 5. Check your MARC data. Was this MARC field added?
> > 6. To delete this field, go back to Tools and select Add/Delete Field (F7)
> > 7. Enter 655 in the Field box
> > 8. In the Field Data box, you can enter \4$aElectronic books.
> > 9. Click on the Delete button. You can also preview this change by clicking on the arrow on the right side and selecting Preview in the 7.5 version of MarcEdit
> {: .solution}
{: .challenge}

>## Delete a range of MARC fields that begin with a number
>
>1. Make sure the file has multiple 9XX Marc fields. Add more to your file if necessary.
>2. Delete all variations of the MARC fields that begin with 9 or delete all 9XX MARC fields.
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select Add/Delete Field (F7)
> > 3. Add 9XX in the Field box
> > 4. Click on the Delete button. You can also preview this change by clicking on the arrow on the right side and selecting Preview in the 7.5 version of MarcEdit
> > 5. Check your MARC data. Were all 9XX fields removed?
> {: .solution}
{: .challenge}

### Add, Delete, or Change information for a subfield in a MARC field
To edit subfield data within a given field, go to Tools and select Edit Subfield data. A new window will open (notice that this is the same window that opened for Add/Delete a field, you can also navigate between the MarcEdit Batch Editing Tools using the labels on the left hand side of the window). From here you can add a new subfield, delete a subfield, or replace text in a subfield. How you do this is selecting one of the options below the data entry fields at the top of the window.

To add a subfield, enter the MARC field and then the subfield. The information or text that goes into that subfield goes into the box called Replace With. Select New Subfield from the options below and then click Replace Text. Even though you are adding a subfield, you still click replace text. For adding a subfield, the information that goes in that field doesn't go in the box called Field Data, see the example below.

To delete a subfield, enter the MARC field and then the subfield. Select Delete Subfield from the options below and then click Remove Text.

To replace text in a subfield, enter the MARC field, the subfield, the text (or information) that needs to be changed, and in the box Replace With the text that will replace what needs to be changed. Then click on Replace Text.

<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/editSubfield.png" width="650">
<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/example_Subfield.png" width="650">

> ## Ability to Preview and Special Undo
>
> In version 7.5, you can preview all of these changes before making the change.
> If you do make the change and see that those changes weren't what you expected, you can do a Special Undo.
> Go to Edit in the top level menu in the MarcEditor and select Special Undo.
> This will only on your most recent batch edit. If you perform an action after your batch change, that will not undo your batch change but the action you just performed.
>
{: .callout}

>## Add and then Delete a MARC subfield to a MARC field in your MARC data
>
>1. Change the $5 for the MARC field 500 from FU to your own Library of Congress Organization Code.
>2. Delete that $5 that you just changed.
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select Edit Subfield Data (F9)
> > 3. Add 500 in the Field box, 5 in the Subfield box, FU in the Field Data box, and your LC Organization Code in the Replace With box
> > 4. Click on the Replace Text button.
> > 5. Check your MARC data. Was FU changed to your LC Organization Code?
> > 6. To delete this subfield, go back to Tools and select Edit Subfield Data (F9)
> > 7. Enter 500 in the Field box, 5 in the Subfield box
> > 8. Click on the Remove Text button.
> {: .solution}
{: .challenge}

> ## Building a MARC field
>
> Sometimes it is necessary to create a MARC field based on other MARC fields.
> This is possible using the function called, Build New Field.
>  ![Build New Field Window](https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/buildNewField.png)
{: .callout}

### Change one or both indicators in a MARC field
Sometimes it is necessary to change one or both indicators of a MARC field in your MARC data. Go to Tools and select Edit Indicators. This will open a new window. Enter the MARC field, the indicators that you would like to change, and the indicators you want. Here you will want to be careful of the combinations of indicators. If you leave the box called Indicators blank and add indicators in the Replace With Indicators box, all the indicators for that MARC field will be changed to what you put in the Replace With Indicators box.

<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/editIndicators.png" width="650">
<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/example_editIndicators.png" width="650">

>## Change an indicator for a MARC field in your MARC data
>
>1. Change the first indicator of the MARC field 050 to 1 for those MARC fields 050 that have a first indicator blank and a second indicator 4.
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select Edit Indicators (F8)
> > 3. Add 050 in the Field box, \4 in the Indicators box, and 14 in the Replace With Indicators box. Leave the Field data box blank
> > 4. Click on the Replace button.
> > 5. Check your MARC data. Were the 050 \4 updated to be 050  14?
> {: .solution}
{: .challenge}

## RDA Helper
Records aren't created equal in that we encounter MARC data that follows different descriptive cataloging standards. There are a number of records cataloged according to the AACR2 standard or even AACR1. Sometimes it is necessary to make sure these records follow the current RDA descriptive cataloging standard. MarcEdit lets you do this through the function called RDA Helper.

Go to Tools and Select RDA Helper. In the window that opens, you can pick and choose how you would like to transform your records to align better with the RDA descriptive standard. For example, you can add the RDA fields 336, 337, and 338 for content, media, and carrier terms. You can update the MARC field 040 to include the subfield e with rda and delete the GMD statement. You can also evaluate the 260/264.

<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/rdaHelper.png" width="650">

>## Run the RDA Helper on your MARC data
>
>1. Run the RDA Helper with these settings: Add 336, 337, 338; Modify the 040; Evaluate the 260/264; Always use the copyright symbol; Expand abbreviations; Remove the GMD.
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select RDA Helper
> > 3. Check off the settings listed above
> > 4. Click the OK button.
> > 5. Check your MARC data. Do you see the changes?
> {: .solution}
{: .challenge}

## Working with MARC fixed fields
Working with fixed fields can be difficult. In the MarcEditor, you can edit one fixed field using the easy editing window. If you put your cursor on that fixed field, such as an 008 or 006, then go to Edit and select Insert/Edit 006 or Insert/Edit 008. This will open up a window where you can edit the fixed field for that specific MARC record.

You can also batch insert an 006 or 008 into your records. Go to Edit and select the appropriate Insert/Edit.

<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/fixedFields.png" width="650">

> ## Batch Editing Fixed Fields in Multiple MARC Records
>
> Sometimes it is necessary to change a fixed field for all records in your MARC data.
> This is possible using the Replace function and regular expressions which will be covered in Lesson 09.
{: .callout}

## Select Records to Edit
There are times when you need to work on a subset of your MARC data. The Select Records for Edit allows you do this.

Go to File, Select the Select Records for Edit. In the window, you will see Display field in the lower right hand corner. This is where you enter the MARC field you want to see displayed once you Import your file. You can enter a MARC field and subfield or just a MARC field. The MARC field and/or subfield that you add in this box will provide the criteria you need to select records you want to edit. Once you have entered the Display field, click on Import File. This will import the MARC (.mrk) file that you are currently working on. You can select another MARC (.mrk) file in the box Source MARC file.

<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/selectRecordsForEdit.png" width="650">
<img src="https://github.com/LibraryCarpentry/lc-marcedit/blob/gh-pages/assets/img/example_selectRecordsForEdit.png" width="650">

## Save and Compile
The MARC data that you manipulate in the MarcEditor is a friendly view that was broken from the binary .mrc file. You will notice that the extension of your file that you are manipulating in the MarcEditor has the file extention of .mrk. If you look at the file in your file directory, sometimes the color is also blue whereas the .mrc or binary MARC file is a sort of purple.

When you save or save as in the MarcEditor, you are saving your latest changes as a .mrk or in the friendly view that was broken from the binary .mrc file.

When you compile, you are saving all of your latest changes and reforming that record into its binary .mrc format that can be used to load the records in external systems such as your ILS or LSP.
