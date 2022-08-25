[!!User Interface Postings](../UserInterface/01a_Bookings.md)  
[!!User Interface Open items](../UserInterface/01d_OpenItems.md)   


# Cancel a posting

You can cancel a posting, for example, if an invoice has been mistakenly posted to a wrong account or a posting must be corrected.   
Once an invoice has been issued and posted, it cannot be simply deleted for legal reasons. The incorrect invoice must be cancelled, recorded as reverse posting in the system, and a new correct posting must be recorded, if necessary.   
When cancelling a posting, a copy of the original posting with the negative turnover amount is created.

#### Prerequisites

- A fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).
- At least one posting has been created, see [Create a manual posting](./04_CreateManualBooking.md).

#### Procedure

*Accounting > Select fiscal year > Post > Tab POSTINGS*

![Postings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Postings]")

1. Select the posting to be cancelled in the postings list.  
  The posting details are displayed in the input line fields.

2. Click the [CANCEL] button.   
  A new posting with a negative turnover amount corresponding to the posting to be cancelled is created. The negative posting is displayed in the postings list. The posting text "Cancel" is displayed in the *Text* column for this posting. The notice "Posted. Debtor/creditor: receipt (number) is cleared." is displayed above the input line.

  > [Info] The open item created by the original posting is automatically cleared by the cancellation posting in the *OPEN ITEMS* tab.  
