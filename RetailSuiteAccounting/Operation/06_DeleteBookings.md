[!!Accounting](RetailSuiteAccounting)

# Delete bookings

The *Accounting* module allows to delete bookings in the *Bookings* tab, for example, if content errors are found or if the booking was created for test purposes.

It is possible to delete single bookings or multiple bookings at once. Bear in mind, however, that the bookings to be deleted must be unprocessed. For detailed information, see [Process bookings](07_ProcessBookings.md). In fact, a booking that has already been processed cannot be deleted, as the [DELETE] button will change to inactive (greyed out) when clicking on a unprocessed booking.

## Delete a single booking

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A booking has been created, see [Create a manual booking](05_CreateManualBooking).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Delete booking](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/DeleteBooking.png "[Delete booking]")

1. Select the booking to be deleted from the list in the *Bookings* tab.

2. The existing booking details are displayed in the input line fields.

3. Click the [DELETE] button.  
A confirmation window is displayed.

  > [Warning] Be aware that the existing booking will be deleted permanently.

4. Click the [Ok] button to confirm the action.  
A message above the input line confirms that the booking has been deleted. The deleted booking will no longer be displayed in the bookings list.

  ![Booking deleted](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/BookingDeleted.png "[Booking deleted]")

### Next steps

 - [Delete multiple bookings](#delete-multiple-bookings)
 - [Process bookings](07_ProcessBookings.md)
 - [Lock a period for bookings](08_LockPeriodBookings.md)
 - [Split a booking](09_SplitBooking.md)
 - [Manage receipts](10_ManageReceipts.md)
 - [Create a balance carried forward](11_CreateBalanceCarriedForward.md)
 - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations.md)
 - [Access bookings from another period](13_AccessBookingsPeriod.md)
 - [Search in accounting](14_SearchAccounting.md)
 - [Provide the accounting data](15_ProviceAccountingData.md)

### See also

  - [Delete](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)

  [comment]: <> (Delete function is actually used to delete multiple bookings. No reference in UI chapters to [DELETE] button.)


## Delete multiple bookings

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- Multiple bookings have been created, see [Create a manual booking](05_CreateManualBooking).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Delete*

![Delete multiple bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/DeleteMultipleBookings.png "[Delete multiple bookings]")

1. Click the *Delete* menu entry in the *EDIT* context menu.   
A window opens for you to select the journal and the sequential numbers of the bookings to be deleted.

  ![Select multiple bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/DeleteMultipleBookings01.png "[Select multiple bookings]")

2. Select the journal where the bookings to be deleted are recorded in the *Journal* drop-down list.

3. Enter the number range of the bookings to be deleted in the *Seq. numbers* field.

  > [Warning] Be aware that the existing bookings will be deleted permanently.

  ![Multiple bookings selected](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/DeleteMultipleBookings02.png "[Multiple bookings selected]")

4. Click the [DELETE] button.   
The selected bookings are deleted and will no longer be displayed in the bookings list.

> [Info] It may be necessary to click on a different tab and switch back the *Bookings* tab to display the changes in the bookings list.

### Next steps

 - [Process bookings](07_ProcessBookings.md)
 - [Lock a period for bookings](08_LockPeriodBookings.md)
 - [Split a booking](09_SplitBooking.md)
 - [Manage receipts](10_ManageReceipts.md)
 - [Create a balance carried forward](11_CreateBalanceCarriedForward.md)
 - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations.md)
 - [Access bookings from another period](13_AccessBookingsPeriod.md)
 - [Search in accounting](14_SearchAccounting.md)
 - [Provide the accounting data](15_ProviceAccountingData.md)

### See also

  - [Delete](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
