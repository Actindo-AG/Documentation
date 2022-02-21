[!!Accounting](Actindo/Accounting)

# Run the accounting wizard
In order to use the *Accounting* module, you need to configure
the master data first. The accounting wizard guides you through
the configuration process. Once the configuration process is finished, the *Accounting* module will be set up and ready to use. Since the *Accounting* module works together with many other modules, it is highly recommended to carry out the configuration as one of the first steps when installing the system.

 > [Info] Note that the *Accounting* module can neither create
 a balance sheet nor an annual financial statement.

The accounting wizard starts automatically when opening the *Accounting* module for the first time. You can cancel the accounting wizard and run it at a later point. In this case, the button [START WIZARD] will be displayed when accessing the *Accounting* module again. Click the button [START WIZARD].  
The accounting wizard will help you enter all necessary data step by step.

## Prerequisites

No prerequisites to fulfill.

## Procedure

### Start wizard

*Accounting*

![Accounting Wizard](/Assets/Screenshots/Accounting/AccountingWizard/AccountingWizard_Start.png "[Accounting Wizard]")

Click the button [START].   
The configuration process starts. The wizard window *Fiscal years* is displayed.

> [Info] The progress in the wizard is displayed on the top left corner in the accounting wizard window.


### Fiscal years

In the first step you have to configure the fiscal years.

![Accounting Wizard Fiscal Year](/Assets/Screenshots/Accounting/AccountingWizard/AccountingWizard_FiscalYear_l.png "[Accounting Wizard Fiscal Year]")

| (1) | Description |
|-----|---------------------|
| **(2)** | **From - To** |
| **(3)** | **Currency** |
| **(4)** | **Cash accounting** |
| **(5)** | **Planning FY** |
| **(6)** | **Button [SAVE & NEW]** |

 1. Enter a description for the fiscal year in the field *Description*. The system shows the current year by default.  

   > [Info] Note that it is possible to enter digits, letters or combinations of characters. The number of characters is limited to 10.

 2.  Enter the starting and finishing date of your fiscal year in the fields *From - To*. The fiscal year shown by default is the current calendar year.

 > [Info] Note that the fiscal year must consist of 12 months. However, it does not have to be a calendar year, for example from 1st April to 31st March.

 3. Click the drop-down list *Currency* and select the base currency. The drop-down list displays all currencies configured in the system. However, the accounting module works with the base currency only.


 4. Click the drop-down list *Cash accounting* and select the appropriate option (**No/Yes**).

 > [Info] The cash accounting refers to a method where receipts are recorded during the period they are received, and expenses are recorded in the period in which they are actually paid. This contrasts accrual accounting, where revenue is recognized when earned rather than when collected, and expenses are recognized when incurred rather than when paid.

 > [Warning] This option has fundamental implications for the system automatic recording of taxes. In case of doubt, please check with your tax advisor.

 5. Click the drop-down list *Planning FY* and select the appropriate option (**No/Fiscal year for planning purposes only**).   

 > [Info] Note that a fiscal year can be set up for planning purposes only. However, the fiscal year for planning purposes will not be recognized as an actual fiscal year by the system, and therefore the automatic functions in the interaction with other modules will not apply.

 6. Click [SAVE & NEW].  
  The new fiscal year is created.    
A small pop-up window and a green check mark confirm that the new fiscal year has been saved. The newly created fiscal year is also displayed in the list.


 7. Click [CONTINUE].  
 The wizard window *Chart of accounts* is displayed.

### Chart of accounts

In this second step, you must select a chart of accounts and an accounting system.

![Accounting Wizard Chart of Accounts](/Assets/Screenshots/Accounting/AccountingWizard/AccountingWizard_ChartAccounts.png "[Accounting Wizard Chart of Accounts]")


1. Click the drop-down list *Chart of accounts* and select the appropriate one:

    - **SKR03 - Standard Chart of accounts**
    - **SKR04 - Standard Chart of accounts new version**
    - **Swiss Chart of accounts KMU**
    - **Swiss Chart of accounts Käfer**

 > [Warning] Note that the Chart of accounts can only be set up once and cannot be changed afterwards. Any later modifications have to be done manually on an individual customer account level.



2. Click the drop-down list *Accounting system* and select one of the options:
    - **German Commercial Code: P&L**
    - **German Commercial Code: Balance partnerships**
    - **German Commercial Code: Balance small, mid-sized, large Corporations**
    - **Cash flow**
    - **US-GAAP: statement of earnings**
    - **US-GAAP: statement of financial position**
    - **US-GAAP: statement of cash flow**
    - **IAS: P&L**
    - **IAS: Balance**
    - **IAS: Cash flow**

  > [Info] Note that the *Accounting* module can neither create
a balance sheet nor an annual financial statement. Therefore, the selection of any of the drop-down list options suggested serves merely a pro-forma purpose.



3. Click the button [CONTINUE].  
The *Accounting* module is set up.  
A small pop-up window and a green check mark confirm that the chart of accounts and the accounting system have been saved.
The wizard window *Installation completed* is displayed.


### Installation completed

In the wizard window *Installation completed* all three progress steps are now checked.

![Accounting Wizard Installation completed](/Assets/Screenshots/Accounting/AccountingWizard/AccountingWizard_InstallationCompleted.png "[Accounting Wizard Installation completed]")


Now click the button [FINALIZE].     
The accounting wizard closes and the system loads all data. This may take a few seconds. Then, the fiscal year selection window is displayed.



### Next steps
- [Manage the tax keys](#headingID)
- [Manage the tax keys](#headingID)

### See also

- [Fiscal year](#headingID)
