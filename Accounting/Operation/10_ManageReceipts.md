[!!Accounting](Actindo/Accounting)

# Manage receipts

Receipts are used to document all transactions and, therefore, play an indispensable role for a correct accounting. There are many different types of receipts, such as invoice, order confirmation, or credit note. For detailed information about the different types of receipts, see [Invoicing / Types of receipts](#to_be_completed).
[comments]: <> (See alt_Doku)

The *BOOK RECEIPTS* tab allows to assign manually incoming receipts that have not been registered yet in the *Accounting* module. Providers can upload their invoices in PDF format in the *Documents* module, which will be then registered by the system and displayed in the *BOOK RECEIPTS* tab.

After being uploaded, the receipts are stored in the *New documents* folder in the *Documents* module. Once they are manually booked, they are moved automatically into the *Booked documents* folder and then placed in the appropriate subfolder according to the following structure:

- 10000-19999 account numbers in case of a debtors'/customers' document
- 70000-70999 account numbers in case of a creditors'/providers' document

Besides, when the receipt is booked in the *BOOK RECEIPTS* tab, it is linked to a particular booking. A blue B (=Beleg, EN: receipt) will be then displayed next to the booking in the bookings list. When clicking on the blue B, the corresponding receipt is displayed.


## Retrieve a receipt

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- An incoming receipt is created, see [Invoicing / Manage receipts / Create receipts](#to_be_completed).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOK RECEIPTS*

![Booking receipts](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BookReceipts_NewDocument.png "[Book receipts]")

1. Select the appropriate currency in the *Currency code* field, if necessary.

  > [Info] Currency exchange rate can also be adjusted if needed in the *Rate* field. For detailed information, see []

[comment]: <> (Fremdwährungsassistent zur Automatisierung? Link?)

2. Enter the total invoice value in the *Turnover* field.

3. Contra Account

4. Enter the invoice number or reference number in *Receipt1* field.

5. Enter the date for the manual booking in the *Date* field. Date format must be TTMMJJ or TT.MM.JJ.

6. Enter a personal account number in the *Account* field, that is, a debtor (customer) or a creditor (provider) account number.

  > [Info] Note that the fields *Date* and *Account* must be filled out to be able to book a receipt. The *Contra Account* field can be specified when splitting the booking.

  [comment]: <> (Check!)

7. Enter any other relevant fixed booking information in the corresponding fields.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent bookings taking this field as reference.

8. Click the [BOOK] button.  
A message above the entry line confirms that the receipt has been linked to the booking. A new booking is displayed in the bookings list in the *BOOKING* tab. A new open item is created in the *OPEN ITEMS* tab.


![Booking receipts](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BookReceipts_no_receipts.png "[Book receipts]")

> [Info] If there is no receipt left to be booked, the message *No documents left to be registered* is displayed when clicking the *BOOK RECEIPTS* tab.


  > [Info]


### Next steps

  - [Book a receipt](#book-a-receipt)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Fakturierung / Belegesorten](#to_be_completed)
  - [Dokumente - Neue / Verbuchte Dokumnete](#to_be_completed)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)


## Book a receipt

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![](/Assets/Screenshots/Accounting/Book/Bookings/.png "[]")

1.

  > [Info]

2. Enter in the ** field.

3. Enter  in the ** field.

4. Enter  in the ** field.

  > [Info]

5. Enter any other relevant fixed booking information in the corresponding fields.

  > [Info]

6. Click the ** button.
The ** window is displayed.

  ![](/Assets/Screenshots/Accounting/Book/Bookings/.png "[]")

7.

8. Click the [] button.


  ![](/Assets/Screenshots/Accounting/Book/Bookings/.png "[]")

  > [Info]

### Next steps

  - [Book a supplier receipt](#book-a-supplier-receipt)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage receipts](10_ManageReceipts.md)
  - [Dokumente - Neue / Verbuchte Dokumnete](#to_be_completed)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)


## Book a supplier receipt

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

### Procedure

- information about the wizard for supplier receipts and its features and its availability

- Lieferantenbelege Option - erweiterter Prozess zu Belege buchen, um Lieferantenbelege zu erfassen

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![SupplierBookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Edit_SupplierBookings.png "[SupplierBookings]")


1.  

  > [Info]

2. Enter in the ** field.

3. Enter  in the ** field.

4. Enter  in the ** field.

  > [Info]

5. Enter any other relevant fixed booking information in the corresponding fields.

  > [Info]

6. Click the ** button.
The ** window is displayed.

  ![Split booking window](/Assets/Screenshots/Accounting/Book/Bookings/.png "[Split booking window]")

7.

8. Click the [] button.


  ![Split booking window](/Assets/Screenshots/Accounting/Book/Bookings/.png "[Split booking window]")

  > [Info]


### Next steps

  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage receipts](10_ManageReceipts.md)
  - [Dokumente - Neue / Verbuchte Dokumnete](#to_be_completed)
  - [Manage open items](03_ManageOpenItems.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)
