[!!Accounting](RetailSuiteAccounting)

# Select the fiscal year

When you open the *Accounting* module for the first time after login or after reloading the system, a window to select the fiscal year is displayed. You have to select the fiscal year, the month and the journal to display the bookings in the corresponding period. You cannot make any action in the *Accounting* module before selecting a fiscal year.

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).

## Procedure

*Accounting*

![Select fiscal year](/Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear01.png "[Select fiscal year]")

1. Select a fiscal year in the *Fiscal year* drop-down list.   
  The *Period* date fields are filled in automatically.

  ![Fiscal year fields](/Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear02.png "[Fiscal year fields]")

2. Select a month in the *Month* drop-down list.

3. Enter a journal number in the *Journal* field. Alternatively, click the [LIST] button to display a new window with the available journals and their bookings.

  > [Info] Journals 1-12 are matched with the corresponding months, irrespectively of whether or not the fiscal year coincides with the calendar year. That means that all bookings registered in the first month of the fiscal year will be found in the journal 1, all bookings registered in the second month of the fiscal year, in the journal 2 and so on.   
  Exceptions to this are special journals, such as the journals 90 to 99, which are defined in the accounting settings for balances carried forward. For detailed information, see [Journal](XX_Journal.md).

4. If required, mark the ![checkbox](/Assets/Icons/Checkbox.png "[checkbox]") *Include fixed bookings* checkbox and select a batch from the displayed list.

  > [Info] If the *Include fixed bookings* checkbox is selected, all fixed bookings in the selected batch will be automatically booked when opening the selected period in the fiscal year.   
  For detailed information about creating a fixed booking, see [Create a fixed booking](06_ManageFixedBookings.md#create-a-fixed-booking).

5. Click the [OK] button in the bottom right corner.   
  The bookings registered in the selected booking period (fiscal year, month and journal) are displayed in the *BOOKINGS* tab in the *Book* menu entry.  

## Next steps

  - [Review an account](02_ReviewAccount.md)
  - [Manage the open items](03_ManageOpenItems.md)
  - [Create a manual booking](04_CreateManualBooking.md)
  - [Cancel a booking](05_CancelBooking.md)
  - [Delete bookings](06_DeleteBookings.md)
  - [Process bookings](07_ProcessBookings.md)
  - [Lock a period for bookings](08_LockPeriodBookings.md)
  - [Split a booking](09_SplitBooking.md)
  - [Manage receipts](10_ManageReceipts.md)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward.md)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations.md)
  - [Access bookings from another period](13_AccessBookingsPeriod.md)
  - [Search in accounting](14_SearchAccounting.md)
  - [Provide the accounting data](15_ProviceAccountingData.md)

## See also

  - [Fiscal year](/RetailSuiteAccounting/UserInterface/01_FiscalYear.md)
  - [Manage the fiscal year](RetailSuiteAccounting/UserInterface/02_ManageFiscalYear.md)
