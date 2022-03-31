[!!Accounting](RetailSuiteAccounting)

# Manage the accounts

The accounts are set up during the configuration process via the accounting wizard, see [Charts of accounts](01_RunAccountingWizard.md#chart-of-accounts). However, you can create, edit or delete an account if necessary in the *Accounting* module, for example if a specific account is not yet available in the system or the settings of an existing one need to be adjusted.

> [Warning] Any modifications in the accounts have far-reaching consequences for the *Accounting* module and the system automatic bookings. It is highly recommended not to make any changes in the accounts, unless you have an in-depth knowledge of their functions. In case of doubt, contact our support team.


## Check the account availability

You may check the availability of a certain account number before creating it as account numbers can only be assigned once.    
Each account number is assigned to a specific number range, which indicates the account class.    
For detailed information about the account classes, see [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md).

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab ACCOUNTS*

![Account availability](/Assets/Screenshots/Accounting/Settings/Accounts/Account_availability.png "[Account availability]")

1. Select the corresponding number range in the drop-down list *Account class*.   
  All accounts of the selected account class are displayed in the list.

2. Check which account numbers are still available by navigating through the list.

### Next steps

- [Create an account](#create-an-account)
- [Edit an account](#edit-an-account)
- [Delete an account](#delete-an-account)
- [Manage the accounts](03_ManageAccounts.md)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Create an account

You can create an account that is not yet available in the system.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).
- The account availability is checked, see [Check the account availability](#check-the-account-availability).
- The tax key validity is checked and, if necessary, updated, see [Edit a tax key](#edit-a-tax-key).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab ACCOUNTS*

![Create an account](/Assets/Screenshots/Accounting/Settings/Accounts/Create_account.png "[Create an account]")

1. Enter an available account number in the field *Account number*.

2. Enter an account name in the field *Description*.

3. Click the drop-down list *Tax type* and select the appropriate option:

      - **( )Not tax**
      - **(I)Input tax**
      - **(V)VAT**
      - **(IV)Input tax and VAT**
      - **(NV)No VAT possible**


4. Click the drop-down list *Tax key/auto* and select the appropriate option.
  > [Info] Before creating an account, it is recommended to check the validity of the tax rate in the corresponding country in the tab TAX KEYS.

5. Click the drop-down list *Special features* and select the appropriate option:

     - **( )Normal**
     - **(L)Locked**
     - **(DA)Debtor collective account**
     - **(CA)Creditor collective account**
     - **(MT)Money transit account**


6. Select the corresponding function for the account in the drop-down list *Function* .   
  For detailed information, see [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md).

[comment]: <> (If reference to UserInterface is made and all drop-down list options explained there, maybe delete drop-down list options in points 3 and 4 too?)

7. Click the drop-down list *Currency* and select the appropriate option.

8. Click the button [SAVE & NEW].   
  The new account is displayed in the account list.

### Next steps

- [Edit an account](#edit-an-account)
- [Delete an account](#delete-an-account)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Edit an account

You can edit an existing account, for example if a tax rate needs to be updated.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab ACCOUNTS*

![Edit an account](/Assets/Screenshots/Accounting/Settings/Accounts/Edit_account.png "[Edit an account]")

1. Select the corresponding number range in the drop-down list *Account class*.   
  All accounts of the selected account class are displayed in the list.

2. Select the account to be edited.
  > [Warning] Be aware that any changes made to an existing account will overwrite the preset values.

3. Edit the fields as appropriate.

4. Click the button [SAVE].   
The account has been edited. The edited account is displayed in the list.


### Next steps

   - [Delete an account](#delete-an-account)
   - [Manage the fiscal year](04_ManageFiscalYear.md)
   - [Manage the customer/supplier](05_ManageCustomerSupplier.md)
   - [Manage the fixed bookings](06_ManageFixedBookings.md)
   - [Manage the BWA reports](07_ManageBWAReports.md)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)


## Delete an account

You can delete an existing account, for example if it is no longer applicable.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab ACCOUNTS*

![Delete an account](/Assets/Screenshots/Accounting/Settings/Accounts/Delete_account.png "[Delete an account]")

1. Select the account to be deleted.
  > [Warning] Be aware that the existing tax key will be deleted permanently.

2. Click the button [DELETE].  
The selected account has been deleted.

### Next steps

- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
