[!!Accounting](Actindo/Accounting)

# Select the fiscal year

When you open the *Accounting* module for the first time after login or after reloading the system, the window to select a fiscal year is displayed. You have to select the fiscal year and the journal to display the bookings in the corresponding period. You cannot make any action in the *Accounting* module before selecting the fiscal year.

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).

## Procedure

*Accounting*

![Select fiscal year](/Assets/Screenshots/Accounting/Select_FiscalYear_view.png "[Select fiscal year]")

1. Select a fiscal year in the *Fiscal year* drop-down list.   
  The *Period* date fields are filled in automatically.

  ![Fiscal year fields](/Assets/Screenshots/Accounting/Select_FiscalYear_window.png "[Fiscal year fields]")

2. Select a month in the *Month* drop-down list.

3. Enter a journal number in the *Journal* field. Alternatively, click the [LIST] button to display a new window with the available journals and their bookings.

  > [Info] The journal number corresponds to the number of the month, so all bookings of the month January can be found in the journal number 1, all bookings of the month February in the journal number 2 and so on.   
  Exceptions to this are special journals, such as the journals 90 to 99, which are defined in the accounting settings for balances carried forward.     

4. If required, select the *Include fixed bookings* checkbox ![checkbox](/Assets/Icons/checkbox.png "[checkbox]") and select a batch in the displayed list.

  > [Info] If the *Include fixed bookings* checkbox is selected, all fixed bookings in the selected batch will be automatically booked when opening the selected period in the fiscal year.   
  For detailed information about creating a fixed booking, see [Create a fixed booking](06_ManageFixedBookings.md#create-a-fixed-booking).

5. Click the [OK] button in the bottom right corner.   
  The *Book* menu entry with the *BOOKINGS* tab is displayed. The selected fiscal year and journal is preselected.  

[comment]: <> (I used "Batch" for Stapel in Fixed bookings. I found it in Internet, e.g. DATEV Website. Batch or stack for Stapel? Actually, posting batch seems to be more usual than booking batch.)

## Next steps

  - [Review an account](#to_be_completed)
  - [Manage the open items](#to_be_completed)
  - [Create a manual booking](#to_be_completed)
  - [Cancel a booking](#to_be_completed)
  - [Delete bookings](#to_be_completed)
  - [Process bookings](#to_be_completed)
  - [Lock a period for bookings](#to_be_completed)
  - [Split a booking](#to_be_completed)
  - [Manage receipts](#to_be_completed)
  - [Create a balance carried forward](#to_be_completed)
  - [Book exchange rate fluctuations](#to_be_completed)
  - [Access bookings from another period](#to_be_completed)
  - [Search in accounting](#to_be_completed)
  - [Provide the accounting data](#to_be_completed)

## See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [To be completed](#to_be_completed)
  [comment]: <> (Repeat references done within the file, e.g. create a fixed booking?)
