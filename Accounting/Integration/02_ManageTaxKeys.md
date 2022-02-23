[!!Accounting](Actindo/Accounting)

# Manage the tax keys

Tax keys are a list of values, each of them linked to a specific tax rate. They are essential for the automatic tax functions, for example the automatic VAT tax booking. Every existing tax rate in the different accounts is assigned a tax key. The *Invoicing* module extracts data on the applicable tax rate from the tax keys.


## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).



## Procedure

*Accounting > Settings > Tax keys*

![Tax keys](/Assets/Screenshots/Accounting/Settings/TaxKeys/TaxKeys_Screen.png "[Tax keys]")


### Create a tax key

1. Click on the button [CLEAR].   
The existing data are cleared. The button [SAVE & NEW] is now activated.

    > [Info] The buttons [SAVE] and [SAVE & NEW] have different functions and exclude each other. For this reason, they are not activated simultaneously.

    ![Create a tax key](/Assets/Screenshots/Accounting/Settings/TaxKeys/TaxKeys_Buttons.png "[Create a tax key]")

   | (1) | Key |
   |-----|---------------------|
   | **(2)** | **Description** |
   | **(3)** | **Valid from - to** |
   | **(4)** | **Tax type** |
   | **(5)** | **Percent / Factor** |
   | **(6)** | **Accounts (VAT/VSt/VAT not due)** |
   | **(7)** | **VAT-ID needed** |
   | **(8)** | **Country** |
   | **(9)** | **SAVE & NEW** |
   | **(10)** | **CLEAR** |

[comment]: <> (Wenn keine Legende/Screenshot-Closeup, wie soll der Kunde wissen, worauf es sich bezieht? Text auf EN -> Screenshots noch auf DE? Abschnitte: hier Screenshot einfach weglassen? Ganzes Bildschirm nicht so einfach lesbar, oder kann man danach darauf klicken und vergrößern?)

[comment]: <> (Style guide: Max. 7 steps. Einige Felder weglassen?)

2. Enter an available tax key in the field *Key*.

    > [Info] If you use a key that has already been assigned, an error message will be displayed.

3. Enter a description for the tax key in the field *Description*, for example VAT 19%.

4. Enter a validity time frame for the tax key in the field *Valid from - to*.

5.  Click the drop-down list *Tax type* and select the appropriate option:
      - **( )Not specified**
      - **(I)Input tax**
      - **(V)VAT**
      - **(IV)Input tax and VAT**
[comment]: <> (Optionen löschen?)

6. Enter the appropriate data in the field *Percent / Factor*.

    > [Info] Companies selling products to foreign EU countries must be aware of the applicable VAT in the shipping country. It is recommended to check the validity of the tax rate in the corresponding country and update it accordingly in this field.

7. Enter the appropriate account(s) in the field *Account (VAT/VSt/VAT not due)*.

8. Click the drop-down list *VAT needed* and select the appropriate option (**No/Yes**).

9. Click the drop-down list *Country* and select the appropriate EU country or the option **No EU tax key**.

10. Click the button [SAVE & NEW].  
The new tax key has been created.


### Edit a tax key

1. Click on the existing tax key to be edited.   
The existing data for the selected tax key are displayed in the corresponding fields.

    > [Warning] Be aware that any changes made to an existing tax key will overwrite the preset values.

2. Edit the fields as appropriate.

3. Click the button [SAVE].   
The tax key has been edited. The edited tax key is displayed in the list.


### Delete a tax key

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
