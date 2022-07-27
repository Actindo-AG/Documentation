[!!Zahlungsabwicklung](RetailSuiteBanking)
[!!User Interface open items](../UserInterface/01d_OpenItems.md)  


# Manage the open items

The *OPEN ITEMS* tab displays any open items in the system, that is, any business transactions that have not yet been completed. The open items function helps to monitor cash movements and avoid liquidity problems.

There are two view modes:

- If no account is selected, the *OPEN ITEMS* tab displays all open items in the *Accounting* module.
- If a personal account is selected, the *OPEN ITEMS* tab displays only the open items for the selected account.

> [Info] An account can be selected either by entering an  account number in the *Account* or *Contra account* field, or by clicking on a booking in the *BOOKINGS* tab.  


## Access all open items

You can display all open items recorded in the system.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab OPEN ITEMS*

![All open items](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/NoAccountSelected.png "[All open items]")

1. Check that no account number is entered in the *Account* or *Contra account* fields.

2. If the *Account* or *Contra account* fields are filled out, clear the content either with the keyboard delete key or with the [CLEAR] button. Press Enter or the tab key.  
The *OPEN ITEMS* tab shows all open items available in the *Accounting* module.

 > [Info] If there are no open items, a blank tab is displayed.

  ![No open items](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/NoOPOS.png "[No open items]")



## Access the open items for an account

You can display all open items recorded in a specific personal account, that is, a creditor or debtor account.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](../Integration/01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](../Integration/04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](./01_SelectFiscalYear.md).

#### Procedure

*Accounting > Select fiscal year > Book > Tab OPEN ITEMS*

![Open items for an account](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/AccountSelected.png "[Open items for an account]")

1. Enter a personal account number in the *Contra account* or in the *Account* field. Alternatively, click on a booking in the *BOOKINGS* tab.
The open items recorded in the corresponding account are displayed in the *OPEN ITEMS* tab.

2. Select the *Standard open items view* or the *Show manually cleared open items* radio button to filter the open items displayed as appropriate.

3. If necessary, you can clear open items manually. To do so, select the bookings to be settled by marking the ![checkbox](../../Assets/Icons/Checkbox.png "[checkbox]") checkbox in the *M* column.  
The amount displayed in the *Amount* box on the right-hand side of the workspace equals 0,00.

  ![Clear manually](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/ClearManually.png "[Clear manually]")

4. Click the [CLEAR MANUALLY] button.  
 The bookings are cleared. The open items disappear from the open items list with the *Standard open items view* radio button selected.

5. If necessary, you can reverse manually cleared bookings. To do so, click the *Show manually cleared open items* radio button.   
 All manually cleared bookings for the selected account are displayed. The manually cleared bookings are marked with an asterisk next to the checkbox.

   ![Manually cleared open items](../../Assets/Screenshots/RetailSuiteAccounting/Book/OpenItems/ManuallyClearedOPOS.png "[Manually cleared open items]")

6. Select the manually cleared bookings to be reversed.  
The amount displayed in the *Amount* box on the right-hand side of the workspace equals 0,00.

7. Click the [CANCEL CLEARING] button to reverse the clearing.  
The manual clearing has been cancelled.
