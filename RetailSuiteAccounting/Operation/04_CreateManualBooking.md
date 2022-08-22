[!!User Interface bookings](../UserInterface/01a_Bookings.md)  
[!!User Interface select fiscal year](../UserInterface/00a_FiscalYear.md)   
[!!User Interface FY/MONTH/JOURNAL](../UserInterface/00_Book.md#fymonthjournal)  


# Create a manual booking

Even though transactions are usually posted automatically through the automated functions across the different modules, you can also record postings manually. In some cases, it is necessary to record transactions manually when a transaction has been performed but not yet recorded, for example a cash payment or an issued invoice.

 > [Info] It is essential to select the correct booking period, that is, the correct fiscal year, month and journal, before making a manual booking. For detailed information, see [Select fiscal year](./01_SelectFiscalYear).

#### Prerequisites

A fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Bookings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Bookings]")

1. If necessary, click the *Currency code* drop-down list and select the appropriate currency for the posting. All available currencies are displayed in the list. By default, the base currency is preselected.

  > [Info] The booking numbers must be sequential and are added by the system automatically.

2. Enter the posting amount in the *Turnover* field.

3. Enter an account number in the *Contra account* field.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list.

4. Enter the date for the manual booking in the *Date* field. The valid date format is *DDMMYY*.

5. Enter an account number in the *Account* field.
  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list.
  > [Info] Note that the fields *Contra account*, *Date* and *Account* must be filled out to be able to create a booking.

6.  If desired, enter any other relevant manual booking information in the corresponding fields.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent bookings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

7. Click the [BOOK] button.  
The manual posting is created. The notice "Posted." is displayed above the input line. The manual posting is displayed in the postings list.

  ![Manual booking created](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/ManualBookingCreated.png "[Manual booking created]")
