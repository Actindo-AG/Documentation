[!!Accounting](Actindo/Accounting)

# Access bookings from another period

A fiscal year is the period over which a company's accounts are calculated, which generally lasts 12 months and which may or may not coincide with the calendar year.

A journal is a chronological record of all accounting transactions of a business within a specified period of time. There are two main types: general journals and special journals. Special journals are specialized lists of transactions records and can be freely determined by the bookkeeper. However, it is highly recommended to use the special journals configured in the system:

| Journal number | Definition |   
| ------------- | ------------- |
| Journals 1-12 | Bookings for months 1-12 |  
| Journal 90 | Balances carried forward bookings for financial accounts |  
| Journal 92 | Impersonal accounts, such as input tax and VAT balances |  
| Journal 93 | Carry forwards for P&L accounts |  
| Journal 98 | Debtors open items |  
| Journal 99 | Creditors open items |

[comment]: <> (Taken from old documentation. Still up to date? Relevant here or better somewhere else, e.g. /ACD-451?)  

[comment]:<> (Table in markdown not possible without header?)

[comment]: <> (See table in old documentation about months - 0-Saldovorträge, 1-12 booking months, 13-15-Subsequent entries...)

The booking month is also relevant for the arrangement of bookings within a booking period. Calendar months, irrespectively of whether or not the fiscal year coincides with the calendar year, are matched per default with the journals 1 to 12. This means, that the first month of a fiscal year will coincide with the journal 1, the second one with the journal 2 and so on.

Journal and months are used to arrange a company's business transactions within a fiscal year. A particular booking period, that is, a fiscal year and a journal, will only contain the bookings recorded in that specific period. Accessing bookings from other periods may be necessary, for example, if a booking from a previous booking period needs to be adjusted or if a transaction performed at a later stage must be manually booked in a specific period.

[comment]: <> (Unsure! Wissentransfer/Jessi fragen)

Moreover, when opening the *Accounting* module for the first time after login or after reloading the system, the window to select a fiscal year is displayed. For detailed information, see [Select fiscal year](01_SelectFiscalYear.md).

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Button FY/MONTH/JOURNAL*

![FY/MONTH/JOURNAL button](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_FYMonthJournal_Button.png "[FY/MONTH/JOURNAL button]")

1. Click the *FY/MONTH/JOURNAL* button.  
The *Select fiscal year* window is displayed.  

  ![Select fiscal year view](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_SelectFiscalYear_View.png "[Select fiscal year view]")

2. Select the appropriate fiscal year in the *Fiscal year* field.
> [Info] The *Period* date fields are filled in automatically.

  ![Select fiscal year window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_SelectFiscalYear_Window.png "[Select fiscal year window]")

3. Select the appropriate month in the *Month* drop-down list.

4. Enter the appropriate journal number in the *Journal* field. Alternatively, click the [LIST] button.  
A new window with the available journals and their bookings is displayed.

  ![Select journal window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_SelectFiscalYear_Window_Journals.png "[Select journal window]")

5. Select the appropriate journal.

6. Click the [OK] button.  
The bookings recorded in the selected booking period are displayed.

## Next steps

  - [Search in accounting](14_SearchAccounting.md)
  - [Provide the accounting data](15_ProviceAccountingData.md)

## See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year)
  - [Select fiscal year](01_SelectFiscalYear.md)
