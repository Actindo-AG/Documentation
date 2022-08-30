# Open items

The *OPEN ITEMS* tab displays any open items in the system, that is, any business transactions that have not yet been completed. The information displayed in the open items view is read-only.

There are two view modes:

- If no account is selected, the *OPEN ITEMS* tab displays all open items in the *Accounting* module.
- If a personal account is selected, the *OPEN ITEMS* tab displays only the open items for the selected account.

An account can be selected either by entering an account number in the *Account* or *Contra account* field, or by clicking on a posting in the *POSTINGS* tab. For detailed information about accessing open items, see [Manage the open items](../Operation/03_ManageOpenItems.md).



## Open items view without account selection

*Accounting > Post > Tab OPEN ITEMS*

![All open items](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/AllOpenItems.png "[All open items]")

- *Fiscal year XXXX/Month X/Journal X*  
This text displays the fiscal year, month and journal currently selected. This information is read-only.

  > [Info] If the fiscal year or the posting period need to be changed, click the [FY/MONTH/JOURNAL] button to display the select fiscal year window. For detailed information, see [Fiscal year](./00a_FiscalYear.md) and [Select a fiscal year](../Operation/01_SelectFiscalYear.md).

- ![Open](../../Assets/Icons/Back02.png "[Open]") (Open)   
Click this arrow to open the *Post extras* side bar. For detailed information about searching in the *Accounting* module, see [Search in accounting](../Operation/14_SearchAccounting.md)

- *Seq. no.*  
This column displays the sequential number.

  > [Info] The posting numbers must be sequential and are added by the system automatically.

- *Date*  
This column displays the posting date. Date format is DDMMYY.

- *BP*  
This column displays the posting period (month/journal).

- *Jnl*  
This column displays the journal.

- *Contra account*  
This column displays the contra account number. For detailed information about the available accounts, see [Chart of accounts](../Integration/01_RunAccountingWizard.md#chart-of-accounts).

- *Tax key*  
This column displays the tax key linked to the contra account. Tax keys can be created, edited and deleted, if necessary. For detailed information about managing tax keys, see [Manage the tax keys](../Integration/02_ManageTaxKeys.md).

- *Receipt1*  
This column displays the receipt 1 value, usually the invoice number.

  > [Info] The information provided in the *Receipt 1* field is essential, as the system identifies and groups together any subsequent postings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt2*  
This column displays the receipt 2 value, which can be any other reference number, such as the order number.

- *Cst1*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 1 has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

  [comment]: <> (Alt-Doku: Das Feld wird beim Eingeben nur dann angesprochen, wenn eine Kostenstellenrechnung für Kost1 eingerichtet ist.)

- *Cst2*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 2 has been set up. For more details, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Debit*  
This column displays the debit amount of the selected account.

- *Credit*  
This column displays the credit amount of the selected account.

- *(Unnamed column)*  
This column displays a ![B](../../Assets/Icons/Beleg.png "[B]") icon if a receipt has been linked to the posting. When clicking on the icon, the linked receipt is displayed in the *Attached document* window. For detailed information, see [Attached document](#attached-document).

[comment]: <> (Comment on Bug file -> suggestion to add a name to column)

- *Text*  
This column displays the posting text, if any has been entered.

- *(Account number) (account name) [currency]*  
This field introduces a list of all existing open items for this account.

- *Balance (currency)*  
This field displays the balance for each existing open item in the preceding account.  


- *Amount (Amount 1 - Amount 2)*  
The information provided in these fields refers to the postings list and is not related to the open items view. For detailed information, see [POSTINGS](./01a_Bookings.md).


In the *Open items* tab, the input line serves the only purpose of selecting an account, if no posting is selected in the *POSTINGS* tab.

> [Info] If a posting is selected in the *POSTINGS* tab, the posting details are displayed in the input line. The open items of the account selected in the *Account* field are displayed in the open items view.

[comment]: <> (Work in progress! To be completed/modified! Screenshots should probably be changed to display empty input line!)

  - *Seq. no.*  
  This field is empty.

  - *Currency code*  
  This field displays the selected basic currency.

  - *Exchange rate*  
  This field displays the exchange of the selected basic currency.

  - *Turnover*  
  This field is empty.

  - *Contra account*  
  Enter a personal account number to display its open items. It is possible to enter both a customer or a supplier account number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

    > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](../Integration/05_ManageCustomerSupplier.md).

  - *Receipt 1*  
  This field is empty.

  - *Receipt 2*  
  This field is empty.

  - *Date*  
  The first day of the selected month is displayed.

  - *Account*   
  Enter a personal account number to display its open items. It is possible to enter both a customer or a supplier account number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

    > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](../Integration/05_ManageCustomerSupplier.md).

  - *COST1*  
  This field is empty.

  - *COST2*  
  This field is empty.

  - *Booking text*  
  This field is empty.


  When a posting or an account is selected, the account/contra account details, as well as their current balances, are displayed under the input line. The information provided in these fields is read-only.

  - *Contra account*  
  This field displays the selected contra account. This field is read-only.

  - *Account*  
  This field displays the selected account. This field is read-only.

  - *Balance (amount)H/S (currency)*  
  This field displays the current balance of the corresponding account. H stands for credit. S stands for debit.

The buttons on the bottom right corner have no specific function in the open items view. For detailed information, see [POSTINGS](./01a_Bookings.md).



## Open items view with account selection

*Accounting > Post > Tab OPEN ITEMS*

![Open items for an account](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/OpenItemsAccount.png "[Open items for an account]")

- *Fiscal year XXXX/Month X/Journal X*  
This text displays the fiscal year, month and journal currently selected. This information is read-only.

  > [Info] If the fiscal year or the posting period need to be changed, click the [FY/MONTH/JOURNAL] button to display the select fiscal year window. For detailed information, see [Fiscal year](./00a_FiscalYear.md) and [Select a fiscal year](../Operation/01_SelectFiscalYear.md).


- ![Previous](../../Assets/Icons/Previous.png "[Previous]")  *Scroll* ![Next](../../Assets/Icons/Next.png "[Next]")  
Your can use the arrow buttons to scroll through the available accounts to search for a specific one. Alternatively, you can enter an account number in the input line.


- *Seq. no.*  
This column displays the sequential number.

  > [Info] The posting numbers must be sequential and are added by the system automatically.

- *Date*  
This column displays the posting date. Date format is DDMMYY.

- *BP*  
This column displays the posting period (month/journal).

- *Jnl*  
This column displays the journal.

- *M*  
This column displays a checkbox to select the open items to be cleared manually, if necessary.

[comment]: <> (Evt. Info hinzufügen: The manually cleared postings are marked with an asterisk next to the checkbox.)


- *Contra account*  
This column displays the contra account number. For detailed information about the available accounts, see [Chart of accounts](../Integration/01_RunAccountingWizard.md#chart-of-accounts).

- *Tax key*  
This column displays the tax key linked to the contra account. Tax keys can be created, edited and deleted, if necessary. For detailed information about managing tax keys, see [Manage the tax keys](../Integration/02_ManageTaxKeys.md).

- *Receipt1*  
This column displays the receipt 1 value, usually the invoice number.

  > [Info] The information provided in the *Receipt 1* field is essential, as the system identifies and groups together any subsequent postings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt2*  
This column displays the receipt 2 value, which can be any other reference number, such as the order number.

- *Cst1*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 1 has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

  [comment]: <> (Alt-Doku: Das Feld wird beim Eingeben nur dann angesprochen, wenn eine Kostenstellenrechnung für Kost1 eingerichtet ist.)

- *Cst2*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 2 has been set up. For more details, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Debit*  
This column displays the debit amount of the selected account.

- *Credit*  
This column displays the credit amount of the selected account.

- *(Unnamed column)*  
This column displays a ![B](../../Assets/Icons/Beleg.png "[B]") icon if a receipt has been linked to the posting. When clicking on the icon, the linked receipt is displayed in the *Attached document* window. For detailed information, see [Attached document](#attached-document).

[comment]: <> (Comment on Bug file -> suggestion to add a name to column)

- *Text*  
This column displays the posting text, if any has been entered.

- *(Account number) (account name) [currency]*  
This field introduces a list of all existing open items for this account.

- *Balance (currency)*  
This field displays the balance for each existing open item in the preceding account.    


- *Standard open items view*  
Click this radio button to display all open items for this account.

- *Show manually cleared open items*  
Click this radio button to display only the manually cleared open items for this account.


- [CLEAR MANUALLY]  
Click this button to clear an open item manually. For detailed information about managing open items, see [Access the open items for an account](../Operation/03_ManageOpenItems.md#access-the-open-items-for-an-account).

- [CANCEL CLEARING]  
Click this button to reverse manually cleared items.

  > [Info] This button is displayed when the *Show manually cleared open items* radio button selected. It is also displayed in the Standard open items view (*Standard open items view* radio button selected), if an open item has been cleared manually).



- *Amount (Amount 1 - Amount 2)*  
The information provided in these fields refers to the postings list and is not related to the open items view. For detailed information, see [POSTINGS](./01a_Bookings.md).



In the *Open items* tab, the input line serves the only purpose of selecting an account or changed to account to be displayed.

[comment]: <> (Work in progress! To be completed/modified! Screenshots should probably be changed to display empty input line or text adapted, e.g., "empty or irrelevant/unrelated"...)

  - *Seq. no.*  
  This field is empty.

  - *Currency code*  
  This field displays the selected basic currency.

  - *Exchange rate*  
  This field displays the exchange of the selected basic currency.

  - *Turnover*  
  This field is empty.

  - *Contra account*  
  This field displays the account currently selected. Enter another personal account number to display its open items. It is possible to enter both a customer or a supplier account number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

    > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](../Integration/05_ManageCustomerSupplier.md).

  - *Receipt 1*  
  This field is empty.

  - *Receipt 2*  
  This field is empty.

  - *Date*  
  The first day of the selected month is displayed.

  - *Account*   
  This field displays the account currently selected. Enter another personal account number to display its open items. It is possible to enter both a customer or a supplier account number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

    > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](../Integration/05_ManageCustomerSupplier.md).

  - *COST1*  
  This field is empty.

  - *COST2*  
  This field is empty.

  - *Booking text*  
  This field is empty.


  When an account is selected, the account/contra account details, as well as their current balances, are displayed under the input line. The information provided in these fields is read-only.

  - *Contra account*  
  This field displays the selected contra account. This field is read-only.

  - *Account*  
  This field displays the selected account. This field is read-only.

  - *Balance (amount)H/S (currency)*  
  This field displays the current balance of the corresponding account. H stands for credit. S stands for debit.

The buttons on the bottom right corner have no specific function in the open items view. For detailed information, see [POSTINGS](./01a_Bookings.md).


## No open items view

If there are no open items, a blank tab and the message "No open items exist" is displayed.

 ![No open items](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/NoOPOS.png "[No open items]")


### Attached document

*Accounting > Post > Tab OPEN ITEMS > Select icon B*

![Attached document](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/AttachedDocument.png "[Attached document]")


- ![Previous](../../Assets/Icons/Previous.png "[Previous]") *Document* ![Next](../../Assets/Icons/Next.png "[Next]")   
These buttons do not have any function here, as there is only one document (or receipt) assigned to a posting.

[comment]: <> (These buttons do have a function in "BELEGE BUCHEN/POST RECEIPTS". Add info? Link?)

- ![First page](../../Assets/Icons/FirstPage02.png "[Previous]") ![First page](../../Assets/Icons/Previous.png "[Previous]") *Page [x]* ![Next](../../Assets/Icons/Next.png "[Next]")  
 The current page number is displayed. Click the arrow first page/previous/next buttons to scroll through the pages.

- (-) *Zoom* (+)  
Click the -/+ buttons to zoom in and out of the document view.

- *Download file*  
Click this button to download the document.

- [CLOSE]  
Click this button to close the window.
