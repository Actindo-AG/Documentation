[!!User Interface Lock months](../UserInterface/01_Header.md#lock-months)  
[!!User Interface Postings](../UserInterface/01a_Bookings.md)  


# Lock a period for postings

Once the postings in a particular posting period are processed, they cannot be changed or deleted anymore, and the corresponding postings period is regarded as closed. However, new postings can be entered in a closed posting period if necessary. To avoid subsequent postings to an already closed posting period, you can lock periods for postings.   

When a posting period is locked, any subsequent transaction will be automatically posted in the next unlocked posting period.    
In contrast to posting processing, locking a posting period can be undone if necessary.

#### Prerequisites

- A fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).
- At least one posting has been created, see [Create a manual posting](./04_CreateManualBooking.md).

#### Procedure

*Accounting > Post > Tab POSTINGS*

![Postings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Postings]")

1. Click the [EDIT] button in the header above the postings list.  
    A context menu is displayed.

    ![Edit](../../Assets/Screenshots/RetailSuiteAccounting/Book/Edit.png "[Edit]")

2. Click the *Lock months...* menu entry in the context menu.     
    The *Lock fiscal months* window is displayed.

    ![Lock months selection window](../../Assets/Screenshots/RetailSuiteAccounting/Book/LockMonths.png "[Lock months selection window]")

3. Click the drop-down list after the month to be locked and select the **Locked** option. Repeat this step for all months to be locked. The drop-down list is active only for those months where postings have been recorded.

    > [Info] Select the **bookable** option in the drop-down list to unlock the corresponding month and make it available for postings again.

4. Click the [OK] button.  
    A pop-up window is displayed while the changes are being saved. As soon as the pop-up window is no longer displayed, the selected months are locked.
