[!!User Interface balances](../UserInterface/01b_Balances.md)  
[!!User Interface account sheet](../UserInterface/01c_AccountSheet.md)  
[!!User Interface accounts](../UserInterface/02b_Accounts.md)  
[!!Manage the accounts](../Integration/03_ManageAccounts.md)  


# Review an account

The *Book* menu entry in the *Accounting* module contains specific functions to display different views of the data available in the system. All bookings recorded in the *Accounting* module can be filtered per account and period and visually displayed for better clarity or for checking purposes.


## Access the balance view of an account

 The *BALANCES* tab offers a T-account view of the current credit and debit situation, and the resulting balance of a selected account.

 The balance value represents the difference between credits and debits in the account. If the debit and credit totals are equal, the balance is settled. If a difference between them exists, there is an outstanding balance to be settled, for example, a payment must be made to bring the account balance to zero.

 > [Info] When clicking the *BALANCES* tab, a blank tab and the message "No account selected" may be displayed. An account must be selected to display the corresponding details. If a booking is selected in the *BOOKINGS* tab, the account and contra account details corresponding to the selected booking will be displayed in the *BALANCES* tab.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab BALANCES*

![Balances - no account selected](../../Assets/Screenshots/RetailSuiteAccounting/Book/Balances/BalancesNoAccount.png "[Balances - no account selected]")

> [Info] When clicking the *BALANCES* tab, a blank tab and the message "No account selected" may be displayed. An account must be selected to display the corresponding details.

1. Enter an account number in the *Contra account* field.  
The balance for the selected account is displayed on the left side of the workspace.

2. Enter an account number in the *Account* field.  
The balance for the selected account is displayed on the right side of the workspace.

3. Select *[All months]* or *[Only this month]* radio button to filter the values to be displayed as necessary.  
The balance for all months (entire fiscal year) or for the current month is displayed.

  ![Balances](../../Assets/Screenshots/RetailSuiteAccounting/Book/Balances/Balances.png "[Balances]")


## Access the account sheet

The *ACCOUNT SHEET* tab displays a chronologically ordered list of all movements in a specific account. Account sheets can be later used for balance sheet calculations and profit and loss statements.

> [Info] When clicking the *ACCOUNT SHEET* tab, a blank tab and the message "No account selected" may be displayed. An account must be selected to display the corresponding details. If a booking is selected in the *BOOKINGS* tab, the details of the account specified in the *Contra Account* field are displayed in the *ACCOUNT SHEET* tab. If the *Contra Account* field is empty, the details of the account specified in the *Account* field are displayed.


#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab ACCOUNT SHEET*

![Account sheet - no account selected](../../Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet/AccountSheetNoAccount.png "[Account sheet - no account selected]")

> [Info] When clicking the *ACCOUNT SHEET* tab, a blank tab and the message "No account selected" may be displayed. An account or contra account must be selected to display the corresponding details.

1. Enter an account number in the *Contra account* or *Account* field. Press Enter.  
A chronologically ordered list of all bookings in the selected account is displayed in the workspace.

  > [Info] If both *Contra account* and *Account* fields are filled out, for example, if a booking from the *BOOKING* tab is selected, the system displays the details related to the account number entered in the *Contra account* field. If no account number is entered in the *Contra account* field, the system displays the details related to the account number entered in the *Account* field.  

2. Select *[All months]* or *[Only this month]* radio button to filter the bookings to be displayed as necessary.  
The bookings for all months (entire fiscal year) or for the current month are displayed.

  ![Account sheet](../../Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet/AccountSheet.png "[Account sheet]")
