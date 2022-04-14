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

Click this button to display the select fiscal year window. For detailed information, see [Fiscal year](00a_FiscalYear.md) and [Select a fiscal year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md).


## EDIT

*Accounting > Select fiscal year > Book > Context menu EDIT*

Click this button to display the *EDIT* context menu.

  ![EDIT](/Assets/Screenshots/RetailSuiteAccounting/Book/Edit.png "[EDIT]")

  - *Cash book takeover*  
  Click this menu option to display the *Cash book takeover* window, see [Cash book takeover](#cash-book-takeover).

  [comment]: <> (RS FH about function and need of procedure. How is it used by customers?)

  - *Bank data takeover*  
  Click this menu option to display the *Bank data synchronizing* window, see [Bank data takeover](#bank-data-takeover).

  [comment]: <> (RS FH about function and need of procedure. How is it used by customers?)

  - ![Lock](/Assets/Icons/Lock02.png "[Lock]") *Process*  
  Click this menu option to process one of several bookings in a booking period. The *Process bookings* window is displayed, see [Process](#process).

  - ![Do not enter](/Assets/Icons/DoNotEnter.png "[Do not enter]") *Delete*  
  Click this menu option to delete one or several bookings simultaneously. The *Delete bookings* window is displayed, see [Delete](#delete).

  - ![Lock](/Assets/Icons/Lock02.png "[Lock]") *Lock months*  
  Click this menu option to lock one or several months for bookings. The *Lock months* window is displayed, see [Lock months](#Lock months).

  - *Balance carried forward*  
  Click this menu option to carry forward balances from the previous fiscal year. The *Balance carried forward: step 1* window is displayed, see [Balance carried forward](#balance-carried-forward).

  - *Foreign currency wizard*  
  Click this menu option to carry forward balances from the previous fiscal year. The *Foreign currency wizard* window is displayed, see [Foreign currency wizard](#foreign-currency-wizard).

  - *Supplier receipts*  
  Click this menu option to carry forward balances from the previous fiscal year. The *Supplier receipts* window is displayed, see [Supplier receipts](#supplier-receipts).

### Cash book takeover  

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Cash book takeover*

  ![Cash book takeover](/Assets/Screenshots/RetailSuiteAccounting/Book/CashBookTakeover.png "[Cash book takeover]")

This window displays all cash payments registered in the cash book, which can be taken over automatically in the *Accounting* module. All information provided in columns is read-only, except for the *T* column.

[comment]: <> (Add link when docu available: For detailed information, see ...)

  - *Seq. no.*  
    Sequential number as registered in the cash book

  - [X]
   *T (Take over booking)*  
   Select this checkbox to take over an individual booking.

  - *BP*  
    Booking period as registered in the cash book

  - *Jnl*  
    Journal as registered in the cash book

  - *Turnover*  
    Turnover value as registered in the cash book. Revenues display a positive sign. Expenditures display a negative sign.

  - *Contra Account*  
    Contra Account as registered in the cash booking

  [comment]: <> (No account in cash book! What does the number stand for? As "Unbekannt!")   

  - *Receipt1*  
    Receipt 1 as registered in the cash book

  - *Receipt2*  
    Receipt 2 as registered in the cash book

  - *Date*  
    Date as registered in the cash book

  - *Account*  
    Account as registered in the cash book

  - *Cst1*  
    Cost 1 as registered in the cash book

  - *Cst2*  
    Cost 2 as registered in the cash book

  - *Text*  
    Free text as registered in the cash book


  - [SELECT ALL]     
    Click this button to select all bookings.

  - [SELECT NOTHING]    
    Click this button to deselect all bookings.

  - *Amount*  
    Total amount of all bookings in the cash book


An individual booking from the cash book can be selected and edited before takeover. Click the booking to be edited. Its details are displayed in the entry line.

[comment]: <> (Unsure! RS FH. Add procedure file? RS HG/FH!)

  - *Seq. no.*  
   This field displays the book sequential number and cannot be modified.  

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

  [comment]: <> (FEHLER: löschen hier nicht mehr möglich! -> even though takeover not yet performed? Probably because it is linked to cash book/Kassenbuch? What is the use of this button here? RS FH)

  - [CLEAR]    
  Click this button to clear all entry line fields.

  - [SPLIT]    
  Click this button to split the selected booking.

  [comment]: <> (Fehlermeldungen: beim klicking auf SPLIT -> Unbekannte Bankbuchung. Wenn man versucht, eine Splitbuchung zu machen -> Meldung: Gebucht und in rot "Umsatz, GegKonto, Datum oder Konto leer! Ungültiges Datum!" Alle Felder waren aber richtig ausgefüllt, jetzt erscheining sie aber alle auf 0, außer GegKonto und Text)

  - [SAVE]    
  Click this button to take over the selected bookings.


### Bank data takeover  

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Bank data takeover*

  ![Bank data synchronizing](/Assets/Screenshots/RetailSuiteAccounting/Book/BankDataSynchronizing.png "[Bank data synchronizing]")

This screen is also available in the *Payment processing* module. Both modules are closely linked with each other.

[comment]: <> (Link when available?)

 - *Bank account*  
 Click the drop-down list to select the bank account which data must be imported.

 - *Load registered ones* [x]  
 Click this checkbox to activate the [SHOW REGISTERED] button.

  > [Info] This function is per default deactivated to reduce system overload and improve performance. This default setting can be changed in *Settings* menu entry of the *Payment processing* module.

  [comment]: <> (Add link when available?)

 - *FY/month*  
 Click the corresponding drop-down list to select the fiscal year and month of the data to be displayed.

 - [RETRIEVE/IMPORT]  
 Click this button to display the *Retrieve bank data* window, see [Retrieve bank data](#retrieve-bank-data).

 - [SHOW REGISTERED]  
 Click this button to display all booked payments.

 - [SHOW HIDDEN]  
 Click this button to display all hidden payments.

 - [QUICK SEARCH]  
 Click this menu to display the context menu. Payments can be searched for using the following search criteria:

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

 - *Seq. no*  
 This column displays the sequential number.

 - *T* (Take over)  
 Click the checkbox in this column to select the payment.

 - *B* (xxx)  
 This column displays the open item status.
  - Green  
  An incoming payment has been matched with an existing open item.
  - Yellow  
  An incoming payment probably matches and existing open item but there are discrepancies to be checked.
  - Red  
  No matching open item found for the payment.

   > [Info] If a payment is processed manually, an *M* will be displayed in this column.

[comment]: <> (B für Beleg, Bearbeiten, Buchhaltung???Change column name accordingly here and in IU Terminology file! Add screenshot/icons)  

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
 This column shows the payment date.

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
 Click this button to upload the payment list.

- [RESET]  
 Click this button to reset the list.

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


### ![Lock](/Assets/Icons/Lock02.png "[Lock]") Process

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Process*

  ![Process bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/ProcessBookings01.png "[Process bookings]")

This window allows to select one or several bookings to be processed simultaneously.

- *Journal from - to*  
Click these drop-down lists to select the journals to be processed. The drop-down lists display the existing journals including the bookings (or postings) recorded in each of them.

- *Month from - to*   
Click these drop-down lists to select the months to be processed. The drop-down lists display all available months in the system.

- [CANCEL]  
Click this button to cancel your selection.

- [OK]  
Click this button to confirm your selection.

For detailed information about processing bookings, see [Process bookings](/RetailSuiteAccounting/Operation/07_ProcessBookings.md).



### ![Do not enter](/Assets/Icons/DoNotEnter.png "[Do not enter]") Delete

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


### ![Lock](/Assets/Icons/Lock02.png "[Lock]") Lock months

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

This window allows to select outstanding balances to be carried forward to the next fiscal year.

- *Carry forward from FY*  
Click the drop-down list to select the year containing the balances to be carried forward.

- *Range from - to*  
Click the drop-down list to select the...

 - **01: Financial accounts**
 - **02: Impersonal accounts**
 - **03: input tax + VAT**
 - **04: P&L**
 - **05: Open items debtors**
 - **06: Open items creditors**


- *Booking date*
Enter the booking date for the balance carried forward.

> [Info] By default, the system displays the first day of the new fiscal year. This can be modified simply by typing in the desired booking date.

- *Delete old balances carried forward from selected FY* [x]  
Select this checkbox to delete the old balances carried forward from the selected fiscal year.


- [CANCEL]

- [CONTINUE]



  ![Retrieve account balances](/Assets/Screenshots/RetailSuiteAccounting/Book/RetrieveAccountBalances.png "[Retrieve account balances]")

- *Carry forward from FY*

- *Range from - to*

- *Date*

- *Accounts*
 - Ctrl + mouse to select


- *Delete old balances carried forward from selected FY*

 - **Yes**
 - **No**


- [BACK]

- [CANCEL]

- [CONTINUE]

For detailed information about processing bookings, see [Create a balance carried forward](/RetailSuiteAccounting/Operation/11_CreateBalanceCarriedForward.md).

### Foreign currency wizard

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Foreign currency wizard*

  ![Foreign currency wizard 1](/Assets/Screenshots/RetailSuiteAccounting/Book/ForeignCurrencyWizardWindow01.png "[Foreign currency wizard 1]")

  ![Foreign currency wizard 2](/Assets/Screenshots/RetailSuiteAccounting/Book/ForeignCurrencyWizardWindow02.png "[Foreign currency wizard 2]")

  ![Foreign currency wizard 3](/Assets/Screenshots/RetailSuiteAccounting/Book/ForeignCurrencyWizardWindow03.png "[Foreign currency wizard 3]")

### Supplier receipts

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Supplier receipts*

  ![Acquire supplier receipts](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsAcquire.png "[Acquire supplier receipts]")

  ![Overview](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsOverview.png "[Overview]")

  ![Financial accounting takeover](/Assets/Screenshots/RetailSuiteAccounting/Book/SupplierReceiptsTakeover.png "[Financial accounting takeover]")


## ASSESSMENTS

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS*

Click this button to display the *ASSESSMENTS* context menu.

![Assessments](/Assets/Screenshots/RetailSuiteAccounting/Book/Assessments.png "[Assessments]")

  - *Account balance*  
  Click this menu option to display the *Account balance* window, see [Account balance](#account-balance).

  - *Account sheet*  
  Click this menu option to display the *Account sheet* window, see [Account sheet](#account-sheet).

  - *Journal*  
  Click this menu option to display the *Journal* window, see [Journal](#journal).

  - *Balance list*  
  Click this menu option to display the *Balance list* window, see [Balance list](#balance-list).

  - *Open items*  
  Click this menu option to display the *Open items* window, see [Open items](#open-items).

  - *BWA*  
  Click this menu option to display the *BWA* window, see [BWA](#bwa).

  - *ProfitCenter*  
  Click this menu option to display the *ProfitCenter* window, see [ProfitCenter](#profitcenter).

  - *Cost unit comparison*  
  Click this menu option to display the *Cost unit comparison* window, see [Cost unit comparison](#cost-unit-comparison).

  - *Other*  
  Click this menu option to display the *Chart of accounts* und *Deb./Cred.* sub-menu, see [Other](#other).


### Account balance

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Account balance*

  ![Account balance](/Assets/Screenshots/RetailSuiteAccounting/Book/AccountBalance.png "[Account balance]")


### Account sheet

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Account sheet*

  ![Account sheet](/Assets/Screenshots/RetailSuiteAccounting/Book/AccountSheet.png "[Account sheet]")


### Journal

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Journal*

  ![Journal](/Assets/Screenshots/RetailSuiteAccounting/Book/Journal.png "[Journal]")


### Balance list

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Balance list*

  ![Balance list](/Assets/Screenshots/RetailSuiteAccounting/Book/BalanceList.png "[Balance list]")

### Open items

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Open items*

  ![Open items](/Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems.png "[Open items]")


### BWA

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry BWA*

  ![BWA](/Assets/Screenshots/RetailSuiteAccounting/Book/BWA.png "[BWA]")


### ProfitCenter

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry ProfitCenter*

  ![ProfitCenter](/Assets/Screenshots/RetailSuiteAccounting/Book/ProfitCenter.png "[ProfitCenter]")


### Cost unit comparison

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Cost unit comparison*

  ![Cost unit comparison](/Assets/Screenshots/RetailSuiteAccounting/Book/CostUnitComparison.png "[Cost unit comparison]")

### Other
*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Other*

#### Chart of accounts

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Account sheet > Sub-menu entry Chart of accounts*

  ![Chart of accounts](/Assets/Screenshots/RetailSuiteAccounting/Book/ChartOfAccounts.png "[Chart of accounts]")

#### Deb./cred.

*Accounting > Select fiscal year > Book > Context menu ASSESSMENTS > Menu entry Account sheet > Sub-menu entry Deb./cred.*

  ![Debtors/Creditors](/Assets/Screenshots/RetailSuiteAccounting/Book/DebtorsCreditors.png "[Debtors/Creditors]")
