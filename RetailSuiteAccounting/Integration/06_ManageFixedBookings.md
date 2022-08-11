[!!User Interface Fixed bookings](../UserInterface/02f_FixedBookings.md)  
[!!User Interface Select fiscal year](../UserInterface/00a_FiscalYear.md)  
[!!Select a fiscal year](../Operation/01_SelectFiscalYear.md)  

# Manage the fixed bookings

Fixed bookings are recurring transactions that must be booked regularly, for example facilities costs. The *FIXED BOOKINGS* tab in the *Accounting* module enables to automate recurring bookings. The fixed bookings to be automated can be applied when selecting the fiscal year, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md). By doing so, the system will apply automatically the configured fixed bookings in the corresponding fiscal year and journal.

Fixed bookings can be created, edited and deleted.

[comment]: <> (FH/Doku: Terminologie muss noch durchgängig geändert werden: booking/book -> posting/post. Hier gemischt.)


## Create fixed bookings

To create fixed bookings, a batch must be selected or a new one must be created first.

### Create a fixed booking batch

You can create a fixed booking batch that is not yet available in the system.

#### Prerequisites

A fiscal year has been selected, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).

#### Procedure

*Accounting > Settings > Tab FIXED BOOKINGS*

![Create a fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/CreateFixedBookingBatch.png "[Create a fixed booking batch]")

1. Click the *Fixed booking batch* drop-down list and select the **New batch** option.

  > [Info] By default, the **New batch** option is preselected in the drop-down list.

2. Enter a batch name in the *Name* field.  

3. Click the [CREATE] button.   
The *Fixed bookings &ndash; Batch* window is displayed.

  ![Fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/FixedBookingBatch.png "[Fixed booking batch]")

4. Click the [SAVE] button.  
The notice *Fixed booking batch applied* is displayed in the upper left corner of the window. The created fixed booking batch has been saved in the *Fixed booking batch* drop-down list.

  > [Info] If you click the [CANCEL] button, the fixed booking batch will be rejected.

5. For the next steps to create a fixed booking, follow the procedure [Add a fixed booking](#add-a-fixed-booking) below.


### Add a fixed booking

You can add fixed postings to an existing or a new fixed posting batch.

#### Prerequisites

- A fiscal year has been selected, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).
- A fixed booking batch is created, see [Create a fixed booking batch](#create-a-fixed-booking-batch).

#### Procedure

*Accounting > Settings > Tab FIXED BOOKINGS*

![Select fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBookingBatch.png "[Select fixed booking batch]")

1. Click the *Fixed posting batch* drop-down list and select the fixed posting batch to which you want to add a fixed posting.  
The *Fixed booking &ndash; Batch* window is displayed.  

  > [Info] If the window is not automatically displayed, click the [EDIT] button to display it.

  ![Add a fixed booking](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/FixedBookingBatch.png "[Add a fixed booking]")

2. Leave the *Seq. no.* field empty. The booking numbers are added by the system automatically.

3. Enter the amount to be posted in the *Turnover* field.  

  > [Info] The fields *Turnover*, *Contra account*, *Date* and *Account* must be filled out to add a fixed booking. Otherwise, a warning message is displayed.

4. Enter a contra account number in the *Contra account* field.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list.

5. Enter the date for the fixed booking in the *Date* field. The valid date format is *DDMMYY*.

6. Enter an account number in the *Account* field.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list.

7. If desired, enter any other relevant fixed posting information in the corresponding fields.

8. Click the [BOOK] button.  
The fixed booking is booked. The notice *Booked* is displayed in the upper left corner of the window. The created fixed booking is displayed in the *Fixed bookings &ndash; Batch* window.

  ![Fixed booking added](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/FixedBookingAdded.png "[Fixed booking added]")

9. Click the [SAVE] button.   
The notice *Fixed booking batch applied* is displayed in the upper left corner of the window. The posting has been saved in the batch.

 > [Info] If you click the [CANCEL] button, the fixed posting will be rejected.


## Edit a fixed booking

You can edit fixed postings included in a fixed posting batch.  

The fixed booking editing process comprises two step steps:

  1. reposting the edited booking as a new booking in the fixed booking batch
  2. deleting the old unedited booking from the fixed booking batch

This two-step editing process prevents inadvertently overwriting.

### Prerequisites

- A fiscal year has been selected, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).
- A fixed booking is created, see [Create a fixed booking](#create-a-fixed-booking).

### Procedure

*Accounting > Settings > Tab FIXED BOOKINGS*

![Select fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBookingBatch.png "[Select fixed booking batch]")

1. Click the *Fixed posting batch* drop-down list and select the fixed posting batch where the fixed posting to be edited is included.     
The *Fixed booking &ndash; Batch* window is displayed.

  > [Info] If the window is not automatically displayed, click the [EDIT] button to display it.

  ![Edit a fixed booking](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBooking.png "[Edit a fixed booking]")

2. Click the fixed booking to be edited.  
The details of the selected fixed posting are displayed in the entry fields.

3. Edit the desired data of the fixed booking in the corresponding fields.

4. Click the [BOOK] button.  
A new fixed booking with the indicated modifications is added to the fixed booking batch with a new sequential number.

5. Select now the old unedited fixed booking to delete it.  
The details of the selected fixed booking are displayed in the entry fields.

6. Click the [DELETE] button.  
A confirmation window is displayed.  

  ![Booking delete confirmation](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/BookingDeleteConfirmation.png "[Booking delete confirmation]")

7. Click [OK] if you want to proceed.  
The notice *Deleted* is displayed in the upper left corner of the window.

8. Click the [SAVE] button.   
The notice *Fixed booking batch applied* is displayed in the upper left corner of the window. All changes to the fixed bookings are saved.

  > [Info] If you click the [CANCEL] button, the changes will be rejected.


## Delete a fixed booking

You can delete a fixed booking in a fixed booking batch.

#### Prerequisites

- A fiscal year has been selected, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).
- A fixed booking is created, see [Create a fixed booking](#create-a-fixed-booking).

#### Procedure

*Accounting > Settings > Tab FIXED BOOKINGS*

![Select fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBookingBatch.png "[Select fixed booking batch]")

1. Click the *Fixed posting batch* drop-down list and select the batch where the fixed posting to be deleted is included.  
The *Fixed booking &ndash; Batch* window is displayed.

  > [Info] If the window is not automatically displayed, click the [EDIT] button to display it.

  ![Delete a fixed booking](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBooking.png "[Delete a fixed booking]")


2. Click the fixed posting to be deleted.
  The details of the selected fixed posting are displayed in the entry fields.

  > [Note] Be aware that the fixed posting will be deleted permanently from the fixed postings batch. The fixed posting itself, however, will not be deleted from the system and will continue to be displayed in the *POSTINGS* tab.

3. Click the [DELETE] button.  
A confirmation window is displayed.  

  ![Booking delete confirmation](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/BookingDeleteConfirmation.png "[Booking delete confirmation]")


4.  Click [OK] if you want to proceed.  
The notice *Deleted* is displayed in the upper left corner of the window. The deleted fixed booking is not longer displayed in the fixed booking batch.

5. Click the [SAVE] button.   
The notice *Fixed booking batch applied* is displayed in the upper left corner of the window. The fixed posting deletion has been saved in the fixed booking batch.

 > [Info] If you click the [CANCEL] button, the deletion will be rejected.



## Delete a fixed booking batch

You can delete a fixed posting batch if it is no longer applicable.

#### Prerequisites

- A fiscal year has been selected, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).
- At least one fixed booking batch is created, see [Create a fixed booking batch](#create-a-fixed-booking-batch).

#### Procedure

*Accounting > Settings > Tab FIXED BOOKINGS*

![Delete fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBookingBatch.png "[Delete fixed booking batch]")

1. Click the *Fixed booking batch* drop-down list and select the fixed booking batch to be deleted.   
The *Fixed bookings &ndash; Batch* window is displayed.

  ![Fixed booking batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/EditFixedBooking.png "[Fixed booking batch]")

  > [Note] Be aware that the selected fixed posting batch will be deleted permanently. The postings contained in it, however, will not be deleted but will still be displayed in the *POSTINGS* tab.

2. Click the [DELETE] button.  
A confirmation window is displayed.

  ![Batch delete confirmation](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/BatchDeleteConfirmation.png "[Batch delete confirmation]")

3. Click [OK] if you want to proceed.  
The selected fixed booking batch is deleted from the *Fixed booking batch* drop-down list.

[comment]: <> (Kein "Deleted" Pop-Up-Fenster angezeigt!)
