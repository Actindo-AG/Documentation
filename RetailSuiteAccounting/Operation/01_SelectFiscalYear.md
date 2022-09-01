[!!User Interface Select fiscal year](../UserInterface/00a_FiscalYear.md)  
[!!User Interface FY/MONTH/JOURNAL](../UserInterface/01_Book.md#fymonthjournal)  
[!!User Interface Fixed postings](../UserInterface/02f_FixedBookings.md)  
[!!Manage the fixed postings](../Integration/06_ManageFixedBookings.md)  



# Select the fiscal year

When you open the *Accounting* module for the first time after login or after reloading the system, a window to select the fiscal year is displayed. You have to select the fiscal year, the month and the journal to display the postings in the corresponding period. You must have selected a fiscal year to perform any action in the *Accounting* module.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year has been created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).

#### Procedure

*Accounting*

![Select fiscal year](../../Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear.png "[Select fiscal year]")

1. Click the *Fiscal year* drop-down list and select a fiscal year.   
  The *Period* date fields are filled in automatically.

2. Click the *Month* drop-down list and select a month. The selected month determines the posting period, this means, the period where the transaction is posted. The accounting month plays a determining role when generating system evaluations.

  > [Info] Apart from the calendar months, special posting periods can also be selected to post balances carried forward, subsequent postings and closing postings. For detailed information, see [Select fiscal year](../UserInterface/00a_FiscalYear.md).

3. Enter a journal number in the *Journal* field. The journal, or posting batch, is a superordinate criterion for the arrangement of postings. Selecting the correct journal is extremely important for the data exports. Alternatively, you can click the [LIST] button to display the *Journals* window with the available journals and the postings contained in each of them.

  ![Journals](../../Assets/Screenshots/RetailSuiteAccounting/Journals.png "[Journals]")

  > [Info] Journals 1-12 are paired with the corresponding fiscal year months, regardless of whether the fiscal year coincides with the calendar year or not. This means that all transactions posted automatically in the first month of the fiscal year will be found in journal 1, all transactions posted in the second month of the fiscal year in the journal 2, and so on. Therefore, when selecting an accounting period to perform a manual posting, make sure that the selected month and journal match. Journals 90 to 99 are special journals preconfigured in the system to post automatically open items and balances to be carried forward from a fiscal year to the next one. The special journals settings can be edited and extended in the *BALANCES CARRIED FORWARD* tab in the *Settings* menu entry. For detailed information, see [Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md). Further journals can be created if necessary.


4. If required, select first the *Include fixed postings* checkbox and then a batch from the displayed list.

  > [Info] If the *Include fixed postings* checkbox is selected, all fixed postings in the selected batch will be automatically posted when opening the selected period in the fiscal year. For detailed information about creating fixed postings, see [Create fixed postings](../Integration/06_ManageFixedBookings.md#create-fixed-postings).

5. Click the [OK] button in the bottom right corner.   
  The postings registered in the selected posting period (fiscal year, month and journal) are displayed in the *POSTINGS* tab in the *Post* menu entry.  
