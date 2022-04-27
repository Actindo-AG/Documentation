[!!Accounting](RetailSuiteAccounting)

# Open items

The *OPEN ITEMS* tab displays any open items in the system, that is, any business transactions that have not yet been completed. The information displayed in the account sheet view is read-only.

There are two view modes:

- If no account is selected, the *OPEN ITEMS* tab displays all open items in the *Accounting* module.
- If a personal account is selected, the *OPEN ITEMS* tab displays only the open items for the selected account.

> [Info] An account can be selected either by entering an  account number in the *Account* or *Contra account* field, or by clicking on a booking in the *BOOKINGS* tab.  

For detailed information about accessing open items, see [Manage the open items](/RetailSuiteAccounting/Operation/03_ManageOpenItems.md).

## Open items view without account selection

*Accounting > Select fiscal year > Book > Tab OPEN ITEMS*

![All open items](/Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/NoAccountSelected.png "[All open items]")

- *Fiscal year XXXX/Month X/Journal X*  
This text displays the fiscal year, month and journal currently selected. This information is read-only.

  > [Info] If the fiscal year or the booking period need to be changed, click the [FY/MONTH/JOURNAL] button to display the select fiscal year window. For detailed information, see [Fiscal year](00a_FiscalYear.md) and [Select a fiscal year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md).

-



> [Info] If there are no open items, a blank tab is displayed.

 ![No open items](/Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/NoOPOS.png "[No open items]")



## Open items view with account selection

*Accounting > Select fiscal year > Book > Tab OPEN ITEMS*

![Open items for an account](/Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/AccountSelected.png "[Open items for an account]")

- *Fiscal year XXXX/Month X/Journal X*  
This text displays the fiscal year, month and journal currently selected. This information is read-only.

  > [Info] If the fiscal year or the booking period need to be changed, click the [FY/MONTH/JOURNAL] button to display the select fiscal year window. For detailed information, see [Fiscal year](00a_FiscalYear.md) and [Select a fiscal year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md).


- *Scroll*


- *Date*  
This column displays the booking date. Date format is DDMMYY.

- *BP*  
This column displays the booking period (month).

- *Jnl*  
This column displays the journal.

- *Contra account*  
This column displays the contra account number. For detailed information about the available accounts, see [Chart of accounts](/RetailSuiteAccounting/Integration/01_RunAccountingWizard.md#chart-of-accounts).

- *Tax key*  
This column displays the tax key linked to the contra account. Tax keys can be created, edited and deleted, if necessary. For detailed information about managing tax keys, see [Manage the tax keys](/RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

- *Receipt 1*  
This column displays the receipt 1 value, usually the invoice number.

  > [Info] The information provided in the *Receipt 1* field is essential, as the system identifies and groups together any subsequent bookings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt 2*  
This column displays the receipt 2 value, which can be any other reference number, such as the order number.

- *Cost 1*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 1 has been set up. For detailed information, see [COST ACCOUNTING](XX_CostAccounting.md).

- *Cost 2*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 2 has been set up. For more details, see [COST ACCOUNTING](XX_CostAccounting.md).

- *Debit*  
This column displays the debit amount of the selected account.

- *Credit*  
This column displays the credit amount of the selected account.

- *(Unnamed column)*  
This column displays a ![B](/Assets/Icons/Beleg.png "[B]") icon if a receipt has been linked to the booking. When clicking on the icon, the linked receipt is displayed in the *Attached document* window. For detailed information, see [Attached document](01a_Book.md#attached-document).

- *Text*  
This column displays the booking text, if any has been entered.

- *Account number - account name [currency]*  


- *Balance (currency)*  
this field displays the balance of the selected account and its currency.


- *Standard open items view*  
Click this radio button to display

- *Show manually cleared open items*  
Click this radio button to display


- [CLEAR MANUALLY]

- [CANCEL CLEARING]
