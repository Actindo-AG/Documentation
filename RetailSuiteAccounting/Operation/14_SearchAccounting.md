[!!User Interface search](../UserInterface/01e_Search.md)  
[!!User Interface accounts](../UserInterface/02b_Accounts.md)  
[!!User Interface bookings](../UserInterface/01a_Bookings.md)  
[!!Manage accounts](../Integration/03_ManageAccounts.md)  


# Search in accounting

An account is an essential part of an accounting system used to track and summarize in chronological order all financial transactions (credits and debits) of the different business elements, such as assets, liabilities, income and expenses.

A booking is every entry recorded as credit or debit in the corresponding accounts.

The *SEARCH* tab in the *Accounting* module allows to search for a specific account or booking using different search criteria. This is useful to locate specific data for correction or checking purposes.


## Search for an account

An account can be searched for by account number or by description.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Post > Tab SEARCH > Tab Accounts*
*Accounting > Select fiscal year > Post > Side bar button Leftward arrow > Tab Accounts*

![Search](../../Assets/Screenshots/RetailSuiteAccounting/Book/Search/Search01.png "[Search]")

> [Info] The *Book extras* side bar can be displayed at any time and in any tab of the *Post* menu entry by clicking the ![Left arrow](../../Assets/Icons/Back02.png "[Left arrow]") (Left arrow) button or hidden by clicking the ![Right arrow](../../Assets/Icons/Close.png "[Right arrow]") (Right arrow) button.

1. Click the *QUICK SEARCH* button.  
A filter list with the *Acc. no.* and *Description* entries is displayed.

  ![Search for an account](../../Assets/Screenshots/RetailSuiteAccounting/Book/Search/BookExtrasAccounts.png "[Search for an account]")

2. Deselect the *Acc. no.* or *Description* checkbox if you want your search text to apply only to the account number or to the description field.

  > [Info] Per default both options are selected through a marked checkbox in the *QUICK SEARCH* context menu. If both options are selected, the search results will display all accounts containing the search text in any of both fields.

3. Enter the search text (account number or description) in the search bar and press the **Enter** key or click the ![Search](../../Assets/Icons/Search.png "[Search]") (Search) button. You can enter any search text, even a partial account number or description.     
  All accounts containing the search text entered in the search bar are displayed in the search results.

4. Click the ![Cross](../../Assets/Icons/Cross02.png "[Cross]") icon to clear the search bar and start a new search.  


## Search for a booking

A posting can be searched for using different search criteria, such as turnover, account, journal, and the corresponding search values.

#### Prerequisites

  - The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
  - A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab SEARCH > Side bar Book extras > Tab Search*

  ![Search](../../Assets/Screenshots/RetailSuiteAccounting/Book/Search/Search02.png "[Search]")

  > [Info] The *Book extras* side bar opens automatically when clicking the *SEARCH* tab. If it has been closed, it can be reopened by clicking the leftward arrow on the right-hand side of the workspace. Similarly, it can be closed again by clicking the rightward arrow.

  1. Select the applicable search criteria by marking the corresponding *Active* checkbox.      

  ![Search for a booking](../../Assets/Screenshots/RetailSuiteAccounting/Book/Search/BookExtrasSearch.png "[Search for a booking]")

  2. Enter the search value in the *Search for* field.

  > [Info] There are two types of wildcards available:
    - An asterisk (*) represents any number of characters.
    - A question mark (?) represents a single character.

  3. Mark the *NOT* checkbox to exclude any entered value from the search, if necessary.

  4. Click the [SEARCH] button.  
  The bookings matching your search criteria are displayed.
