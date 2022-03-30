[!!Accounting](Accounting)

# Run the accounting wizard

In order to use the *Accounting* module, you need to configure the master data first. The accounting wizard guides you through the configuration process. Once the configuration process is finished, the *Accounting* module will be set up and ready to use. Since the *Accounting* module works together with many other modules, it is highly recommended to carry out the configuration as one of the first steps when installing the system.

 > [Info] The *Accounting* module can neither create a balance sheet nor an annual financial statement.

The accounting wizard starts automatically when opening the *Accounting* module for the first time. You can cancel the accounting wizard and run it at a later point. In this case, the [START WIZARD] button will be displayed when accessing the *Accounting* module again. Click then the [START WIZARD] button. The accounting wizard will help you enter all necessary data step by step.

## Prerequisites

No prerequisites to fulfill.

## Procedure

### Start wizard

*Accounting*

![Accounting wizard](/Assets/Screenshots/Accounting/AccountingWizard/AccountingWizard.png "[Accounting wizard]")

Click the [START] button.   
The configuration process starts. The *Fiscal years* wizard window is displayed.

> [Info] The progress in the wizard is displayed on the top left corner in the accounting wizard window.


### Fiscal years

In the first step you have to configure the fiscal years.

![Fiscal Year](/Assets/Screenshots/Accounting/AccountingWizard/FiscalYear.png "[Fiscal Year]")

 1. Enter a description for the fiscal year in the *Description* field. The system shows the current year by default.  

   > [Info] It is possible to enter digits, letters or combinations of characters. The number of characters is limited to 10.

 2.  Enter the starting and finishing date of your fiscal year in the *From - To* fields. The fiscal year shown by default is the current calendar year.

 > [Info] The fiscal year must consist of 12 months. However, it does not have to be a calendar year, for example from 1st April to 31st March.

 3. Select the base currency in the *Currency* drop-down list. The drop-down list displays all currencies configured in the system. However, the accounting module works with the base currency only.


 4. Select the appropriate option (**No/Yes**) in the *Cash accounting* drop-down list.

 > [Info] The cash accounting refers to a method where receipts are recorded during the period they are received, and expenses are recorded in the period in which they are actually paid. This contrasts accrual accounting, where revenue is recognized when earned rather than when collected, and expenses are recognized when incurred rather than when paid.

 > [Warning] This option has fundamental implications for the system automatic recording of taxes. In case of doubt, please check with your tax advisor.

 5. Select the appropriate option (**No/Fiscal year for planning purposes only**) in the *Planning FY* drop-down list.   

 > [Info] Note that a fiscal year can be set up for planning purposes only. However, the fiscal year for planning purposes will not be recognized as an actual fiscal year by the system, and therefore the automatic functions in the interaction with other modules will not apply.

 6. Click [SAVE & NEW].  
  The new fiscal year is created.    
A small pop-up window and a green check mark confirm that the new fiscal year has been saved. The newly created fiscal year is also displayed in the list.

 7. Click [CONTINUE].  
 The *Chart of accounts* wizard window is displayed.


### Chart of accounts

In this second step, you must select a chart of accounts and an accounting system.

![Chart of Accounts](/Assets/Screenshots/Accounting/AccountingWizard/ChartAccounts.png "[Chart of Accounts]")


1. Select the appropriate option in the *Chart of accounts* drop-down list:

    - **SKR03 - Standard Chart of accounts**
    - **SKR04 - Standard Chart of accounts new version**
    - **Swiss Chart of accounts KMU**
    - **Swiss Chart of accounts Käfer**

 > [Warning] The Chart of accounts can only be set up once and cannot be changed afterwards. Any later modifications have to be done manually on an individual customer account level.

2. Select the appropriate option in the *Accounting system* drop-down list:
    - **German Commercial Code: P&L**
    - **German Commercial Code: Balance partnerships**
    - **German Commercial Code: Balance small, mid-sized, large corporations**
    - **Cash flow**
    - **US-GAAP: statement of earnings**
    - **US-GAAP: statement of financial position**
    - **US-GAAP: statement of cash flow**
    - **IAS: P&L**
    - **IAS: Balance**
    - **IAS: Cash flow**

  > [Info] The *Accounting* module can neither create a balance sheet nor an annual financial statement. Therefore, the selection of any of the drop-down list options suggested serves merely a pro-forma purpose.

3. Click the [CONTINUE] button.  
The *Accounting* module is set up.  
A small pop-up window and a green check mark confirm that the chart of accounts and the accounting system have been saved.
The *Installation completed* wizard window is displayed.


### Installation completed

In the *Installation completed* wizard window all three progress steps are now checked.

![Installation completed](/Assets/Screenshots/Accounting/AccountingWizard/InstallationCompleted.png "[Installation completed]")

Now click the [FINALIZE] button.     
The accounting wizard closes and the system loads all data. This may take a few seconds. Then, the fiscal year selection window is displayed.

### Next steps

- [Manage the tax keys](02_ManageTaxKeys.md)
- [Manage the accounts](03_ManageAccounts.md)
- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [User interface Fiscal year](#headingID)
