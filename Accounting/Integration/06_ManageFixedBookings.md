[!!Accounting](Actindo/Accounting)

# Manage the fixed bookings

The *FIXED BOOKINGS* tab in the *Accounting* module enables to automate recurring bookings. The fixed bookings to be automated can be applied when selecting the fiscal year, see [Select the fiscal year](01_Select-the-fiscal-year.md). By doing so, the system will apply automatically the setup fixed bookings in the corresponding fiscal year and journal.


## Create a fixed booking

To create a fixed booking, an existing batch must be selected or a new one must be created first.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).


### Procedure

#### Create a fixed booking batch

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab*

![Create a fixed booking batch](/Assets/Screenshots/Accounting/Settings/FixedBookings/Create_FixedBookingBatch.png "[Create a fixed booking batch]")

1. Click the *Fixed booking batch* drop-down list to check if an applicable batch already exists.

2. If an applicable batch does not exist, select the *New batch* option.

  > [Info]  Per default, the drop-down list displays the *New batch* option.

3. Enter a batch name in the *Name* field.

4. Click the [CREATE] button.   
A new window opens where the new fixed bookings can be registered.


#### Create a fixed booking

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab > Fixed booking batch drop-down list*

![Create a fixed booking](/Assets/Screenshots/Accounting/Settings/FixedBookings/Create_FixedBooking.png "[Create a fixed booking]")

1. Click the *Fixed booking batch* drop-down list and select the fixed booking batch where the fixed booking must be registered.   
The fixed booking window opens automatically. If it does not, click the [CREATE] button.

2. Enter a value in the *Turnover* field.

  > [Info] The booking numbers must be sequential and are added by the system automatically.

3. Enter a contra account number in the *Contra account* field.

  > [Info] When you start typing in the number, a context menu is displayed. You can also select the appropriate option from the menu.

4. Enter the date for the fixed booking in the *Date* field. Date format must be TTMMJJ or TT.MM.JJ.

5. Enter an account number in the *Account* field.

  > [Info] When you start typing in the number, a context menu is displayed. You can also select the appropriate option from the menu.

6. Enter a surname in the *Surname* field.

  > [Info] Note that the fields *Contra account*, *Date* and *Account* must be filled out to be able to create a new fixed booking.

7. Enter any other relevant fixed booking information in the corresponding fields.

8. Click the [BOOK] button.  
A message in the window upper left corner confirms that the booking is registered. The newly created fixed booking is displayed in the fixed booking batch.

  ![Fixed booking created](/Assets/Screenshots/Accounting/Settings/FixedBookings/FixedBookings_Created.png "[Fixed booking created]")

9. Click the [SAVE] button.   
The booking is now saved in the batch.

 > [Info] If you click the [CANCEL] button, the fixed booking will not be saved.

### Next steps

- [Edit a fixed booking](#edit-a-fixed-booking)
- [Delete a fixed booking](#delete-a-fixed-booking)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Edit a fixed booking

You can edit existing fixed bookings registered in a fixed booking batch.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fixed booking batch is created, see [Create a fixed booking batch](#create-a-fixed-booking-batch).
- A fixed booking is created, see [Create a fixed booking](#create-a-fixed-booking).

### Procedure

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab*

![Edit a fixed booking batch](/Assets/Screenshots/Accounting/Settings/FixedBookings/Edit_FixedBookingBatch.png "[Edit a fixed booking batch]")

1. Click the *Fixed booking batch* drop-down list and select the fixed booking batch where the fixed booking to be edited is registered.  
The fixed booking window opens automatically. If it does not, click the [MODIFY] button.

2. Click on the existing fixed booking to be edited.
The existing fixed booking details are displayed in the fields.

  ![Edit a fixed booking](/Assets/Screenshots/Accounting/Settings/FixedBookings/Edit_FixedBookings.png "[Edit a fixed booking]")


3. Make any necessary changes in the fields.

4. Click the [BOOK] button.  
The edited fixed booking is added to the fixed booking batch with a **new** sequential number.

  > [Info] The old fixed booking can be now deleted from the batch. This two-step editing process prevents inadvertently overwriting.

5. Click the [SAVE] button.   
The edited fixed booking is now saved in the batch.  

  > [Info] If you click the [CANCEL] button, the changes will not be saved.

### Next steps

- [Delete a fixed booking](#delete-a-fixed-booking)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Delete a fixed booking

You can delete an existing fixed booking in a fixed booking batch or a complete fixed booking batch.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fixed booking batch is created, see [Create a fixed booking batch](#create-a-fixed-booking-batch).
- A fixed booking is created, see [Create a fixed booking](#create-a-fixed-booking).

### Procedure

#### Delete an existing fixed booking batch

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab*

![Delete an existing batch](/Assets/Screenshots/Accounting/Settings/FixedBookings/Delete_ExistingBatch.png "[Delete an existing batch]")

1. Click the *Fixed booking batch* drop-down list and select the fixed booking batch to be deleted.   

  > [Warning] Be aware that the existing fixed booking batch will be deleted permanently.

2. Click the [DELETE] button.  
A window comes up asking for confirmation. The selected fixed booking batch is deleted.

  > [Info] Note that you may need to refresh the page with the F5 key to see the changes in the Fixed booking batch drop-down list.


#### Delete an existing fixed booking

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab*

![Delete an existing batch](/Assets/Screenshots/Accounting/Settings/FixedBookings/Delete_ExistingBatch.png "[Delete an existing batch]")

1. Click the *Fixed booking batch* drop-down list and select the batch where the fixed booking to be deleted is registered.    
The fixed booking window opens automatically. If it does not, click the [MODIFY] button.

  ![Delete a fixed booking](/Assets/Screenshots/Accounting/Settings/FixedBookings/Delete_FixedBooking.png "[Delete a fixed booking]")

2. Click on the existing fixed booking to be deleted.
The existing booking details are displayed in the fields.

  > [Warning] Be aware that the existing fixed booking will be deleted permanently.

3. Click the [DELETE] button.  
A window comes up asking for confirmation. The selected fixed booking is deleted from the batch.

4. Click the [SAVE] button.   
The deletion is now saved in the batch.

 > [Info] If you click the [CANCEL] button, the deletion will not be saved.

### Next steps

- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
