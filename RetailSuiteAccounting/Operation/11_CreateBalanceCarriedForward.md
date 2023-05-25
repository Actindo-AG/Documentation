[!!User interface Postings header](../UserInterface/01_Header.md)  
[!!User interface Settings Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md)  

# Create a balance carried forward

At the turn of the fiscal year, outstanding balances of the accounts of the balance sheet must be carried forward to the next one. Closing balances will then be transferred as opening balances into the new fiscal year.

By using the balance carry forward, outstanding account balances and open items are transferred from one fiscal year to the next. 

Special journals are preconfigured in the system to carry balances and open items forward. For example, journal 98 contains all balances carried forward for debtors open items, and 99 the balances carried forward for creditors open items. These settings can be completely customized. For detailed information, see [User Interface Settings Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md).

#### Prerequisites

- A new fiscal year has been created, see [Create a fiscal year](../Integration04_ManageFiscalYear.md#create-a-fiscal-year).
- The new fiscal year has been selected, see [Select fiscal year](./01_SelectFiscalYear.md).
- The balance carried forward function is configured, see [User Interface Settings Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md).

#### Procedure

*Accounting > Book > Tab BOOKINGS*

![Postings](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Postings]")

1. Click the [EDIT] button in the header above the postings list.  
    A context menu is displayed.

    ![Edit](../../Assets/Screenshots/RetailSuiteAccounting/Book/Edit.png "[Edit]")

2. Click the *Balance carried forward...* menu entry in the context menu.     
    The *Balance carried forward: step 1* window is displayed.

    > [Info] The *Cost accounting* field is displayed only when cost centers and/or cost objects have been created in the fiscal year from which the balance is carried forward.

    ![Balance carried forward: step 1](../../Assets/Screenshots/RetailSuiteAccounting/Book/BalanceCarriedForward01.png "[Balance carried forward: step 1]")  

3. Click the *Carry forward from FY* drop-down list and select the appropriate fiscal year. All available fiscal years prior to the currently selected fiscal year are displayed in the list.

4. Click the *Range from - to* drop-down lists and select the account classes to be carried forward. The account classes as preconfigured in the *BALANCE CARRIED FORWARD* tab are displayed.

5. Make sure that the posting date is the first date of the new fiscal year.

    > [Info] Balances carried forward are performed at the start of the fiscal year. By default, the first day of the new fiscal year is preselected as the posting date.

6. Select the appropriate option(s) in the *Cost accounting* field if you also want to carry forward cost centers, cost objects or inactive cost centers/objects.

7. Select the *Delete old balances carried forward from selected FY* checkbox if necessary.

    > [Info] Previous balances carried forward  will be then replaced by the new balances carried forward. The original posting in the previous fiscal year is not deleted though.

8. Click the [CONTINUE] button.  
    The *Retrieve account balances* window is displayed.

    ![Retrieve account balances](../../Assets/Screenshots/RetailSuiteAccounting/Book/RetrieveAccountBalances.png "[Retrieve account balances]")

9. Select the account balances to be carried forward in the *Accounts* field.

    > [Info] To select multiple items, press and hold the **Ctrl** key while clicking with the mouse the corresponding accounts balances.

10. Click the [CONTINUE] button.  
    The *Carry balances forward* window is displayed. The pop-up window *Balance carried forward completed* is displayed. The selected balances have been carried forward.

    ![Balance carried forward completed](../../Assets/Screenshots/RetailSuiteAccounting/Book/BalanceCarriedForwardCompleted02.png "[Balance carried forward completed]")

11. Click the [CLOSE] button.  
    The *Carry balances forward* window is closed.
