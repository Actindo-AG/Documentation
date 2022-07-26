[!!User Interface split booking](../UserInterface/01a_Bookings.md#split-booking)   
[!!User Interface book](../UserInterface/01_Book.md)  

# Split a booking

In some occasions, it may be necessary to split a booking to keep track of different items separately, for example if an invoice includes products with different tax rates or if total costs must be divided into two or more cost centres. Split bookings can affect both debit and credit accounts, that is, incoming and outgoing invoices.

The [SPLIT] button in the *BOOKINGS* tab allows to split bookings during the manual booking process. For detailed information about creating a manual booking, see [Create a manual booking](./04_CreateManualBooking.md).

Once the splitting has been performed, the different split (partial) bookings are assigned to the corresponding accounts. The split bookings are then displayed in the bookings list underneath the main booking.

> [Info] Splitting a booking must be performed during the manual booking process. When splitting an invoice after the booking has been automatically registered following a business transaction or after it has been manually created, the system creates a copy of the existing main booking with the newly assigned contra accounts.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Split booking](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/SplitBooking.png "[Split booking]")

1. Select the appropriate currency for the booking in the *Currency code* drop-down list.

  > [Info] The booking numbers must be sequential and are added by the system automatically.

2. Enter the total invoice value in the *Turnover* field.

3. Enter the date for the manual booking in the *Date* field. Date format must be DDMMYY.

4. Enter a personal account number in the *Account* field, that is, a debtor (customer) or a creditor (provider) account number.

  > [Info] The fields *Date* and *Account* must be filled out to be able to split a booking. The *Contra Account* field can be specified when splitting the booking.

5. Enter any other relevant booking information in the corresponding fields.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent bookings taking this field as reference.

6. Click the [SPLIT] button.  
The *Split booking* window is displayed.  

  ![Split booking window](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/SplitBooking01.png "[Split booking window]")

7. Split the booking as necessary assigning each split booking to the corresponding contra account.

8. Click the [BOOK] button after each split booking.  
A message in the top left corner of the *Split booking* window confirms each split booking. The split bookings are now listed underneath the main booking in the *Split booking* window.

  ![Bookings split](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/SplitBooking02.png "[Bookings split]")

  > [Info] When the total invoice amount has been divided, the remainder will equal 0. At this point, the [SAVE] button is activated and can be selected.

9. Click the [SAVE] button.  
A message in the top left corner of the *Split booking* window confirms that the split bookings have been recorded.
