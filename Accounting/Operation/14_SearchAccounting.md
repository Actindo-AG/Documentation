[!!Accounting](Actindo/Accounting)

# Search in accounting

An account is an essential part of an accounting system used to track and summarize in chronological order all financial transactions (credits and debits) of the different business elements, such as assets, liabilities, income and expenses.

A booking is every entry recorded as credit or debit in the corresponding accounts.

The *Search* tab in the *Accounting* module allows to search for a specific account or booking using different search criteria. This is useful to locate specific data for correction or checking purposes.

[comment]: <> (Explain briefly what the search is used for and at what time.)


## Search for an account

An account can be searched for by account number or by description.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

### Procedure

*Accounting > Select fiscal year > Book > Tab SEARCH > Side bar Book extras > Tab Accounts*

![Search](/Assets/Screenshots/Accounting/Book/Search/Search01.png "[Search]")

> [Info] The *Book extras* side bar opens automatically when clicking the *SEARCH* tab. If it has been closed, it can be reopened by clicking the leftward arrow on the right-hand side of the workspace. Analogously, click the rightward arrow to close it again.

1. Click the *QUICK SEARCH* button.  
The *QUICK SEARCH* context menu is displayed.

  ![Search for an account](/Assets/Screenshots/Accounting/Book/Search/BookExtrasAccounts.png "[Search for an account]")

2. Unselect the *Acc. no.* or *Description* checkbox if you want your search text to apply only to the account number or to the description field.

  > [Info] Per default both options are selected through a marked checkbox in the *QUICK SEARCH* context menu. If both options are selected, the search results will display all accounts containing the search text in any of both fields.

3. Enter the search text (account number or description) in the search bar and press Enter or click the ![Search](/Assets/Icons/Search.png "[Search]") icon.  

  > [Info] The *QUICK SEARCH* function works like a filter. That means that you can enter any search text, also a partial account number or description, and the search results will display all accounts containing exactly the search text entered in the search bar.

4. It is also possible to scroll through the accounts by clicking the simple and double arrows in the lower part of the *Book extras* side bar. You can also jump directly to any page by entering a page number and pressing Enter in the *Page* field.

4. Click the ![Cross](/Assets/Icons/Cross02.png "[Cross]") icon to clear the search.  
The whole chart of accounts is displayed again.


### Next steps

  - [Search for a booking](#search-for-a-booking)
  - [Provide the accounting data](15_ProvideAccountingData.md)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year)
  - [Select fiscal year](01_SelectFiscalYear.md)


## Search for a booking

A booking can be searched for using different search criteria, such as turnover, account, journal, and the applicable search values.

### Prerequisites

  - The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
  - A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

### Procedure

*Accounting > Select fiscal year > Book > Tab SEARCH > Side bar Book extras > Tab Search*

  ![Search](/Assets/Screenshots/Accounting/Book/Search/Search02.png "[Search]")

  > [Info] The *Book extras* side bar opens automatically when clicking the *SEARCH* tab. If it has been closed, it can be reopened by clicking the leftward arrow on the right-hand side of the workspace. Analogously, click the rightward arrow to close it again.

  1. Select the applicable search criteria by marking the corresponding *Active* checkbox.      

    ![Search for a booking](/Assets/Screenshots/Accounting/Book/Search/BookExtrasSearch.png "[Search for a booking]")

  2. Enter the search value in the *Search for* field.

  > [Info] There are two types of wildcards available:
    - An asterisk (*) represents any number of characters.
    - A question mark (?) represents a single character.

  3. Mark the *NOT* checkbox to exclude any entered value from the search, if necessary.

  4. Click the [SEARCH] button.  
  The bookings matching your search criteria are displayed.


### Next steps

  - [Provide the accounting data](15_ProvideAccountingData.md)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year)
  - [Select fiscal year](01_SelectFiscalYear.md)
