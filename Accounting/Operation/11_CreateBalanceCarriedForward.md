[!!Accounting](Actindo/Accounting)

# Create a balance carried forward

At the turn of the fiscal year, any outstanding balances must be carried forward to the next one. Closing balances will then be transferred as opening balances into the new fiscal year.

The *Balance carried forward* menu entry of the *EDIT* context menu in the *BOOKINGS* allows to transfer outstanding account balances and open items from one fiscal year to the next one. This is possible for both personal (debtors' and creditors') accounts and impersonal accounts, for example bank or tax accounts.

Special journals are preconfigured in the system to carry  balances and open items forward. For example, journal 98 contains all balances carried forward for debtors' open items. These settings can be completely customized. For detailed information, see [Balance carried forward](#to_be_completed).

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A new valid fiscal years is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- The balance carried forward function is configured, see [Balance carried forward](#to_be_completed).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Balance carried forward*

![Balance carried forward](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BalanceCarriedForward.png "[Balance carried forward]")

1. Click the *Balance carried forward* menu entry.  
The *Balance carried forward: step 1* wizard window is displayed.

  ![Balance carried forward wizard](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BalanceCarriedForward_Wizard.png "[Balance carried forward wizard]")

2. Select the fiscal year in the *Carry forward from FY* field.

3. Select the accounts to be carried forward from the *Range from - to* drop-down lists.

4. Enter the booking date.

  > [Info] By default, the system displays the first date of the new fiscal year. This can be modified simply by typing in the desired booking date.

5. Select the *Delete old balances carried forward from selected FY* checkbox if necessary.

6. Click the [CONTINUE] button.  
The *Retrieve account balances* window is displayed.

7. Select the account balances to be carried forward in the *Accounts* fields.

  > [Info] Use Ctrl and mouse click to select multiple items.

8. Click the [CONTINUE] button.  
A message confirms that the balance is carried forward. The wizard window closes automatically.

  ![Retrieve account balances](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_BalanceCarriedForward_Wizard2.png "[Retrieve account balances]")


## Next steps

  - [Book exchange rate fluctuations](12_BookExchangeRateFluctuations)
  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

## See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [User Interface Balance carried forward](#to_be_completed)
