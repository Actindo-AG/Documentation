[!!Accounting](RetailSuiteAccounting)  
[!!User Interface Tax rates](../UserInterface/01a_TaxRates.md)  
[!!Manage the tax classes](./02_ManageTaxClasses.md)  
[!!Manage the tax zones](./03_ManageTaxZones.md)  


# Manage the tax rates

Generally speaking, a tax rate is the percentage to which a product is taxed and depends on the product type (tax class) and the territory where it is to be taxed (tax zone). The *Taxes* module allows to configure different tax rates according to a combination of tax class and tax zone.

Tax rates can be created, edited and deleted to adapt the automatic taxation feature to the customer's specific and changing needs.


## Create a tax rate

Create a tax rate to cover a specific tax regime.

#### Prerequisites  

- An applicable tax class is created, see [Create a tax class](./02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone is created, see [Create a tax zone](./02_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab TAX RATES*

![Tax rates](../../Assets/Screenshots/Taxes/Settings/TaxRates/TaxRates.png "[Tax rates]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create tax rate* view is displayed.  

  ![Create a tax rate](../../Assets/Screenshots/Taxes/Settings/TaxRates/CreateTaxRate.png "[Create a tax rate]")

2. Enter the applicable tax rate in the *Tax rate* field. The tax rate is entered as a percentage. You can only enter numbers in the *Tax rate* field.

3. Enter the corresponding tax key in the *Tax key* field. The tax keys are managed in the *Accounting* module, see [Manage the tax keys](../../RetailSuiteAccounting/Integration/02_ManageTaxKeys.md).

  > [Info] Choosing the right tax key is essential for the automatic posting function in the *Accounting* module, as the *Taxes* module provides the *Order management* module with the configured tax key, which in turn is used by the *Order management* module to post the transaction in the *Accounting* module.

[comment]: <> (Check with FH if this is correct. It is possible to save the tax rate without tax key. How does it affect performance with Fakturierung, if no tax key or a wrong tax key, z.B. already in use with other tax rate/Steuersatz, is used? Does it affect bookings/posting in Accounting? Does the system give an error message? Or does it simply not work/book automatically the transaction?)

4. Click the *Tax zone* drop-down list and select the appropriate tax zone. All available tax zones are displayed in the list.

5. Click the *Tax class* drop-down list and select the appropriate tax class. All available tax classes are displayed in the list.

6. Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to enter the applicable validity period start date in the *Start date* field.

  > [Info] The validity period start date of a new tax rate cannot be earlier than the start date of an existing tax rate with same tax class and tax zone. Otherwise, an error message is displayed and the new tax rate is rejected.

7. If desired, click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to enter the applicable validity period end date in the *End date* field.

  > [Info] If no end date is entered, the tax rate continues to be valid for an unspecified period of time, that means, that no new tax class can be created with the same tax class and tax zone until an end date has been entered, or a new tax rate with the same tax class and tax zone is created with a start date after the start date of the existing tax rate.

[comment]: <> (Check nochmals!)


8. Click the [SAVE] button.  
The *Create tax rate* view is closed and the list of tax rates is displayed again.  

8. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.   
The new tax rate is displayed in the list of tax rates.


## Edit a tax rate

Edit a tax rate to adjust any of the configured parameters.

> [Info] Editing a tax rate has far-reaching consequences for the proper functioning of the system, as the *Taxes* module interacts with the *Order management* and *Accounting* modules. In case of doubt, contact our customer support.

#### Prerequisites

A tax rate is created, see [Create a tax rate](#create-a-tax-rate).

#### Procedures

*Taxes > Settings > Tab TAX RATES*

![Tax rates](../../Assets/Screenshots/Taxes/Settings/TaxRates/TaxRates.png "[Tax rates]")

1. Click the tax rate to be edited in the list of tax rates.  
The *Edit tax rate* view is displayed.

  ![Edit tax rate](../../Assets/Screenshots/Taxes/Settings/TaxRates/EditTaxRate.png "[Edit tax rate]")

2. Edit the desired data in the corresponding field(s).

  > [Info] Be aware that any changes made to an existing tax rate will overwrite the previously configured values.

3. Click the [SAVE] button.  
The *Edit tax rate* view closes automatically and the list of tax rates is displayed again.  

4. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.   
The edited tax rate is displayed in the list of tax rates.


## Delete a tax rate

Delete a tax rate that is no longer applicable.

> [Warning] Be aware that any deletion is permanent and cannot be undone.

#### Prerequisites

A tax rate is created, see [Create a tax rate](#create-a-tax-rate).

#### Procedures

*Taxes > Settings > Tab TAX RATES*

![Tax rates](../../Assets/Screenshots/Taxes/Settings/TaxRates/TaxRates.png "[Tax rates]")

1. Select the checkbox of the tax rate to be deleted.  
The editing toolbar is displayed.

  > [Warning] Be aware that the existing tax rate will be deleted permanently.

2. Click the [DELETE] button in the upper right corner.  
The selected tax rate has been deleted.

[comment]: <> (16.08.22 - DELETE Button not working. Bug reported.)
