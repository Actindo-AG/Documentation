[!!Buchhaltung](Actindo/Buchhaltung)

# Manage the accounts for POS

To connect the POS system with accounting, the following accounts must be created for each store:

- an account for representing the pay desk
- an account for cashless payments, e.g. credit or deposit card payments
- a transit account used as contra account for cash deposits or withdrawals not linked to any order or return

The accounts are all created in the same way. The account creation is explained in the following.


## Check the account availability

You may check the availability of a certain account number before creating it as account numbers can only be assigned once.    
Each account number is assigned to a specific number range, which indicates the account class.    
For detailed information about the account classes, see [User Interface Buchhaltung](/Buchhaltung/UserInterface/00_UserInterface.md).

### Prerequisites

- The accounting is configured via the configuration wizard.
- A valid fiscal year is created.

### Procedure

*Buchhaltung > Select the fiscal year > Einstellungen > Tab KONTEN*

![Account availability](/Assets/Screenshots/Buchhaltung/Einstellungen/Konten/Konten01.png "[Account availability]")

| (1) | **drop-down list *Account class*** |
|-----|---------------------|
|**(2)**|**Account list**|


1. Select the corresponding number range in the drop-down list *Account class* .   
  All accounts of the selected account class are displayed in the list.

2. Check which account numbers are still available by navigating through the list.

### Next steps

- [Create an account](#create-an-account)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Buchhaltung](/Buchhaltung/UserInterface/00_UserInterface.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Assign the accounts](06_CreateStore.md#assign-the-accounts)
- [Manage the POS order process](VenduoPOS/Operation/06_ManageOrderProcess.md)


## Create an account

To connect the POS system with accounting, create accounts for your POS store.

### Prerequisites

The account availability is checked, see [Check the account availability](#check-the-account-availability).

### Procedure

*Buchhaltung > Select the financial year > Einstellungen > Tab KONTEN*

![Create Account](/Assets/Screenshots/Buchhaltung/Einstellungen/Konten/Konten02.png "[CreateAccount]")

| (1) | **Field *Account number*** |
|-----|---------------------|
|**(2)**| **Field *Account name*** |
|**(3)**| **drop-down list *Tax type*** |
|**(4)**| **drop-down list *Function*** |
|**(5)**| **Button [SPEICHERN & NEU]** |

1. Enter an available account number in the field *Account number*.

2. Enter an account name in the field *Account name*.

3. Select a tax type for the account in the drop-down list *Tax type*.

4. Select the corresponding function for the account in the drop-down list *Function* .   
  For detailed information, see [User Interface Buchhaltung](/Buchhaltung/UserInterface/00_UserInterface.md).

5. Click the button [SPEICHERN & NEU].   
  The new account is displayed in the account list.

> [Info] Repeat this procedure for each account you want to create.

### Next steps

- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Buchhaltung](/Buchhaltung/UserInterface/00_UserInterface.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Assign the accounts](06_CreateStore.md#assign-the-accounts)
- [Manage the POS order process](VenduoPOS/Operation/06_ManageOrderProcess.md)
