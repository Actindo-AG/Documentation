[!!User interface Debtors/creditors](./02a_DebtorsCreditors.md)
[!!Manage the cost accounting](../Integration/08_ManageCostAccounting.md)

# Cost accounting

*Accounting > Settings > Tab COST ACCOUNTING*

![Cost accounting - not defined](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostAccountingNo.png "[Cost accounting - not defined]")

- *Cost accounting*  
    Click the corresponding drop-down list to select the relevant accounting period (fiscal year and month) and the cost center/object. The following drop-down lists are displayed:
    - Fiscal year drop-down list  
        Click the drop-down list to select the relevant fiscal year. All available fiscal years are displayed in the list.  
    - Month drop-down list  
        Click the drop-down list to select the relevant month. The following options are available:  
        - **0 - Balances carried forward**
        - **1 - 12 - (months)**
        - **13 - 15 - Subsequent postings**  
    - Cost accounting drop-down list  
        Click the drop-down list to select the cost type. The following options are available:  
        - **Cost 1 - Cost center**  
            Select this option to display the available cost centers in the selected accounting period or to create a new one.
        - **Cost 2 - Cost object**  
            Select this option to display the available cost objects in the selected accounting period or to create a new one.   

  All available cost centers or objects in the selected accounting period are displayed in the list. Depending on the selected cost type in the cost accounting drop-down list, the list and the input fields vary:
  - [Cost center](#cost-center)
  - [Cost object](#cost-object)

[comment]: <> (Monat drop-down list: es fehlt 16-19 Abschlussbuchungen und 99 Allgemeiner Monat? FETA ticket)



## Cost center

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 1 - Cost center*

![Cost center](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostAccounting01.png "[Cost center]")

The list displays all available cost centers in the selected accounting period. All fields are read-only. If no cost center has been created in the selected accounting period, the *No cost centers defined* notice is displayed.

- *Cost.*  
    Cost center number.

- *Description*  
    Cost center descriptive name.

- *Inactive*  
    Cost center status. The word **Inactive** is displayed if the cost center has been deactivated. An inactive cost center is locked for postings. 

- *Active from*  
    Validity start date. The posting period in which the cost center has been created and/or set to active is displayed.

The input fields below allow to enter or modify the cost center details.

- ![Radio button](../../Assets/Icons/RadioButtonChecked.png "[Radio button]") *Active*   
    Select this radio button to activate the cost center after saving.

- ![Radio button](../../Assets/Icons/RadioButtonChecked.png "[Radio button]") *Inactive*    
    Select this radio button to deactivate the cost center after saving.

- *Cost center*  
    Enter the cost center number. Only numbers are allowed. The number of digits is limited to 4.

- *Description*  
    Enter a descriptive name for the cost center.

- *Text*  
    Enter a longer description or comments to the cost center. The text is not displayed in the list.

- *Allocation to cost objects*  
    Specify how to allocate costs from different cost centers to individual cost objects. This field is only displayed if at least one cost object has been created. The following button is displayed:
    - [ALLOCATION TABLE]   
        Click this button to display the *Allocation table* window, see [Allocation table](#allocation-table).

- [SAVE & NEW]  
    Click this button to save the new cost center. The button is locked if a cost center has been selected. For detailed information about creating a cost center, see [Create a cost center](../Integration/08_ManageCostAccounting.md#create-a-cost-center).

- [SAVE]  
    Click this button to save any changes made to the selected cost center. The button is only unlocked if a cost center has been selected. For detailed information about editing a cost center, see [Edit a cost center](../Integration/08_ManageCostAccounting.md#edit-a-cost-center).

- [DELETE]  
    Click this button to delete the selected cost center. The button is only unlocked if a cost center has been selected. For detailed information about deleting a cost center, see [Delete a cost center](../Integration/08_ManageCostAccounting.md#delete-a-cost-center).

- [CLEAR]  
    Click this button to clear all input fields.

- [PRINT]  
    Click this button to print the cost center or object. The *Print cost center/object* window is displayed, see [Print cost center/object](#print-cost-center/object).

[comment]: <> (Eigentlich heißt das Fenster Cost center/object, aber ich habe zu Print cost center/object umbenannt hier.)



## Cost object

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 2 - Cost object*

![Cost object](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostAccounting02.png "[Cost object]")

The list displays all available cost objects in the selected accounting period. All fields are read-only. If no cost object has been created in the selected accounting period, the *No cost objects defined* notice is displayed.

- *Cost.*  
    Cost object number.

- *Description*  
    Cost object descriptive name.

- *Inactive*  
    Cost object status. The word **Inactive** is displayed if the cost object has been deactivated. An inactive cost object is locked for postings. 

- *Active from*  
    Validity start date. The posting period in which the cost object has been created and/or set to active is displayed.

- *ProfitCenter*  
    Assigned profit center.

The input fields below allow to enter or modify the cost object details.

- ![Radio button](../../Assets/Icons/RadioButtonChecked.png "[Radio button]") *Active*   
    Select this radio button to activate the cost object after saving.

- ![Radio button](../../Assets/Icons/RadioButtonChecked.png "[Radio button]") *Inactive*    
    Select this radio button to deactivate the cost object after saving.

- *Cost object*  
    Enter the cost object number. Only numbers are allowed. The number of digits is limited to 5.

- *Description*   
    Enter a descriptive name for the cost object.

- *Text*  
    Enter a longer description or comments to the cost object. The text is not displayed in the list.

- *Debtor*  
    Enter the debtor or customer number, if necessary. Alternatively, click the [SEARCH] button to search for a debtor or customer.
    - [SEARCH]  
        Click this button to select a customer or debtor for the *Debtor* field. Th *Select address* window is displayed, see [Select address](#select-address).  

- *ProfitCenter*  
    Click the drop-down list to select the appropriate profit center. All available profit centers are displayed in the list. If no profit center must be assigned to the cost object, select the **No ProfitCenter** option. If no profit center has been created, the **0 - No group** option is displayed. Click the [EDIT...] button to edit or create a profit center.
    - [EDIT...]  
        Click this button to edit or create a profit center. The *ProfitCenter* window is displayed, see [ProfitCenter](#profitcenter).

- [SAVE & NEW]  
    Click this button to save the new cost object. The button is locked if a cost object has been selected. For detailed information about creating a cost object, see [Create a cost object](../Integration/08_ManageCostAccounting.md#create-a-cost-object).

- [SAVE]  
    Click this button to save any changes made to the selected cost object. The button is only unlocked if a cost object has been selected. For detailed information about editing a cost object, see [Edit a cost object](../Integration/08_ManageCostAccounting.md#edit-a-cost-object).

- [DELETE]  
    Click this button to delete the selected cost object. The button is only unlocked if a cost object has been selected. A cost object can only be deleted if no costs from any cost center are assigned to it. For detailed information about deleting a cost object, see [Delete a cost object](../Integration/08_ManageCostAccounting.md#delete-a-cost-object).

- [CLEAR]  
    Click this button to clear all input fields.

- [PRINT]  
    Click this button to print the cost center or object. The *Print cost center/object* window is displayed, see [Print cost center/object](#print-cost-center/object).

[comment]: <> (Eigentlich heißt das Fenster Cost center/object, zu Print cost center/object hier umbenannt. FETA Ticket dazu)



### Print cost center/object

*Accounting > Settings > Tab COST ACCOUNTING > Button PRINT*  

![Print cost center/object](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostCenterObject.png "[Print cost center/object]")

- *Cost center/object*  
    Click the drop-down list to select whether the cost centers or cost objects are to be printed. The following options are available:
    - **Cost 1 - Cost center**   
        The cost centers within this list will be printed according to the settings specified in the following.
    - **Cost 2 - Cost object**    
        The cost objects within this list will be printed according to the settings specified in the following.

- [x] *Active*   
    Select the checkbox to include all active cost centers/objects for printing.

- [x] *Inactive*   
    Select the checkbox to include all inactive cost centers/objects for printing.

- *Numbers from-to*  
    Enter the cost centers/objects number range to be printed.

- *Month*  
    Click the drop-down list to select the desired month to be printed. All available months are displayed in the list.

- *Fiscal year*  
    Click the drop-down list to select the desired fiscal year to be printed. All available fiscal years are displayed in the list.

- [CANCEL]  
    Click this button to cancel the printing process. The *Print cost center/object* window is closed.

- [PRINT]  
    Click this button to print the cost centers/objects according to the selected settings. A print preview is displayed in the window.


### Allocation table

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 1 - Cost center > Button ALLOCATION TABLE*

![Allocation table](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/AllocationTable01.png "[Allocation table]")

- *Select ProfitCenter*  
    Click the drop-down list to select a profit center. All available profit centers are displayed in the list. Additionally, the following options are available:
    - **All ProfitCenters**   
        All available profit centers will be included.
    - **0 - No group**   
        No profit center will be included.   

  The columns in the allocation list change according to the selected profit center option.

- [UPDATE]  
    Click this button to update the table.

    > [Info] Note that any changes made must be saved first by clicking the [SAVE] button at the bottom. Otherwise, all changes will be rejected when updating the list.

- [CHANGE PERIOD]  
    Click this button to change the period. The *Select period* window is displayed, see [Select period](#select-period).

- [EXCEL]  
    Click this button to display the *EXCEL* context menu. The following options are available:  
    - **Export current page**  
        Click this option to export the allocation table currently displayed. The allocation table is exported in Excel format and saved by default in the Downloads folder in your device.
    - **Export all**  
        Click this option to export all available allocation tables. The allocation tables are exported in Excel format and saved by default in the Downloads folder in your device.

      > [Info] The [EXCEL] button is only displayed if the *Statistics* module is installed.

The list displays the allocation of costs among the cost centers and objects. Depending on the selected profit center option, the displayed columns may vary.

- *Cost center*  
    Cost center name. This field is read-only.

- Cost object  
    Double-click a cost object field to activate the field and define the cost allocation. The following options are available:
    - If the **Percentage** option is selected in the drop-down list in the *Allocation* column, enter a percentage value in the field.
    - If the **Formula** option is selected in the drop-down list in the *Allocation* column, click the drop-down list and select the appropriate option:
        - **Active**   
            Select this option to apply the formula specified in the *Formula* column to the selected cost object.
        - **Inactive**   
            Select this option to ignore the formula for the selected cost object.   

    For each available cost object, a single column is displayed in the list.

- *&#931; %*  
    Total sum or total percentage of all cost objects. The displayed number changes automatically. The total must equal 100 to be saved. That means that all cost centers' costs must be allocated to the individual cost objects. Otherwise, an error message is displayed when clicking the [SAVE] button.

- *Allocation*   
    Double-click this field to activate it. Click the drop-down list to select the allocation method. The following options are available:  
    - **Percentage**   
        Select this option to allocate costs based on individual percentages per cost object.
    - **Formula**  
        Select this option to allocate costs based on a formula defined in the *Formula* field.

- *Formula*  
    Double-click this field to activate it and enter an Excel formula. The basic calculating operations (+, -, *, /) are permitted.

- [CLOSE]  
    Click this button to close the *Allocation table* window.

- [PRINT]  
    Click this button to print the allocation table. The *Allocation table* window is displayed, see [Print allocation table](#print-allocation-table).

- [SAVE]  
    Click this button to save any changes made to the allocation table. The *Saving...* pop-up window is displayed.

#### Select period

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 1 - Cost center > Button ALLOCATION TABLE > Button CHANGE PERIOD*

![Select period](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/SelectPeriod.png "[Select period]")

- ![Cancel](../../Assets/Icons/Cross07.png "[Cancel]") (Cancel)   
    Click this button to cancel changing the period. All changes are rejected. The *Select period* window is closed.

- *FY*    
    Click the drop-down list to select the desired fiscal year. All available fiscal years are displayed in the list.

- *Month*  
    Click the drop-down list to select the desired month. All available months are displayed in the list.

- [OK]  
    Click this button to confirm the selected period. The *Select period* window is closed. The *Allocation table* window is displayed for the selected period.

#### Print allocation table

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 1 - Cost center > Button ALLOCATION TABLE > Button PRINT*

![Allocation table](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/AllocationTable02.png "[Allocation table]")

- *Month from - to*   
    Click the drop-down lists to select the desired month range. If you want to select only a single month, select the same month in both drop-down lists. The drop-down lists display all available months in the system. The following options are available:  
    - **0 - Balances carried forward**
    - **1 - 12 - (calendar month)**
    - **13 - 15 - Subsequent postings**
    - **99 - General month**

[comment]: <> (Monate stimmen mit Drop-down list oben nicht überein. 99 allg. Monat nicht dabei. 16-25 Nachtr. Buchungen auch nicht dabei. Evtl. FETA ticket)

- *Fiscal year*  
    Click the drop-down list to select the desired fiscal year. All available fiscal years are displayed.

- [CANCEL]  
    Click this button to cancel the print process. The *Print allocation table* window is closed.

- [PRINT]  
    Click this button to print the allocation table according to the selected settings. A print preview is displayed in the window.


### Select address

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 2 - Cost object > Button SEARCH*

![Select address](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/SelectAddress.png "[Select address]")

For a detailed description of this window and the corresponding functions, see [Customer/supplier list](./02a_DebtorsCreditors.md#customer/supplier-list).


### ProfitCenter  

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost 2 - Cost object > Button EDIT*

![Edit ProfitCenter](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/ProfitCenter.png "[Edit ProfitCenter]")

**ProfitCenter**

- ProfitCenter  
    Click the drop-down list to select a profit center. All available profit centers are displayed in the list. By default, the first profit center is preselected. The details to the selected profit center are displayed in the *Selected ProfitCenter* section and can be edited.

- [NEW...]  
    Click this button to create a profit center. The input fields in *Selected ProfitCenter* section are cleared.


**Selected ProfitCenter**

- *Number/name*  
    Enter or modify the profit center number in the first field. Only numbers greater than 0 are allowed. The number of digits is limited to 3.   
    Enter or modify the profit center name in the second field.

- *Description*  
    Enter or modify a description to the profit center.

- [DELETE]  
    Click this button to delete the selected profit center.

- [SAVE]  
    Click this button to save the new profit center or any changes made.
