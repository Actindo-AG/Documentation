[!!User Interface Select fiscal year](../UserInterface/00a_FiscalYear.md)  
[!!User Interface Settings fiscal years](../UserInterface/02d_FiscalYears.md)  
[!!Select fiscal year](../Operation/01_SelectFiscalYear.md)  
[!!User Interface FY/MONTH/JOURNAL](../UserInterface/00_Book.md#fymonthjournal)   
[!!Manage the fiscal year](../Integration/04_ManageFiscalYear.md)  



# Access postings from another period

A fiscal year is the period over which a company's accounts are calculated, which generally lasts 12 months and which may or may not coincide with the calendar year.

Journal and months are used to arrange a company's business transactions within a fiscal year. A particular posting period will only contain the postings recorded in that specific period. Accessing postings from other periods may be necessary, for example, if a posting from a previous posting period needs to be adjusted or if a transaction performed at a later stage must be manually booked in a specific period.

A journal is a chronological record of all accounting transactions within a specified period of time. There are two main types of journals preconfigured in the system:

  - General journals (1-12) are matched with the fiscal year months, regardless of whether the fiscal year coincides with the calendar year or not. That means, the first fiscal year month corresponds to journal 1, the second to journal 2 and so on.

  - Special journals (90-99) are specialized lists of transactions records preconfigured in the system for the balances carried forward. Further journals can be created.

Special months are also preconfigured in the system for special business transactions, such as balances carried forward or subsequent postings.

#### Prerequisites

- A valid fiscal year has been created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Post > Tab POSTINGS*

![Postings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Postings]")

1. Click the *FY/MONTH/JOURNAL* button.  
The *Select fiscal year* window is displayed.  

  ![Select fiscal year](../../Assets/Screenshots/RetailSuiteAccounting/SelectFiscalYear.png "[Select fiscal year]")

2.  Click the *Fiscal year* drop-down list and select a fiscal year.  
The *Period* date fields are filled in automatically.

3. Click the *Month* drop-down list and select a month. The selected month determines the posting period, this means, the period where the transaction is posted.

  > [Info] Apart from the calendar months, special posting periods can also be chosen to post balances carried forward, subsequent postings or closing postings. For detailed information, see [Select fiscal year](../UserInterface/00a_FiscalYear.md).

4. Enter a journal number in the *Journal* field. Alternatively, click the [LIST] button.  
The *Journals* window is displayed with the available journals and their postings.

  ![Journals](../../Assets/Screenshots/RetailSuiteAccounting/Journals.png "[Journals]")

  > [Info] Journals 1-12 are paired with the corresponding calendar months, regardless of whether the fiscal year coincides with the calendar year or not. Therefore, it is highly recommended to select the first month of the fiscal year with journal 1, the second month of the fiscal year with journal 2, and so on. Journals 90 to 99 are special journals configured in the accounting settings for balances carried forward. For detailed information, see [Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md).

[comment]: <> (Journals 1-12 are assigned to the corresponding months, regardless of whether the fiscal year coincides with the calendar year or not. This means that all postings registered in the first month of the fiscal year will be found in the journal 1, all postings registered in the second month of the fiscal year in the journal 2, and so on. - Ich denke, das stimmt so nicht - Prüfen!)

[comment]: <> (Alter Text: Journals 1-12 are matched with the corresponding months, irrespectively of whether or not the fiscal year coincides with the calendar year. Make sure that the month and the journal selected match before clicking the [OK] button.)

[comment]: <> (Macht es hier Sinn, die Fixed bookings checkbox hinzuzufügen. Ich denke nicht.)


6. Click the [OK] button in the bottom right corner.   
  The postings registered in the selected posting period (fiscal year, month and journal) are displayed in the *POSTINGS* tab in the *Post* menu entry.  