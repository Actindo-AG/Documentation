# Tax rates

*Taxes > Settings > Tab TAX RATES*

![Tax rates](../../Assets/Screenshots/Taxes/Settings/TaxRates/TaxRates.png "[Tax rates]")

The *TAX RATES* tab displays a list of all available tax rates. The default configuration covers all standard cases for a company based in Germany delivering within the European Union, without exceeding any tax delivery threshold and paying taxes on sales revenue in Germany.

[comment]: <> (Bestätigen mit FH)

Tax rates can be created, edited and deleted to adapt the system to the customer's needs, also dealing with special tax regimes within or outside the European Union. For detailed information about creating, editing or deleting tax rates, see [Manage the tax rates](../Integration/01_ManageTaxRates.md).


**List**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
 Click this button to update the list of tax rates.
- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all tax rates in the list are selected.

  [comment]: <> (Alle Tax rates ausgewählt, aber es ist nicht möglich, etwas zu machen, i.e. keine Editing toolbar angezeigt.)

- [EDIT]   
  Click this button to edit the selected tax rate. This button is only displayed, when the checkbox of a tax rate is selected. Alternatively, you can click directly a row in the list to edit a tax rate. The *Edit tax rate* view is displayed, see [Edit tax rate](#edit-tax-rate).   
  For detailed information, see [Edit a tax rate](../Integration/01_ManageTaxRates.md#edit-a-tax-rate).

[comment]: <> (Ändern in der Zukunft? In neuer UI, Edit-Fenster werden einfach den Namen des ausgewählten Tax rates/Produktes, usw.; Create-Fenster werden "New ..." heißen. Besprochen in UX-Docu Meeting 08.08.22)

- [DELETE]  
Click this button to delete the selected tax rate. This button is only displayed, when the checkbox of a tax rate is selected.   
For detailed information, see [Delete a tax rate](../Integration/01_ManageTaxRates.md#delete-a-tax-rate).


The list displays all available tax rates. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Tax zone*  
All configured tax zones. By default, the following tax zones are displayed:

  - **Domestic**
  - **EU**
  - **Third country**

  Tax zones can be created, edited and deleted, see [Create a tax zone](../Integration/03_ManageTaxZones.md#create-a-tax-zone).

- *Tax class*  
All configured tax classes. By default, the following tax zones are displayed:

  - **Standard rate**
  - **Reduced rate**  

  Tax zones can be created, edited and deleted, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-zone).

- *Tax rates*  
Applicable tax rates expressed as percentage and its validity period. Tax rates can be edited, see [Edit a tax rate](../Integration/01_ManageTaxRates.md#edit-a-tax-rate).

- *Tax key*  
Applicable tax keys. The tax keys can be checked, created, edited and deleted in the *Accounting* module, see [Manage the tax keys](../../RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
Click this button to create a tax rate. The *Create tax rate* view is displayed, see [Create tax rate](#create-tax-rate).

- *Rows per page*   
Click the drop-down list to select the number of rows to be displayed per page.

- *[x-x] of [x]*  
This text displays the number of tax rates currently displayed and the total number of tax rates in the list. This text is read-only.

- ![First page](../../Assets/Icons/FirstPage03.png "[First page]") - ![Last page](../../Assets/Icons/LastPage03.png "[Last page]") (First page) - (Last page)  
![Previous page](../../Assets/Icons/PreviousPage02.png "[Previous page]") - ![Next page](../../Assets/Icons/NextPage02.png "[Next page]") (Previous page) - (Next page)  
Click these buttons to navigate the tax rates list.

[comment]: <> (Page navigation items necessary?)


## Create tax rate

*Taxes > Settings > Tab TAX RATES > Button Add*

![Create tax rate](../../Assets/Screenshots/Taxes/Settings/TaxRates/CreateTaxRate.png "[Create tax rate]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
Click this button to close the *Create tax rate* view and return to the tax rates list. All changes are rejected.

- *Tax rate*  
Enter the applicable tax rate.

- *Tax key*  
Enter the applicable tax key. The tax keys can be checked, created, edited and deleted in the *Accounting* module, see [Manage the tax keys](../../RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

- *Tax zone*  
Click the drop-down list and select the applicable tax zone.

- *Tax class*  
Click the drop-down list and select the applicable tax class.

- *Start date*   
Enter the start date of the tax rate validity period. You can enter the date with the keyboard or clicking the ![Add](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button. The date format must be YYYY.MM.DD. hh:mm:ss.

- *End date*  
Enter the end date of the tax rate validity period. You can enter the date with the keyboard or clicking the ![Add](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button. The date format must be YYYY.MM.DD. hh:mm:ss.

- [SAVE]  
Click this button to save the new tax rate, close the *Create tax rate* view and return to the tax rates list.


## Edit tax rate

[comment]: <> (Evtl. Create/edit tax rate?)

*Taxes > Settings > Tab TAX RATES > Select a tax rate*

![Edit tax rate](../../Assets/Screenshots/Taxes/Settings/TaxRates/EditTaxRate.png "[Edit tax rate]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
Click this button to close the *Edit tax rate* view and return to the tax rates list. All changes are rejected.

- *Tax rate*  
Click the field to edit the tax rate.

- *Tax key*  
Click the field to edit the tax key. The tax keys can be checked, created, edited and deleted in the *Accounting* module, see [Manage the tax keys](../../RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

- *Tax zone*  
Click the drop-down list to select a different tax zone.

- *Tax class*  
Click the drop-down list to select a different tax class.

- *Start date*   
Click the field to edit the start date of the tax rate validity period. You can enter the date with the keyboard or clicking the ![Add](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button. The date format must be YYYY.MM.DD. hh:mm:ss.

- *End date*  
Click the field to edit the end date of the tax rate validity period. You can enter the date with the keyboard or clicking the ![Add](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button. The date format must be YYYY.MM.DD. hh:mm:ss.

- [SAVE]  
Click this button to save the changes, close the *Edit tax rate* view and return to the tax rates list.
