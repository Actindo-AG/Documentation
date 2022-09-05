[!!User Interface Balance carried forward](../UserInterface/01_Book.md#balance-carried-forward)  
[!!User Interface Settings Balance carried forward](../UserInterface/02h_BalanceCarriedForward.md)  


# Create a balance carried forward

At the turn of the fiscal year, any outstanding balances must be carried forward to the next one. Closing balances will then be transferred as opening balances into the new fiscal year.

By using the balance carry forward, outstanding account balances and open items can be transferred from one fiscal year to the next. This is possible for both personal accounts (debtors and creditors) and impersonal accounts (for example bank or tax accounts).

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

  ![Balance carried forward: step 1](../../Assets/Screenshots/RetailSuiteAccounting/Book/BalanceCarriedForward01.png "[Balance carried forward: step 1]")  

  [comment]: <> (The *Cost accounting* field is displayed only when cost centers and/or cost units have been created in the fiscal year from which the balance is carried forward.)

3. Click the *Carry forward from FY* drop-down list and select the appropriate fiscal year. All available fiscal years prior to the currently selected fiscal year are displayed in the list.

4. Click the *Range from - to* drop-down lists and select the account classes to be carried forward. The account classes as preconfigured in the *BALANCE CARRIED FORWARD* tab are displayed.

5. If necessary, change the posting date in the *Posting date* field. By default, the first day of the new fiscal year is preselected.

6. Select the appropriate option(s) in the *Cost accounting* field if you also want to carry forward cost centers, cost units or inactive cost centers/units.

7. Select the *Delete old balances carried forward from selected FY* checkbox if necessary.

  > [Info] Previously balances carried forward will be then replaced by the new balances carried forward. The original posting in the previous fiscal year is not deleted though.

[comment]: <> (Was genau passiert dann? Wird empfohlen, das zu machen? Oder könnte das Probleme geben, weil Daten gelöscht werden? Weitere Info notwendig. -> Die ursprüngliche Buchung wird nicht gelöscht, nur die Buchung, die als Saldovortrag, also im Journal 98, angezeigt wird. Der neue Saldovortrag wird dann angezeigt.)

8. Click the [CONTINUE] button.  
The *Retrieve account balances* window is displayed.

  ![Retrieve account balances](../../Assets/Screenshots/RetailSuiteAccounting/Book/RetrieveAccountBalances.png "[Retrieve account balances]")


9. Select the account balances to be carried forward in the *Accounts* field.

  > [Info] To select multiple items, press and hold the **Ctrl** key while clicking with the mouse the corresponding accounts balances.

10. Click the [CONTINUE] button.  
The *Carry balances forward* window is displayed. The pop-up window *Balance carried forward completed* is displayed. The selected balances have been carried forward.

  ![Balance carried forward completed](../../Assets/Screenshots/RetailSuiteAccounting/Book/BalanceCarriedForwardCompleted02.png "[Balance carried forward completed]")

  [comment]: <> (Wenn keine Kostenrechnung vorgetragen, pop-window zeigt nur Saldovortrag durchgeführt an. S. Screenshot BalanceCarriedForwardCompleted01. Welches verwenden?)

11. Click the [CLOSE] button.  
The *Carry balances forward* window is closed.
