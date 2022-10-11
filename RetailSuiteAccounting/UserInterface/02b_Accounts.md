# Accounts

*Accounting > Settings > Tab ACCOUNTS*

![Accounts](../../Assets/Screenshots/RetailSuiteAccounting/Settings/Accounts/CreateAccount.png "[Accounts]")

- *Account class*  
  Click the drop-down list to select an account class. Depending on the chart of accounts set up in the system, the available account classes may vary. For detailed information about the available charts of accounts, see [Chart of accounts](../Integration/01_RunAccountingWizard.md#chart-of-accounts).

  > [Info] Individual accounts within each account class can also be created, edited or deleted. For detailed information, see [Manage the accounts](../Integration/03_ManageAccounts.md).

The list displays all available accounts of the selected account class. All fields are read-only.

- *No.*  
  Account number.

- *I*  
  Indication of change. An **I** is displayed if the account has been manually created or edited by the user.

- *From*  
  Validity start date of the account.

- *To*  
  Validity end date of the account.  

- *Automatic*  
  Indication of the automatic tax key function. The letter **A** is displayed if the automatic tax key function has been set up for the account.

- *Tax type*   
  Abbreviation of the tax type configured for the account. The following options are available:  
  - Empty     
    No tax type is configured for the account.
  - **I**   
    The input tax is configured for the account.
  - **V**   
    The VAT is configured for the account.
  - **IV**   
    The input tax and the VAT are configured for the account.
  - **NV**   
    No VAT can be configured for the account.

[comment]: <> (Werden zukünftig Abkürzungen übersetzt? Wie?)

- *Tax key*  
  Tax key number configured for the account. Tax keys are set up together with the chart of accounts.

- *Spec. feat.*  
  Special feature configured for the account. The following options are available:   
  - Empty     
    No special feature is configured for the account.
  - **L**   
    The account is locked for postings. This option is applicable only to impersonal accounts.
  - **DA**   
    All debtor's transactions are registered in this collective account in addition to the regular individual personal accounts.
  - **CA**   
    All creditor's transactions are registered in this collective account in addition to the regular individual personal accounts.
  - **MT**   
    This account is used to register card payments temporarily until they are processed in the *Payment processing* module and then transferred to the corresponding bank account.

[comment]: <> (Werden zukünftig Abkürzungen übersetzt? Wie? VD zweimal! Prüfen im neuen UI!)

- *Function*  
  Specific function configured for the account. The following options are available:
  - Empty   
    No specific function is configured for the account.
  - **BA**   
    The account is configured for bank account transactions.
  - **C**   
    The account is configured for cash account transactions
  - **RA**   
    The account is configured for income received as a result of business activities.
  - **RAM**   
    The account is configured for income received as a result of business activities, which is posted manually.
  - **CS**    
    The account is configured for funds being moved from the debit/credit card holder's account to the seller's account following a debit/credit card payment.
  - **DD**     
    The account is configured for discounts granted to customers (debtors).
  - **DC**    
    The account is configured for discounts obtained from suppliers (creditors).
  - **GR**   
    The account is configured for costs of goods received.
  - **PA**   
    The account is configured for costs of presettlements.
  - **EE**   
    The account is configured for expenses incurred as a result of transactions in foreign currencies and exchange rate differences.
  - **IE**   
    The account is configured for income received as a result of transactions in foreign currencies and exchange rate differences.


[comment]: <> (Werden zukünftig Abkürzungen übersetzt? Wie?)

- *Description*  
  Descriptive name of the account.


The input fields below allow to create, edit or delete accounts. For detailed information about creating, editing or deleting accounts, see [Manage the accounts](../Integration/03_ManageAccounts.md).

- *Account number*  
  Enter or modify the account number.

- *Description*  
  Enter or modify a descriptive account name.

- *Valid from*   
  Enter or modify the account validity start date.

- *to*  
  Enter or modify the account validity end date.

- *Tax type*  
  Click the drop-down list to select the appropriate tax type for the account. The tax type determines how the tax paid or collected in the account is to be registered in the system. The following options are available:
  - **() No tax**  
    No tax type is configured for the account. The *Tax key/auto* drop-down lists are locked.
  - **(I) Input tax**  
    The input tax is configured for the account.
  - **(V) VAT**  
    The VAT is configured for the account.
  - **(IV) Input tax and VAT**  
    The input tax and the VAT are configured for the account.
  - **(NV) No VAT possible**  
    No VAT can be configured for the account.


- *Tax key/auto*    
  Click the first drop-down list to select the appropriate tax key for the account. All available tax keys are displayed in the list. If desired, click the second drop-down list and select the **Automatic** option to deduct the applicable tax rate from the gross invoice amount and post the tax amount automatically to the corresponding tax account. Otherwise, leave the second drop-down list empty. The drop-down lists are locked if the **() No tax** option is selected in the *Tax type* drop-down list.

  > [Info] Tax keys are set up once together with the chart of accounts and are no longer updated. Therefore, the tax rate linked to the tax key must be checked for validity and updated if necessary, see [Edit a tax keys](../Integration/02_ManageTaxKeys.md#edit-a-tax-key).

- *Special features*   
  Click the drop-down list to select a special feature for the account. The following options are available:   
  - **() None**  
    No special feature is configured for the account.
  - **(L) Locked**  
    The account is locked for postings. This option is applicable only to impersonal accounts.
  - **(DA) Debtor collective account**  
    All debtor's transactions are registered in this collective account in addition to the regular individual personal accounts. The *Collective account* fields are displayed. The *Function* drop-down list is hidden. The *Tax type* drop-down list, the *Tax key/auto* drop-down list and the *Advance VAT return code* drop-down list are locked.
  - **(CA) Creditor collective account**  
    All creditor's transactions are registered in this collective account in addition to the regular individual personal accounts. The *Collective account* fields are displayed. The *Function* drop-down list is hidden. The *Tax type* drop-down list, the *Tax key/auto* drop-down list and the *Advance VAT return code* drop-down list are locked.
  - **(MT) Money transit account**
    This account is used to register card payments temporarily until they are processed in the *Payment processing* module and then transferred to the corresponding bank account.


- *Function*  
  Click the drop-down list to select a specific function configured for this account. The drop-down list is only displayed if the **() None**, the **(L) Locked** or the **(MT) Money transit account** option is selected in the *Special features* drop-down list. The following options are available:
  - **None**  
    No specific function is configured for the account.
  - **Bank account**   
    The account is configured for bank account transactions.
  - **Checkout**   
    The account is configured for cash account transactions
  - **Revenue account**   
    The account is configured for income received as a result of business activities.
  - **Revenue account, only manual**   
    The account is configured for income received as a result of business activities, which is posted manually.
  - **Debit/credit card settlement**    
    The account is configured for funds being moved from the debit/credit card holder's account to the seller's account following a debit/credit card payment.
  - **Discount debtors (granted)**   
    The account is configured for discounts granted to customers (debtors).
  - **Discount creditors (obtained)**    
    The account is configured for discounts obtained from suppliers (creditors).
  - **Goods receipt**   
    The account is configured for costs of goods received.
  - **Presettlement account**   
    The account is configured for costs of presettlements.
  - **Expenses from exchange rate differences**   
    The account is configured for expenses incurred as a result of transactions in foreign currencies and exchange rate differences.
  - **Income from exchange rate differences**   
    The account is configured for income received as a result of transactions in foreign currencies and exchange rate differences.


[comment]: <> (FS: Bitte Inhalt der Funktionen prüfen! Info fehlt: Vorverrechnungskonto)

- *Collective account*  
  Enter the account number range for the accounts whose transactions will be registered in the collective account. The drop-down list is only displayed if the **(DA) Debtor collective account** or the **(CA) Creditor collective account** option is selected in the *Special features* drop-down list.

- *Advance VAT return code*  
  The **Not in advance VAT return** option is preselected. Currently, no other option is available in the drop-down list.

[comment]: <> (Soll komplett rausfliegen? Bestätigen!)

- *Account suggestion*  
  Enter a related account number which will be displayed by default in the *Contra Account* field of the input line in the *POSTINGS* tab when the current account is selected. This will save time when posting manually.

- *Currency*  
  Click the drop-down list to select the appropriate currency for the account. All available currencies are displayed in the list.  

  > [Info] Be aware that the system can only post transactions with the same currency. This means that the currency selected in customer/supplier accounts and the corresponding impersonal (contra) accounts must coincide. For instance, this would be the case if a customer based in Switzerland buys a product from a company based in Germany.

- *Payment method*   
  Click the drop-down list to select the appropriate payment method. All available payment methods are displayed. This drop-down list is only displayed if the **Revenue account** or the **Revenue account, only manual** option is selected in the *Function* drop-down list.

- *Country*   
  Click the drop-down list and select the appropriate delivery country, which determines the applicable taxation. All available countries are displayed in the list. This drop-down list is only displayed if the **Revenue account** or the **Revenue account, only manual** option is selected in the *Function* drop-down list.


- [SAVE & NEW]  
  Click this button to save a new account. The button is locked if an account has been selected. For detailed information about creating an account, see [Create an account](../Integration/03_ManageAccounts.md#create-an-account).

- [SAVE]  
  Click this button to save any changes made to the selected account. The button is only unlocked if an account has been selected. For detailed information about editing an account, see [Edit an account](../Integration/03_ManageAccounts.md#edit-an-account).

  > [Info] Be aware that all saved changes will overwrite the existing account data.

- [DELETE]  
  Click this button to delete the selected account. The button is only unlocked if an account has been selected. For detailed information, see [Delete an account](../Integration/03_ManageAccounts.md#delete-an-account).

  > [Warning] **Loss of data**   
  Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored.       
  Problems may occur due to unresolved dependencies.   
  Make sure you really want to delete the selected data.

- [CLEAR]  
  Click this button to clear all fields.

- [HELP]  
  This function is currently not available.
