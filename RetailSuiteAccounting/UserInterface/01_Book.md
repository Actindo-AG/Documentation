[!!Accounting](RetailSuiteAccounting)

# Book

*Accounting > Select fiscal year > Book*

  ![Book](/Assets/Screenshots/RetailSuiteAccounting/Book/FYMonthJournalButton.png "[Book]")

The Accounting *Book* menu entry is used to manage all existing bookings and to create new ones.

The *Book* User Interface is composed of the following tabs:

  - [BOOKINGS](01a_Book.md)
  - [BALANCES](01b_Book.md)
  - [ACCOUNT SHEET](01c_Book.md)
  - [OPEN ITEMS](01d_Book.md)
  - [SEARCH](01e_Book.md)
  - [BOOK RECEIPTS](01f_Book.md)


Additionally, the following cross-tab functions are contained.


## FY/MONTH/JOURNAL

*Accounting > Select fiscal year > Book > Button FY/MONTH/JOURNAL*

  ![Book](/Assets/Screenshots/RetailSuiteAccounting/Book/FYMonthJournalButton.png "[Book]")

Click the [FY/MONTH/JOURNAL] button to display the select fiscal year window. For detailed information, see [Fiscal year](00a_FiscalYear.md) and [Select a fiscal year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md).

New fiscal years can be created, edited or deleted. For detailed information about managing fiscal years, see [Manage the fiscal year](/RetailSuiteAccounting/Integration/04_ManageFiscalYear.md).

## EDIT

*Accounting > Select fiscal year > Book > Context menu EDIT*

Click the *EDIT* button to display the context menu.

  ![EDIT](/Assets/Screenshots/RetailSuiteAccounting/Book/Edit.png "[EDIT]")

  - *Cash book takeover*  
  Click this menu entry to take over automatically cash payments registered in the cash book. The *Cash book takeover* window is displayed, see [Cash book takeover](#cash-book-takeover).

  [comment]: <> (RS FH about function and need of procedure. How is it used by customers?)

  - *Bank data takeover*  
  Click this menu entry to take over bank and payment details registered in the *Payment processing* module. The *Bank data synchronizing* window is displayed, see [Bank data takeover](#bank-data-takeover).

  [comment]: <> (RS FH about function and need of procedure. How is it used by customers? FH: It can probably be deleted. It is no longer/hardly? used and will be deleted in next releases. To be confirmed!)

  - ![Lock](/Assets/Icons/Lock02.png "[Lock]") *Process*  
  Click this menu entry to process one of several bookings in a booking period. The *Process bookings* window is displayed, see [Process](#process).

  - ![Do not enter](/Assets/Icons/DoNotEnter.png "[Do not enter]") *Delete*  
  Click this menu entry to delete one or several bookings simultaneously. The *Delete bookings* window is displayed, see [Delete](#delete).

  - ![Lock](/Assets/Icons/Lock02.png "[Lock]") *Lock months*  
  Click this menu entry to lock one or several months for bookings. The *Lock months* window is displayed, see [Lock months](#lock-months).

  - *Balance carried forward*  
  Click this menu entry to carry forward balances from the previous fiscal year. The *Balance carried forward: step 1* window is displayed, see [Balance carried forward](#balance-carried-forward).

  - *Foreign currency wizard*  
  Click this menu entry to carry book automatically currency exchange differences. The *Foreign currency wizard* window is displayed, see [Foreign currency wizard](#foreign-currency-wizard).

  - *Supplier receipts*  
  Click this menu entry to book specifically supplier receipts. The *Supplier receipts* window is displayed, see [Supplier receipts](#supplier-receipts).


### Cash book takeover  

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Cash book takeover*

  ![Cash book takeover](/Assets/Screenshots/RetailSuiteAccounting/Book/CashBookTakeover.png "[Cash book takeover]")

This window displays all cash payments registered in the cash book, which can be taken over automatically in the *Accounting* module. All information provided in columns is read-only, except for the *T* column.

[comment]: <> (Add link when docu available: For detailed information, see ...)

  - *Seq. no.*  
    Sequential number as registered in the cash book.

  - [x] *T (Take over booking)*  
   Select this checkbox to take over an individual booking.

  - *BP*  
    Booking period as registered in the cash book.

  - *Jnl*  
    Journal as registered in the cash book.

  - *Turnover*  
    Turnover value as registered in the cash book. Revenues display a positive sign. Expenditures display a negative sign.

  - *Contra Account*  
    Contra Account as registered in the cash booking.

  [comment]: <> (No account in cash book! What does the number stand for? As "Unbekannt!")   

  - *Receipt1*  
    Receipt 1 as registered in the cash book.

  - *Receipt2*  
    Receipt 2 as registered in the cash book.

  - *Date*  
    Date as registered in the cash book.

  - *Account*  
    Account as registered in the cash book.

  - *Cst1*  
    Cost 1 as registered in the cash book.

  - *Cst2*  
    Cost 2 as registered in the cash book.

  - *Text*  
    Free text as registered in the cash book.


  - [SELECT ALL]     
    Click this button to select all bookings.

  - [SELECT NOTHING]    
    Click this button to deselect all bookings.

  - *Amount*  
    Total amount of all bookings in the cash book.


An individual booking from the cash book can be selected and partially edited before takeover. Click the booking to be edited. Its details are displayed in the entry line.

[comment]: <> (Unsure! RS FH. Add operartion file? RS FH!)

  - *Seq. no.*  
   This field displays the booking sequential number and cannot be modified.  

  - *Turnover*  
  This field displays the turnover and cannot be modified.

  - *Contra account*  
  Enter the appropriate contra account, see [Chart of accounts](/RetailSuiteAccounting/Integration/01_RunAccountingWizard.md#chart-of-accounts). This field is compulsory.

  > [Info] When you start typing in an account number, a context menu is displayed. You can also select the appropriate option from the menu.

  - *Receipt1*  
  Enter the appropriate value. The existing value can also be modified.

  - *Receipt2*  
  Enter the appropriate value. The existing value can also be modified.

  - *Date*  
  This field displays the date and cannot be modified.

  - *Account*  
  This field displays the account and cannot be modified.

  - *Cost1*  
  Enter the appropriate value. The existing value can also be modified.

  - *Cost2*  
  Enter the appropriate value. The existing value can also be modified.

  - *Text*  
  Enter the appropriate free text. The existing value can also be modified.

  - [BOOK]    
  Click this button to book the edited booking.

  - [DELETE]    
  Click this button to delete the selected booking.

  [comment]: <> (FEHLER: löschen hier nicht möglich! -> even though takeover not yet performed? Probably because it is linked to cash book/Kassenbuch? What is the use of this button here? RS FH)

  - [CLEAR]    
  Click this button to clear all entry line fields.

  - [SPLIT]    
  Click this button to split the selected booking.

  [comment]: <> (Fehlermeldungen: beim klicking auf SPLIT -> Unbekannte Bankbuchung. Wenn man versucht, eine Splitbuchung zu machen -> Meldung: Gebucht und in rot "Umsatz, GegKonto, Datum oder Konto leer! Ungültiges Datum!" Alle Felder sind aber richtig ausgefüllt, jetzt zeigen sie aber alle 0, außer Beleg 1, GegKonto und Text)

  - [SAVE]    
  Click this button to take over the selected bookings.


### Bank data takeover  

[comment]: <> (This function is supposed to be deleted in a next release. Delete from here? Still in use? for how long? Worth completing it? RS FH/HG!)

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Bank data takeover*

  ![Bank data synchronizing](/Assets/Screenshots/RetailSuiteAccounting/Book/BankDataSynchronizing.png "[Bank data synchronizing]")

This screen is also available in the *Payment processing* module. Both modules are closely linked with each other.

[comment]: <> (Link when available?)

  - *Bank account*  
  Click the drop-down list to select the bank account where data must be imported from.

 - *Load registered* [x]  
  Click this checkbox to activate the [SHOW REGISTERED] button.

  > [Info] This function is per default deactivated to reduce system overload and improve performance. This default setting can be changed in the *Settings* menu entry of the *Payment processing* module.

  [comment]: <> (Add link when available)

  - *FY/month*  
  Click the corresponding drop-down list to select the fiscal year and month of the data to be displayed.

  - [RETRIEVE/IMPORT]  
  Click this button to display the *Retrieve bank data* window, see [Retrieve bank data](#retrieve-bank-data).

[comment]: <> (RS FH needed. I did not manage to import bank data.)

  - [SHOW REGISTERED]  
  Click this button to display all booked payments.

  - [SHOW HIDDEN]  
  Click this button to display all hidden payments.

  - [QUICK SEARCH]  
  Click this button to display the *QUICK SEARCH* context menu. Payments can be searched for using the following search criteria:

  - *Turnover*
  - *Contra account*
  - *Receipt1*
  - *Receipt2*
  - *Account*
  - *Text*
  - *Reference*
  - *Recipient*

 [comment]: <> (Vorsicht: Übersetzung von Verwendungszweck? "Purpose code" is mentioned by FH in training video, but really used in this area?)

 - [Search bar]  
 Enter here the value to be searched for. You can press ENTER to start the search.

 - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross)  
 Click this button to delete the entered value.

 - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
 Click this button to search for payments matching the entered values and search criteria.

The imported bank data are displayed in the following columns:

 - *Seq. no.*  
 This column displays the sequential number.

 - *T* (Take over)  
 Click the checkbox in this column to select the payment.

 - *B* (xxx)  
 This column displays the payment status.

  - Green  
  An incoming payment has been matched with an existing open item.
  - Yellow  
  An incoming payment probably matches and existing open item but there are discrepancies to be checked.
  - Red  
  No matching open item found for the payment.

    > [Info] If a payment is processed manually, a *M* will be displayed in this column.

[comment]: <> (B für Beleg, Bearbeiten, Buchhaltung??? Change column name accordingly here and in IU Terminology file! Add screenshot/icons)  

  - S (Search)  
  The ![Search](/Assets/Icons/Search.png "[Search]") (Search) icon is displayed in this column. Click this button to search for open items.

 [comment]: <> (New window opens up. Name? Add and describe!)

 - *Turnover*  
 This column displays the turnover value.

 - *Contra account*  
 This column displays the contra account assigned, if any.

 - *Receipt1*  
 This column displays the receipt 1 value, usually the invoice number.

 - *Receipt2*  
 This column displays the receipt 2 value.

 > [Info] The following payment reference details are displayed in the columns view and used by the system to match each payment with an existing open item:
  - Customer number
  - Invoice number
  - Order number
  - Customer name
  - Customer e-mail address


 - *Date*  
 This column displays the payment date.

 - *Account*  
 This column displays the account assigned, if any.

 - *Text*  
 This column displays the booking text, if any.

- ![First page](/Assets/Icons/FirstPage.png "[First page]") - ![Last page](/Assets/Icons/LastPage.png "[Last page]") (Fist page) - (Last page)  
 ![Previous page](/Assets/Icons/PreviousPage.png "[Previous page]") - ![Next page](/Assets/Icons/NextPage.png "[Next page]") (Previous page) - (Next page)  
Click these buttons to navigate the payment list.

- *Page [x] of [x]*  
Enter a page number to go to a specific page.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
 Click this button to update the payment list.

- [RESET]  
 Click this button to reset the payment list view.

 [comment]: <> (Unsure! Check!)


- Green [x]
- Yellow [x]
- Red [x]
- Grey [x]
- [M] [x]

[comment]: <> (Check last two!)

- [SELECT GREEN]
- [SELECT YELLOW]
- [RESET SELECTION]

The payments can also be processed manually. Click any payment in the list to display its values in the entry line fields.

- *Seq. no.*

- *Turnover*

- *Contra account*

- *Receipt1*

- *Receipt2*

- *Date*

  -  ![Calendar](/Assets/Icons/Calendar.png "[Calendar]") (Calendar)


- *Account*

- *Cost1*

- *Cost2*

- *Text*


- [BOOK]

- [DELETE]

- [CLEAR]

- [SPLIT]

- [TAKE OVER MARKED]

- [HIDE MARKED]

- [SHOW MARKED]



- *Last retrieval*

- [LEARN FILE]

- [CANCEL]


#### Retrieve bank data

![Retrieve bank data](/Assets/Screenshots/RetailSuiteAccounting/Book/RetrieveBankData.png "[[Retrieve bank data]")

- *Bank*
- *Account / routing number*
- *Date from*  
 - **Automatic**  
 - **Selection** [Date field]
- *Import definition*
- *Edit*
- *CSV file*
- *Select file*
- *No file selected*


- [CANCEL]
- [FINALIZE]


### Process

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Process*

  ![Process bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/ProcessBookings01.png "[Process bookings]")

This window allows to select one or several bookings to be processed simultaneously.

- *Journal from - to*  
Click these drop-down lists to select the journals to be processed. The drop-down lists display the existing journals including the bookings (or postings) recorded in each of them.

- *Month from - to*   
Click these drop-down lists to select the months to be processed. The drop-down lists display all available months in the system. The following options are available:  

  - **0 - Balances carried forward**
  - **1 - 12 - (months)**
  - **13 - 15 - Subsequent bookings**
  - **16 - 25 - Closing bookings**
  - **99 - General month**


- [CANCEL]  
Click this button to cancel your selection.

- [OK]  
Click this button to confirm your selection.

For detailed information about processing bookings, see [Process bookings](/RetailSuiteAccounting/Operation/07_ProcessBookings.md).



### Delete

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Delete*

  ![Delete bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/DeleteBookings.png "[Delete bookings]")

  This window allows to select one or several bookings in a journal to be deleted simultaneously.

  - *Journal*  
  Click this drop-down list to select the journal containing the bookings (or postings) to be deleted. The drop-down list displays the existing journals including the bookings recorded in each of them.

  - *Seq. nos.*   
  Enter the sequential numbers corresponding to the bookings to be deleted.

  - [CANCEL]  
  Click this button to cancel your selection.

  - [DELETE]  
  Click this button to delete the selected bookings.

  For detailed information about processing bookings, see [Delete bookings](/RetailSuiteAccounting/Operation/06_DeleteBookings.md).


### Lock months

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Lock months*

  ![Lock months](/Assets/Screenshots/RetailSuiteAccounting/Book/LockMonths.png "[Lock months]")

  This window allows to select one or several months to be locked for bookings. Locked months can also be unlocked and made bookable again.

  - *[x] - [x] month*  
  Click this drop-down list to select the appropriate option. The following options are available:

   - **Locked**  
   Select this option to lock the month for bookings.

   > [Info] No further bookings will be recorded in the selected month. Any further bookings will be recorded in the next bookable month.

   - **Bookable**  
   Select this option to unlock a previously locked month. The selected month will be bookable again.


  - [CANCEL]  
  Click this button to cancel your selection.

  - [OK]  
  Click this button to confirm your selection.

  For detailed information about processing bookings, see [Lock a period for bookings](/RetailSuiteAccounting/Operation/08_LockPeriodBookings.md).

### Balance carried forward

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Balance carried forward*

  ![Balance carried forward: step 1](/Assets/Screenshots/RetailSuiteAccounting/Book/BalanceCarriedForward01.png "[Balance carried forward: step 1]")

The *Balance carried forward: Step 1* window allows to select balances to be carried forward to the next fiscal year.

- *Carry forward from FY*  
Click the drop-down list to select the year containing the balance(s) to be carried forward.

- *Range from - to*  
Click the drop-down list to select the account(s) containing the balance(s) to be carried forward. The following options are available:

 - **01: Financial accounts**
 - **02: Impersonal accounts**
 - **03: Input tax + VAT**
 - **04: P&L**
 - **05: Open items debtors**
 - **06: Open items creditors**


- *Booking date*  
Enter the booking date for the balance(s) carried forward.

  > [Info] By default, the system displays the first day of the new fiscal year. This can be modified simply by typing in the desired booking date.

- *Delete old balances carried forward from selected FY* [x]  
Select this checkbox to delete the old balance(s) carried forward from the selected fiscal year.

- [CANCEL]  
Click this button to cancel your selection.

- [CONTINUE]  
Click this button to proceed to the *Retrieve account balances* window.


  ![Retrieve account balances](/Assets/Screenshots/RetailSuiteAccounting/Book/RetrieveAccountBalances.png "[Retrieve account balances]")

The *Retrieve account balances* window confirms the values previously selected and offers the possibility to narrow down the account selection.

- *Carry forward from FY*  
The previously selected fiscal year is displayed. This field is read-only.

- *Range from - to*  
The previously selected account range is displayed. These fields are read-only.

- *Date*  
The previously selected booking date is displayed. This field is read-only.

- *Accounts*  
The accounts containing a balance to be carried forward are displayed together with the balance amount. The balance amount can be both positive or negative.

  >[Info] Hold the Ctrl (control) key and click on each account with the left mouse button to select multiple accounts simultaneously.

- *Delete old balances carried forward from selected FY*  
The previously selected value (**Yes/No**) date is displayed. This field is read-only.

- [BACK]  
Click this button to go back to the previous step.

- [CANCEL]  
Click this button to cancel the whole process.

- [CONTINUE]  
Click this button to proceed to carry the selected balances forward.

For detailed information about creating a balance carried forward, see [Create a balance carried forward](/RetailSuiteAccounting/Operation/11_CreateBalanceCarriedForward.md).


### Foreign currency wizard

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Foreign currency wizard*

  ![Foreign currency wizard](/Assets/Screenshots/RetailSuiteAccounting/Book/ForeignCurrencyWizardWindow01.png "[Foreign currency wizard]")

  The *Foreign currency wizard* window allows to search for accounts containing exchange rate differences and  book these differences automatically in special revenues and expenses accounts set up for this purpose.

- *Fiscal year*  
Click the drop-down list to select the applicable fiscal year.

- *Range of accounts*  
Click the drop-down list to select the applicable accounts. The following accounts can be selected:

 - **Open items debtors and creditors**  
 Select this option to check for exchange rate differences in debtors and creditors accounts.
 - **Open items debtors**  
 Select this option to check for exchange rate differences in debtors accounts.
 - **Open items creditors**  
 Select this option to check for exchange rate differences in creditors accounts.
 - **Individual**  
 Select this option to enter a self-defined account number range. When selecting this option, two new fields (*from* - *to*) are displayed. Enter the applicable account number range in these fields.

    ![Foreign currency wizard - Individual](/Assets/Screenshots/RetailSuiteAccounting/Book/ForeignCurrencyWizardWindow02.png "[Foreign currency wizard - Individual]")


  - *Booking date*  
  Enter the corresponding booking date.

  > [Info] You can type in the booking date or use the ![Calendar](/Assets/Icons/Calendar.png "[Calendar]") (Calendar) icon.

  - [BACK]   
  This button is greyed out, as there is no previous step.

[comment]: <> (Comment added in the BUGS document for improvement, e.g. "ABBRECHEN/CANCEL" button instead, like in Saldovortrag function)

  - [CONTINUE]  
  Click this button to proceed to the next step.


![Foreign currency wizard - Account selection](/Assets/Screenshots/RetailSuiteAccounting/Book/ForeignCurrencyWizardWindow03.png "[Foreign currency wizard - Account selection]")

- *Account selection*  
Click the drop-down list to select the account(s) containing the exchange rate difference(s) to be booked.

- [BACK]  
Click this button to go back to the previous step.

- [CONTINUE]  
Click this button to book the exchange rate difference(s) in the applicable revenues or expenses accounts.

For detailed information about booking exchange rate fluctuations, see [Book exchange rate fluctuations](/RetailSuiteAccounting/Operation/12_BookExchangeRateFluctuations.md).



### Supplier receipts

#### Acquire a receipt

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Supplier receipts > Tab Acquire*

  ![Acquire supplier receipts](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsAcquire.png "[Acquire supplier receipts]")

The *Acquire* tab displays all unregistered supplier receipts uploaded to the *New supplier receipts* folder in the *Documents* module.

- ![Previous](/Assets/Icons/Previous.png "[Previous]") *Document* ![Next](/Assets/Icons/Next.png "[Next]")   
Click the arrow previous/next buttons to scroll through the documents.

- ![First page](/Assets/Icons/FirstPage02.png "[Previous]") ![First page](/Assets/Icons/Previous.png "[Previous]") *Page [x]* ![Next](/Assets/Icons/Next.png "[Next]")  
The current page number is displayed. Click the arrow first page/previous/next buttons to scroll through the pages.

- (-) *Zoom* (+)  
Click the -/+ buttons to zoom in and out of the document view.

- *Download file*  
Click this button to download the document.

- *Turnover*  
Enter the turnover value to be registered. This field is compulsory.

- *ContraAcct*  
Select the appropriate contra account. This field is compulsory.

  >[Info] You can type it in or select it from the drop-down list. When you start typing, a context menu is displayed.

- *Reference1*  
Enter an applicable reference value.

[comment]: <> (Receipt1?)

- *Reference2*  
Enter an applicable reference value.

[comment]: <> (Receipt2?)

- *Date*  
Enter the booking date. Date format must be DDMMYY. This field is compulsory.

- *Supplier*  
Select the appropriate supplier account. This field is compulsory.

  >[Info] You can type it in or select it from the drop-down list. When you start typing, a context menu is displayed.

- *Booking text*  
Enter an appropriate booking text. This field is compulsory.

[comment]: <> (Posting text in the actual UI and in file Operation/10_ManageReceipts.md? Check and unify!)

- *Payment target*  
Click the drop-down list to select the appropriate payment target. The following options are available:

 - **1 - 8 d 2%, 30 d net**
 - **2 - 30 d net**


- *Exchange rate*  
Enter the applicable exchange rate, if necessary.

- *Cost center*  
Enter the appropriate cost center, if necessary.

[comment]: <> (In other functions called Cost1? Check and unify)

- *Cost unit*  
Enter the appropriate cost unit, if necessary.

[comment]: <> (In other functions called Cost2? Check and unify)

- *Commentary for auditors*  
Enter any relevant comments for potential auditors.

- [ACQUIRE]  
Click this button to register the receipt in the system.

- [SPLIT]  
Click this button to perform a split booking, if necessary.

#### Overview

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Supplier receipts > Tab Overview*

  ![Overview](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsOverview.png "[Overview]")

The *Overview* tab displays all receipts that have been acquired (or preregistered) in the system via the *Acquire* tab. The acquired receipts can be searched for using the [QUICK SEARCH] button. The overview can also be filtered using the filter function.

  ![Search and filter functions](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsOverview02.png "[Search and filter functions]")

- [QUICK SEARCH]  
Click this button to display the *QUICK SEARCH* context menu. All search criteria are selected per default through a marked checkbox. Deselect any search criteria as necessary. The following search criteria are available:

 - *Status*  
 - *Supplier*
 - *ContraAcct*
 - *Doc*  
 - *Reference1*
 - *Reference2*
 - *Booking text*
 - *Date*
 - *Amount*
 - *Flag*
 - *Comment*
 - *Comments*
 - *Reason for rejection*
 - *Created by*
 - *Modified by*
 - *Date (creation)*
 - *Date (modification)*
 - *Rejected*
 - *Supervisor*
 - *Cost center*
 - *Cost unit*


 - [Search bar]  
 Enter here the value to be searched for. You can press ENTER to start the search.

 - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross)  
 Click this button to delete the entered value.

 - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
 Click this button to search for receipts matching the entered values and search criteria.


- [(X) ACTIVE FILTERS]

- *ACTIVE* (checkbox)  
 Mark this checkbox to activate the search criteria.

- *FILTER BY*  
The following filter values are available:

  - Status  
 Click the drop-down list to select one or several of the following filter criteria:

   - **New**
   - **Released**
   - **Pending**
   - **Rejected**
   - **Completed**   

 - Supplier  
Enter the appropriate supplier account.

  - ContraAcct  
Enter the appropriate contra account.

  - Reference1  
Enter an appropriate reference value.

  - Reference2  
Enter an appropriate reference value.

  - Bookings text  
Enter an appropriate booking text.

  - Date  
Click the drop-down list to select the applicable search criteria:
    - Select **=** to search for an exact date.
    - Select **between** to search for a date range.
    - Select **before** to search for a period up to a specific date.
    - Select **after** to search for a period after a specific date.  

    > [Info] You can type in the booking date or use the ![Calendar](/Assets/Icons/Calendar.png "[Calendar]") (Calendar) icon.

  - Payment target  
Click the drop-down list to select the applicable payment target. The following options are available:

    - **1 - 8 d 2%, 30 d net**
    - **2 - 30 d net**

 - Created by  
Enter the name of the applicable user.

  - Modified by  
Enter the name of the applicable user.

  - Rejected by  
Enter the name of the applicable user.

  - Date (creation)  
Click the drop-down list to select the applicable search criteria:
    - Select **=** to search for an exact date.
    - Select **between** to search for a date range.
    - Select **before** to search for a period up to a specific date.
    - Select **after** to search for a period after a specific date.  

    > [Info] You can type in the booking date or use the ![Calendar](/Assets/Icons/Calendar.png "[Calendar]") (Calendar) icon.

  - Date (modification)  
Click the drop-down list to select the applicable search criteria:
    - Select **=** to search for an exact date.
    - Select **between** to search for a date range.
    - Select **before** to search for a period up to a specific date.
    - Select **after** to search for a period after a specific date.  

    > [Info] You can type in the booking date or use the ![Calendar](/Assets/Icons/Calendar.png "[Calendar]") (Calendar) icon.

  - Rejected  
Click the drop-down list to select the applicable search criteria (**Yes/No**).

  - Supervisor  
Enter the name of the applicable supervisor.

- [CANCEL]  
Click this button to cancel your selection.

- [APPLY]  
Click this button to apply the search criteria and values.


![Columns layout and sorting](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsOverview03.png "[Columns layout and sorting]")

All acquired receipts are displayed in the columns view. The column width can be modified using the mouse. To do so, place the mouse pointer on the vertical dividing line between two columns titles. The mouse pointer changes to a double-headed arrow. Press the left mouse button and move the line using drag and drop until it has reached the required width.

When placing the cursor on a column header, three vertical points are displayed to the right of the column title. Click the ![Points](/Assets/Icons/Points02.png "[Points]") (Points) icon to display the context menu. The following menu entries are available:

- ![Sort ascending](/Assets/Icons/SortAscending.png "[Sort ascending]") Sort ascending  
  Click this entry to sort the rows in ascending order.
- ![Sort descending](/Assets/Icons/SortDescending.png "[Sort descending]") Sort descending  
  Click this entry to sort the rows in descending order.
- ![Columns](/Assets/Icons/Columns02.png "[Columns]") Columns  
  Place the mouse on this entry to display the *Columns* sub-menu. Add or remove columns by marking or unmarking the corresponding checkbox.
- ![Checbox](/Assets/Icons/Checkbox02.png "[Checkbox]") Filter  
  Place the mouse on this entry to display the search bar. Enter a search value in the search bar and click the checkbox to filter the rows according to the search value.


All information provided in columns is read-only, except for the *Doc* column.

- *Status*  
There are five possible statuses, all of them identified with a different color code. Hover the mouse over the status icon reveal its meaning. The five statuses available are:
  - ![New](/Assets/Icons/New.png "[New]") New
  - ![Released](/Assets/Icons/Released.png "[Released]") Released
  - Pending
  - ![Rejected](/Assets/Icons/Rejected.png "[Rejected]") Rejected
  - Completed

  > [Info] This function works together with the *Purchasing* module, where the receipt is checked and released (or rejected) by the assigned supervisor. The status changes here accordingly. For detailed information about booking supplier receipts, see [Book a supplier receipt](/RetailSuiteAccounting/Operation/10_ManageREceipts.md#book-a-supplier-receipt).

[comment]: <> (Icons missing! To be completed.)

- *Supplier*  
The supplier account number is displayed.

- *ContraAcct*  
The contra account number is displayed.

- *Doc*  
Click the ![B](/Assets/Icons/Beleg02.png "[B]") icon to display the acquired receipt in a new window.

[comment]: <> (Describe new window? Angehängtes Dokument window. See 01a_Book.md, Document attached.)

- *Reference1*  
The reference 1 value is displayed, if available.

- *Reference2*  
The reference 2 value is displayed, if available.

- *Booking text*  
The booking text is displayed.

- *Date*  
The date is displayed.

- *Amount*  
The turnover amount is displayed.

- *Payment target*  
The selected payment target is displayed.

- *Flag*  
A color name may be displayed here if the receipt has been flagged in the *Purchasing* module.

[comment]: <> (Einkauf / Lieferantenbelege prüfen / Beleg markieren / Flag + Comments)  

- *Comment*  
A brief comment may be displayed here if the receipt has been flagged in the *Purchasing* module.

- *Comments*  
If a comment has been added, the ![Comment](/Assets/Icons/Comment.png "[Comment]") comment icon is displayed. Click the icon to read the comment(s) in a new window.

- *Reason for rejection*  
If the receipt has been rejected and a reason has been given, the ![Comment](/Assets/Icons/Comment.png "[Comment]") comment icon is displayed. Hover over the icon with the mouse to read the comment.

- *Created by*  
The assigned user name is displayed.

- *Modified by*  
The assigned user name is displayed.

- *Rejected by*  
The assigned user name is displayed.

- *Date (created)*  
The creation date is displayed.

- *Date (modification)*  
The modification date is displayed.

- *Rejected*  
If rejected, a struck-through red-colored **Yes** is displayed.

- *Supervisor*  
The assigned supervisor name is displayed.


- ![First page](/Assets/Icons/FirstPage.png "[First page]") - ![Last page](/Assets/Icons/LastPage.png "[Last page]") (Fist page) - (Last page)  
 ![Previous page](/Assets/Icons/PreviousPage.png "[Previous page]") - ![Next page](/Assets/Icons/NextPage.png "[Next page]") (Previous page) - (Next page)  
Click these buttons to navigate the receipt list.

- *Page [x] of [x]*  
Enter a page number to go to a specific page.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
 Click this button to update the receipt list.

- [RESET]  
 Click this button to reset the receipt list view.

 [comment]: <> (Unsure! What does RESET button do?)


#### Financial accounting takeover

 *Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Supplier receipts > Tab Financial accounting takeover*


  ![Financial accounting takeover](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsTakeover.png "[Financial accounting takeover]")

The *Financial account takeover* tab displays all receipts with **Released** status. An extra column displaying checkboxes is added.

- [x] (Checkbox)  
Click the checkbox in the column header to select all receipts listed. Click the checkbox in one or more individual receipts to take over only the selected ones.

When selecting a receipt, changes can still be made before takeover. For detailed information about booking supplier receipts, see [Book a supplier receipt](/RetailSuiteAccounting/Operation/10_ManageREceipts.md#book-a-supplier-receipt).

- [SPEICHERN]  
Click this button to save any changes made to receipt data.

- [SPLIT]  
Click this button to perform a split booking, if necessary.

[comment]: <> (New window. Describe? RS HG!)

- [TAKE OVER SELECTED ONES]  
Click this button to register the selected receipts in the system.



## EVALUATIONS

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS*

This menu allows to create and print out different sorts of evaluation reports for analysis or overview purposes. Click the *EVALUATIONS* button to display the context menu.

![Evaluations](/Assets/Screenshots/RetailSuiteAccounting/Book/Evaluations.png "[Evaluations]")

  - *Account balance*  
  Click this menu entry to display the *Account balance* window, see [Account balance](#account-balance).

  - *Account sheet*  
  Click this menu entry to display the *Account sheet* window, see [Account sheet](#account-sheet).

  - *Journal*  
  Click this menu entry to display the *Journal* window, see [Journal](#journal).

  - *Balance list*  
  Click this menu entry to display the *Balance list* window, see [Balance list](#balance-list).

  - *Open items*  
  Click this menu entry to display the *Open items* window, see [Open items](#open-items).

  - *BWA*  
  Click this menu entry to display the *BWA* window, see [BWA](#bwa).

  - *ProfitCenter*  
  Click this menu entry to display the *ProfitCenter* window, see [ProfitCenter](#profitcenter).

  - *Cost unit comparison*  
  Click this menu entry to display the *Cost unit comparison* window, see [Cost unit comparison](#cost-unit-comparison).

  - *Other*  
  Click this menu entry to display the *Chart of accounts* und *Deb./Cred.* sub-menu, see [Other](#other).


### Account balance

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Account balance*

  ![Account balance](/Assets/Screenshots/RetailSuiteAccounting/Book/AccountBalance.png "[Account balance]")

- *Account*  
Enter the account number to be displayed.

- *Date*  
Enter the period to be included. The currently selected fiscal year is displayed by default.

- *Sorting*  
Click the drop-down list to select the sorting mode. The following options are available:

  - **Date**
  - **Amount**  

  If sorting by date is selected, the *Debit-credit interest rate* fields are displayed.  

- *Debit-credit interest rate*  
Enter the corresponding values in both fields.

- *Sorting*  
Click the drop-down list to select the sorting mode. The following options are available:
 - **normal**
 - **by cost centers**

[comment]: <> (Other options possible?)

- [CLOSE]  
Click this button to close the window.

- [PRINT]  
Click this button to create the evaluation report in a printable format.

[comment]: <> (New window opens with evaluation. Describe?)

### Account sheet

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Account sheet*

  ![Account sheet](/Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet.png "[Account sheet]")

- *Newly booked accounts* [x]  
Select the checkbox to include only the newly added bookings.

- *Kennzeichen zurücksetzen* [x]  
Select the checkbox to...

[comments]: <> (Setzen Sie einen Haken in das Kästchen, wenn nur die neu hinzugefügten Buchungen in dem Kontenblatt ausgegeben werden soll. Damit diese Funktion greift, muss zusätzlich das Feld Kennzeichen zurücksetzen angewählt werden. Stimmt das so? Was macht diese Funktion/Checkbox? Was ist mit "Kennzeichen" gemeint?)

- *Month*  
Enter the period to be included.

- *Date*  
You can narrow down the period to be included specifying the dates. Date format must be DDMMYY.

- *Accounts*  
Enter the account number range to be displayed.

- *Sorting*  
Click the drop-down list to select the sorting mode. The following options are available:
 - **normal**
 - **by cost centers**

[comment]: <> (Other options possible?)

[comment]: <> (Altdoku: Das Kontenblatt lässt sich nach Kostenstellen und Kostenträgern sortieren und auswerten. Bei einer Auswahl in diesem Feld werden nur Buchungen ausgegeben, die den ausgewählten Kostenträger oder Kostenstelle betreffen. Stimmt so? Was debeutet hier "normal"?)

- [CANCEL]  
Click this button to cancel your selection.

- [PRINT]  
Click this button to create the evaluation report in a printable format.


### Journal

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Journal*

  ![Journal](/Assets/Screenshots/RetailSuiteAccounting/Book/Journal.png "[Journal]")

- *Month*  
Enter the month(s) to be included.

- *Journals*  
Enter the journal(s) to be included.

- *Sorting*  
Click the drop-down list to select the sorting mode.  The following options are available:
 - **normal**
 - **by cost centers**

[comment]: <> (Other options possible?)

[comment]: <> (Altdoku: Das Journal lässt sich nach Kostenstellen und Kostenträgern sortieren und auswerten. Bei einer Auswahl in diesem Feld werden nur Buchungen ausgegeben, die den ausgewählten Kostenträger oder Kostenstelle betreffen. Stimmt es so? Was bedeutet hier "normal"?)

- [CANCEL]  
Click this button to cancel your selection.

- [PRINT]  
Click this button to create the evaluation report in a printable format.


### Balance list

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Balance list*

  ![Balance list](/Assets/Screenshots/RetailSuiteAccounting/Book/BalanceList.png "[Balance list]")

- *Month*  
Click the drop-down list to select the month to be included. The following options are available:  

  - **0 - Balances carried forward**
  - **1 - 12 - (months)**
  - **13 - 15 - Subsequent bookings**
  - **16 - 25 - Closing bookings**
  - **99 - General month**


- *Accounts*  
Click the drop-down list to select the accounts to be displayed. The following options are available:  

 - **Impersonal accounts**  
 Select this option to include impersonal accounts only.
 - **Customers (10000 - 69999)**  
 Select this option to include customers accounts only.
 - **Suppliers (70000 - 99999)**  
 Select this option to include suppliers accounts only.
 - **Individual**  
 Select this option to enter a self-defined account number range. When selecting this option, two new fields (*Accounts from* - *Accounts to*) are displayed. Enter the applicable account number range in these fields.

   ![Balance list](/Assets/Screenshots/RetailSuiteAccounting/Book/BalanceList02.png "[Balance list]")


- *Layout*  
Click the drop-down list to select the preferred layout. There are two options available:  

 - **normal**
 - **balance list**

 [comment]: <> (Difference? to be completed!)

- *Sorting*  
Click the drop-down list to select the sorting mode.  The following options are available:
 - **normal**
 - **by cost centers**

[comment]: <> (Other options possible?)

[comment]: <> (Altdoku: Das Journal lässt sich nach Kostenstellen und Kostenträgern sortieren und auswerten. Bei einer Auswahl in diesem Feld werden nur Buchungen ausgegeben, die den ausgewählten Kostenträger oder Kostenstelle betreffen. Stimmt es so? Was bedeutet hier "normal"?)

- [CANCEL]  
  Click this button to cancel your selection.

- [PRINT]  
  Click this button to create the evaluation report in a printable format.

### Open items

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Open items*

  ![Open items](/Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems.png "[Open items]")

  - *Accounts*  
  Click the drop-down list to select the accounts to be displayed. The following options are available:  

    - **Customers (10000 - 69999)**  
    Select this option to include customers accounts only.
    - **Suppliers (70000 - 99999)**  
    Select this option to include suppliers accounts only.
    - **Individual**  
    Select this option to enter a self-defined account number range. When selecting this option, two new fields (*Accounts*) are displayed. Enter the applicable account number range in these fields.

      ![Open items](/Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems02.png "[Open items]")

  - *Month up to*  
  Click the drop-down list to select the month(s) to be included. The following options are available:
    - **0 - Balances carried forward**
    - **1 - 12 - (months)**
    - **13 - 15 - Subsequent bookings**
    - **16 - 25 - Closing bookings**
    - **99 - General month**

    > [Info] The field name *Month up to* implies that actually a month range is selected. This means that all months between month 0 and the selected drop-down list option are displayed.

  - *Format*  
  Click the drop-down list to select the preferred format. The following options are available:
    - **Short format**  
    - **Short format, reduce bookings**  
    - **Detailed**


  - [x] *Print manually cleared open items*   
  Select the checkbox to include all manually cleared open items.

  - [CANCEL]  
  Click this button to cancel your selection.

  - [PRINT]  
  Click this button to create the evaluation report in a printable format.


### BWA

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry BWA*

  ![BWA](/Assets/Screenshots/RetailSuiteAccounting/Book/BWA.png "[BWA]")

  - *Sorting*  
Click the drop-down list to select the sorting mode. The following options are available:
 - **normal**
 - **by cost centers**

[comment]: <> (Other options possible?)

- [x] *Print cost center allocation*  
Select the checkbox to display the cost center allocation.

- *Month from - to*  
Click the drop-down list to select the month range to be included. The following options are available:

  - **0 - Balances carried forward**
  - **1 - 12 - (months)**
  - **13 - 15 - Subsequent bookings**
  - **16 - 25 - Closing bookings**
  - **99 - General month**   


- *Comparison year* - *Comparison year 2*  
Click the drop-down list to select two different years to be compared with each other. If no year for comparison exists, the option **no year for comparison** is displayed.

- *BWA number*  
Click the drop-down list to select the BWA report type to be created. The following options are available per default:

  - **1: Profit and loss account**
  - **2: Cash basis accounting**
  - **3: Liquidity statement**
  - **4: Liquidity**
  - **5: Monthly balance**

  > [Info] These evaluation reports are preconfigured in the system. All available reports can be completely customized or used as provided, and new reports can also be created. Any newly created reports will be displayed in the drop-down list. For detailed information about creating and managing BWA reports, see [Manage BWA reports](/RetailSuiteAccounting/Operation/07_ManageBWAReports.md).

- *Layout*  
Click the drop-down list to select the preferred layout. The following options are available:

  - **Month - cum. - cum. previous year**
  - **13 months cumulative**
  - **Previous year comparison**
  - **13 months with comparison**


- *Show account*  
Click the drop-down list to select whether or not the account number is to be included.

- [CANCEL]  
Click this button to cancel your selection.

- [PRINT]  
Click this button to create the evaluation report in a printable format.


For detailed information about creating a BWA evaluation, see [Create a PDF evaluation](/RetailSuiteAccounting/Operation/15_ProvideAccountingData.md#create-a-pdf-evaluation).


### ProfitCenter

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry ProfitCenter*

  ![ProfitCenter](/Assets/Screenshots/RetailSuiteAccounting/Book/ProfitCenter.png "[ProfitCenter]")

- *Month*  
Click the drop-down list to select the month to be included. The following options are available:  

  - **0 - Balances carried forward**
  - **1 - 12 - (months)**
  - **13 - 15 - Subsequent bookings**
  - **16 - 25 - Closing bookings**
  - **99 - General month**  


- *Comparison year*  
Click the drop-down list to select a comparison year. If no comparison year is needed, select the option **no comp. year**.

- *Cost unit group*  
Click the drop-down list to select a cost unit group. If no cost unit group is needed, select the option *0 - no group*.  

  > [Info] For detailed information about creating and managing cost units, see [COST ACCOUNTING](XX_CostAccounting.md).

[comment]: <> (Check how it works!?)

- *BWA number*  
Click the drop-down list to select the BWA report type to be created. The following options are available:

    - **1: Profit and loss account**
    - **2: Cash basis accounting**
    - **3: Liquidity statement**
    - **4: Liquidity**
    - **5: Monthly balance**

  > [Info] These evaluation reports are preconfigured in the system. All available reports can be completely customized or used as provided, and new reports can also be created. Any newly created reports will be displayed in the drop-down list. For detailed information about creating and managing BWA reports, see [Manage BWA reports](/RetailSuiteAccounting/Operation/07_ManageBWAReports.md).

- *Layout*  
Click the drop-down list to select the preferred layout. The following options are available:  

  - **Month - Month previous year**
  - **Month - cum. - cum. previous year**
  - **13 months**
  - **Front page**


- [CANCEL]  
  Click this button to cancel your selection.

- [PRINT]  
  Click this button to create the evaluation report in a printable format.


### Cost unit comparison

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Cost unit comparison*

  ![Cost unit comparison](/Assets/Screenshots/RetailSuiteAccounting/Book/CostUnitComparison.png "[Cost unit comparison]")

- *Month*  
Click the drop-down list to select the month to be included. The following options are available:  

  - **0 - Balances carried forward**
  - **1 - 12 - (months)**
  - **13 - 15 - Subsequent bookings**
  - **16 - 25 - Closing bookings**
  - **99 - General month**  


- *Cost unit group*  
Click the drop-down list to select a cost unit group. There are two default options available:

  - **ALL GROUPS**
  - **0 - no group**

  [comment]: <> (When cost unit group(s) created, do they appear in the drop-down list, as it is the case for Kostenstellen/cost centers? Where are cost units created?)

  > [Info] For detailed information about creating and managing cost units, see [COST ACCOUNTING](XX_CostAccounting.md).

[comment]: <> (Check how it works!?)

- *BWA number*  
Click the drop-down list to select the BWA report type to be created. The following options are available:

    - **1: Profit and loss account**
    - **2: Cash basis accounting**
    - **3: Liquidity statement**
    - **4: Liquidity**
    - **5: Monthly balance**

  > [Info] These evaluation reports are preconfigured in the system. All available reports can be completely customized or used as provided, and new reports can also be created. Any newly created reports will be displayed in the drop-down list. For detailed information about creating and managing BWA reports, see [Manage BWA reports](/RetailSuiteAccounting/Operation/07_ManageBWAReports.md).

- [CANCEL]  
  Click this button to cancel your selection.

- [PRINT]  
  Click this button to create the evaluation report in a printable format.


### Other
*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Other*

When clicking the *Other* menu entry of the EVALUATIONS context menu, a sub-menu is displayed containing two additional entries: *Chart of accounts* and *Deb./Cred.*.

#### Chart of accounts

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Account sheet > Sub-menu entry Chart of accounts*

  ![Chart of accounts](/Assets/Screenshots/RetailSuiteAccounting/Book/ChartOfAccounts.png "[Chart of accounts]")

- *Accounts*  
Enter the account number range to be displayed.

- *Sorting*  
Click the drop-down list to select the sorting mode. The following options are available:

  - **by number**
  - **by name**


- *[x] ONLY booked*  
Select this checkbox to display only booked accounts.

- [CANCEL]  
  Click this button to cancel your selection.

- [PRINT]  
  Click this button to create the evaluation report in a printable format.

#### Deb./cred.

*Accounting > Select fiscal year > Book > Context menu EVALUATIONS > Menu entry Account sheet > Sub-menu entry Deb./cred.*

  ![Debtors/Creditors](/Assets/Screenshots/RetailSuiteAccounting/Book/DebtorsCreditors.png "[Debtors/Creditors]")

- *Accounts*  
Enter the account number range to be displayed.

- [CANCEL]  
  Click this button to cancel your selection.

- [PRINT]  
  Click this button to create the evaluation report in a printable format.
