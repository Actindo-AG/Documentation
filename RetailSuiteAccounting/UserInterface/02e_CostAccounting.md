# Cost accounting

*Accounting > Settings > Tab COST ACCOUNTING*

![Cost accounting - not defined](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostAccountingNo.png "[Cost accounting - not defined]")

> [Info] If no cost center has been created in the selected accounting period yet, the notice "No cost centers defined" is displayed when clicking the *COST ACCOUNTING* tab.


- *Cost accounting*  
Click the corresponding drop-down list to select the relevant accounting period (fiscal year and month) and the cost center/unit:

  - (Fiscal year drop-down list)  
  Click the drop-down list to select the relevant fiscal year. The fiscal years already configured in the system are displayed in the drop-down list.  

  - (Month drop-down list)  
  Click the drop-down list to select the relevant month. The following options are available:  

    - **0 - Balances carried forward**
    - **1 - 12 - (months)**
    - **13 - 15 - Subsequent postings**  

  - (Cost accounting drop-down list)  
  Click the drop-down list to select the desired option. The following options are available:  

    - **Cost 1 - Cost center**  
    Select this option to display the available cost centers in the selected accounting period or to create a new one.
    - **Cost 2 - Cost unit**
    Select this option to display the available cost units in the selected accounting period or to create a new one.  

    Depending on the option selected in the cost accounting drop-down list (**Cost 1 - Cost center** or **Cost 2 - Cost unit**), the input fields and the information displayed vary.

[comment]: <> (Monat drop-down list: es fehlt 16-19 Abschlussbuchungen und 99 Allgemeiner Monat?)


## Cost center

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost1 - Cost center*

![Cost center](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostAccounting01.png "[Cost center]")

The cost centers available in the selected accounting period, if any, are displayed in a column view. All information displayed in columns is read-only.

- *Cost.*  
Cost center number.

- *Description*  
Cost center description.

- *Inactive*  
If the cost center has been set to inactive, the word *Inactive* is displayed. Otherwise, the column is empty.

- *Active from*  
Validity start date.

[comment]: <> (Allgemeine Info fehlt! Wie kann man aktivieren? Wann kommt das Datum vor?)


The input fields allow to enter or modify cost center details.

- ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *Active/Inactive* (radio button)  
Click the corresponding radio button to select the appropriate option. The *Active* radio button is selected by default.

- *Cost center*  
Enter the cost center number. It is possible to enter up to 4 digits.

- *Description*  
Enter a short description for the cost center.

- *Text*  
Enter a longer text description for the cost center, if desired.

- *Allocation to cost unit*  
It is possible to allocate costs from different cost centers to individual cost units. To do so, click the [ALLOCATION TABLE] button.

- [ALLOCATION TABLE]  
Click this button to display the *Allocation table* window, see [Allocation table](#allocation-table).


- [SAVE & NEW]  
Click this button to save a newly created cost center.  

- [SAVE]  
Click this button to save any changes made to an existing cost center.  

  > [Info] Be aware that the saved changes will overwrite the cost center existing details. To prevent this, make sure that the input fields are empty by clicking the [CLEAR] button. The [SAVE & NEW] button becomes then active.

- [DELETE]  
Click this button to delete a selected cost center.

- [CLEAR]  
Click this button to clear all input fields. The [SAVE & NEW] button becomes active.

- [PRINT]  
Click this button to print the cost center/unit. The *Print cost center/unit* window is displayed.

[comment]: <> (Eigentlich heißt das Fenster Cost center/unit, aber ich habe zu Print cost center/unit umbenannt hier.)

[comment]: <> (Wir haben keine Prozedur in Integration über "Create/Edit/Delete cost center/cost unit". Hinzufügen! RS mit FH)


## Cost unit

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost2 - Cost unit*

![Cost unit](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostAccounting02.png "[Cost unit]")


The cost units available in the selected accounting period, if any, are displayed in a column view. All information displayed in columns is read-only.

- *Cost.*  
Cost unit number.

- *Description*  
Cost unit description.

- *Inactive*  
If the cost unit has been set to inactive, the word *Inactive* is displayed. Otherwise, the column is empty.

- *Active from*  
Validity start date.

[comment]: <> (Allgemeine Info fehlt! Wie kann man aktivieren? Wann kommt das Datum vor?)

- *ProfitCenter*  
Assigned ProfitCenter.


The input fields allow to enter or modify cost unit details.

- ![Radio button](../../Assets/Icons/RadioButton02.png "[Radio button]") *Active/Inactive* (radio button)  
Click the corresponding radio button to select the appropriate option. The *Active* radio button is selected by default.

- *Cost unit*  
Enter the cost unit number. It is possible to enter up to 5 digits.

- *Description*  
Enter a short description for the cost unit.

- *Text*  
Enter a longer text description for the cost unit, if desired.

- *Debtor*  
Enter the debtor or customer number, if necessary. Alternatively, click the [SEARCH] button to search for a debtor or customer.

- [SEARCH]  
Click this button to display the *Select address* window, see [Select address](#select-address).

- *ProfitCenter*  
Click the drop-down list to select the appropriate ProfitCenter. All available ProfiCenters are displayed in the list. If no ProfitCenter has been created yet, **0 - No group** is displayed.

[comment]: <> (Unsicher, check mit FH!)

- [EDIT]  
Click this button to edit or add a ProfitCenter. The *ProfitCenter* window is displayed, see [ProfitCenter](#profitcenter).


- [SAVE & NEW]  
Click this button to save a newly created cost unit.  

- [SAVE]  
Click this button to save any changes made to an existing cost unit.  

  > [Info] Be aware that the saved changes will overwrite the cost unit existing details. To prevent this, make sure that the input fields are empty by clicking the [CLEAR] button. The [SAVE & NEW] button becomes then active.

- [DELETE]  
Click this button to delete a selected cost unit.

- [CLEAR]  
Click this button to clear all input fields. The [SAVE & NEW] button becomes active.

- [PRINT]  
Click this button to print the cost center/unit. The *Print cost center/unit* window is displayed.

[comment]: <> (Eigentlich heißt das Fenster Cost center/unit, aber ich habe zu Print cost center/unit umbenannt hier.)


## Print cost center/unit

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost1 - Cost center > Button PRINT*
*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost2 - Cost unit > Button PRINT*

![Print cost center/unit](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/CostCenterUnit.png "[Print cost center/unit]")


- *Cost center/unit*  
Click the drop-down list to select whether the cost center(s) or cost unit(s) are to be printed.

- *Active/inactive*  
Click the checkbox to select one of the options, or both, to be printed.

- *Numbers from-to*  
Enter a cost center/unit number range to be printed.

- *Month*  
Click the drop-down list to select the desired month to be printed.

- *Fiscal year*  
Click the drop-down list to select the desired fiscal year to be printed.


- [CANCEL]  
Click this button to cancel the process. The window is closed.

- [PRINT]  
Click this button to print out the cost center/unit with the selected settings.


### Allocation table

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost1 - Cost center > Button ALLOCATION TABLE*

![Allocation table](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/AllocationTable01.png "[Allocation table]")

- *Select ProfitCenter*  
Click the drop-down list to select a specific ProfitCenter. You can also select **All ProfitCenters** to include them all or **0 - No group** to include none.

- [UPDATE]  
Click this button to update the table after making any changes.

  > [Info] Bear in mind that the changes must be saved first clicking the [SAVE] button at the bottom. Otherwise, the changes will be rejected.

- [CHANGE PERIOD]  
Click this button to change the period. The *Select period* window is displayed, see [Select period](#select-period).

- [EXCEL]  
Click this button to display the *EXCEL* context menu. The following option is available:  

  - *Export current page*  
  Click this option to export the allocation table currently displayed. The allocation table is exported in Excel format and saved by default in the Downloads folder in your computer.

  - *Export all*  
  Click this option to export all available allocation tables. The allocation tables are exported in Excel format and saved by default in the Downloads folder in your computer.

[comment]: <> (Check! One file, several files, one excel with several tabs?)

The allocation table displays the distribution of costs among cost centers and units. The information displayed is read-only.

- *Cost center*  
The available cost center(s) are displayed in this column.

- (Cost units)  
The available cost unit(s) are displayed in a row. Double click in the corresponding table cell to activate the input field. The following options are available:

  - If the *Allocation* column is set to *Percentage*, enter a percentage value.
  - If the *Allocation* column is set to *Formula*, click the drop-down list to select **Active/inactive**. The basic calculating operations (+, -, *, /) are permitted.


- (Sigma sign %)  
The cell content changes automatically depending on the allocation method and percentage values entered. The individual percentages entered must equal 100 %. That means that all costs are allocated to the individual cost units. The cell turns then green. Otherwise, an error message is displayed when trying to save the table.

[comment]: <> (Check mit FH! Generell mehr Info gebraucht für dieses Kapitel. Evtl. Prozedur in Integration.)

- *Allocation*   
Doble click the corresponding table cell to activate the drop-down list. Click the drop-down list to select the allocation method. The following options are available:  

  - **Percentage**  
  Select this option to allocate costs based on individual percentages per unit.
  - **Formula**  
  Select this option to allocate costs based on a formula.


- *Formula*  
Double click the corresponding table cell to enter an Excel formula.

[comment]: <> (Unsicher, wie die Formel funktioniert! Check! The basic calculating operations +, -, *, / are permitted. -> stimmt so?)

- [CLOSE]  
Click this button to close the window.

- [PRINT]  
Click this button to print the allocation table. The *Allocation table* window to select the month(s) and fiscal year to be printed is displayed, see [Print allocation table](#print-allocation-table).

- [SAVE]  
Click this button to save the allocation table after making any changes. A pop-up window is displayed while the changes are being saved.


### Select address

[comment]: <> (Fenster/Unterkapitel umbenennen zu Search debtor?)

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost2 - Cost unit > Button SEARCH*

![Select address](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/SelectAddress.png "[Select address]")

> [Info] The *Customer/supplier list* tab is also available in the *DEBTORS/CREDITORS* tab, see [Customer/supplier list](./02a_DebtorsCreditors.md#customer-supplier-list).

- [EXCEL]  
Click this button to display the *EXCEL* context menu. The following options are available:  

  - *Export current page*  
  Click this option to export the customer/supplier list page currently displayed. The customer/supplier list is exported in Excel format and saved by default in the *Downloads* folder in your computer.

  - *Export all*  
  Click this option to export all customer/supplier list pages. The customer/supplier list is exported in Excel format and saved by default in the *Downloads* folder in your computer.


- [QUICK SEARCH]  
Click this button to display the *QUICK SEARCH* context menu. All search criteria are selected by default through a marked checkbox. Deselect any search criteria as necessary. The following search criteria are available:

  - *No.*  
  - *Short name*
  - *Company*  
  - *Forename*
  - *Surname*
  - *Address*
  - *Address 2*
  - *ZIP*
  - *Location*
  - *Country*
  - *Content*
  - *Currency*
  - *Comments*
  - *Phone*
  - *Phone 2*
  - *Cell phone*
  - *Fax*
  - *Email*
  - *VAT ID*
  - *Type of customer*
  - *Customer number*


  [comment]: <> (in the system as No -> add point)
  [comment]: <> (in the system: Firma -> localise)
  [comment]: <> (in the system: First name)
  [comment]: <> (in the system: Name)
  [comment]: <> (in the system: City)  

- [Search bar]  
  Click the search bar to enter the search text (letters or numbers).

- ![Delete](../../Assets/Icons/Cross02.png "[Delete]") (Delete)  
  Click this button to delete the search text and to clear the search results.

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)  
  Click this button to start the search. The search can also be started by pressing ENTER.

- (x) [ACTIVE FILTERS]  
Click this button to display the context menu.

  - *ACTIVE* (checkbox)  
  Mark this checkbox to activate the search criteria.

  - *FILTER BY*  
  The following filter values are available:
    - *Price group*  

  - *FILTER CRITERION*  
  Click the drop-down list to select the appropriate filter criterion. The created price groups are displayed.

  > [Info] Price groups can be created in the *Settings* menu entry of the *Material management* and the *Order management* module. A customer can be assigned a specific price group in the *Order management* sub-tab of the *DEBTORS/CREDITORS* tab, see [Invoicing](./02a_DebtorsCreditors.md#invoicing-1).

  [comment]: <> (Other "Filter by" options available depending on settings?)

- [CANCEL]  
 Click this button to cancel your selection.

- [APPLY]  
 Click this button to apply the search criteria and values.


All customer/supplier details are displayed in a column view. Depending on the settings, the displayed columns may vary. To add or delete columns, click the ![Points](../../Assets/Icons/Points02.png "[Points]") (Points) icon to display the context menu. Then, hover the mouse over the ![Columns](../../Assets/Icons/Columns02.png "[Columns]") (Columns) menu entry to display all available options. Select or deselect the columns as desired.

- *No.*  
Customer/supplier number. Customer numbers range from 10000 to 69999 and supplier numbers, from 70000 to 99999.

- *Short name*  
Short name given to the customer/supplier.

- *Company*  
Company name.

- *Forename*  
Customer/supplier first name.

- *Surname*  
Customer/supplier last name.

- *Address*  
Customer/supplier address.

- *Address 2*  
Complimentary address information.

- *ZIP*  
Customer/supplier zip code.

- *Location*   
Customer/supplier city or town.

- *Country*  
Customer/supplier country.

- *Content*  
Files or links added to the customer/supplier information.  

- *Currency*  
Base currency used by customer/supplier.

- *Comments*  
Comments added on the customer/supplier information.

- *Phone*  
Customer/supplier contact phone number.

- *Phone 2*  
Customer/supplier second contact phone number.    

- *Cell phone*  
Customer/supplier cell phone number.

- *Fax*  
Customer/supplier fax number.

- *Email*  
Customer/supplier email address.

- *VAT ID*  
Customer/supplier VAT identification number, if applicable.

- *Type of customer*  
Type of customer/supplier as defined by the user.

- *Customer number*  
Reference customer/supplier number as defined by the user.


By right-clicking on a row, a context menu is displayed containing the following options:

- *Show documents of the customer/supplier*  
Click this option to access the customer/supplier order Overview in the *Order management* module
- *Show articles of supplier*  
Click this option to access the supplier product list in the *Material management* module.

[comment]: <> (Add link when available)


- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
 Click this button to update the receipt list.

- [RESET]  
 Click this button to reset the receipt list view.


### ProfitCenter  

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost2 - Cost unit > Button EDIT*

![Edit ProfitCenter](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/ProfitCenter.png "[Edit ProfitCenter]")

**ProfitCenter**

- (ProfitCenter drop-down list)  
Click the drop-down list to edit an existing ProfitCenter. The ProfitCenter details are displayed in the *Selected ProfitCenter* section.

- [NEW]  
Click this button to add a ProfitCenter. The input fields in *Selected ProfitCenter* section are cleared.

**Selected ProfitCenter**
- *Number/name*  
Enter or modify the ProfitCenter number and/or name.

- *Description*  
Enter or modify the ProfitCenter description.

- [DELETE]  
Click this button to delete the selected ProfitCenter.

- [SAVE]  
Click this button to save the newly created ProfitCenter or any other changes made.


####  Select period

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost1 - Cost center > Button ALLOCATION TABLE > Button CHANGE PERIOD*

![Select period](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/SelectPeriod.png "[Select period]")

- *FY*    
Click the drop-down list to select the desired fiscal year.

- *Month*  
Click the drop-down list to select the desired month.  

- [OK]  
Click this button to confirm the selected settings.


#### Print allocation table

*Accounting > Settings > Tab COST ACCOUNTING > Drop-down option Cost1 - Cost center > Button ALLOCATION TABLE > Button PRINT*

![Allocation table](../../Assets/Screenshots/RetailSuiteAccounting/Settings/CostAccounting/AllocationTable02.png "[Allocation table]")

- *Month from - to*  
Click the drop-down lists to select the desired month range.

- *Fiscal year*  
Click the drop-down list to select the desired fiscal year.

- [CANCEL]  
Click this button to cancel the process and close the window.

- [PRINT]  
Click this button to generate a file in a printable format. A table allocation preview is displayed in a new window.
