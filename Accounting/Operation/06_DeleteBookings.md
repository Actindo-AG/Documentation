[!!Accounting](Actindo/Accounting)

# Delete bookings

The *Accounting* module allows to delete bookings in the *Bookings* tab, for example, if ...

It is possible to delete single bookings or to delete multiple bookings at once.

[comment]: <> (Info in CancelBooking: Once an invoice has been issued and booked, it cannot be simply deleted for legal reasons. The incorrect invoice must be cancelled, recorded as reverse booking in the system, and a new correct booking must be recorded, if necessary.)

 Explain briefly at what time a booking deletion is used and the consequences.

## Delete a single booking

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking has been created [05_Create a manual booking](05_CreateManualBooking).

[comment]: <> (A booking must be created, but not necessarily manually created. Same for Prerequisites in 05_CancelBooking.md)

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Delete booking](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Delete_Booking.png "[Delete booking]")

1. Select the booking to be deleted from the list in the *Bookings* tab.

2. The existing booking details are displayed in the input line fields.

3. Click the *DELETE* button.  
A window comes up asking for confirmation.
  > [Warning] Be aware that the existing booking will be deleted permanently.

4. Click the [OK] button to confirm.
A message above the input line confirms that the booking has been deleted. The deleted booking disappears from the bookings list.

  ![Booking deleted](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Booking_Deleted.png "[Booking deleted]")

### Next steps

  - [Delete multiple bookings](#delete-multiple-bookings)
  - [Process bookings](07_ProcessBookings)
  - [Lock a period for bookings](08_LockPeriodBookings)
  - [Split a booking](09_SplitBooking)
  - [Manage receipts](10_ManageReceipts)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)


## Delete multiple bookings

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking has been created [05_Create a manual booking](05_CreateManualBooking).

[comment]: <> (A booking must be created, but not necessarily manually created. Same for Prerequisites in 05_CancelBooking.md)

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Bookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Cancel_Booking.png "[Bookings]")

1. Select the booking to be cancelled from the list in the *Bookings* tab.

2. The existing booking details are displayed in the input line fields.

3. Click the *CANCEL* button.   
A new  booking is created in the bookings list with a negative turnover value and marked as **Cancel** in the *Booking text* field.

  ![Booking cancelled](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Booking_Cancelled.png "[Booking cancelled]")


### Next steps

  - [Delete bookings](06_DeleteBookings)
  - [Process bookings](07_ProcessBookings)
  - [Lock a period for bookings](08_LockPeriodBookings)
  - [Split a booking](09_SplitBooking)
  - [Manage receipts](10_ManageReceipts)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)
