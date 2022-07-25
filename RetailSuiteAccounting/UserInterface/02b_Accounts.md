
[!!Accounting](RetailSuiteAccounting)

# Accounts

*Accounting > Select fiscal year > Settings > Tab ACCOUNTS*

![Accounts](/Assets/Screenshots/RetailSuiteAccounting/Settings/Accounts/Accounts.png "[Accounts]")

- *Account class*  
Click the drop-down list to select an account class. Depending on the Chart of accounts set up in the system, the available account  classes may vary. For detailed information about setting up the chart of accounts, see [Chart of accounts](/RetailSuiteAccounting/Integration/01_RunAccountingWizard.md#chart-of-accounts).

  > [Info] Individual accounts can also be created, edited or deleted. For detailed information, see [Manage the accounts](/RetailSuiteAccounting/Integration/03_ManageAccounts.md).

The accounts are displayed in a column view. All information provided in columns is read-only.


- ![Sort](/Assets/Icons/Sort03.png "[Sort]") (Sort)  
Click this button to sort in ascending or descending order the displayed accounts.

- *No.*  
Account number.

- *I*  
A mark (|) is displayed if the account has been created or edited by the user.

- *From*  
Validity start date of the account.

- *To*  
Validity end date of the account.  

- *Automatic*  
The letter A is displayed if the automatic tax key function has been configured for the account.

[comment]: <> (Automatik -> mehr Info?)

- *Tax type*   
Abbreviation of the tax type configured for the account. The following options are available:  

  - (none): No tax
  - *I*: Input tax
  - *V*: VAT
  - *IV*: Input tax and VAT
  - *NV*: No VAT possible

[comment]: <> (Abkürzungen im System nicht übersetzt. Auf DE lassen? Wenn ja, durchgängig, also, auch in Integration und Operation)

- *Tax key*  
Tax key number configured for the account. Tax keys are configured together with the Chart of accounts.

  > [Info] Tax keys can also be created, edited or deleted. For detailed information, see [Manage the tax keys](/RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

- *Spec. feat.*  
Abbreviation of a special feature configured for the account. The following options are available:   

  - (none): Normal
  - *L*: Locked
  - *DA*: Debtor collective account
  - *CA*: Creditor collective account
  - *MT*: Money transit account

[comment]: <> (Abkürzungen im System nicht übersetzt. Auf DE lassen? Wenn ja, durchgängig, also, auch in Integration und Operation)

- *Function*  
Abbreviation of a specific function configured for the account. The following options are available:

  - (none): No specific function
  - *B*: Bank account
  - *K*: Checkout
  - *E*: Revenue account
  - *EM*: Revenue account, only manual
  - *V*: Debit/credit card settlement
  - *S*: Discount debtors (granted)
  - *SK*: Discount creditors (obtained)
  - *WE*: Goods receipt
  - *VKV*: Presettlement account
  - *KA*: Expenses from exchange rate differences
  - *KE*: Income from exchange rate differences


[comment]: <> (Abkürzungen auf DE belassen. Übersetzen? S. o. andere Abkürzungen)

- *Description*  
Account description.

The entry fields allow to create, edit or delete accounts. For detailed information about creating, editing or deleting accounts, see [Manage the accounts](/RetailSuiteAccounting/Integration/03_ManageAccounts.md).

- *Account number*  
Enter or modify the account number.

- *Description*  
Enter or modify the account description. Letters, numbers or a combination of both can be used.

- *Valid from - to*  
Enter or modify the account validity period.

- *Tax type*  
Click the drop-down list to select the appropriate tax type for the account. The tax type determines how the tax paid or collected in the account is to be registered in the system.

  - **( )No tax**  
  No tax defined for the account.  
  - **(I)Input tax**  
  Input tax configured for the account.
  - **(V)VAT**  
  VAT (value added tax) configured for the account.
  - **(IV)Input tax and VAT**  
  Input tax and VAT (value added tax) configured for the account.
  - **(NV)No VAT possible**  
  It is not possible to configure a VAT (value added tax) for the account.

[comment]: <> (Stimmt das so?)

- *Tax key/auto*    
  Click the first drop-down list to select the appropriate tax key for the account. Click the second drop-down list and select **Automatic** to book automatically the selected tax key to all bookings in the account, if desired.

- *Special features*  

  - **( )Normal**  
  No special features configured for the account.
  - **(L)Locked**  
  The account is locked and not bookable.
  - **(DA)Debtor collective account**  
  All debtor's open items are registered in this account.
  - **(CA)Creditor collective account**  
  All creditor's open items are registered in this account.
  - **(MT)Money transit account**
  The account is used to register cash movements temporarily.

[comment]: <> (Stimmt das so?)

- *Function*  
Click the drop-down list to select a specific function for this account.

  - **none**  
  No specific function defined for the account.
  - **Bank account**  
  Bank account transactions.
  - **Checkout**  
  Cash account transactions.
  - **Revenue account**  
  Income received as a result of business activities.
  - **Revenue account, only manual**  
  Income received as a result of business activities, booked manually.
  - **Debit/credit card settlement**  
  Funds being moved from the debit/credit card holder's account to the seller's account following a debit/credit card payment.  
  - **Discount debtors (granted)**  
  Discounts granted to customers or debtors.
  - **Discount creditors (obtained)**  
  Discounts obtained from creditors (suppliers).
  - **Goods receipt**  
  Costs of goods received.
  - **Presettlement account**  

  - **Expenses from exchange rate differences**  
  Expenses incurred as a result of transactions in foreign currencies and exchange rate differences.
  - **Income from exchange rate differences**  
  Income received as a result of transactions in foreign currencies and exchange rate differences.

[comment]: <> (Vorverrechnungskonto? Vgl. EC-/Kreditkarte-Verrenchung. Andere müssen auch gegengeprüft werden!)

- *Advance VAT return code*  
Click the drop-down list to select the appropriate option or **not in advance VAT return**, if the Advance VAT return is not applicable.

[comment]: <> (Soll rausfliegen?)

- *Account suggestion*  
You can enter an account number to be displayed by default in the *Account* field of the input line in the *Bookings* tab, when the current account is selected as contra account.

[comment]: <> (Stimmt das so?)

- *Currency*  
Click the drop-down list to select the appropriate currency for the account.



- [SAVE & NEW]  
Click this button to create a new account. For detailed information about creating an account, see [Create an account](/RetailSuiteAccounting/Integration/03_ManageAccounts.md#create-an-account).

- [SAVE]  
Click this button to save any changes made to an existing account.

  > [Info] The saved changes will overwrite the account existing details. To prevent this, click the [CLEAR] button to create a new account. For detailed information about editing an account, see [Edit an account](/RetailSuiteAccounting/Integration/03_ManageAccounts.md#edit-an-account).

- [DELETE]  
Click this button to delete the selected account.

  > [Warning] Be aware that the selected account will be deleted permanently. For detailed information, see [Delete an account](/RetailSuiteAccounting/Integration/03_ManageAccounts.md#delete-an-account).

- [CLEAR]  
Click this button to clear all entry fields. The button [SAVE & NEW] becomes active again.

- [HELP]  
Click this button to open the help function.
