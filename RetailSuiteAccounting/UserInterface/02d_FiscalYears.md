# Fiscal years

*Accounting > Settings > Tab FISCAL YEARS*

![Fiscal years](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FiscalYears/CreateFiscalYear.png "[Fiscal years]")


- *Description*  
Fiscal year description. It may consist of letters, numbers or a combination of characters.

- *Planning*  
If the fiscal year has been set up for planning purposes, the word *PLANNING* is displayed. Otherwise, the column is empty.

[comment]: <> (Im System noch auf Deutsch: PLANUNG)

- *From*  
Fiscal year start date.

- *To*  
Fiscal year end date.

- *Currency*  
Currency selected for the fiscal year.

- *Cash accounting*  
If cash accounting has been selected, the word *CASH* is displayed. Otherwise, the column is empty.

[comment]: <> (Im System noch auf Deutsch: IST)



The entry fields allow to create, edit or delete fiscal years. For detailed information about creating, editing or deleting fiscal years, see [Manage the fiscal year](../Integration/04_ManageFiscalYear.md).

- *Description*  
Enter or modify the fiscal year. Letters, numbers or a combination of characters can be used. The number of characters is limited to 10.

- *From - to*  
Enter or modify the fiscal year start and end date.

  > [Info] The fiscal year must consist of 12 months. However, it does not have to be a calendar year, for example from 1st April to 31st March.

  > [Info] Fiscal years cannot overlap in time, for example, fiscal years 2022 and 2022-2023 cannot coexist. If two fiscal years overlap, an error message will be displayed. However, a fiscal year for planning purposes can overlap in time with actual fiscal years.

- *Currency*  
Click the drop-down list to select the appropriate currency.

  > [Info] The drop-down list displays all currencies configured in the system. However, the *Accounting* module works with the base currency only.

- *Cash accounting*  
Click the drop-down list to select the appropriate option (**No/Yes**).

  > [Info] The cash accounting refers to a method where receipts are recorded during the period they are received, and expenses are recorded in the period in which they are actually paid. This contrasts with accrual accounting, where revenue is recognized when earned rather than when collected, and expenses are recognized when incurred rather than when paid.

  > [Warning] This option has fundamental implications for the system automatic recording of taxes. In case of doubt, please check with your tax advisor.

- *Planning FY*  
Click the drop-down list to select the appropriate option (**No/Fiscal year for planning purposes only**).

  > [Info] Note that a fiscal year can be set up for planning purposes only. However, the fiscal year for planning purposes will not be recognized as an actual fiscal year by the system, and therefore the automatic functions in the interaction with other modules will not apply.


- [SAVE & NEW]  
Click this button to create a new fiscal year. For detailed information about creating a new fiscal year, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).

- [SAVE]  
Click this button to save any changes made to an existing fiscal year.

  > [Info] The saved changes will overwrite the selected fiscal year existing details. For detailed information about editing a fiscal year, see [Edit a fiscal year](../Integration/04_ManageFiscalYear.md#edit-a-fiscal-year).

- [DELETE]  
Click this button to delete the selected fiscal year.

  > [Warning] Be aware that the selected fiscal year will be deleted permanently. For detailed information, see [Delete a fiscal year](../Integration/04_ManageFiscalYear.md#delete-a-fiscal-year).

- [CLEAR]
Click this button to clear all entry fields. The button [SAVE & NEW] becomes active again.

- [HELP]  
Click this button to open the help function.

- [IMPORT]  
Click this button to import postings from a file. The *Import postings* window is displayed.

- [EXPORT]
Click this button to export postings into a file. The *Export postings* window is displayed.


## Import postings

*Accounting > Settings > Tab FISCAL YEARS > Button IMPORT*

![Import postings](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FiscalYears/ImportBookings.png "[Import postings]")

> [Info] The import function is also available in the *Extras* menu entry.

- *Import from:*  
A list of the available import options is displayed:

  - *Compeso 7.x fiscal year backups*
  - *Import of data in CVS format*
  - *Import of data in CVS format from invoicing solution*
  - *Import of data in GDI standard interface format*
  - *Import of openTRANS INVOIC XLM data*
  - *Import of data in FQBATCH format from Schilling Software GmbH*


- [COMPESO 7.X]  
Click this button to import data in Compeso proprietary format. Follow the instructions provided in the following windows.

[comment]: <> (Alle folgenden Fenster hinzufügen? Sie sind auch unterschiedlich für jede Option/jedes Format, auch wenn ähnlich und relativ selbsterklärend)

- [CSV]  
Click this button to import data in CSV format. Follow the instructions provided in the following windows.

- [CSV LS-MOTOR]  
Click this button to import data in CSV format from an invoicing solution. Follow the instructions provided in the following windows.

[comment]: <> (LS ENGINE?)

- [GDI]  
Click this button to import data in GDI standard interface format. Follow the instructions provided in the following windows.

- [OPENTRANS]  
Click this button to import data in openTRANS INVOIC XML format. Follow the instructions provided in the following windows.

- [SCHILLING BUCHHALTUNG]  
Click this button to import data in Schilling Software proprietary FQBATCH format. Follow the instructions provided in the following windows.



## Export postings

*Accounting > Settings > Tab FISCAL YEARS > Button EXPORT*

![Export postings](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FiscalYears/ExportBookings.png "[Export postings]")

> [Info] The export function is also available in the *Extras* menu entry. For detailed information, see [Provide the accounting data](../Operation/15_ProvideAccountingData.md).

- *Export to*  
A list of the available import options is displayed:

  - *Export of data in BMD format*
  - *Export of data in CSV format*
  - *Export of data in DATEV CSV format*
  - *Export of data in GDI standard interface format*
  - *Export of data in GDPdU format*
  - *Export of open items*
  - *Export of balance lists in CSV format*
  - *Compeso SALDEN.DAT*
  - *Export postings for SAP*
  - *Varial balances*
  - *Export of balance lists in CSV format (Zahlwerk)*


- [BMD]  
Click this button to export data in BMD format. Follow the instructions provided in the following windows.

- [CSV]  
Click this button to export data in CSV format. Follow the instructions provided in the following windows.

- [DATEV CSV]  
Click this button to export data in DATEV compatible CSV format. Follow the instructions provided in the following windows. For detailed information, see [Export the data for DATEV](../Operation/15_ProvideAccountingData.md#export-the-data-for-DATEV).

- [GDI]  
Click this button to export data in GDI format. Follow the instructions provided in the following windows.

- [GDPDU EXPORT]  
Click this button to export data in GDPdU-compliant audit file format. Follow the instructions provided in the following windows. For detailed information, see [Export the data GDPdU-compliant](../Operation/15_ProvideAccountingData.md#export-the-data-GDPdU-compliant).

- [OPEN ITEMS]  
Click this button to export open items. Follow the instructions provided in the following windows.

- [BALANCE LISTS]  
Click this button to export balance lists in CSV format. Follow the instructions provided in the following windows.

- [SALDEN.DAT]  
Click this button to export data in Compeso SALDEN.DAT proprietary format. Follow the instructions provided in the following windows.

- [SAP]  
Click this button to export data in SAP compatible format. Follow the instructions provided in the following windows.

- [VARIAL]  
Click this button to export data in VARIAL compatible format. Follow the instructions provided in the following windows.

- [ZAHLWERK]  
Click this button to export balance lists in Zahlwerk compatible CSV format. Follow the instructions provided in the following windows.
