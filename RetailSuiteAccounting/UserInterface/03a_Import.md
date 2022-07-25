[!!Accounting](RetailSuiteAccounting)

# Import

*Accounting > Select fiscal year > Extras > Tab IMPORT*

![Import](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Import.png "[Import]")

> [Info] The import function is also available in the *FISCAL YEARS* tab of the *Settings* menu entry, see [Import bookings](02d_Settings.md#import-bookings).

- *Import from:*  
A list of the available import options is displayed:

  - *Compeso 7.x fiscal year backups*
  - *Import of data in CVS format*
  - *Import of data in CVS format from invoicing solution*
  - *Import of data in GDI standard interface format*
  - *Import of openTRANS INVOIC XLM data*
  - *Import of data in FQBATCH format from Schilling Software GmbH*


- [COMPESO 7.X]  
Click this button to import data in Compeso proprietary format. Follow the instructions provided in the following windows, see [Compeso 7.X](#compeso-7x).

- [CSV]  
Click this button to import data in CSV format. Follow the instructions provided in the following windows, see [CSV](#csv).

- [CSV LS-MOTOR]  
Click this button to import data in CSV format from an invoicing solution. Follow the instructions provided in the following windows, see [CSV LS-Motor](#csv-ls-motor).

[comment]: <> (LS ENGINE?)

- [GDI]  
Click this button to import data in GDI standard interface format. Follow the instructions provided in the following windows, see [GDI](#gdi).

- [OPENTRANS]  
Click this button to import data in openTRANS INVOIC XML format. Follow the instructions provided in the following windows, see [openTRANS](#opentrans).

- [SCHILLING BUCHHALTUNG]  
Click this button to import data in Schilling Software proprietary FQBATCH format. Follow the instructions provided in the following windows, see [Schilling Accounting](#schilling-accounting).


## Compeso 7.X

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button COMPESO 7.X*

![Import Compeso 7.X Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso01.png "[Import Compeso 7.X Step 1]")

**Step 1**

*Files*  
A list of compatible files is displayed. The following files are permitted:

  - *backup.ctl*  
  - *backup.dat*
  - *abrzr.dat*

- [Choose file]  
Click this button to select a file from your computer to be uploaded. If no file has been selected yet, the message "No file chosen" is displayed.

- [UPLOAD]  
Click this button to upload the selected file. The *Compeso 7.x: Step 2* is displayed.

- [CONTINUE]  
Click this button to proceed to the next step.


![Import Compeso 7.X Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Compeso02.png "[Import Compeso 7.X Step 2]")

**Step 2**

- *Converting...*  
This message is displayed during the import process.  

- [CANCEL]  
Click this button to cancel the process.


[comment]: <> (Der Prozess geht nicht weiter, System hängt. Ich habe versucht eine exportierte DAT-Datei -Reiter EXPORT- zu importieren, aber es scheint nicht zu funktioniere. Bug?)


## CSV

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button CSV*

![Import CSV Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSV01.png "[Import CSV Step 1]")

![Import CSV Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSV01DMS.png "[Import CSV Step 1]")

**Step 1**

- *Files*  
A list of compatible files is displayed. In this case, only CSV files can be imported.

- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Local file*  
Click this radio button to select a file from your computer to be uploaded. The [Choose file] button is displayed.
- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *DMS*  
Click this radio button to select a file from a DMS to be uploaded. The [SEARCH] button is displayed.

- [Choose file]  
Click this button to select a file from your computer to be uploaded. If no file has been selected yet, the message "No file chosen" is displayed.

- [SEARCH]  
Click this button to search for the file to be uploaded. The *Search file* window is displayed, see [Select file](#select-file).

- [UPLOAD]  
Click this button to upload the selected file. The selected file is uploaded. The [UPLOAD] button becomes grayed out.

- *File content*  
Click the drop-down list to select to appropriate file content. The following options are available:

  - **Customers/suppliers**	 
  - **Chart of Accounts**	  
  - **Bookings**  
  - **eBay sales history**

[comment]: <> (eBay sales history ist relevant für alle Kunden? Weglassen? Andere Optionen je nach Einstellungen/Module/Plugins?)

- *Import def.*  
Click the drop-down list to select the appropriate import definition.

  - **Lexware Pro (customers)**
  - **Lexware Pro (suppliers)**


- [Edit]  
Click this button to edit the selected import definition. The *Import/export definitions* window is displayed, see [Import/export definitions](#importexport-definitions).

- *Split bookings*  
Click the drop-down list to select the appropriate import setting for split bookings. The following options are available:

  - **With different tax rates**
  - **For more than one product**
  - **Always**


- [CONTINUE]  
Click this button to proceed to the next step.


![Import CSV Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSV02.png "[Import CSV Step 2]")

**Step 2**

 - *Log file*  
The import log file is available in this step.

- *View log file*  
The import log file can be viewed in this step.

- [VIEW]  
Click this button to visualize the import log file.

- [CONTINUE]  
Click this button to proceed to the next step.


![Import CSV Step 3](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSV03.png "[Import CSV Step 3]")

**Step 3**

> [Info] Depending on the imported data, the screen displayed varies.

- *Bookings*  
The import file contains bookings to be imported. Otherwise, the message "No bookings in the import file" is displayed.

  - *Take over bookings?*  
  Select **No** if you do not want the system to take over the bookings in the import file. The default setting is **Yes**.

  - *Overwrite existing ones?*  
  Select **No** if you do not want the system to overwrite the existing bookings. The default setting is **Yes**.


- *Impersonal accounts*

  The import file contains impersonal accounts to be imported. Otherwise, the message "No impersonal accounts in the import file" is displayed.

  - *Take over impersonal accounts?*  
  Select **No** if you do not want the system to take over the impersonal accounts in the import file. The default setting is **Yes**.

  - *Overwrite existing ones?*  
  Select **No** if you do not want the system to overwrite the existing impersonal accounts. The default setting is **Yes**.


- *Personal accounts*  

  The import file contains personal accounts to be imported. Otherwise, the message "No personal accounts in the import file" is displayed.

  - *Take over personal accounts?*  
  Select **No** if you do not want the system to take over the personal accounts in the import file. The default setting is **Yes**.

  - *Overwrite existing ones?*  
  Select **No** if you do not want the system to overwrite the existing personal accounts. The default setting is **Yes**.


[comment]: <> (Ich gehe davon aus, dass es so funktioniert. Weiter testen oder RS mit FH.)

- [FINALIZE]  
Click this button to complete the import process.



![Import CSV Step 4](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSV04.png "[Import CSV Step 4]")

**Step 4**

- *Importing...*  
This message is displayed during the import process.  

- [CANCEL]  
Click this button to cancel the process.


![Import CSV Step 5](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSV05.png "[Import CSV Step 5]")

**Step 5**

[comment]: <> (Leeres Fenster. Kommentar in OneNote Bugs-Datei.)



## CSV LS-Motor

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button CSV LS-MOTOR*

![Import CSV LS-Motor Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSVLSMotor01.png "[Import CSV LS-Motor Step 1]")

![Import CSV LS-Motor Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/CSVLSMotor01DMS.png "[Import CSV LS-Motor Step 1]")

**Step 1**

- *Files*  
A list of compatible files is displayed. In this case, only txt files can be imported.

[comment]: <> (txt oder X.txt? Unterschied oder X gehört zum Namen? Ich kann keine txt Datei hochladen. Fehlermeldung: No such file or directory)

- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Local file*  
Click this radio button to select a file from your computer to be uploaded. The [Choose file] button is displayed.
- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *DMS*  
Click this radio button to select a file from a DMS to be uploaded. The [SEARCH] button is displayed.

- [Choose file]  
Click this button to select a file from your computer to be uploaded. If no file has been selected yet, the message "No file chosen" is displayed.

- [SEARCH]  
Click this button to search for the file to be uploaded. The *Search file* window is displayed, see [Select file](#select-file).

- [UPLOAD]  
Click this button to upload the selected file. The selected file is uploaded. The [UPLOAD] button becomes grayed out.


- *CustomerX.txt*  
Click the drop-down list to select the appropriate import definition.

  - **AfterBuy CSV**
  - **Auction Master CSV**
  - **Invoicing: new receipts**


- *OrdersX.txt*  
  Click the drop-down list to select the appropriate import definition.

    - **AfterBuy CSV**
    - **Auction Master CSV**
    - **Invoicing: new receipts**


[comment]: <> (Andere Optionen abhängig von Einstellungen/Kunden/Plugins usw.? Faktura: Belege neu/Invoicing: new receipts weglassen?)


- [Edit]  
Click this button to edit the selected import definition. The *Import/export definitions* window is displayed, see [Import/export definitions](#importexport-definitions).

- [CONTINUE]  
Click this button to proceed to the next step.


**Step 2**

[comment]: <> (Ich komme nicht zum Step 2 - Probleme mit Hochladen der txt-Datei!)

- to be completed


## GDI

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button GDI*

![Import GDI Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/GDI01.png "[Import GDI Step 1]")

![Import GDI Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/GDI01DMS.png "[Import GDI Step 1]")


**Step 1**

- *Files*  
A list of compatible files is displayed. In this case, only STD files can be imported.

- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Local file*  
Click this radio button to select a file from your computer to be uploaded. The [Choose file] button is displayed.
- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *DMS*  
Click this radio button to select a file from a DMS to be uploaded. The [SEARCH] button is displayed.

- [Choose file]  
Click this button to select a file from your computer to be uploaded. If no file has been selected yet, the message "No file chosen" is displayed.

- [SEARCH]  
Click this button to search for the file to be uploaded. The *Search file* window is displayed, see [Select file](#select-file).

- [UPLOAD]  
Click this button to upload the selected file. The selected file is uploaded. The [UPLOAD] button becomes grayed out.

- [CONTINUE]  
Click this button to proceed to the next step.



![Import GDI Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/GDI02.png "[Import GDI Step 2]")

**Step 2**

 - *Log file*  
The import log file is available in this step.

- *View log file*  
The import log file can be viewed in this step.

- [VIEW]  
Click this button to visualize the import log file.

- [CONTINUE]  
Click this button to proceed to the next step.



![Import GDI Step 3](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/GDI03.png "[Import GDI Step 3]")

**Step 3**

> [Info] Depending on the imported data, the screen displayed varies.


- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Create new fiscal year*
 - *FY name*
 - *From - to*


-  ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") Add bookings to FY
  - *Import into FY*
  - *From - to*


- *Impersonal accounts*

  The import file contains impersonal accounts to be imported. Otherwise, the message "No impersonal accounts in the import file" is displayed.

  - *Take over impersonal accounts?*  
  Select **No** if you do not want the system to take over the impersonal accounts in the import file. The default setting is **Yes**.

  - *Overwrite existing ones?*  
  Select **No** if you do not want the system to overwrite the existing impersonal accounts. The default setting is **Yes**.


- *Personal accounts*  

  The import file contains personal accounts to be imported. Otherwise, the message "No personal accounts in the import file" is displayed.

  - *Take over personal accounts?*  
  Select **No** if you do not want the system to take over the personal accounts in the import file. The default setting is **Yes**.

  - *Overwrite existing ones?*  
  Select **No** if you do not want the system to overwrite the existing personal accounts. The default setting is **Yes**.


[comment]: <> (Ich gehe davon aus, dass es so funktioniert. Weiter testen oder RS mit FH.)


- [FINALIZE]  
Click this button to complete the import process.


![Import GDI Step 4](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/GDI04.png "[Import GDI Step 4]")

**Step 4**

- *Importing...*  
This message is displayed during the import process.  

- [CANCEL]  
Click this button to cancel the process.



![Import GDI Step 5](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/GDI05.png "[Import GDI Step 5]")

**Step 5**

- to be completed

[comment]: <> (Leeres Fenster. Komment in OneNote Bugs-Datei.)


## openTRANS

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button openTRANS*

![Import openTRANS Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Opentrans01.png "[Import openTRANS Step 1]")

![Import openTRANS Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Opentrans01DMS.png "[Import openTRANS Step 1]")


**Step 1**

- *Files*  
A list of compatible files is displayed. In this case, only xml files can be imported.

- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Local file*  
Click this radio button to select a file from your computer to be uploaded. The [Choose file] button is displayed.
- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *DMS*  
Click this radio button to select a file from a DMS to be uploaded. The [SEARCH] button is displayed.

- [Choose file]  
Click this button to select a file from your computer to be uploaded. If no file has been selected yet, the message "No file chosen" is displayed.

- [SEARCH]  
Click this button to search for the file to be uploaded. The *Search file* window is displayed, see [Select file](#select-file).

- [UPLOAD]  
Click this button to upload the selected file. The selected file is uploaded. The [UPLOAD] button becomes grayed out.

- *Creditor/supplier number*  
Enter the creditor/supplier number.  

- [CONTINUE]  
Click this button to proceed to the next step.


![Import openTRANS Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Opentrans02.png "[Import openTRANS Step 2]")

**Step 2**

 - *Log file*  
The import log file is available in this step.

- *View log file*  
The import log file can be viewed in this step.

- [VIEW]  
Click this button to visualize the import log file.

- [CONTINUE]  
Click this button to proceed to the next step.

[comment]: <> (Fehlermeldung " Konnte kein passendes Wareneingangskonto finden, bzw. kein Konto ist als Wareneingangskonto markiert Steuerschlüssel 0, Datum 2009-05-13..." Keine KOMM_NO! in Logdatei. WEITER Schaltfläche ausgegraut / nicht klickbar)



## Schilling Accounting

*Accounting > Select fiscal year > Extras > Tab IMPORT > Button Schilling Accounting*

![Import Schilling Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Schilling01.png "[Import Schilling Step 1]")

![Import Schilling Step 1](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Schilling01DMS.png "[Import Schilling Step 1]")

**Step 1**

- *Files*  
A list of compatible files is displayed. In this case, only txt files can be imported.

- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *Local file*  
Click this radio button to select a file from your computer to be uploaded. The [Choose file] button is displayed.
- ![Radio button](/Assets/Icons/RadioButton02.png "[Radio button]") *DMS*  
Click this radio button to select a file from a DMS to be uploaded. The [SEARCH] button is displayed.

- [Choose file]  
Click this button to select a file from your computer to be uploaded. If no file has been selected yet, the message "No file chosen" is displayed.

- [SEARCH]  
Click this button to search for the file to be uploaded. The *Search file* window is displayed, see [Select file](#select-file).

- [UPLOAD]  
Click this button to upload the selected file. The selected file is uploaded. The [UPLOAD] button becomes grayed out.

- [CONTINUE]  
Click this button to proceed to the next step.


![Import Schilling Step 2](/Assets/Screenshots/RetailSuiteAccounting/Extras/Import/Schilling02Fehler.png "[Import Schilling Step 2]")

**Step 2**

- *Converting...*  
This message is displayed during the import process.  

- [CANCEL]  
Click this button to cancel the process.


[comment]: <> (Der Prozess geht nicht weiter, System hängt. Ich habe versucht eine exportierte DAT-Datei -Reiter EXPORT- zu importieren, aber es scheint nicht zu funktioniere. Bug?)



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


#### Select file

![Select file](/Assets/Screenshots/RetailSuiteAccounting/Settings/CustomerSupplier/SelectFile.png "[Select file]")

- *New documents*  
The new uploaded documents are contained in this folder.

- *Registered documents*  
The documents that have been registered in the system are contained in this folder.

- *Printed documents*  
The documents that have been printed are contained in this folder.

  > [Info] Further folders can be created in the *Documents* module.

- *Name*  
Name of folder or file.

- *Size*  
Size of folder or file.

- *Type*  
Type of item.

- *Changed*  
Date and time when the folder or file were modified.

- *Owner*  
Person owning the folder or file.

- [CLOSE]  
Click this button to close the window.

- [OPEN]  
Click this button to select the file.
