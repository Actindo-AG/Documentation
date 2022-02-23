[!!Accounting](Actindo/Accounting)

# Manage the tax keys

Tax keys are a list of values, each of them linked to a specific tax rate. They are essential for the automatic tax functions, for example the automatic VAT tax booking. Every existing tax rate in the different accounts is assigned a tax key. The *Invoicing* module extracts data on the applicable tax rate from the tax keys.

## Check the tax key availability

You may check the availability of a certain tax key before creating it, as tax keys can only be assigned once.    
For detailed information about the tax keys, see [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md).

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab TAX KEYS*

![Tax key list](/Assets/Screenshots/Accounting/Settings/TaxKeys/TaxKey_List.png "[Tax key list]")

1. Check which tax keys are still available by navigating through the list.
2.

[comment]: <> (Ich parke das hier. Zu bearbeiten!)

Click on the button [CLEAR].   
The existing data are cleared. The button [SAVE & NEW] is now activated.

> [Info] The buttons [SAVE] and [SAVE & NEW] have different functions and exclude each other. For this reason, they are not activated simultaneously.

### Next steps

- [Create a tax key](#create-a-tax-key)
- [Edit a tax key](#edit-a-tax-key)
- [Delete a tax key](#delete-a-tax-key)
- [Manage the accounts](03_ManageAccounts.md)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Create a tax key

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).
- Check that the tax key to be created available, see [Check tax key availability](#check-the-tax-key-availability).

### Procedure

*Accounting > Settings > Tax keys*

![Create a tax key](/Assets/Screenshots/Accounting/Settings/TaxKeys/Create_TaxKey.png "[Create a tax key]")

1. Enter an available tax key in the field *Key*.

    > [Info] If you use a key that has already been assigned, an error message will be displayed.

2. Enter a description for the tax key in the field *Description*, for example VAT 19%.

3. Enter a validity time frame for the tax key in the field *Valid from - to*.

4.  Click the drop-down list *Tax type* and select the appropriate option:
      - **( )Not specified**
      - **(I)Input tax**
      - **(V)VAT**
      - **(IV)Input tax and VAT**

5. Enter the appropriate data in the field *Percent / Factor*.

    > [Info] Companies selling products to foreign EU countries must be aware of the applicable VAT in the shipping country. It is recommended to check the validity of the tax rate in the corresponding country and update it accordingly in this field.

6. Enter the appropriate account(s) in the field *Account (VAT/VSt/VAT not due)*.

7. Click the drop-down list *VAT needed* and select the appropriate option (**No/Yes**).

8. Click the drop-down list *Country* and select the appropriate EU country or the option **No EU tax key**.

9. Click the button [SAVE & NEW].  
The new tax key has been created.

### Next steps

- [Edit a tax key](#edit-a-tax-key)
- [Delete a tax key](#delete-a-tax-key)
- [Manage the accounts](03_ManageAccounts.md)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
- [Invoicing Turnover treshold activation](#headingID)
- [Leistungsarten / Steuersätze / Steuerklasse](#headingID)


## Edit a tax key

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).


### Procedure

*Accounting > Settings > Tax keys*


1. Click on the existing tax key to be edited.   
The existing data for the selected tax key are displayed in the corresponding fields.

    > [Warning] Be aware that any changes made to an existing tax key will overwrite the preset values.

2. Edit the fields as appropriate.

3. Click the button [SAVE].   
The tax key has been edited. The edited tax key is displayed in the list.


### Next steps

- [Delete a tax key](#delete-a-tax-key)
- [Manage the accounts](03_ManageAccounts.md)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
- [Invoicing Turnover treshold activation](#headingID)
- [Leistungsarten / Steuersätze / Steuerklasse](#headingID)


## Delete a tax key

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).


### Procedure

*Accounting > Settings > Tax keys*


1. Select the tax key to be deleted.

2. Click the button [DELETE].  
The selected tax key will be deleted.

    > [Warning] Be aware that the existing tax key will be deleted permanently.


### Next steps

- [Manage the accounts](03_ManageAccounts.md)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
- [Invoicing Turnover treshold activation](#headingID)
- [Leistungsarten / Steuersätze / Steuerklasse](#headingID)
