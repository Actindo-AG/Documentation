[!!Accounting](Actindo/Accounting)

# Process bookings

The *Lock months* menu entry of the *EDIT* context menu in the *BOOKINGS* tab allows to lock or unlock months to process the bookings...


[comment]: <> (Unsure, double check info/RS FH)

- information about the consequences of locking a certain period
- information about how to unlock a certain period
- information about the difference to process bookings

- Explain why locking a certain period for bookings is important, what it is used for and at what time.

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking or multiple bookings have been created, see [05_Create a manual booking](05_CreateManualBooking).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Lock months*

![Lock months](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_LockMonths.png "[Lock months]")

1. Click the *Lock months* menu entry in the *EDIT* context menu.
A window opens for you to select the booking months to be locked.

  ![Lock months window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_LockMonths_Window.png "[Lock months window]")

2. Select the journal(s) where the bookings to be processed are recorded in the *Journal* drop-down lists.

3. Select the month(s) where the bookings to be processed are recorded in the *Month* drop-down lists.

  > [Info] Be aware that, once the bookings have been processed, they cannot be changed or deleted any more.

4. Click the [OK] button.
A confirmation window is displayed. The selected bookings are processed. The [DELETE] button is now greyed out.

[comment]: <> (Where do I see that bookings have been processed? Nothing changes in Bookings tab)

## Next steps

  - [Split a booking](09_SplitBooking)
  - [Manage receipts](10_ManageReceipts)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

## See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)
