[!!User Interface select fiscal year](../UserInterface/00a_FiscalYear.md)  
[!!User Interface FY/MONTH/JOURNAL](../UserInterface/00_Book.md#fymonthjournal)  
[!!User Interface fixed bookings](../UserInterface/02f_FixedBookings.md)  
[!!Manage fixed bookings](../Integration/06_ManageFixedBookings.md)  



# Select the fiscal year

When you open the *Accounting* module for the first time after login or after reloading the system, a window to select the fiscal year is displayed. You have to select the fiscal year, the month and the journal to display the bookings in the corresponding period. You cannot make any action in the *Accounting* module before selecting a fiscal year.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).

#### Procedure

*Accounting*

![Select fiscal year](../../Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear01.png "[Select fiscal year]")

1. Select a fiscal year in the *Fiscal year* drop-down list.   
  The *Period* date fields are filled in automatically.

  ![Fiscal year fields](../../Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear02.png "[Fiscal year fields]")

2. Select a month in the *Month* drop-down list.

3. Enter a journal number in the *Journal* field. Alternatively, click the [LIST] button to display a new window with the available journals and their bookings.

  > [Info] Journals 1-12 are matched with the corresponding months, irrespectively of whether or not the fiscal year coincides with the calendar year. That means that all bookings registered in the first month of the fiscal year will be found in the journal 1, all bookings registered in the second month of the fiscal year, in the journal 2 and so on.   
  Exceptions to this are special journals, such as the journals 90 to 99, which are defined in the accounting settings for balances carried forward. For detailed information, see [Journal](XX_Journal.md).

4. If required, mark the ![checkbox](../../Assets/Icons/Checkbox.png "[checkbox]") *Include fixed bookings* checkbox and select a batch from the displayed list.

  > [Info] If the *Include fixed bookings* checkbox is selected, all fixed bookings in the selected batch will be automatically booked when opening the selected period in the fiscal year.   
  For detailed information about creating a fixed booking, see [Create a fixed booking](../Integration/06_ManageFixedBookings.md#create-a-fixed-booking).

5. Click the [OK] button in the bottom right corner.   
  The bookings registered in the selected booking period (fiscal year, month and journal) are displayed in the *BOOKINGS* tab in the *Book* menu entry.  
