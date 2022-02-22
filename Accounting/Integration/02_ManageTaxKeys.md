[!!Accounting](Actindo/Accounting)

# Manage the tax keys

Tax keys are a list of values, each of them linked to a specific tax rate. They are essential for the automatic tax functions, for example the automatic VAT tax booking. Every existing tax rate in the different accounts is assigned a tax key. The module *Invoicing* extracts data on the applicable tax rate from the tax keys.


### Prerequisites

- The accounting is configured via the configuration wizard.
- A valid fiscal year is created.

### Procedure

*Accounting > Settings > Tax keys*

You can create, edit, delete or restore your tax keys.   

![Tax keys](/Assets/Screenshots/Accounting/Settings/TaxKeys/Settings_TaxKeys.png "[Tax keys]")

> [Note] The buttons [SAVE] and [SAVE & NEW] have different functions and exclude each other. For this reason, they are not activated simultaneously.

### Create a tax key

1. Click on the button [CLEAR].   
The existing data are cleared. The button [SAVE & NEW] is now activated.

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

2. Enter an available (unassigned) tax key in the field *Key*.

    > [Note] If you use a key that has already been assigned, an error message will be displayed.

3. Enter a description for the tax key in the field *Description*, for example VAT 19%.

4. Enter a validity time frame for the tax key in the field *Valid from - to*.

5.  Click the drop-down list *Tax type* and select the appropriate option:
      - **( )Not specified**
      - **(I)Input tax**
      - **(V)VAT**
      - **(IV)Input tax and VAT**

6. Enter the appropriate data in the field *Percent / Factor*.

    > [Note] Companies selling products to foreign EU countries must be aware of the applicable VAT in the shipping country. It is recommended to check the validity of the tax rate in the corresponding country and update it accordingly in this field.

7. Enter the appropriate account(s) in the field *Account (VAT/VSt/VAT not due)*.

8. Click the drop-down list *VAT needed* and select the appropriate option (**No/Yes**).

9. Click the drop-down list *Country* and select the appropriate EU country or the option **No EU tax key**.

10. Click the button [SAVE & NEW].  
The new tax key has been created.


### Edit a tax key

You can edit existing tax keys from the previously configured chart of accounts, for example if a tax percentage must be updated. Use the button [SAVE] to modify existing tax keys.

> [Warning] Be aware that the existing tax key will be then overwritten, that means, that the existing tax key will be completely replaced by the edited one.

![Edit a tax key](/Assets/Screenshots/Accounting/Settings/TaxKeys/TaxKeys_Button_Save1.png "[Edit a tax key]")

1. Click on the existing tax key to be edited.   
The existing data for the selected tax key are displayed in the corresponding fields.

2. Edit the fields as appropriate. Click the button [SAVE].   
The tax key has been edited. The edited tax key is displayed in the list.


### Delete a tax key

You can delete tax keys that are not applicable to your business. You can also restore the originally configured chart of accounts.

![Delete a tax key](/Assets/Screenshots/Accounting/Settings/TaxKeys/TaxKeys_Button_Delete_Restore.png "[Delete a tax key]")

| (1) | Delete |
|-----|---------------------|
| **(2)** | **Restore** |


1. Click the button [DELETE].  
The selected tax key will be deleted.

    > [Warning] Be aware that the existing tax key will be deleted permanently.

2. Click the button [RESTORE].   
The tax keys will be restored to their original state.

  > [Warning] Be aware that all manual changes will be lost.

[comment]: <> (To be checked with Flo Heusel.)

### Next steps
- [Manage the tax keys](#headingID)
- [Manage the tax keys](#headingID)
- [Set up an account / check tax rate](#headingID)

### See also

- [Invoicing / Turnover treshold activation](#headingID)
- [Leistungsarten / Steuersätze / Steuerklasse](#headingID)
