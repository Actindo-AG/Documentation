[!!Accounting](Actindo/Accounting)

# Split a booking

In some occasions, it may be necessary to split a booking to keep track of different items separately, for example if an invoice includes products with different tax rates or if total costs must be divided into two or more cost centres. Split bookings can affect both debit and credit accounts, that is, incoming and outgoing invoices.

The [SPLIT] button in the *BOOKINGS* tab allows to split bookings during the manual booking process. For detailed information about how to create a manual booking, see [Create a manual booking](05_CreateManualBooking).

Once the splitting has been performed, the different split (partial) bookings are assigned to the corresponding accounts. The split bookings are then displayed in the bookings list underneath the main booking.

> [Info] Splitting a booking must be performed during the manual booking process. When splitting an invoice after the booking has been automatically registered following a business transaction or after it has been manually created, the system creates a copy of the existing main booking with the newly assigned contra accounts.

[comment]: <> (Flo in Video aus Belege Buchen tab, aber wann ist es üblicherweise gemacht?)

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Split booking](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_SplitBooking.png "[Split booking]")

1. Select the appropriate currency for the booking in the  *Currency code* drop-down list.

  > [Info] The booking numbers must be sequential and are added by the system automatically.

2. Enter the total invoice value in the *Turnover* field.

3. Enter the date for the manual booking in the *Date* field. Date format must be TTMMJJ or TT.MM.JJ.

4. Enter a personal account number in the *Account* field, that is, a debtor (customer) or a creditor (provider) account number.

  > [Info] Note that the fields *Date* and *Account* must be filled out to be able to split a booking. The *Contra Account* field can be specified when splitting the booking.

5. Enter any other relevant fixed booking information in the corresponding fields.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent bookings taking this field as reference.

6. Click the *SPLIT* button.  
The *Split booking* window is displayed.  

  ![Split booking window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_SplitBooking_Window.png "[Split booking window]")

7. Split the booking as necessary assigning each split booking to the corresponding contra account.

8. Click the [BOOK] button after each split booking.  
A message in the top left corner of the *Split booking* window confirms each split booking. The split bookings are now listed underneath the main booking in the *Split booking* window.

  ![Split booking window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Booking_Split.png "[Split booking window]")

  > [Info] When the total invoice amount has been divided, the remainder will equal 0. At this point, the [SAVE] button is activated and can be selected.

9. Click the [SAVE] button.  
A message in the top left corner of the *Split booking* window confirms that the split bookings have been recorded.


## Next steps

  - [Manage receipts](10_ManageReceipts)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

## See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage receipts](10_ManageReceipts.md)
  - [Dokumente - Neue / Verbuchte Dokumnete](#to_be_completed)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)
