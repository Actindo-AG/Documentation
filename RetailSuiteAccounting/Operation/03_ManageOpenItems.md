[!!Accounting](Actindo/Accounting)

# Manage the open items

The *Open items* tab displays any open items in the system, that is, any business transactions that have not yet been completed. The open items function helps to monitor cash movements and avoid liquidity problems.

There are two view modes:

- If no account is selected, the *Open items* tab displays all open items in the *Accounting* module.
- If an account is selected, the *Open items* tab displays only the open items for the selected account.

> [Info] An account can be selected either by entering an  account number in the *Account* or *Contra account* field, or by clicking on a booking in the *Bookings* tab.  


## Access all open items

You can display all open items recorded in the system within the selected booking period.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

### Procedure

*Accounting > Select fiscal year > Book > Tab OPEN ITEMS*

![Open items - No account selected](/Assets/Screenshots/Accounting/Book/OpenItems/OpenItens_NoAccountSelected.png "[Open items - No account selected]")

[comment]: <> (New screenshots to be done when demo data are uploaded)

1. Check that no account number is entered in the *Account* or *Contra account* fields.

2. If the *Account* or *Contra account* fields are filled out, clear the content either with the keyboard delete key or with the [CLEAR] button. Press Enter or the tab key.  
The *Open items* tab shows all open items available in the *Accounting* module.

 > [Info] If there are no open items, a blank tab is displayed.

  ![Open items - No open items](/Assets/Screenshots/Accounting/Book/OpenItems/OpenItems_no_OPOS.png "[Open items - No open items]")

### Next steps

  - [Access the open items for an account](#access-the-open-items-for-an-account)
  - [Create a manual booking](04_CreatedManualBooking)
  - [Cancel a booking](05_CancelBooking)
  - [Delete bookings](06_DeleteBookings)
  - [Process bookings](07_ProcessBookings)
  - [Lock a period for bookings](08_LockPeriodBookings)
  - [Split a booking](09_SplitBooking)
  - [Manage receipts](10_ManageReceipts)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)


## Access the open items for an account

You can display all open items recorded in a specific account within the selected booking period.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).

### Procedure

*Accounting > Select fiscal year > Book > Tab OPEN ITEMS*

![Open items - Account selected](/Assets/Screenshots/Accounting/Book/OpenItems/OpenItens_AccountSelected.png "[Open items - Account selected]")

1. Enter a personal account number in the *Contra account* or in the *Account* field. Alternatively, click on a booking in the *Bookings* tab.
The open items recorded in the corresponding account are displayed in the *Open items* tab.

2. Select the *Standard open items view* or the *Show manually settled open items* radio button to filter the open items displayed as appropriate.

3. If necessary, you can clear open items manually. To do so, select the bookings to be settled by marking the ![checkbox](/Assets/Icons/Checkbox.png "[checkbox]") checkbox in the *M* column.
The amount displayed in the *Amount* box on the right-hand side of the workspace equals 0,00.

  ![Open items - Account selected](/Assets/Screenshots/Accounting/Book/OpenItems/OpenItems_ClearManually_Checkbox.png "[Open items - Account selected]")

4. Click the [CLEAR MANUALLY] button.  
 The bookings are settled. The open items disappear from the open items list with the *Standard open items view* radio button selected.

5. If necessary, you can reverse manually cleared bookings. To do so, click the *Show manually settled open items* radio button to display again all manually cleared bookings for the selected account. The manually cleared bookings are marked with an asterisk next to the checkbox.

6. Select the manually cleared bookings to be reversed.  
The amount displayed in the *Amount* box on the right-hand side of the workspace equals 0,00.

7. Click the [CANCEL CLEARING] button to reverse the clearing.  
The manual clearing has been cancelled.

[comment]: <> (Testen nochmals, evtl. RS Flo Heusel.)

### Next steps

  - [Create a manual booking](04_CreatedManualBooking)
  - [Cancel a booking](05_CancelBooking)
  - [Delete bookings](06_DeleteBookings)
  - [Process bookings](07_ProcessBookings)
  - [Lock a period for bookings](08_LockPeriodBookings)
  - [Split a booking](09_SplitBooking)
  - [Manage receipts](10_ManageReceipts)
  - [Create a balance carried forward](11_CreateBalanceCarriedForward)
  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

### See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Zahlungsabwicklung Offene Posten](#to_be_completed)
