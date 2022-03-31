[!!Accounting](Actindo/Accounting)

# Book exchange rate fluctuations

Suppliers who issue invoices in a foreign currency, for example GBP, can also manage these invoices in the *Accounting* module. For this purpose, the corresponding accounts must be set up in the foreign currency. For detailed information, see [Manage accounts](/Accounting/Integration/04_ManageAccounts.md).

However, the *Accounting* module can only work with the base currency configured in the system. Due to currency exchange rate fluctuations, there can be a difference between the converted amount booked at the time of ordering (open item) and the amount booked at the time of payment.  

 To counteract these fluctuations, the system retrieves once a day the current foreign currency exchange rates as published by the ECB and applies them automatically, therefore always working with the most up-to-date information.

 The *Foreign currency wizard* menu entry of the *EDIT* context menu in the *BOOKINGS* allows to book this difference automatically.

[comment]: <> (Describe the procedure to book exchange rate fluctuations using the foreign currency wizard in compliance with the editorial style guide.)

 [comment]: <> (Explain briefly what the foreign currency wizard is used for and at what time you have to book exchange rate fluctuations.)

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal years is created, see [Create fiscal year](04_ManageFiscalYear.md#create-a-fiscal-year).
- A fiscal year is selected, see [Select fiscal year](01_SelectFiscalYear.md).
- The corresponding accounts are set up in the foreign currency, see [Manage accounts](/Accounting/Integration/04_ManageAccounts.md).

## Procedure

*Accounting > Select fiscal year > Book > Tab BOOKINGS > Context menu EDIT > Menu entry Foreign currency wizard*

![Foreign currency wizard](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_ForeignCurrencyWizard.png "[Foreign currency wizard]")

1. Click the *Foreign currency wizard* menu entry.  
The *Foreign currency wizard* window is displayed.

  ![Foreign currency wizard window](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_ForeignCurrencyWizard_Window.png "[Foreign currency wizard window]")

2. Select the appropriate fiscal year in the *Fiscal year* field.

3. Select the applicable accounts in the *Range of accounts* drop-down list.

  > [Info] If you select the *Individual* option, the *from - to* fields are displayed. You can enter here the corresponding account numbers.

  ![Foreign currency wizard - individual account](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_ForeignCurrencyWizard_Window2.png "[Foreign currency wizard - individual account]")

4. Enter the posting date.

  > [Info] You can type in the posting date or use the ![Calendar](/Assets/Icons/Calendar.png "[Calendar]") icon.

5. Click the [CONTINUE] button.  
The next wizard window is displayed.

  ![Account selection](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_ForeignCurrencyWizard_AccountSelection2.png "[Account selection]")

  > [Info] The system checks the relevant accounts within the selected range and fiscal year. If no accounts are find, the following message is displayed:

  ![No accounts found](/Assets/Screenshots/Accounting/Book/Bookings/Bookings_ForeignCurrencyWizard_noAccounts2.png "[No accounts found]")

6. Select the applicable account in the *Account selection* drop-down list.  

7. Click the [CONTINUE] button.   
The ...

[comment]: <> (Still to find out how booking in diff. currencies works! No accounts found message.)

## Next steps

  - [Access bookings from another period](13_AccessBookingsAnotherPeriod)
  - [Search in accounting](14_SearchAccounting)
  - [Provide the accounting data](15_ProviceAccountingData)

## See also

  - [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md)
  - [Manage accounts](/Accounting/Integration/04_ManageAccounts.md)
