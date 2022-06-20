[!!Accounting](RetailSuiteAccounting)

# Balance carried forward

*Accounting > Select fiscal year > Settings > Tab BALANCE CARRIED FORWARD*

![Balance carried forward](/Assets/Screenshots/RetailSuiteAccounting/Settings/BalanceCarriedForward/BalanceCarriedForward.png "[Balance carried forward]")

This tab displays the special journals preconfigured in the system to carry balances and open items forward. Besides, it allows to customize the preconfigured journals as well as to create new ones. For detailed information about creating a balance carried forward, see [Create a balance carried forward](/RetailSuiteAccounting/Operation/11_CreateBalanceCarriedForward.md).


- *Account class*  
Click the drop-down list to select the desired account class. Each account class is linked to a special journal preconfigured in the system as detailed in the table below:

  | Account class  | Journal       | Description  |
  |:-------------:|:-------------:|:-------------:|
  | 1      | 90 | Financial accounts |
  | 2      | 91 | Impersonal accounts |
  | 3      | 92 | Input tax + VAT |
  | 4      | 93 | P&L |
  | 8      | 98 | Open items debtors |
  | 9      | 99 | Open items creditors |

  This preconfigured values can be edited, if necessary. Account classes 5-7 are freely configurable.

- *Journal*  
The journal displayed in this field is preconfigured and changes according to the account class selected (see table above). The preconfigured values can be edited, if necessary.

- *Description*  
The description displayed in this field is preconfigured and changes according to the account class selected (see table above). The preconfigured values can be edited, if necessary.

- *Function*  
Click the drop-down list to select the appropriate function for the selected account class. This value is preselected for the preconfigured account classes as follows:

  - **Balances**  
  This function is used to transfer outstanding account balances from one fiscal year to the next one. This value is preselected for the preconfigured account classes 1 to 4.

  - **Open items**  
  This function is used to transfer open items from one fiscal year to the next one. This value is preselected for the preconfigured account classes 8 and 9, that is personal accounts (debtors and creditors).


- *Debit/credit account*  
Enter the applicable debit/credit accounts, if necessary. This value is preset for the preconfigured account classes.

- *Contra account*  
Enter the applicable contra account. This value is preset for the preconfigured account classes 3 and 4.

- *Accounts from - to*  
Enter the applicable accounts. These values are preset for the preconfigured account classes.


- [SAVE]  
Click this button to save any changes made.

  > [Warning] Any changes made will overwrite the preconfigured values.

- [DELETE]  
Click this button to delete a selected account class.

  > [Info] The preconfigured account classes cannot be deleted, therefore the [DELETE] is grayed out when these account classes are selected.

[comment]: <> (Unsicher, denn selbsterstellte Kontenklassen lassen sich mit LÖSCHEN-Button auch NICHT löschen. Es ist tatsächlich immer ausgegraut. Bug?)

- [CLEAR]  
Click this button to clear all entry fields.  

[comment]: <> (Button scheint nicht zu funktionieren. Bug?)

- [HELP]  
Click this button to open the help function.
