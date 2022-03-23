[!!Accounting](Actindo/Accounting)

# Manage receipts

Receipts are used to document all transactions and, therefore, play an indispensable role for a correct accounting. There are many different types of receipts, such as invoice, order confirmation, or credit note. For detailed information about the different types of receipts, see [Invoicing / Types of receipts](#to_be_completed).

[comments]: <> (See alt_Doku for reference)

The *BOOK RECEIPTS* tab allows to assign manually incoming receipts that have not been registered yet in the *Accounting* module. Suppliers can upload their invoices in PDF format in the *Documents* module, which will be then recognized by the system and displayed in the *BOOK RECEIPTS* tab.

[comment]: <> (Check with Heusel: 3 options to manage receipts: BELEGE BUCHEN, BELEG ZUORDNEN und extra Funktion LIEFERANTENBELEGE. ALLE unverbuchten Belege werden werden aber unter BELEGE BUCHE gezeigt, nicht nur externe Belege... Also, was ist der Unterschied zwischen BELEGE BUCHEN und LIEFERANTENBELEGE???)

After being uploaded, the receipts are stored in the *New documents* folder in the *Documents* module. Once they are booked, they are moved automatically into the *Booked documents* folder and then placed in the appropriate subfolder according to the following structure:

- 10000-19999 account numbers in case of a debtors'/customers' document
- 70000-70999 account numbers in case of a creditors'/suppliers' document

Besides, when a receipt is booked in the *BOOK RECEIPTS* tab, it is linked to the assigned booking. A ![Receipt](/Assets/Icons/Beleg.png "[Receipt]") icon will be then displayed next to the booking in the bookings list. When clicking on the ![Receipt](/Assets/Icons/Beleg.png "[Receipt]") icon, the corresponding receipt is displayed.

[comment]: <> (Viel Info: evtl. zusammenfassen bzw. verteilen)

## Retrieve a receipt

[comment]: <> (Maybe change name to "Assign a receipt")

The [ASSIGN RECEIPT] button in the *BOOKINGS* tab allows to assign a receipt that has not been registered yet to an existing booking. Any unregistered receipts are displayed in the *BOOK RECEIPTS* tab and can be registered using this option. For detailed information about this procedure, see [Book a receipt](#book-a-receipt).   

[comment]: <> (Rephrase)

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- A manual booking is created, see [Create a manual booking](04_CreateManualBooking.md).
- A receipt is uploaded, see [Documents / New Documents](#to_be_completed).

[comments]: <> (Unsure! Does it need to be a manual booking? Probably not. Also, check interaction with Invoicing. Check with Heusel.)

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS*

![Assign receipt](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_AssignReceipt.png "[Assign receipt]")

1. Select the booking to be assigned a receipt from the bookings list in the *Bookings* tab.  
The existing booking details are displayed in the input line fields.

2. Click the [ASSIGN RECEIPT] button.  
The *Attach Document* window is displayed.

  ![Attach document](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_AttachDocument_Window.png "[Attach document]")

3. Select the document to be assigned to the booking from the *New documents* folder.

  ![Select document](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_AttachDocument_Window2.png "[Select document]")

4. Click the [ACCEPT DOCUMENT] button.  
The selected document is now assigned to the booking. A ![Receipt](/Assets/Icons/Beleg.png "[Receipt]") icon (=Beleg, EN: receipt) will be then displayed next to the booking in the bookings list.

  ![Receipt assigned](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_ReceiptAssigned.png "[Receipt assigned]")

  > [Info] When clicking the ![Receipt](/Assets/Icons/Beleg.png "[Receipt]") icon, the corresponding receipt is displayed. Click the [CANCEL ASSIGNMENT] button if the assignment needs to be undone.

  ![Cancel assignment](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_AttachedDocument_Window.png "[Cancel assignment]")


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

The *BOOK RECEIPTS* tab allows to assign manually incoming receipts that have not been registered yet in the *Accounting* module. Providers can upload their invoices in PDF format in the *Documents* module, which will be then recognized by the system and displayed in the *BOOK RECEIPTS* tab.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- An incoming receipt is uploaded, see [Documents / New Documents](#to_be_completed).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOK RECEIPTS*

![Book receipts - new receipt](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BookReceipts_NewDocument.png "[Book receipts - new receipt]")

  > [Info] The incoming receipts uploaded in the *New documents* folder in the *Documents* module are displayed here. If there are no receipts to be booked, the message *No documents left to be registered* is displayed when clicking the *BOOK RECEIPTS* tab.

  ![Book receipts - no receipts](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BookReceipts_no_receipts.png "[Book receipts - no receipts]")

1. Select the appropriate currency in the *Currency code* field, if necessary.

  > [Info] Currency exchange rate can also be adjusted if needed in the *Rate* field.

[comment]: <> (Fremdwährungsassistent zur Automatisierung? Link?)

2. Enter the total invoice value in the *Turnover* field.

3. Enter an account number in the *Contra Account* field.

4. Enter the date for the manual booking in the *Date* field. Date format must be TTMMJJ or TT.MM.JJ.

5. Enter the creditor (supplier) account number in the *Account* field.

  > [Info] Note that the fields *Contra Account*, *Date*,  *Account* must be filled out to be able to book a receipt.

6. Enter any other relevant fixed booking information in the corresponding fields.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent bookings taking this field as reference.

  ![Booking receipts](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BookReceipts_NewDocument2.png "[Book receipts - no receipts]")

7. Click the [BOOK] button.  
A message above the entry line confirms that the receipt has been linked to the booking. A new booking is displayed in the bookings list in the *BOOKING* tab. A ![Receipt](/Assets/Icons/Beleg.png "[Receipt]") icon (=Beleg, EN: receipt) is displayed next to the booking in the bookings list.

  ![Bookings - document linked](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BookReceipts_DocumentLinked2.png "[Booking - Bookings - document linked]")

  > [Info] If there are further unregistered incoming receipts, they will be displayed in the *BOOK RECEIPTS* tab. Otherwise, the message "No documents left to be registered" is displayed.

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

The *Supplier receipts* menu entry of the *EDIT* context menu in the *BOOKINGS* is an enhanced function to book specifically supplier receipts.

Suppliers can upload their invoices in PDF format in the *New supplier documents* folder in the *Documents* module, which will be then recognized by the system and displayed in the *Acquire* tab.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- The appropriate plug-in is installed, see [Install plug-in XZY](#to_be_completed).

### Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Supplier receipts*

![SupplierBookings](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_Edit_SupplierBookings.png "[SupplierBookings]")

[comment]: <> (Check and add screenshots. RS Nesim)

1.  Click the *Supplier receipt* menu entry.  
The *Supplier receipts* window is displayed.

  > [Info] The incoming receipts uploaded in the *New supplier documents* folder in the *Documents* module are displayed here. If there are no receipts to be booked, the message *No documents left to be registered* is displayed.

2. Enter the total invoice value in the *Turnover* field.

  > [Info] Currency exchange rate can also be adjusted if needed in the *Exchange rate* field.

3. Enter an account number in the *ContraAcct* field.

4. Enter the date for the manual booking in the *Date* field. Date format must be TTMMJJ or TT.MM.JJ.

5. Enter the creditor account number in the *Supplier* field.

6. Enter a description account number in the *Posting text* field.

  > [Info] Note that the fields *ContraAcct*, *Date*,  *Supplier* and *Posting text* must be filled out to be able to acquire a receipt.

6. Enter any other relevant fixed booking information in the corresponding fields.

  > [Info] Even though it is not compulsory, it is highly recommended to fill in the *Reference1* field, as the system identifies and groups together any subsequent bookings taking this field as reference.

  ![](/Assets/Screenshots/Accounting/Book/Bookings/.png "[Book receipts ]")

7. Select the appropriate payment target for the receipt in the *Payment target* drop-down list.

8. Click the [ACQUIRE] button.  

  ![](/Assets/Screenshots/Accounting/Book/Bookings/.png "[]")


[SPLIT] button


  ![](/Assets/Screenshots/Accounting/Book/Bookings/.png "[]")

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
