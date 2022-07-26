[!!User Interface BWA assignment](../UserInterface/02i_BWAAssignment.md)
[!!User Interface evaluations](../UserInterface/01_Book.md#evaluations)
[!!Create a PDF evaluation](../Operation/15_ProvideAccountingData.md#create-a-pdf-evaluation)


# Manage the BWA reports

[comment]: <> (BWA reports or Accounting Reports? See Accounting Reports view -> ZUORDNUNG BWA tab)

The business evaluation (BWA) is a reporting system based on company financial data and provides information about the company's current cost and revenue situation and, consequently, its  profitability. BWA reports serve as a basis for managerial future decisions, and they are widely used by capital investors and credit institutions for company assessment. BWA is an essential planning and controlling tool for the company's future development.

The *BWA assignment* tab in the *Accounting* module enables to create new BWA reports, to copy one of the predefined system reports and edit it, or to delete any of them. All available reports can be completely customized.

 > [Warning] Be aware that any deletion is permanent and cannot be undone, and any changes made will overwrite the preset values.

When customizing existing reports, bear in mind that the reports use the standard accounts set up in the *Accounting* module configuration process. For detailed information, see [Charts of accounts](./01_RunAccountingWizard.md#chart-of-accounts). If the accounts have been customized manually, they will have to be set up again individually for the BWA reports. Otherwise, the BWA reports will not recognized them.


## Create a BWA report

You can create a BWA report that is not yet available in the system.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](./01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](./04_ManageFiscalYear.md#create-a-fiscal-year).

#### Procedure

*Accounting > Select the fiscal year > Settings > Tab BWA ASSIGNMENT*

![Create a BWA report](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/CreateBWAReport.png "[Create a BWA report]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the right bottom corner.  
The *Create* view is displayed.

2. Enter a name in the *Report name* field.

3. Click the [SAVE] button.  
The new BWA report has been saved.

  ![BWA report created](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/BWAReportCreated.png "[BWA report created]")

4. Click the newly created report in the list.  
The *Accounting report lines* section is displayed.

  ![Add report lines](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/AddReportLines.png "[Add report lines]")

5. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.  
The *Create* section is displayed.

  ![Create report lines](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/CreateReportLines02.png "[Create report lines]")

6. Enter any relevant information in the corresponding fields. You can also add different formulas to it. For detailed information, see [BWA assignment](../UserInterface/02i_BWAAssignment.md).

7. Click the [SAVE] button.  
The new report lines have been saved in the report.


## Edit a BWA report

You can edit an existing BWA report to make any necessary changes, for example, change the report name and layout, and edit or delete report lines.

 > [Warning] Be aware that any changes made to an existing BWA report will overwrite the existing values. If you are taking one of the predefined system reports as a basis, it is highly recommended to make a copy of it first. For detailed information, see [BWA assignment](../UserInterface/02i_BWAAssignment.md).

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](./01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](./04_ManageFiscalYear.md#create-a-fiscal-year).
- A BWA report is created, see [Create a BWA report](#create-a-BWA-report).

#### Procedure

*Accounting > Select the fiscal year > Settings > Tab BWA ASSIGNMENT*

![Edit a BWA report](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/EditBWAReport.png "[Edit a BWA report]")

1. Select the BWA report to be edited by clicking the checkbox on the left.   
The toolbar is displayed in the right upper corner.

2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Add]") (Edit) button to edit the BWA report.  
The *Edit* section is displayed.

3. Click the *Report name* field and make any necessary changes.

4. Click the *Columns* button in the right upper corner.   
The columns bar is displayed. You can add or delete columns, and change their order by clicking and moving them with the mouse.

  ![Edit BWA report layout](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/EditBWAReportLayout.png "[Edit BWA report layout]")

5. Click the [APPLY] button.   
The changes are applied.

  > [Info] The width of the individual columns in the table header can also be modified using the mouse.

6. Select any accounting report line to be edited by clicking the checkbox on the left.  
The toolbar is displayed in the right upper corner.

  ![Edit report lines](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/EditReportLines.png "[Edit report lines]")

7. Click the ![Edit](../../Assets/Icons/Edit01.png "[Add]") (Edit) button to edit the selected accounting report line.  
The *Edit* section is displayed.   

  > [Warning] Be aware that any changes made to an existing BWA report will overwrite the existing values.

  You can also delete an accounting report line. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button in the toolbar to delete the selected accounting report line.  

   > [Warning] Be aware that the existing accounting report line will be deleted permanently.

8. Click the [SAVE] button.   
The existing BWA report has been edited.


[comments]: <> (clear with HG: you can also edit the BWA report/the accounting report lines by clicking on the report name or line name -> same editing options as described above are displayed. Shall we describe it as an alternative or better not?)


## Delete a BWA report

You can delete an existing BWA report, either one of the predefined system reports or a newly created one.

#### Prerequisites

- The accounting is configured via the configuration wizard, see [Run the accounting wizard](./01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Create a fiscal year](./04_ManageFiscalYear.md#create-a-fiscal-year).
- A BWA report is created, see [Create a BWA report](#create-a-BWA-report).

#### Procedure

*Accounting > Select the fiscal year > Settings > Tab BWA ASSIGNMENT*

![Delete a BWA report](../../Assets/Screenshots/RetailSuiteAccounting/Settings/BWAAssignment/DeleteBWAReport.png "[Delete a BWA report]")

1. Select the BWA report to be deleted by clicking the checkbox on the left.   
The toolbar is displayed in the right upper corner.

  > [Warning] Be aware that the existing BWA report will be deleted permanently.

2. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button to delete the BWA report.  
The selected BWA report is deleted.
