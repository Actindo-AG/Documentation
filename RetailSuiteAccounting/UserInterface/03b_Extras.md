[!!Accounting](RetailSuiteAccounting)

# EXPORT

*Accounting > Select fiscal year > Extras > Tab EXPORT*

![Export](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Export.png "[Export]")

> [Info] The export function is also available in the *FISCAL YEARS* tab of the *Settings* menu entry, see [Export bookings](02d_Settings.md#export-bookings).


- *Export to*  
A list of the available export options is displayed:

  - *Export of data in BMD format*
  - *Export of data in CSV format*
  - *Export of data in DATEV CSV format*
  - *Export of data in GDI standard interface format*
  - *Export of data in GDPdU format*
  - *Export of open items*
  - *Export of balance lists in CSV format*
  - *Compeso SALDEN.DAT*
  - *Export bookings for SAP*
  - *Varial balances*
  - *Export of balance lists in CSV format (Zahlwerk)*


- [BMD]  
Click this button to export data in BMD format. Follow the instructions provided in the following windows, see [BMD](#bmd).

- [CSV]  
Click this button to export data in CSV format. Follow the instructions provided in the following windows, see [CSV](#csv).

- [DATEV CSV]  
Click this button to export data in DATEV compatible CSV format. Follow the instructions provided in the following windows, see [DATEV CSV](#datev-csv). For detailed information about exporting data in DATEV compatible CSV, see [Export the data for DATEV](/RetailSuiteAccounting/Operation/15_ProvideAccountingData.md#export-the-data-for-DATEV).

- [GDI]  
Click this button to export data in GDI format. Follow the instructions provided in the following windows, see [GDI](#gdi).

- [GDPDU EXPORT]  
Click this button to export data in GDPdU-compliant audit file format. Follow the instructions provided in the following windows, see [GDPDU export](#gdpdu-export). For detailed information about exporting data in GDPdU-compliant audit file format, see [Export the data GDPdU-compliant](/RetailSuiteAccounting/Operation/15_ProvideAccountingData.md#export-the-data-GDPdU-compliant).

- [OPEN ITEMS]  
Click this button to export open items. Follow the instructions provided in the following windows, see [Open items](#open-items).

- [BALANCE LISTS]  
Click this button to export balance lists in CSV format. Follow the instructions provided in the following windows, see [Balance lists](#balance-lists).

- [SALDEN.DAT]  
Click this button to export data in Compeso SALDEN.DAT proprietary format. Follow the instructions provided in the following windows, see [SALDEN.DAT](#salden-dat).

- [SAP]  
Click this button to export data in SAP compatible format. Follow the instructions provided in the following windows, see [SAP](#sap).

- [VARIAL]  
Click this button to export data in VARIAL compatible format. Follow the instructions provided in the following windows, see [Varial](#varial).

- [ZAHLWERK]  
Click this button to export balance lists in Zahlwerk compatible CSV format. Follow the instructions provided in the following windows, see [Zahlwerk](#zahlwerk).


## BMD

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button BMD*

![Export BMD Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportBMD01.png "[Export BMD Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Tax mapping*  
The tax mapping is preconfigured in the system but can be edited.

- [Edit]  
Click this button to edit the tax mapping. The *BMD tax mapping* window is displayed, see [BMD tax mapping].

- [CONTINUE]  
Click this button to proceed to the next step.


![Export BMD Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportBMD02.png "[Export BMD Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process.

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.

[comment]: <> (Nach einiger Sekunden bzw. kurz vor dem Step 3 ABBRECHEN Button ändert sich zu SCHLIESSEN, was nicht wirklich Sinn macht, denn man schließt tatsächlich das Fenster, also man bricht der Export ab.)



![Export BMD Step 3](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportBMD03.png "[Export BMD Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [WEITER]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## CSV

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button CSV*

![Export CSV Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV01.png "[Export CSV Step 1]")

![Export CSV Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV01cust.png "[Export CSV Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Selection*  
Click the applicable radio button to select the appropriate option:
  - ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Export all*
  - ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *All from last export on (if last export exists, otherwise all)*
  - *Set marker to export time*  
  Mark the checkbox if time is to be exported.

[comment]: <> (Unsicher, RS mit FH)

- *File content*  
Click the drop-down list to select the applicable file content. The following options are available:

  - **Customers/suppliers**
  - **Chart of accounts**
  - **Bookings**  


- *Export def.*  
Click the drop-down list to select the appropriate export definition. The export definitions are preconfigured in the system but they can be edited. The following options are available:
  - **Lexware Pro (customers)**
  - **Lexware Pro (suppliers)**


- [Edit]  
Click this button to edit the export definitions. The *Import/export definitions* is displayed, see [Import/export definitions](#importexport-definitions).

- *Export*  
Click the drop-down list to select the specific data to be exported. The following options are available:  

  - **Customer/suppliers**
  - **Customers only**
  - **Suppliers only**
  - **Custom**  
  When selecting this option, the following field is displayed:
	   - *Selection from - to*  
     Specify the account number range to be exported. You can enter the account numbers manually with the keyboard or use the increase/decrease arrows.


- [CONTINUE]  
Click this button to proceed to the next step.


![Export CSV Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV02.png "[Export CSV Step 2]")

**Step 2**


- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process.

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Export CSV Step 3](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV03.png "[Export CSV Step 3]")


**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [WEITER]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## DATEV CSV

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button DATEV CSV*

![Import DATEV CSV Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS01.png "[Import DATEV CSV Step 1]")

![Import DATEV CSV Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS01cust.png "[Import DATEV CSV Step 1]")

For detailed information about exporting data for DATEV, see [Export the data for DATEV](/RetailSuiteAccounting/Operation/15_ProvideAccountingData.md#export-the-data-for-datev).

**Step 1**


- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Selection*  
Click the applicable radio button to select the appropriate option:
  - ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Export all*
  - ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *All from last export on (if last export exists, otherwise all)*
  - *Set marker to export time*  
  Mark the checkbox if time is to be exported.


- *Impersonal accounts*  
Click the drop-down list to select the impersonal accounts to be exported. The following options are available:  

  - **Only individually changed**  
  - **All**  
  - **Custom**  
  When selecting this option, the *Custom (e.g. 1200, 1800-1850)* field is displayed.
  - **No**  

- *Custom (e.g. 1200, 1800-1850)*  
Enter an account number or an account number range to be exported.

- *Export subbookings*  
Click the drop-down list to select the appropriate option (**Yes/No**).

[comment]: <> (Check was Unterbuchungen sind)

- *Personal accounts*  
Click the drop-down list to select the impersonal accounts to be exported. The following options are available:  

  - **Yes**  
  - **Custom**  When selecting this option, the *Custom (e.g. 10000, 39999-49999)* field is displayed.
  - **No**  

- *Custom (e. g. 10000, 39999-49999)*    
Enter an account number or an account number range to be exported.

- *Export only booking-relevant master data records*  
 (**No/Yes**)

- *Take Receipt 2 field in the export document from booking record field*  

  - **Receipt 1**
  - **Receipt 2**
  - **Receipt 3**
  - **Receipt 4**


- *Add tax keys also in split bookings of automatic accounts*
(**No/Yes**)

- *Saved personal accounts length*  

- *DATEV advisor number*
- *DATEV client number*

- [CONTINUE]


![Import DATEV CSV Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS02.png "[Import DATEV CSV Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process.

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Import DATEV CSV Step 3](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS03.png "[Import DATEV CSV Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [WEITER]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## GDI

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button GDI*

![Import GDI Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/GDI01.png "[Import GDI Step 1]")

**Step 1**

![Import GDI Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/GDI02.png "[Import GDI Step 2]")

**Step 2**


![Import GDI Step 3](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/GDI03.png "[Import GDI Step 3]")

**Step 3**



## GDPdU export

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button GDPDU EXPORT*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**


## Open items

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button OPEN ITEMS*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**


## Balance lists

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button BALANCE LISTS*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**


## SALDEN.DAT

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button SALDEN.DAT*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**



## SAP

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button SAP*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**



## Varial

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button VARIAL*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**



## Zahlwerk

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button ZAHLWERK*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**



### Tax mapping

![Tax mapping](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BMDTaxMapping.png "[Tax mapping]")


Tax mapping  
Actindo tax control key  
BMD control key  

![Create tax mapping](/Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BMDTaxMapping02.png "[Create tax mapping]")


CREATE
DELETE

**Add/Edit**

actindo	Actindo
BMD	BMD

	SAVE
	CLEAR


### Import/export definitions

![Import/export definitions](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/ImportExportDefinitionsLexware.png "[Import/export definitions]")

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

  - ![Up](/Assets/Icons/ArrowUp.png "[Up]") (Up)  
  Use this button to move a selected field up in the list.

  - ![Down](/Assets/Icons/ArrowDown.png "[Down]") (Down)  
  Use this button to move a selected field down in the list.

  - ![Left](/Assets/Icons/ArrowLeft.png "[Left]") (Left)  
  Use this button to move a selected field left, from the *Possible fields* list to the *Fields in the definition* list.

  - ![Right](/Assets/Icons/ArrowRight.png "[Right]") (Right)  
  Use this button to move a selected field right, from the *Fields in the definition* list to the *Possible fields* list.

**Column**  
The letter and number in brackets indicate the column where a selected field is placed.

**Possible fields**  
This list displays all fields available for the selected import/export definition.


[INSERT IGNORE FIELD]  
Click this button to enter an "ignore field", that is, to indicate that the field in that position does not need to be exported or imported, in the *Fields in the definition* list.

**CSV format definition**

- *Field separating character*  
Enter the character to be used to separate fields. This value may be set up by default to comma or semicolon.

- *Escape character*  
Enter the character to be used to escape. This value may be set up by default to backslash.

[comment]: <> (Further info needed! RS HG)

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

- *Incorrect tow end character*  
Click the drop-down list to select the appropriate option (**Ignore/Repair**).

- *Number format*  
Click the drop-down list to select the desired number format.

- [SAVE]  
Click this button to save the changes.



#### New import/export definition  

![New import/export definition](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/NewImportExportDefinitionKdLf.png "[New import/export definition]")

- *For*  
Click the drop-down list to select the import/export definition type where the new definition will be added.  

- *Name*  
Enter a name for the new import/export definition to be created.

- [SAVE & NEW]  
Click this button to create a new import/export definition.  


#### Rename import/export definition  

![Rename import/export definition ](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/RenameImportExportDefinitionKdLf.png "[Rename import/export definition ]")

- *For*  
Click the drop-down list to select the import/export definition type where the new definition will be renamed.  

- *Old name*  
The previously given name is displayed. This field is read-only.

- *New name*  
Enter a new name for the selected import/export.

- [SAVE]  
Click this button to rename the selected import/export definition.  
