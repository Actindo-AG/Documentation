[!!Accounting](Actindo/Accounting)

# Manage the fixed bookings

The *Fixed bookings* tab in the *Accounting* module enables to automate recurring bookings. The fixed bookings to be automated can be applied when selecting the fiscal year, see [Select the fiscal year](01_Select-the-fiscal-year.md). By doing so, the system will apply automatically the setup fixed bookings in the corresponding fiscal year and journal, and therefore, this bookings will not have to be entered manually.


## Create a new fix booking batch

Before creating a fixed booking, an existing batch must be selected or a new one must be created.

[comment]: <> (Maybe better to create two separate sub-procedures: Create a new fixed booking batch and Modify an existing fixed booking batch??? In Sandbox, nothing different seems to happen when clicking on ANLEGEN and ÄNDERN. Fixed booking window opens automatically when selecting from drop-down list. Maybe separate procedure for Delete batch? or sub-procedures? create / modify? / delete)

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).

### Procedure

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab*

![Create a new batch](/Assets/Screenshots/Accounting/Settings/FixedBookings/Create_NewBatch.png "[Create a new batch")

1. Click the *Fixed booking batch* drop-down list to check if an applicable batch already exists.

2. If an applicable batch does not exist, select the *New batch* option.

  > [Info]  Per default, the drop-down list displays the *New batch* option.

3. Enter a batch name in the *Name* field.

4. Click the [CREATE] button.   
A new window opens up where the new fixed bookings can be registered.

[comment]: <> (Heusel fragen: WAS MACHT ÄNDERN?)

## Delete an existing fix booking batch

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fixed booking batch is created, see [Create a new batch](#create-a-new-batch).

### Procedure

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab*

![Delete an existing batch](/Assets/Screenshots/Accounting/Settings/FixedBookings/Delete_ExistingBatch.png "[Delete an existing batch]")

1. Click the *Fixed booking batch* drop-down list and select the fixed booking batch to be deleted.   
The fixed booking window opens automatically.

  > [Warning] Be aware that the existing fixed booking batch will be deleted permanently. Deleting a batch will also delete all fixed bookings contained in it.

2. Click the [DELETE] button.  
A window comes up asking for confirmation. The selected fixed booking batch is deleted.

  > [Info] Note that you may need to refresh the page with the F5 key to see the changes in the Fixed booking batch drop-down list.

### Next steps

- [Create a fixed booking](#create-a-fixed-booking)
- [Edit a fixed booking](#edit-a-fixed-booking)
- [Delete a fixed booking](#delete-a-fixed-booking)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Create a fixed booking

You can create fixed bookings in an existing batch.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fixed booking batch is created, see [Create a new batch](#create-a-new-batch).

### Procedure

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab > Fixed booking batch drop-down list*

![Create a fixed booking](/Assets/Screenshots/Accounting/Settings/FixedBookings/Create_FixedBookings.png "[Create a fixed booking]")

1. Enter a value in the *Turnover* field.

  > [Info] The booking numbers must be sequential and are added by the system automatically.

2. Enter a contra account number in the *Contra account* field.

  > [Info] When you start typing in the number, a context menu is displayed. You can also select the appropriate option from the menu.

3. Enter the date for the fixed booking in the *Date* field. Date format must be TTMMJJ or TT.MM.JJ.

4. Enter an account number in the  *Account* field.

  > [Info] When you start typing in the number, a context menu is displayed. You can also select the appropriate option from the menu.

5. Enter a surname in the *Surname* field.

  > [Info] Note that the fields *Contra account*, *Date* and *Account* must be filled out to be able to create a new fixed booking.

6. Enter any other relevant fixed booking information in the corresponding fields.

7. Click the [BOOK] button.  
A message in the window upper left corner confirms that the booking is registered. The newly created fixed booking is displayed in the fixed booking batch.

  ![Fixed booking created](/Assets/Screenshots/Accounting/Settings/FixedBookings/FixedBookings_Created.png "[Fixed booking created]")

8. Click the [SAVE] button.   
The booking is now saved in the batch.

 > [Info] If you click the [CANCEL] button, the booking will not be saved.

### Next steps

- [Edit a fixed booking](#edit-a-fixed-booking)
- [Delete a fixed booking](#delete-a-fixed-booking)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Edit a fixed booking

[comment]: <> (Heusel fragen: Button SPEICHERN does not seem to work. Bug? In Buchen werden aber alle Versuche mit einer neuen Lfd. Nr. anscheinend gespeichert! Noch testen!)

You can edit an existing fixed booking, for example if a setting must be changed.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fixed booking batch is created, see [Create a fixed booking batch](#create-a-batch).
- A fixed booking  is created, see [Create a fixed booking](#create-a-fixed-booking).

### Procedure

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab > Fixed booking batch drop-down list*

![Edit a fixed booking](/Assets/Screenshots/Accounting/Settings/FixedBookings/Edit_FixedBookings.png "[Edit a fixed booking")

1. Click the *Fixed booking batch* drop-down list and select the batch where the fixed booking to be edited is registered.  
The fixed booking window opens automatically. If the fixed booking window does not open automatically, click the [MODIFY] button.

2. Click on the existing fixed booking to be edited.
The existing fixed booking details are displayed in the fields.

  > [Warning] Be aware that any changes made to an existing fixed booking will overwrite the existing values.

[comment]: <> (Flo Heusel: from here on... nothing happens!)

3. Click the [SAVE] button.   
The edited fixed booking is now saved in the batch.

 > [Info] If you click the [CANCEL] button, the ... will not be saved.

  > [Info] Note that you may need to refresh the page with the F5 key to see the changes in the Fixed booking batch drop-down list.

### Next steps

- [Delete a fixed booking](#delete-a-fixed-booking)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Delete a fixed booking

You can delete an existing fixed booking, for example if it is no longer applicable.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fixed booking batch is created, see [Create a new batch](#create-a-new-batch).

### Procedure

*Accounting > Select the fiscal year > Settings > FIXED BOOKINGS tab > Fixed booking batch drop-down list*

![Delete a fixed bookings](/Assets/Screenshots/Accounting/Settings/FixedBookings/Delete_FixedBookings.png "[Delete a fixed booking")

1. Click the *Fixed booking batch* drop-down list and select the batch where the fixed booking to be deleted is registered.  
The fixed booking window opens automatically.

2. Click on the existing fixed booking to be deleted.
The existing booking details are displayed in the fields.

  > [Warning] Be aware that the existing fixed booking will be deleted permanently.

3. Click the [DELETE] button.  
A window comes up asking for confirmation. The selected fixed booking is deleted.

4. Click the [SAVE] button.   
The deletion is now saved in the batch.

 > [Info] If you click the [CANCEL] button, the deletion will not be saved.

### Next steps

- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
