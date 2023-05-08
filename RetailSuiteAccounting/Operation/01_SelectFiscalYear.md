[!!Manage the fiscal year](../Integration/04_ManageFiscalYear.md)
[!!Manage the fixed postings](../Integration/06_ManageFixedBookings.md)
[!!User interface Select fiscal year](../UserInterface/00a_FiscalYear.md)
[!!User interface Postings header](../UserInterface/01_Header.md)
[!!User interface Settings fiscal years](../UserInterface/02d_FiscalYears.md)
[!!User interface Fixed postings](../UserInterface/02f_FixedBookings.md)

# Select the fiscal year

A fiscal year is the period over which a company's accounts are calculated, which generally lasts 12 months and which may or may not coincide with the calendar year.

A journal is a chronological record of all accounting transactions posted within a specified period of time. There are two main types of journals preconfigured in the system:
- General journals (1-12) are paired with the corresponding fiscal year months, regardless of whether the fiscal year coincides with the calendar year or not. This means that all transactions posted automatically in the first month of the fiscal year will be found in journal 1, all transactions posted in the second month of the fiscal year in the journal 2, and so on. Therefore, when selecting a posting period to perform a manual posting, make sure that the selected month and journal match.
- Special journals (90-99) are preconfigured in the system to post automatically open items and balances to be carried forward from a fiscal year to the next one. The special journals settings can be edited and extended in the *BALANCES CARRIED FORWARD* tab in the *Settings* menu entry.    
For detailed information, see [Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md). Further journals can be created if necessary.

Special months are also preconfigured in the system for special business transactions, such as balances carried forward or subsequent postings.   
For detailed information, see [Fiscal year](../UserInterface/00a_FiscalYear.md).

Journals and months are used to arrange a company's business transactions within a fiscal year. A particular posting period contains only the postings made in that specific period.



## Start the *Accounting* module

When you open the *Accounting* module for the first time after logging in or after reloading the system, a window to select the fiscal year is displayed. You have to select the fiscal year, the month and the journal to display the postings in the corresponding period. You must have selected a fiscal year to perform any action in the *Accounting* module.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year has been created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).

#### Procedure

*Accounting*

![Select fiscal year](../../Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear.png "[Select fiscal year]")

1. Click the *Fiscal year* drop-down list and select a fiscal year. All available fiscal years are displayed in the list.    
    The *Period* date fields are filled in automatically.

2. Click the *Month* drop-down list and select a month. The selected month determines the posting period, this means, the period where the transaction is posted. The accounting month plays a determining role when generating system evaluations.

3. Enter a journal number in the *Journal* field. Alternatively, you can click the [LIST] button to select a journal in the *Journals* window, which is displaying all available journals and the postings contained in each of them. The journal, or posting batch, is a superordinate criterion for the arrangement of postings. Selecting the correct journal is extremely important for the data exports.

    ![Journals](../../Assets/Screenshots/RetailSuiteAccounting/Journals.png "[Journals]")

4. If required, select first the *Include fixed postings* checkbox and then a batch from the displayed list.

    > [Info] If the *Include fixed postings* checkbox is selected, all fixed postings in the selected batch will be automatically posted when opening the selected period in the fiscal year. For detailed information about creating fixed postings, see [Create fixed postings](../Integration/06_ManageFixedBookings.md#create-fixed-postings).

5. Click the [OK] button in the bottom right corner.   
    The *POSTINGS* tab in the *Post* menu entry is displayed for the selected posting period.  All postings registered in this posting period are displayed in the list of postings.



## Access postings from another period

Once a posting period has been selected, it is possible to change to a different one. Accessing postings from other periods may be necessary, for example, if a posting needs to be adjusted or if a transaction performed at a later stage must be manually posted in a specific period. The posting period can be changed from each tab within the *Post* menu entry.

#### Prerequisites

- A valid fiscal year has been created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Post*

![Postings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Postings]")

1. Click the *FY/MONTH/JOURNAL* button in the postings header.  
    The *Select fiscal year* window is displayed.  

    ![Select fiscal year](../../Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear.png "[Select fiscal year]")

2. Click the *Fiscal year* drop-down list and select a fiscal year. All available fiscal years are displayed in the list.    
    The *Period* date fields are filled in automatically.

3. Click the *Month* drop-down list and select a month.  The selected month determines the posting period, this means, the period where the transaction is posted. The accounting month plays a determining role when generating system evaluations.

4. Enter a journal number in the *Journal* field. Alternatively, you can click the [LIST] button to select a journal in the *Journals* window, which is displaying all available journals and the postings contained in each of them. The journal, or posting batch, is a superordinate criterion for the arrangement of postings. Selecting the correct journal is extremely important for the data exports.

    ![Journals](../../Assets/Screenshots/RetailSuiteAccounting/Journals.png "[Journals]")

5. If required, select first the *Include fixed postings* checkbox and then a batch from the displayed list.

    > [Info] If the *Include fixed postings* checkbox is selected, all fixed postings in the selected batch will be automatically posted when opening the selected period in the fiscal year. For detailed information about creating fixed postings, see [Create fixed postings](../Integration/06_ManageFixedBookings.md#create-fixed-postings).

6. Click the [OK] button in the bottom right corner.   
    The *POSTINGS* tab in the *Post* menu entry is displayed for the selected posting period.  All postings registered in this posting period are displayed in the list of postings.
