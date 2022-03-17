[!!Accounting](Actindo/Accounting)

# Lock a period for bookings

The *Lock months* menu entry of the *EDIT* context menu in the *BOOKINGS* tab allows to lock months for bookings.

Once the bookings have been processed, the booking period (month) is closed and no further changes can be made. The booking period can be locked in the system to avoid any automatic bookings for this period. When a booking period is locked, any subsequent transaction will be booked automatically in the following bookable booking period.

[comment]: <> (Still unsure: journal vs month - why is it called "Monat sperren" and not "Journal/BP sperren"?)

It is also possible to unlock a locked booking period. Then, this period becomes bookable again. Any subsequent transaction will be booked automatically in the first bookable (unlocked) journal.

> [Info] In contrast to the processing of bookings, months locking can be undone if necessary, that is, locked months can be made bookable again. For detailed information about process bookings, see [Process bookings](07_ProcessBookings.md).

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking or multiple bookings have been created, see [Create a manual booking](05_CreateManualBooking).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Lock months*

![Lock months](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_LockMonths.png "[Lock months]")

1. Click the *Lock months* menu entry in the *EDIT* context menu.  
A window opens for you to select the month(s) to be locked for bookings.

  ![Lock months window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_LockMonths_Window2.png "[Lock months window]")

2. Lock the month(s) as necessary by selecting *Locked* in the drop-down list of the corresponding month(s).

  > [Info] This action can be reversed by selecting the *bookable* option in the drop-down list for the corresponding month(s).

3. Click the [OK] button.  
A pop-up window is displayed shortly to confirm that the changes are being saved. The selected month(s) are now locked for bookings.

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
