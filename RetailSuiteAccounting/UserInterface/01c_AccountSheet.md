# Account sheet

*Accounting > Post > Tab ACCOUNT SHEET*

![Account sheet](../../Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet/AccountSheet.png "[Account sheet]")

The *ACCOUNT SHEET* tab displays a chronologically ordered list of all movements in a specific account.   

An account and/or contra account must be selected to display the corresponding details. Otherwise, the notice *No account selected* is displayed.    

You can either select an account in the *POSTINGS* tab and switch to the *ACCOUNT SHEET* tab or directly enter an account and/or contra account number in the input line in the bottom. For detailed information about accessing an account sheet, see [Access the account sheet](../Operation/02_ReviewAccount.md#access-the-account-sheet).  

If a contra account number is specified in the *Contra account* field of the input line, the account sheet for the corresponding contra account is displayed. If no contra account number is entered, but an account number is specified in the *Account* field of the input line, the account sheet for the corresponding account is displayed.

[comment]: <> (Verweis auf Header.md)

- ![Previous](../../Assets/Icons/Previous.png "[Previous]") (Previous)
  Click this button to display the account sheet of the previous available account number.

- ![Next](../../Assets/Icons/Next.png "[Next]") (Next)
  Click this button to display the account sheet of the next available account number.


**Account sheet for account**   

The list displays all postings for the selected account whose number and name are specified in the list's title. All fields are read-only.

- *Date*  
  Posting date. The valid date format is DDMMYY.

- *PP*  
  Month number of the posting period.

- *Jnl*  
  Journal number of the posting period.

- *Contra account*  
  Contra account number.

- *Tax key*  
  Tax key applied to the posting.

- *Receipt 1*  
  Receipt 1 value, usually the invoice number. The information provided in this field is essential, as the system identifies and groups together any subsequent postings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt 2*  
  Receipt 2 value, which can be any other reference number, such as the order number.

- *Cost 1*  
  Number of the selected cost center. This field is only applicable if at least one cost center has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Cost 2*  
  Number of the selected cost object. This field is only applicable if at least one cost object has been set up. For more details, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Debit*  
  Debit amount of the selected account.

- *Credit*  
  Credit amount of the selected account.

- *(Unnamed column)*
  Indication of whether a receipt has been linked to the posting. If a receipt has been linked to the posting, the ![B](../../Assets/Icons/Beleg.png "[B]") (B) button is displayed. Click the button to display the corresponding receipt in the *Attached document* window. For detailed information, see [Attached document](#attached-document).

- *Text*  
  Posting text.

- *Total turnover (currency)*  
  Total turnover of the selected account in the specified currency.

- *Balance (currency)*  
  Balance of the selected account in the specified currency.

- ![Radio button](../../Assets/Icons/Radiobutton02.png "[Radio button]") *All months*  
  Select this radio button to display the balances for all months.

- ![Radio button](../../Assets/Icons/Radiobutton02.png "[Radio button]")  *Only this month*  
  Select this radio button to display the balances only for the selected month.

- *Show (all/the last [XXX]) postings*    
  Click the drop-down list to select the preferred display filter.


### Attached document

[comment]: <> (HG: vgl. 01_Book
-> vielleicht reicht auch ein Verweis auf das entsprechende Kapitel)

*Accounting > Post > Tab ACCOUNT SHEET > Button B*

![Attached document](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/AttachedDocument.png "[Attached document]")

- ![Previous](../../Assets/Icons/Previous.png "[Previous]") *Document* ![Next](../../Assets/Icons/Next.png "[Next]")   
  These buttons do not have any function here, as there is only one document (or receipt) assigned to a posting.

[comment]: <> (These buttons do have a function in "BELEGE BUCHEN/BOOK RECEIPTS". Add info? Link?)

- ![First page](../../Assets/Icons/FirstPage02.png "[Previous]") ![First page](../../Assets/Icons/Previous.png "[Previous]") *Page [x]* ![Next](../../Assets/Icons/Next.png "[Next]")  
  The current page number is displayed. Click the arrow first page/previous/next buttons to scroll through the pages.

- (-) *Zoom* (+)  
  Click the -/+ buttons to zoom in and out of the document view.

- *Download file*  
  Click this button to download the document.

[comment]: <> (HG: vgl. 01_Book)

- [CANCEL ASSIGNMENT]  
  Click this button to unassign the receipt from the selected posting. The *Attached document* window is closed.

- [CLOSE]  
  Click this button to close the *Attached document* window.


[comment]: <> (Verweis auf Input line muss noch rein -> ggf. input line als eigenen header in 01a_Bookings oder ebenso wie die anderen Funktionen in separatem Dokument, damit man darauf verweisen kann.)
