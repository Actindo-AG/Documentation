[!!User Interface Postings](../UserInterface/01a_Bookings.md)  
[!!User Interface Select fiscal year](../UserInterface/00a_FiscalYear.md)   
[!!User Interface FY/MONTH/JOURNAL](../UserInterface/00_Book.md#fymonthjournal)  


# Create a manual posting

Even though transactions are usually posted automatically through the automated functions across the different modules, you can also record postings manually. In some cases, it is necessary to record transactions manually when a transaction has been performed but not yet recorded, for example a cash payment or an issued invoice.

 > [Info] It is essential to select the correct posting period, that is, the correct fiscal year, month and journal, before making a manual posting. For detailed information, see [Select fiscal year](./01_SelectFiscalYear).

[comment]: <> (Ist posting period nicht nur der ausgewählte Monat? Ja, Spaltenname BP zeigt das Monat an, aber im SelectFiscalYear-Fenster musst man alle 3 Kriterien -FY, Monat und Journal- auswählen, damit man eine Periode angezeigt bekommt. Ich meine, Unterschied zwischen Journal und Monat ist trotzdem nicht ganz deutlich...)

#### Prerequisites

A fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Post > Tab POSTINGS*

![Postings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Postings]")

1. If necessary, click the *Currency code* drop-down list and select the appropriate currency for the posting. All available currencies are displayed in the list. By default, the base currency is preselected.

2. Enter the posting amount in the *Turnover* field. This field is mandatory.

   > [Info] The fields *Turnover*, *Contra account*, *Date* and *Account* must be filled to create a manual posting.

3. Enter an account number in the *Contra account* field.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list.

4. Enter a reference number, usually the invoice number, in the *Receipt 1* field.

 > [Info] Even though it is not mandatory, it is highly recommended to fill in the *Receipt 1* field, as it is used as a reference to identify and assign any subsequent postings, for example for an invoice settlement or a credit note in case of refund.

5. Enter the date for the manual posting in the *Date* field. The valid date format is *DDMMYY*.

6. Enter an account number in the *Account* field.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can also select the corresponding account in the list.

7.  If desired, enter any other relevant manual posting information in the corresponding fields.

8. Click the [BOOK] button.  
The manual posting is created. The notice "Posted." is displayed above the input line. The manual posting is displayed in the postings list.
