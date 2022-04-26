[!!Accounting](RetailSuiteAccounting)

# Bookings

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

  ![Book](/Assets/Screenshots/RetailSuiteAccounting/Book/FYMonthJournalButton.png "[Book]")

The *BOOKINGS* tab displays all existing bookings in the selected booking period in chronological order. The booking details displayed in columns are read-only.

- *Seq. no.*  
This column displays the sequential number.

  > [Info] The booking numbers must be sequential and are added by the system automatically.

- *BP*  
This column displays the booking period (month/journal).

- *Turnover*  
This column displays the turnover value.

- *Contra account*  
This column displays the contra account number. For detailed information about the available accounts, see [Chart of accounts](/RetailSuiteAccounting/Integration/01_RunAccountingWizard.md#chart-of-accounts).

- *Receipt1*  
This column displays the receipt 1 value, usually the invoice number.

  > [Info] The information provided in the *Receipt 1* field is essential, as the system identifies and groups together any subsequent bookings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt2*  
This column displays the receipt 2 value, which can be any other reference number, such as the order number.

- *Date*  
This column displays the booking date. Date format is DDMMYY.

- *Account*  
This column displays the account number, usually a personal account number, that is, a customer or supplier account number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

  > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](/RetailSuiteAccounting/Integration/05_ManageCustomerSupplier.md).

- *Cst1*  
This column displays the cost unit number selected. This is only applicable is a cost center accounting for cost 1 has been set up. For detailed information, see [COST ACCOUNTING](XX_CostAccounting.md).

[comment]: <> (Alt-Doku: Das Feld wird beim Eingeben nur dann angesprochen, wenn eine Kostenstellenrechnung für Kost1 eingerichtet ist.)

- *Cst2*  
This column displays the cost unit number selected. This is only applicable is a cost center accounting for cost 2 has been set up. For more details, see [COST ACCOUNTING](XX_CostAccounting.md).

- *(Unnamed column)*  
This column displays a ![B](/Assets/Icons/Beleg.png "[B]") icon if a receipt has been linked to the booking. When clicking on the icon, the linked receipt is displayed in a new window.

[comment]: <> (Comment on Bug file -> suggestion to add a name to column)

- *Text*  
This column displays the booking text, if any has been entered.


- *Fiscal year XXXX/Month X/Journal X*  
This text displays the fiscal, month and journal currently selected. This information is read-only.

- *Show (all/the last [XXX]) bookings*    
Click the drop-down list to select the preferred display filter.


- *Amount*  
The total amount of all bookings displayed.
  - *Amount 1*  
  Click this button to manually set an amount 1. A new window opens where the amount can be entered and confirmed with [OK].
  - *Amount 2*  
  Click this button to manually set an amount 2. A new window opens.  A new window opens where the amount can be entered and confirmed with [OK].

[comment]: <> (Function of Summe 1 & Summe 2??? Describe new window? RS FH!)


The entry line allows to create a booking manually. For detailed information, see [Create a manual booking](/RetailSuiteAccounting/Operation/04_CreateManualBooking.md).


- *Seq. no.*  
 Enter the booking number. Booking numbers must be sequential. The system adds the next available number automatically if the field is left empty.

- *Currency code*  
Click the drop-down menu to select the appropriate currency.  

  > [Info] It is possible to set up accounts in different currencies. However, the *Accounting* module can only work with the base currency configured in the system. For detailed information about managing and booking exchange rate fluctuations, see [Book exchange rate fluctuations](/RetailSuiteAccounting/Operation/12_BookExchangeRateFluctuations.md).

- *Exchange rate*  
This field updates automatically when changing the currency. It can also be modified manually.

  > [Info] The system retrieves once a day the current foreign currency exchange rates as published by the ECB and applies them automatically, therefore always working with the most up-to-date information.

- *Turnover*  
Enter the turnover value. Turnover values can be positive (incomes) or negative (expenses). This field is compulsory to manually create a booking.

- *Contra account*  
Enter the appropriate contra account. For detailed information about the available accounts, see [Chart of accounts](/RetailSuiteAccounting/Integration/01_RunAccountingWizard.md#chart-of-accounts). This field is compulsory to manually create a booking.

  > [Info] When you start typing in an account number, a context menu is displayed. You can also select the appropriate option from the menu.

- *Receipt1*  
Enter an appropriate reference value, such as the invoice number.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent bookings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt2*  
Enter any other appropriate reference value, such as order number.

- *Date*  
Enter the booking date. Date format must be DDMMYY.

- *Account*   
Enter the appropriate account number, for example a personal account number, that is, customer or supplier number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

  > [Info] Customer and supplier personal accounts can be created, edited and deleted. For detailed information, see [Manage the customer/supplier](/RetailSuiteAccounting/Integration/05_ManageCustomerSupplier.md).

- *COST1*  
Enter the appropriate value. This is only applicable is a cost center accounting for cost 1 has been set up. For detailed information, see [COST ACCOUNTING](XX_CostAccounting.md).

- *COST2*  
Enter the appropriate value. This is only applicable is a cost center accounting for cost 2 has been set up. For detailed information, see [COST ACCOUNTING](XX_CostAccounting.md).

- *Booking text*  
Enter any appropriate booking text. Booking text can contain a combination of letters and numbers.


When creating a manual booking or selecting an existing booking, the account/contra account details, as well as their current balances, are displayed under the entry line.

- *Contra account*  
This field displays the selected contra account. This field is read-only.

- *Account*  
This field displays the selected account. This field is read-only.

- *Balance (amount)H/S (currency)*  
This field displays the current balance of the corresponding account. H stands for credit. S stands for debit.



- [BOOK]    
Click this button to record the booking in the entry line.

- [CANCEL]
Click this button to cancel the selected booking. For detailed information, see [Cancel a booking](/RetailSuiteAccounting/Operation/05_CancelBooking.md).

- [DELETE]    
Click this button to delete the selected booking. For detailed information, see [Delete a single booking](/RetailSuiteAccounting/Operation/06_DeleteBookings.md#delete-a-single-booking).

- [CLEAR]    
Click this button to clear all entry line fields.

- [SPLIT]    
Click this button to split a booking during the manual booking process. The *Split booking* window is displayed, see [Split booking](#splitbooking). For detailed information about splitting a booking, see [Split a booking](/RetailSuiteAccounting/Operation/09_SplitBooking.md).

- [ASSIGN RECEIPT]  
Click this button to assign a receipt to the selected booking. For detailed information, see [Retrieve a receipt](/RetailSuiteAccounting/Operation/10_ManageReceipts.md#retrieve-a-receipt).


## Split booking

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Button SPLIT*

![Split booking window](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/SplitBooking01.png "[Split booking window]")

The information displayed in columns is read-only.

- *Seq. no.*  
This columns displays the sequential number.

- *BP*  
This column displays the booking period (month).

- *Jnl*  
This column displays the journal.

- *Turnover*  
This column displays the turnover value.

- *Contra account*  

- *Receipt1*
- *Receipt2*
- *Date*
- *Account*
- *Cost1*
- *Cost2*
- *Text*


[comment]: <> (There seems to be an unnamed column between Kst2 and Text, usually where B/Belege come in. When clicking on a booking with a linked receipt, the B icon does not appear here. No option to link a receipt here either, so left out from description. Bug/comment?)


- *REMAINDER*

- *Amount*

- *Seq. no.*
- *Turnover*
- *Contra account*
- *Receipt1*
- *Receipt2*
- *Date*
- *Account*
- *Cost1*
- *Cost2*
- *Text*

Rate
Booked.
Split bookings recorded.


7. Split the booking as necessary assigning each split booking to the corresponding contra account.

8. Click the [BOOK] button after each split booking.  
A message in the top left corner of the *Split booking* window confirms each split booking. The split bookings are now listed underneath the main booking in the *Split booking* window.

  ![Bookings split](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/SplitBooking02.png "[Bookings split]")

  > [Info] When the total invoice amount has been divided, the remainder will equal 0. At this point, the [SAVE] button is activated and can be selected.

9. Click the [SAVE] button.  
A message in the top left corner of the *Split booking* window confirms that the split bookings have been recorded.
