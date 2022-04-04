[!!Accounting](RetailSuiteAccounting)

# Manage the fiscal year

The fiscal year is set up during the configuration process via the accounting wizard. For detailed information, see [Fiscal years](01_RunAccountingWizard.md#fiscal-years). After the initial fiscal year is set up during configuration, any subsequent fiscal years must be manually created. It is essential to create a new fiscal year in the system at the beginning of the new fiscal year.

> [Info] If the system cannot find a fiscal year to book any newly issued invoices, they will remain unrecognized and will have to be booked again manually via the *Invoicing* module, once the new fiscal year has been created.  

## Create a fiscal year

You can create a fiscal year that is not yet available in the system.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](01_RunAccountingWizard.md).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab FISCAL YEARS*

![Create a fiscal year](/Assets/Screenshots/RetailSuiteAccounting/Settings/FiscalYears/CreateFiscalYear.png "[Create a fiscal year]")

1. Enter a description for the fiscal year in the *Description* field.

 > [Info] It is possible to enter digits, letters or combinations of characters. The number of characters is limited to 10.

2.  Enter the starting and finishing date of your fiscal year in the *From - To* fields. The fiscal year shown by default is the current calendar year.

  > [Info] The fiscal year must consist of 12 months. However, it does not have to be a calendar year, for example from 1st April to 31st March.

  > [Info] Fiscal years cannot overlap in time, for example, fiscal years 2022 and 2022-2023 cannot coexist. If two fiscal years overlap, an error message will be displayed. However, a fiscal year for planning purposes can overlap in time with actual fiscal years.

3. Click the *Currency* drop-down list and select the base currency. The drop-down list displays all currencies configured in the system. However, the accounting module works with the base currency only.

4. Click the *Cash accounting* drop-down list and select the appropriate option (**No/Yes**).

  > [Info] The cash accounting refers to a method where receipts are recorded during the period they are received, and expenses are recorded in the period in which they are actually paid. This contrasts accrual accounting, where revenue is recognized when earned rather than when collected, and expenses are recognized when incurred rather than when paid.

  > [Warning] This option has fundamental implications for the system automatic recording of taxes. In case of doubt, please check with your tax advisor.

5. Click the *Planning FY* drop-down list and select the appropriate option (**No/Fiscal year for planning purposes only**).   

  > [Info] Note that a fiscal year can be set up for planning purposes only. However, the fiscal year for planning purposes will not be recognized as an actual fiscal year by the system, and therefore the automatic functions in the interaction with other modules will not apply.

6. Click the [SAVE & NEW] button.  
The new fiscal year is created. A small pop-up window confirms that the new fiscal year has been saved. The newly created fiscal year is displayed in the list.

### Next steps

- [Edit a fiscal year](#edit-a-fiscal-year)
- [Delete a fiscal year](#delete-a-fiscal-year)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [Financial year](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
- [Financial years](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
- [Select the financial year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md)


## Edit a fiscal year

You can edit an available fiscal year, for example if a setting must be changed.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](#create-a-fiscal-year).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab FISCAL YEARS*

![Edit a fiscal year](/Assets/Screenshots/RetailSuiteAccounting/Settings/FiscalYears/EditFiscalYear.png "[Edit a fiscal year]")

1. Click on the existing fiscal year to be edited.   
The existing data for the selected fiscal year are displayed in the corresponding fields.

    > [Warning] Be aware that any changes made to an existing fiscal year will overwrite the preset values.

2. Edit the fields as appropriate.

3. Click the [SAVE] button.   
The fiscal year has been edited. The edited fiscal year is displayed in the list.

### Next steps

- [Delete a fiscal year](#delete-a-fiscal-year)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [Financial year](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
- [Financial years](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
- [Select the financial year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md)


## Delete a fiscal year

You can delete an existing fiscal year, for example if it is no longer applicable.

### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](#create-a-fiscal-year).

### Procedure

*Accounting > Select the fiscal year > Settings > Tab FISCAL YEARS*

![Delete a fiscal year](/Assets/Screenshots/RetailSuiteAccounting/Settings/FiscalYears/DeleteFiscalYear.png "[Delete a fiscal year]")

1. Select the fiscal year to be deleted.
  > [Warning] Be aware that the existing fiscal year will be deleted permanently.

2. Click the [DELETE] button.  
The selected fiscal year will be deleted.

### Next steps

- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [Financial year](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
- [Financial years](/RetailSuiteAccounting/UserInterface/00_UserInterface.md)
- [Select the financial year](/RetailSuiteAccounting/Operation/01_SelectFiscalYear.md)
