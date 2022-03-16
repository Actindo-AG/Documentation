[!!Accounting](Actindo/Accounting)

# Delete bookings

The *Accounting* module allows to delete bookings in the *Bookings* tab, for example, if content errors are found or if the booking was created for test purposes.

It is possible to delete single bookings or multiple bookings at once. Bear in mind, however, that the bookings to be deleted must be unprocessed, that is, cannot have any related document, payment or cancellation running.

> [Warning] Be aware that any bookings deleted will no longer be available in the system.

## Delete a single booking

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking has been created, see [05_Create a manual booking](05_CreateManualBooking).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Delete booking](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Delete_Booking.png "[Delete booking]")

1. Select the booking to be deleted from the list in the *Bookings* tab.

2. The existing booking details are displayed in the input line fields.

3. Click the *DELETE* button.  
A confirmation window is displayed.
  > [Warning] Be aware that the existing booking will be deleted permanently.

4. Click the [Ok] button to confirm the action.  
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
- Multiple bookings have been created, see [05_Create a manual booking](05_CreateManualBooking).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Delete*

![Bookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Delete_MultipleBookings.png "[Bookings]")

1. Click the *Delete* menu entry in the *EDIT* context menu.   
A window opens for you to select the journal and the sequential numbers of the bookings to be deleted.

  ![Bookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Delete_MultipleBookings_Window1.png "[Bookings]")

2. Select the journal where the bookings to be deleted are recorded in the *Journal* drop-down list.

3. Enter the number range of the bookings to be deleted in the *Seq. numbers* field.

  > [Warning] Be aware that the existing bookings will be deleted permanently.

  ![Bookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Delete_MultipleBookings_Window2.png "[Bookings]")

  [comment]: <> (New screenshot needed - Unschärfe!)

4. Click the [DELETE] button.   
The selected bookings are deleted and will no longer be displayed in the bookings list.

  [comment]: <> (After clicking DELETE, nothing happens: no confirmation window/confirmation message. Journal/seq. numbers selection window turns blank and no further reaction. Page must be reloaded (F5) to display changes. After reloading the changes have been made, i.e. deleted bookings are actually deleted and do not appear in the list any more. RS FH)

### Next steps

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
