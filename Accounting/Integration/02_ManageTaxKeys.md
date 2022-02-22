[!!Accounting](Actindo/Accounting)

# Manage the tax keys

Tax keys are a list of values, each of them linked to a specific tax rate. They are essential for the automatic tax functions, for example the automatic VAT tax booking. Every existing tax rate in the different accounts is assigned a tax key. The module *Invoicing* also extracts data on the applicable tax rate from the tax keys.


### Prerequisites

- The accounting is configured via the configuration wizard.
- A valid fiscal year is created.

### Procedure

### Create a tax key

*Accounting > Settings > Tax keys*

To create a new tax key, you have to click the button [CLEAR] first.
The button [SAVE & NEW] is now active.

> [Note] The buttons [SAVE] and [SAVE & NEW] have different functions and exclude each other.


![Tax keys](/Assets/Screenshots/Accounting/Settings/TaxKeys/Settings_TaxKeys.png "[Tax keys]")

1. Click on the button [CLEAR].   
The existing data are cleared.

    ![Create a tax key](/Assets/Screenshots/Accounting/Settings/TaxKeys/TaxKeys_Button_Save&New.png "[Create a tax key]")

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

    > [Note] If you use a number that has already been assigned, an error message will be displayed.

3. Enter a description for the tax key in the field *Description*, for example VAT 19%.

4. Enter a validity time frame for the tax key in the field *Valid from - to*.

5.  Click the drop-down list *Tax type* and select the appropriate option:
      - **( )Not specified**
      - **( )Input tax**
      - **( )VAT**
      - **( )Input tax and VAT**

6.






### Edit a tax key

You can use existing tax keys from the previously configured chart of accounts and edit it, for example if a tax percentage must be updated. The button [SAVE] can be used to modify existing tax keys.

> [Warning] Be aware that the existing tax key will be then overwritten, that means, that the values stored under the edited tax key will be lost.




### Delete a tax key



> [Warning] If you information about the consequences of cancelation and deletion
