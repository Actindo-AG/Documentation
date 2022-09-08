# CSV export definition

*Accounting > Extras > Tab CSV FORMAT DEF.*

![CSV format definition](../../Assets/Screenshots/RetailSuiteAccounting/Extras/CSVFormatDef/CSVFormatDef.png "[CSV format definition]")


**Name**

- (Drop-down list)  
Click the drop-down list to select a preconfigured import/export definition type. If there are any available, the second drop-down list displays the preconfigured definitions of the selected type.

[comment]: <> (Bedeutung von Asterisk neben Namen?)

- (Drop-down list)  
Click the drop-down list to select the desired preconfigured import/export definition.

- [ADD]  
Click this button to create an import/export definition. The *New import/export definition* window is displayed, see [New import/export definition](#new-importexport-definition).

- [EDIT]  
Click this button to rename an import/export definition. The *Rename import/export definition* is displayed, see [Rename import/export definition](#rename-importexport-definition).

- [DELETE]  
Click this button to delete an import/export definition. A confirmation window is displayed.


**Fields in the definition**  
This list displays all fields contained in the selected import/export definition. Use the arrow buttons to modify the fields in the list:

  - ![Up](../../Assets/Icons/ArrowUp.png "[Up]") (Up)  
  Use this button to move a selected field up in the list.

  - ![Down](../../Assets/Icons/ArrowDown.png "[Down]") (Down)  
  Use this button to move a selected field down in the list.

  - ![Left](../../Assets/Icons/ArrowLeft.png "[Left]") (Left)  
  Use this button to move a selected field left, from the *Possible fields* list to the *Fields in the definition* list.

  - ![Right](../../Assets/Icons/ArrowRight.png "[Right]") (Right)  
  Use this button to move a selected field right, from the *Fields in the definition* list to the *Possible fields* list.

**Column**  
The letter and number in brackets indicate the column where a selected field is placed.

**Possible fields**  
This list displays all fields available for the selected import/export definition.


[INSERT IGNORE FIELD]  
Click this button to add an "ignore field" command, that is, to indicate that the field in that position does not need to be exported or imported, in the *Fields in the definition* list.

**CSV format definition**

- *Field separating character*  
Enter the character to be used to separate fields. This value may be set up by default to comma or semicolon.

- *Escape character*  
Enter the character to be used in escape sequences, that is, combinations of characters used to represent non-printable and special characters, such as tabs or new lines. This value may be set up by default to backslash.

- *Column name*  
Click the drop-down list to select the appropriate option (**Yes/No**) to include or not the column name in the export/import.

- *Date format*  
Click the drop-down list to select the desired date and time format.

- *Example data set*  
An example of a data set with the current field definition is displayed. This field is read-only.

[comment]: <> (Unsure! Check!)

- *Field delimiting character*  
Enter the character to be used to separate fields. This value may be set up by default to quotation mark.

- *Row end character*  
Click the drop-down list to select the appropriate option, either **Automatic** or the applicable operating system.

- *Character set*  
Click the drop-down list to select the appropriate option, either **Automatic** or the applicable encoding.

- *Incorrect row end character*  
Click the drop-down list to select the appropriate option (**Ignore/Repair**).

- *Number format*  
Click the drop-down list to select the desired number format.

- [SAVE]  
Click this button to save the changes.


## New import/export definition  

*Accounting > Extras > Tab CSV FORMAT DEF. > Button Add*

![New import/export definition](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Import/NewImportExportDefinitionKdLf.png "[New import/export definition]")

- *For*  
Click the drop-down list to select the import/export definition type where the new definition will be added.  

- *Name*  
Enter a name for the new import/export definition to be created.

- [SAVE & NEW]  
Click this button to create a new import/export definition.  


## Rename import/export definition  

*Accounting > Extras > Tab CSV FORMAT DEF. > Button Edit*

![Rename import/export definition](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Import/RenameImportExportDefinitionKdLf.png "[Rename import/export definition]")

- *For*  
Click the drop-down list to select the import/export definition type where the new definition will be renamed.  

- *Old name*  
The previously given name is displayed. This field is read-only.

- *New name*  
Enter a new name for the selected import/export definition.

- [SAVE]  
Click this button to rename the selected import/export definition.
