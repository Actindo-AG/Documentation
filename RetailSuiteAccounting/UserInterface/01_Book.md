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

  [comment]: <> (Look for info)

  - *Bank details takeover*  
  Click this menu option to display the *Bank details synchronizing* window, see [Bank details takeover](#bank-details-takeover).

  [comment]: <> (Look for info)

  - ![Lock](/Assets/Icons/Lock02.png "[Lock]") *Process*  
  Click this menu option to process one of several bookings in a booking period. The *Process bookings* window is displayed, see [Process](#process).

  - ![Do not enter](/Assets/Icons/DoNotEnter.png "[Do not enter]") *Delete*  
  Click this menu option to delete one or several bookings at a time. The *Delete bookings* window is displayed, see [Delete](#delete).

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

This window displays all cash payments registered in the cash book, which can be taken over automatically in the *Accounting* module. For detailed information, see [Cash book](#to-be-completed). All information provided in columns is read-only, except for the *T* column.

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


  - [SELECT ALL] button   
    Click this button to select all bookings.

  - [SELECT NOTHING] button  
    Click this button to deselect all bookings.

  - *Amount*  
    Total amount of all bookings in the cash book


An individual booking from the cash book can be selected and edited before takeover. Click the booking to be edited. Its details are displayed in the entry line.

[comment]: <> (Add procedure file?)

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

  - [BOOK] button  
  Click this button to book the edited booking.

  - [DELETE] button  
  Click this button to delete the selected booking.

  [comment]: <> (FEHLER: löschen hier nicht mehr möglich! -> even though takeover not yet performed? Probably because it is linked to cash book/Kassenbuch? What is the use of this button here? RS FH)

  - [CLEAR] button  
  Click this button to clear all entry line fields.

  - [SPLIT] button  
  Click this button to split the selected booking.

  [comment]: <> (Fehlermeldungen: beim klicking auf SPLIT -> Unbekannte Bankbuchung. Wenn man versucht, eine Splitbuchung zu machen -> Meldung: Gebucht und in rot "Umsatz, GegKonto, Datum oder Konto leer! Ungültiges Datum!" Alle Felder waren aber richtig ausgefüllt, jetzt erscheining sie aber alle auf 0, außer GegKonto und Text)

  - [SAVE] button  
  Click this button to take over the selected bookings.


### Bank details takeover  

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Bank details takeover*

  ![Bank details synchronizing](/Assets/Screenshots/RetailSuiteAccounting/Book/BankDetailsSynchronizing.png "[Bank details synchronizing]")

This screen is also contained in the *Payment processing* module.

### ![Lock](/Assets/Icons/Lock02.png "[Lock]") Process

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Process*

  ![Process bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/ProcessBookings01.png "[Process bookings]")

For detailed information about processing bookings, see [Process Bookings](/RetailSuiteAccounting/Operation/07_ProcessBookings.md).

### ![Do not enter](/Assets/Icons/DoNotEnter.png "[Do not enter]") Delete

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Delete*

  ![Delete bookings](/Assets/Screenshots/RetailSuiteAccounting/Book/DeleteBookings.png "[Delete bookings]")

### ![Lock](/Assets/Icons/Lock02.png "[Lock]") Lock months

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Lock months*

  ![Lock months](/Assets/Screenshots/RetailSuiteAccounting/Book/LockMonths.png "[Lock months]")

### Balance carried forward

*Accounting > Select fiscal year > Book > Context menu EDIT > Menu entry Balance carried forward*

  ![Balance carried forward: step 1](/Assets/Screenshots/RetailSuiteAccounting/Book/BalanceCarriedForward01.png "[Balance carried forward: step 1]")

  ![Retrieve account balances](/Assets/Screenshots/RetailSuiteAccounting/Book/RetrieveAccountBalances.png "[Retrieve account balances]")

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
