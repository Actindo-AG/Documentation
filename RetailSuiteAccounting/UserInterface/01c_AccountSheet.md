
# Account sheet

The *ACCOUNT SHEET* tab displays a chronologically ordered list of all movements in a specific account. The information displayed in the account sheet view is read-only.


## Account sheet view without account selection

*Accounting > Select fiscal year > Book > Tab ACCOUNT SHEET*

![Account sheet - no account selected](../../Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet/AccountSheetNoAccount.png "[Account sheet - no account selected]")

When clicking the *ACCOUNT SHEET* tab, a blank tab and the message "No account selected" may be displayed. An account must be selected to display the corresponding details. If a booking is selected in the *BOOKINGS* tab, the details of the account specified in the Contra Account field are displayed in the *ACCOUNT SHEET* tab. If the Contra Account field is empty, the details of the account specified in the Account field are displayed.

For detailed information about accessing an account sheet, see [Access the account sheet](../Operation/02_ReviewAccount.md#access-the-account-sheet).


## Account sheet view with account selection

*Accounting > Select fiscal year > Book > Tab ACCOUNT SHEET*

![Account sheet](../../Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet/AccountSheet.png "[Account sheet]")

- *Fiscal year XXXX/Month X/Journal X*  
This text displays the fiscal year, month and journal currently selected. This information is read-only.

  > [Info] If the fiscal year or the booking period need to be changed, click the [FY/MONTH/JOURNAL] button to display the select fiscal year window. For detailed information, see [Fiscal year](./00a_FiscalYear.md) and [Select a fiscal year](../Operation/01_SelectFiscalYear.md).


- ![Previous](../../Assets/Icons/Previous.png "[Previous]")  *Scroll* ![Next](../../Assets/Icons/Next.png "[Next]")  
Your can use the arrow buttons to scroll through the available accounts to search for a specific one. Alternatively, you can enter an account number in the entry line.

- *Account sheet for account (account number) (account name)*  
The number and name of the selected account are displayed.

- *Date*  
This column displays the booking date. Date format is DDMMYY.

- *BP*  
This column displays the booking period (month).

- *Jnl*  
This column displays the journal.

- *Contra account*  
This column displays the contra account number. For detailed information about the available accounts, see [Chart of accounts](../Integration/01_RunAccountingWizard.md#chart-of-accounts).

- *Tax key*  
This column displays the tax key linked to the contra account. Tax keys can be created, edited and deleted, if necessary. For detailed information about managing tax keys, see [Manage the tax keys](../Integration/02_ManageTaxKeys.md).

- *Receipt 1*  
This column displays the receipt 1 value, usually the invoice number.

  > [Info] The information provided in the *Receipt 1* field is essential, as the system identifies and groups together any subsequent bookings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt 2*  
This column displays the receipt 2 value, which can be any other reference number, such as the order number.

- *Cost 1*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 1 has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Cost 2*  
This column displays the cost unit number selected.

  > [Info] This is only applicable is a cost center accounting for cost 2 has been set up. For more details, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Debit*  
This column displays the debit amount of the selected account.

- *Credit*  
This column displays the credit amount of the selected account.

- *(Unnamed column)*
This column displays a ![B](../../Assets/Icons/Beleg.png "[B]") icon if a receipt has been linked to the booking. When clicking on the icon, the linked receipt is displayed in the *Attach document* window. For detailed information, see [Attach document](./01a_Bookings.md#attach-document).

- *Text*  
This column displays the booking text, if any has been entered.

- *Total turnover (currency)*  
This field displays the total turnover of the selected account and its currency.

- *Balance (currency)*  
this field displays the balance of the selected account and its currency.


- *All months*  
Click this radio button to display the balances for all months.

- *Only this month*  
Click this radio button to display the balances only for the selected month.

- *Show (all/the last [XXX]) bookings*    
Click the drop-down list to select the preferred display filter.
