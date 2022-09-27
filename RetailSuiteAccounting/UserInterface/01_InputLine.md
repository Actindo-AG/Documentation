# Post input line

*Accounting > Post*

![Post](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Post]")

In all tabs of the *Post* menu entry, an identical footer with the input line is displayed. The contained elements and the corresponding functions are described below.

- *Seq. no.*  
 Enter the posting number. Posting numbers must be sequential. The system adds the next available number automatically if the field is left empty.

- *Currency code*  
Click the drop-down menu to select the appropriate currency.  

  > [Info] It is possible to set up accounts and post transactions in different currencies, but the *Accounting* module can only work with the base currency configured in the system. For detailed information about managing and posting exchange rate fluctuations, see [Post exchange rate fluctuations](../Operation/12_BookExchangeRateFluctuations.md).

- *Exchange rate*  
This field updates automatically when changing the currency. It can also be modified manually.

  > [Info] The system retrieves once a day the current foreign currency exchange rates as published by the ECB and applies them automatically, therefore always working with the most up-to-date information.

- *Turnover*  
Enter the turnover value. Turnover values can be positive (incomes) or negative (expenses). This field is compulsory.

- *Contra account*  
Enter the appropriate contra account. This field is compulsory.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list. Alternatively, use the search function to find the account number, see [Search for an account](../Operation/13_SearchAccounting.md#search-for-an-account).


- *Receipt1*  
Enter an appropriate reference value, such as the invoice number.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent postings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt2*  
Enter any other appropriate reference value, such as order number.

- *Date*  
Enter the posting date. The valid date format is DDMMYY.

- *Account*   
Enter the appropriate account number, for example a personal account number, that is, customer or supplier number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

  > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](../Integration/05_ManageCustomerSupplier.md).

- *COST1*  
Enter the appropriate value.

  > [Info] This is only applicable if at least one cost center has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *COST2*  
Enter the appropriate value.

  > [Info] This is only applicable if at least one cost unit has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Posting text*  
Enter any appropriate posting text. Posting text can contain a combination of letters and numbers.


When creating a manual posting or selecting an existing posting, the account/contra account details, as well as their current balances, are displayed under the input line.

- *Contra account*  
This field displays the selected contra account. This field is read-only.

- *Account*  
This field displays the selected account. This field is read-only.

- *Balance (amount)H/S (currency)*  
This field displays the current balance of the corresponding account. H stands for credit. S stands for debit.


- [POST]    
Click this button to post the transaction entered in the input line.

- [CANCEL]  
Click this button to cancel the selected posting. For detailed information, see [Cancel a posting](../Operation/05_CancelBooking.md).

- [DELETE]    
Click this button to delete the selected posting. For detailed information, see [Delete a single posting](../Operation/06_DeleteBookings.md#delete-a-single-posting).

- [CLEAR]    
Click this button to clear all input line fields.

- [SPLIT]    
Click this button to split a manual posting. The *Split posting* window is displayed, see [Split posting](#split-posting). For detailed information about splitting a posting, see [Split a posting](../Operation/09_SplitBooking.md).

- [ASSIGN RECEIPT]  
Click this button to assign a receipt to the selected posting. The *Attach document* window is displayed, see [Attach a document](#attach-document). For detailed information, see [Retrieve a receipt](../Operation/10_ManageReceipts.md#retrieve-a-receipt).
