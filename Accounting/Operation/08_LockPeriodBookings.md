[!!Accounting](Actindo/Accounting)

# Lock a period for bookings

The *Lock months* menu entry of the *EDIT* context menu in the *BOOKINGS* tab allows to lock months for bookings.


- information about the consequences of locking a certain period
- information about how to unlock a certain period - done
- information about the difference to process bookings - link to process bookings + update 07_ProcessBookings.md if necessary

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
A window opens for you to select the months to be locked for bookings.

  ![Lock months window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_LockMonths_Window.png "[Lock months window]")

2. Lock the month(s) as necessary by selecting *Locked* in the drop-down list of the corresponding month(s).

  > [Info] This action can be reversed by selecting the *bookable* option in the drop-down list for the corresponding month(s).

3. Click the [OK] button.  
A pop-up window is displayed shortly to confirm that the change is being saved. The selected month(s) are now locked for bookings.

[comment]: <> (More info/research needed!)

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
