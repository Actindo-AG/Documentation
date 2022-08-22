# Tax rates

*Taxes > Settings > Tab TAX RATES*

![Tax rates](../../Assets/Screenshots/Taxes/Settings/TaxRates/TaxRates.png "[Tax rates]")



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


- *Tax class*  
All configured tax classes. By default, the following tax zones are displayed:

  - **Standard rate**
  - **Reduced rate**  


- *Tax rates*  
Applicable tax rates expressed as percentage and its validity period.

- *Tax key*  
Applicable tax keys.

- *ID*  
Tax rate identification number. The ID number is automatically assigned by the system when the tax rate is created.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
Click this button to create a tax rate. The *Create tax rate* view is displayed, see [Create tax rate](#create-tax-rate).


## Create tax rate

*Taxes > Settings > Tab TAX RATES > Button Add*

![Create tax rate](../../Assets/Screenshots/Taxes/Settings/TaxRates/CreateTaxRate.png "[Create tax rate]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
Click this button to close the *Create tax rate* view and return to the list of tax rates. All changes are rejected.

- *Tax rate*  
Enter the applicable tax rate.

- *Tax key*  
Enter the applicable tax key.

- *Tax zone*  
Click the drop-down list and select the applicable tax zone. All available tax zones are displayed in the list.

- *Tax class*  
Click the drop-down list and select the applicable tax class. All available tax classes are displayed in the list.

- *Start date*   
Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to enter the applicable validity period start date.

- *End date*  
Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to enter the applicable validity period end date.

- [SAVE]  
Click this button to save the new tax rate, close the *Create tax rate* view and return to the list of tax rates.


## Edit tax rate


*Taxes > Settings > Tab TAX RATES > Select a tax rate*

![Edit tax rate](../../Assets/Screenshots/Taxes/Settings/TaxRates/EditTaxRate.png "[Edit tax rate]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
Click this button to close the *Edit tax rate* view and return to the list of tax rates. All changes are rejected.

- *Tax rate*  
Click the field to edit the tax rate.

- *Tax key*  
Click the field to edit the tax key. The tax keys can be checked, created, edited and deleted in the *Accounting* module, see [Manage the tax keys](../../RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

- *Tax zone*  
Click the drop-down list to select a different tax zone.

- *Tax class*  
Click the drop-down list to select a different tax class.

- *Start date*   
Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to edit the validity period start date.

- *End date*  
Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to edit the validity period end date.

- [SAVE]  
Click this button to save the changes, close the *Edit tax rate* view and return to the list of tax rates.
