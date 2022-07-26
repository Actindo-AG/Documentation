[!!Accounting](RetailSuiteAccounting)

# Access bookings from another period

A fiscal year is the period over which a company's accounts are calculated, which generally lasts 12 months and which may or may not coincide with the calendar year.

A journal is a chronological record of all accounting transactions within a specified period of time. There are two main types of journals preconfigured in the system:

  - General journals (1-12) are matched with the fiscal year months, irrespectively of whether or not the fiscal year coincides with the calendar year. That means, the first fiscal year month corresponds to journal 1, the second to journal 2 and so on.

  - Special journals (90-99) are specialized lists of transactions records preconfigured in the system for the balances carried forward. Further journals can be created.

Special months are also preconfigured for in the system for special business transactions, such as balances carried forward or subsequent bookings.

Journal and months are used to arrange a company's business transactions within a fiscal year. A particular booking period will only contain the bookings recorded in that specific period. Accessing bookings from other periods may be necessary, for example, if a booking from a previous booking period needs to be adjusted or if a transaction performed at a later stage must be manually booked in a specific period.

Moreover, when opening the *Accounting* module for the first time after login or after reloading the system, the window to select a fiscal year is displayed. For detailed information, see [Select fiscal year](01_SelectFiscalYear.md).

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](/RetailSuiteAccounting/Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](RetailSuiteAccounting/Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Button FY/MONTH/JOURNAL*

![FY/MONTH/JOURNAL button](/Assets/Screenshots/RetailSuiteAccounting/Book/FYMonthJournalButton.png "[FY/MONTH/JOURNAL button]")

1. Click the *FY/MONTH/JOURNAL* button.  
The *Select fiscal year* window is displayed.  

  ![Select fiscal year view](/Assets/Screenshots/RetailSuiteAccounting/Book/SelectFiscalYearView.png "[Select fiscal year view]")

2. Select the appropriate fiscal year in the *Fiscal year* field.
> [Info] The *Period* date fields are filled in automatically.

  ![Select fiscal year window](/Assets/Screenshots/RetailSuiteAccounting/Book/SelectFiscalYearWindow.png "[Select fiscal year window]")

3. Select the appropriate month in the *Month* drop-down list.

4. Enter the appropriate journal number in the *Journal* field. Alternatively, click the [LIST] button.  
A new window specifying the available journals and the number of bookings contained in each of them is displayed.

  ![Select journal window](/Assets/Screenshots/RetailSuiteAccounting/Book/SelectFiscalYearJournals.png "[Select journal window]")

5. Select the appropriate journal.

  > [Info] Journals 1-12 are matched with the corresponding months, irrespectively of whether or not the fiscal year coincides with the calendar year. Make sure that the month and the journal selected match before clicking the [OK] button.

6. Click the [OK] button.  
The bookings recorded in the selected booking period are displayed.


## See also

  - [BUCHUNGEN](/RetailSuiteAccounting/UserInterface/XX_Buchungen.md)
  - [Create fiscal year](/RetailSuiteAccounting/Integration/04_ManageFiscalYear.md#create-a-fiscal-year)
  - [Select fiscal year](01_SelectFiscalYear.md)
