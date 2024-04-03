[!!Create a store in POS](./06_CreateStore.md)
[!!Manage the POS order process](../Operation/06_ManageOrderProcess.md)
[!!User interface Accounts](../../RetailSuiteAccounting/UserInterface/02b_Accounts.md)


# Manage the accounts for POS

To connect the POS system with accounting, the following accounts must be created for each store:

- an account for representing the pay desk
- an account for cashless payments, for instance credit or deposit card payments
- a transit account used as contra account for cash deposits or withdrawals not linked to any order or return

The accounts are all created in the same way. The account creation is explained in the following.


## Check the account availability

You may check the availability of a certain account number before creating it as account numbers can only be assigned once.    
Each account number is assigned to a specific number range, which indicates the account class.    

[comment]: <> (add link to account classes in Accounting module if available)


#### Prerequisites

- The accounting is configured via the configuration wizard.
- A valid fiscal year is created.

#### Procedure

*Accounting > Select the fiscal year > Settings > Tab ACCOUNTS*

![Accounts](../../Assets/Screenshots/RetailSuiteAccounting/Settings/Accounts/CreateAccount.png "[Accounts]")

1. Select the corresponding number range in the *Account class* drop-down list.   
    All accounts of the selected account class are displayed in the list.

2. Check which account numbers are still available by navigating through the list.



## Create an account

To connect the POS system with accounting, create accounts for your POS store.

#### Prerequisites

The account availability is checked, see [Check the account availability](#check-the-account-availability).

#### Procedure

*Accounting > Select the fiscal year > Settings > Tab ACCOUNTS*

![Accounts](../../Assets/Screenshots/RetailSuiteAccounting/Settings/Accounts/CreateAccount.png "[Accounts]")

1. Enter an available account number in the *Account number* field.

2. Enter an account name in the *Account name* field.

3. Select a tax type for the account in the *Tax type* drop-down list .

4. Select the corresponding function for the account in the *Function* drop-down list .   

[comment]: <> (add link to Accounting module if available)

5. Click the [SAVE & NEW] button.   
    The new account is displayed in the account list.

> [Info] Repeat this procedure for each account you want to create.
