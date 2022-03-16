[!!Accounting](Actindo/Accounting)

# Process bookings

The *Process* menu entry of the *EDIT* context menu in the *BOOKINGS* tab allows to process bookings entered in several booking periods simultaneously.

Any business transaction is first entered in the corresponding journal. Once the transaction is recorded as a journal entry, it must be processed, that is, booked to an account in the general ledger. This is necessary to ensure a correct bookkeeping. Therefore, the bookings must be processed when the accounting for a particular period is finalized.

Once the bookings have been processed, they cannot be changed or deleted any more. If any corrections are necessary, the bookings must be first cancelled, see [Cancel a booking](05_CancelBooking.md). Then, a new correct booking must be created, see [Create a manual booking](04_CreateManualBooking.md).  

[comment]: <> (Unsure, double check info/RS FH)

 > [Info] It is possible to lock one or several months by clicking the *Lock months* menu entry in the *EDIT* context menu. For detailed information about locking months, see [Lock a period for bookings](08_LockPeriodBookings).

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking or multiple bookings have been created, see [Create a manual booking](05_CreateManualBooking).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Process*

![Process bookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Process_Bookings.png "[Process bookings]")

1. Click the *Process* menu entry in the *EDIT* context menu.   
A window opens for you to select the booking period of the bookings to be processed.

  ![Process bookings selection window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Process_Bookings_Window.png "[Process bookings selection window]")

2. Select the journal(s) where the bookings to be processed are recorded in the *Journal* drop-down lists.

3. Select the month(s) where the bookings to be processed are recorded in the *Month* drop-down lists.

  > [Info] Be aware that, once the bookings have been processed, they cannot be changed or deleted any more.

4. Click the [OK] button.   
A confirmation window is displayed. The selected bookings are processed. The [DELETE] button is now greyed out.

[comment]: <> (Where do I see that bookings have been processed? Nothing changes in Bookings tab)

## Next steps

  - [Lock a period for bookings](08_LockPeriodBookings)
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
