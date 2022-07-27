# Export

*Accounting > Select fiscal year > Extras > Tab EXPORT*

![Export](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Export.png "[Export]")

> [Info] The export function is also available in the *FISCAL YEARS* tab of the *Settings* menu entry, see [Export bookings](./02d_FiscalYears.md#export-bookings).


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
Click this button to export data in DATEV compatible CSV format. Follow the instructions provided in the following windows, see [DATEV CSV](#datev-csv). For detailed information about exporting data in DATEV compatible CSV, see [Export the data for DATEV](../Operation/15_ProvideAccountingData.md#export-the-data-for-DATEV).

- [GDI]  
Click this button to export data in GDI format. Follow the instructions provided in the following windows, see [GDI](#gdi).

- [GDPDU EXPORT]  
Click this button to export data in GDPdU-compliant audit file format. Follow the instructions provided in the following windows, see [GDPDU export](#gdpdu-export). For detailed information about exporting data in GDPdU-compliant audit file format, see [Export the data GDPdU-compliant](../Operation/15_ProvideAccountingData.md#export-the-data-GDPdU-compliant).

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

![Export BMD Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportBMD01.png "[Export BMD Step 1]")

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
Click this button to edit the tax mapping. The *BMD tax mapping* window is displayed, see [BMD tax mapping](#bmd-tax-mapping).

- [CONTINUE]  
Click this button to proceed to the next step.


![Export BMD Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportBMD02.png "[Export BMD Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.    

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.

[comment]: <> (Nach einiger Sekunden bzw. kurz vor dem Step 3 ABBRECHEN Button ändert sich zu SCHLIESSEN, was nicht wirklich Sinn macht, denn man schließt tatsächlich das Fenster, also man bricht der Export ab.)



![Export BMD Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportBMD03.png "[Export BMD Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## CSV

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button CSV*

![Export CSV Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV01.png "[Export CSV Step 1]")

![Export CSV Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV01cust.png "[Export CSV Step 1]")

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
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *Export all*
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *All from last export on (if last export exists, otherwise all)*
  - *Set marker to export time*  
  Mark the checkbox if time is to be exported.

[comment]: <> (Unsicher, RS mit FH)

- *File content*  
Click the drop-down list to select the applicable file content. The following options are available:

  - **Customers/suppliers**
  - **Chart of accounts**
  - **Bookings**  


- *Export def.*  
Click the drop-down list to select the appropriate export definition. The export definitions are preconfigured in the system but can be edited. All created export definitions are displayed in the drop-down list.


- [Edit]  
Click this button to add, edit or delete an export definition. The *Import/export definitions* window is displayed, see [Import/export definitions](#importexport-definitions).

- *Export*  
Click the drop-down list to select the specific data to be exported. The following options are available:  

  - **Customer/suppliers**
  - **Customers only**
  - **Suppliers only**
  - **Custom**  
  When selecting this option, the *Selection from - to* fields are displayed.


- *Selection from - to*  
Enter the account number range to be exported. You can enter the account numbers manually with the keyboard or use the increase/decrease arrows.


- [CONTINUE]  
Click this button to proceed to the next step.


![Export CSV Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV02.png "[Export CSV Step 2]")

**Step 2**


- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.    

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Export CSV Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportCSV03.png "[Export CSV Step 3]")


**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## DATEV CSV

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button DATEV CSV*

![Export DATEV CSV Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS01.png "[Export DATEV CSV Step 1]")

![Export DATEV CSV Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS01cust.png "[Export DATEV CSV Step 1]")

For detailed information about exporting data for DATEV, see [Export the data for DATEV](../Operation/15_ProvideAccountingData.md#export-the-data-for-datev).

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
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *Export all*
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *All from last export on (if last export exists, otherwise all)*
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
Click the drop-down list to select the personal accounts to be exported. The following options are available:  

  - **Yes**  
  - **Custom**   
  When selecting this option, the *Custom (e.g. 10000, 39999-49999)* field is displayed.
  - **No**  


- *Custom (e.g. 10000, 39999-49999)*    
Enter an account number or an account number range to be exported.

- *Export only booking-relevant master data records*  
 Click the drop-down list to select the appropriate option (**Yes/No**).

- *Take Receipt 2 field in the export document from booking record field*  
Click the drop-down list to select the appropriate option. The following options are available:  

  - **Receipt 1**
  - **Receipt 2**
  - **Receipt 3**
  - **Receipt 4**


- *Add tax keys from automatic accounts also in split bookings*  
Click the drop-down list to select the appropriate option (**Yes/No**).

- *Saved personal accounts length*  
Click the drop-down list to select the appropriate option. The account length refers to the number of character used to define personal accounts (5-9) and intends to avoid exporting incomplete account numbers.

- *DATEV advisor number*  
Enter the DATEV advisor number, if applicable.

- *DATEV client number*  
Enter the DATEV client  number, if applicable.

- [CONTINUE]  
Click this button to proceed to the next step.


![Export DATEV CSV Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS02.png "[Export DATEV CSV Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Export DATEV CSV Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportDatevCVS03.png "[Export DATEV CSV Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## GDI

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button GDI*

![Export GDI Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/GDI01.png "[Export GDI Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Impersonal accounts*  
Click the drop-down list to select the impersonal accounts to be exported. The following options are available:  

  - **Only individually changed**  
  - **All**  
  - **No**  


- *Personal accounts*  
Click the drop-down list and select the appropriate option (**Yes/No**).

- [CONTINUE]  
Click this button to proceed to the next step.


![Export GDI Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/GDI02.png "[Export GDI Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.



![Export GDI Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/GDI03.png "[Export GDI Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)


## GDPdU export

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button GDPDU EXPORT*

![Export GDPDU Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportGDPdU01.png "[Export GDPDU Step 1]")

 For detailed information about exporting data in GDPdU-compliant audit file format, see [Export the data GDPdU-compliant](../Operation/15_ProvideAccountingData.md#export-the-data-GDPdU-compliant).


**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Personal accounts*  
Click the drop-down list and select the appropriate option (**Yes/No**).


- *Export only booking-relevant master data records*  
 Click the drop-down list to select the appropriate option (**Yes/No**).

- *Saved personal accounts length*  
Click the drop-down list to select the appropriate option. The account length refers to the number of character used to define personal accounts (5-9) and intends to avoid exporting incomplete account numbers.

- *DATEV advisor number*  
Enter the DATEV advisor number, if applicable.

- *DATEV client number*  
Enter the DATEV client  number, if applicable.

- [CONTINUE]  
Click this button to proceed to the next step.


![Export GDPDU Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportGDPdU02.png "[Export GDPDU Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Export GDPDU Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/ExportGDPdU03.png "[Export GDPDU Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)


## Open items

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button OPEN ITEMS*

![Export Open items Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/OpenItems01.png "[Export Open items Step 1]")

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
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *Export all*
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *All from last export on (if last export exists, otherwise all)*
  - *Set marker to export time*  
  Mark the checkbox if time is to be exported.


- *Items*  
Click the drop-down list to select the items to be exported. The following options are available:

  - **Open items**
  - **Paid items**
  - **Open and paid items**


- *File content*  
Click the drop-down list to select the applicable file content. The following options are available:

  - **Customers/suppliers**
  - **Chart of accounts**
  - **Bookings**  


- *Export def.*  
Click the drop-down list to select the appropriate export definition. The export definitions are preconfigured in the system but can be edited. All created export definitions are displayed in the drop-down list.

- [Edit]  
Click this button to add, edit or delete an export definition. The *Import/export definitions* window is displayed, see [Import/export definitions](#importexport-definitions).

- [CONTINUE]  
Click this button to proceed to the next step.


![Export Open items Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/OpenItems02.png "[Export Open items Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.



![Export Open items Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/OpenItems03.png "[Export Open items Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## Balance lists

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button BALANCE LISTS*

![Export Balance lists Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BalanceList01.png "[Export Balance lists Step 1]")

![Export Balance lists Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BalanceList01cust.png "[Export Balance lists Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Accounts*  
Click the drop-down list to select the accounts to be exported. The following options are available:  
  - **Impersonal accounts**  
  - **Customers (10000-69999)**  
  - **Suppliers (70000-99999)**  
  - **Custom**  
    When selecting this option, the *Account from* and *Account to* fields are displayed.


- *Account from*  - *Account to*  
Enter the account number range to be exported.

- [CONTINUE]  
Click this button to proceed to the next step.



![Export Balance lists Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BalanceList02.png "[Export Balance lists Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Export Balance lists Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BalanceList03.png "[Export Balance lists Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## SALDEN.DAT

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button SALDEN.DAT*

![Export SALDEN.DAT Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/SALDEN.DAT01.png "[Export SALDEN.DAT Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Impersonal accounts*  
Click the drop-down list to select the impersonal accounts to be exported. The following options are available:  

  - **Only individually changed**  
  - **All**  
  - **No**  


- *Personal accounts*  
Click the drop-down list to select the appropriate option (**Yes/No**).

- [CONTINUE]  
Click this button to proceed to the next step.



![Export SALDEN.DAT Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/SALDEN.DAT02.png "[Export SALDEN.DAT Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.



![Export SALDEN.DAT Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/SALDEN.DAT03.png "[Export SALDEN.DAT Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## SAP

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button SAP*

![Export SAP Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/SAP01.png "[Export SAP Step 1]")


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
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *Export all*
  - ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *All from last export on (if last export exists, otherwise all)*
  - *Set marker to export time*  
  Mark the checkbox if time is to be exported.


- *Creation from*  
Enter a start creation date for the bookings to be exported.

- *Creation to*  
Enter an end creation date for the bookings to be exported.

- [CONTINUE]  
Click this button to proceed to the next step.



![Export SAP Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/SAP02.png "[Export SAP Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.



![Export SAP Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/SAP03.png "[Export SAP Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## Varial

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button VARIAL*

![Export Varial Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Varial01.png "[Export Varial Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Date from*   
Enter a start date for the bookings to be exported.

- *Date to*  
Enter an end date for the bookings to be exported.

- *File suffix*  
Enter a file suffix, if applicable. Only numbers can be used.

[comment]: <> (Info fehlt über VARIAL Datei-Suffix. Nichts gefunden.)



![Export Varial Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Varial02.png "[Export Varial Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.



![Export Varial Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Varial03.png "[Export Varial Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



## Zahlwerk

*Accounting > Select fiscal year > Extras > Tab EXPORT > Button ZAHLWERK*

![Export Zahlwerk Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Zahlwerk01.png "[Export Zahlwerk Step 1]")

![Export Zahlwerk Step 1](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Zahlwerk01cust.png "[Export Zahlwerk Step 1]")

**Step 1**

- *Fiscal year*  
Click the drop-down list to select the fiscal year to be exported.

- *Period*  
Specify the period to be exported.  

  - *Months*  
  Enter the month range to be exported.

  - *Journals*  
  Enter the journal range to be exported.

- *Accounts*  
Click the drop-down list to select the accounts to be exported. The following options are available:  
  - **Impersonal accounts**  
  - **Customers (10000-69999)**  
  - **Suppliers (70000-99999)**  
  - **Custom**  
    When selecting this option, the *Account from* and *Account to* fields are displayed.


- *Account from*  - *Account to*  
Enter the account number range to be exported.

- [CONTINUE]  
Click this button to proceed to the next step.


![Export Zahlwerk Step 2](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Zahlwerk02.png "[Export Zahlwerk Step 2]")

**Step 2**

- *Exporting*  
This message is displayed during the export process.  

- [CANCEL]  
Click this button to cancel the process. After a few seconds, the [CANCEL] button changes to a [CLOSE] button.  

- [CLOSE]  
Click this button to close the window. This will cancel the export.   

A pop-up window confirms that the selected data have been exported correctly. Click the OK button to proceed to the next step.


![Export Zahlwerk Step 3](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/Zahlwerk03.png "[Export Zahlwerk Step 3]")

**Step 3**

- *Exported files*  
The exported file(s) are displayed and can be downloaded by clicking on the file name(s).

- [CONTINUE]  

[comment]: <> (WEITER/CONTINUE Button bei allen Exporten ausgegraut > CLOSE Button? --> Bug)



### BMD tax mapping

![BMD tax mapping](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BMDTaxMapping.png "[BMD tax mapping]")


**Tax mapping**

- *Actindo tax key*  
Tax key as mapped in the Actindo system.

- *BMD tax key*  
Tax key as mapped in the BMD system.

[comment]: <> (Steuercode ist ein zweideutiger Term. Reden wir hier von "tax key" oder "control key"? Im System "tax control key" und "Steuercode". Vorsicht / RS FH dazu.)

- [Checkbox]  
Select the checkbox to edit or delete a tax key. The *Edit* section is displayed.

- [CREATE]  
Click this button to create a tax key. The *Add* section is displayed.

- [DELETE]  
Click this button to delete a selected tax key from the list.

- ![Refresh](../../Assets/Icons/Refresh03.png "[Refresh]") (Refresh)  
Click this button to refresh the list after making any changes.


**Add/Edit**  

![Create tax mapping](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Export/BMDTaxMapping02.png "[Create tax mapping]")

> [Info] When clicking the [CREATE] button, the *Add* section is displayed. When marking a checkbox from the tax key list, the tax key details are displayed in the entry fields, where they can be edited. The *Add* section name changes to *Edit*.


- *Actindo*  
Click the drop-down list to select the applicable tax sort in the Actindo system.

- *BMD*  
Click the drop-down list to select the applicable tax sort in the BMD system.

- [SAVE]  
Click this button to save any changes made.

- [CLEAR]  
Click this button to reset both fields to their initial status.


### Import/export definitions

![Import/export definitions](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Import/ImportExportDefinitionsLexware.png "[Import/export definitions]")

**Name**

- (Drop-down list)  
Click the drop-down list to select a preconfigured import/export definition type. If there are any available, the second drop-down list displays the preconfigured definitions of the selected type.

[comment]: <> (Bedeutung von Asterisk neben Namen?)

- (Drop-down list)  
Click the drop-down list to select the desired preconfigured import/export definition.

- [ADD]  
Click this button to create an import/export definition. The *New import/export definition* window is displayed, see [New import/export definition](#new-importexport-definition).

- [EDIT]  
Click this button to rename an import/export definition. The *Rename import/export definition* window is displayed, see [Rename import/export definition](#rename-importexport-definition).

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



#### New import/export definition  

![New import/export definition](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Import/NewImportExportDefinitionKdLf.png "[New import/export definition]")

- *For*  
Click the drop-down list to select the import/export definition type where the new definition will be added.  

- *Name*  
Enter a name for the new import/export definition to be created.

- [SAVE & NEW]  
Click this button to create a new import/export definition.  


#### Rename import/export definition  

![Rename import/export definition ](../../Assets/Screenshots/RetailSuiteAccounting/Extras/Import/RenameImportExportDefinitionKdLf.png "[Rename import/export definition ]")

- *For*  
Click the drop-down list to select the import/export definition type where the new definition will be renamed.  

- *Old name*  
The previously given name is displayed. This field is read-only.

- *New name*  
Enter a new name for the selected import/export definition.

- [SAVE]  
Click this button to rename the selected import/export definition.  