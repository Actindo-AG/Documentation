[!!Accounting](RetailSuiteAccounting)  
[!!Fakturierung](RetailSuiteFaktBase)  
[!!User Interface tax rates](../UserInterface/XX_TaxClasses.md)  
[!!Manage the tax rates](./01_ManageTaxRates.md)  
  


# Manage the tax classes

Each product or group of products is assigned a tax class. The tax class is determined by the competent tax authorities of the territory where the product or group of products is to be taxed. Therefore it usually differs from territory to territory.

There are two main tax classes in most territories: the standard and the reduced tax rate class. However, there can also be special taxes, such as super-reduced or zero taxes.

The *TAX CLASSES* tab allows to create any number of tax classes to be assigned to a product or group of products. Once a tax class is created in this tab, it becomes available to be selected in the *Tax class* drop-down list when creating or editing a tax rate in the *TAX RATES* tab. For detailed information about creating or editing a tax rate, see [Manage the tax rates](./01_ManageTaxRates.md).


## Create a tax class

Create a new tax class to be assigned to a product or group of products.

#### Prerequisites  

No prerequisites to fulfill.

#### Procedures

*Taxes > Settings > Tab TAX CLASSES*

![Tax classes](../../Assets/Screenshots/Taxes/Settings/TaxClasses/TaxClasses.png "[Tax classes]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line is displayed.  

2. Click the entry field to be edited.  
  The field becomes active and the cursor is displayed.

3. Enter the desired tax class name in the entry line.  

4. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved. The newly created tax class is displayed in the *Tax class* drop-down list in the *TAX RATES* tab.

  > [Info] It may be necessary to refresh the list view to display the changes made. To do so, click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.


## Edit a tax rate

Edit a tax class name if necessary.

#### Prerequisites

A tax class is created, see [Create a tax rate](#create-a-tax-class).

#### Procedures

*Taxes > Settings > Tab TAX CLASSES*

![Tax classes](../../Assets/Screenshots/Taxes/Settings/TaxClasses/TaxClasses.png "[Tax classes]")

1. Click the entry field to be edited.  
  The field becomes active and the cursor is displayed.

2. Edit the tax class name as necessary.

3. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved. The edited tax class is displayed in the *Tax class* drop-down list in the *TAX RATES* tab.

  > [Info] It may be necessary to refresh the list view to display the changes made. To do so, click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.


## Delete a tax rate

Delete a tax class that is no longer applicable.  

> [Warning] Be aware that any deletion is permanent and cannot be undone.

#### Prerequisites

A tax class is created, see [Create a tax class](#create-a-tax-class).

#### Procedures

*Taxes > Settings > Tab TAX CLASSES*

![Tax classes](../../Assets/Screenshots/Taxes/Settings/TaxClasses/TaxClasses.png "[Tax classes]")

1. Select the tax class you want to delete.

  > [Warning] Be aware that the deletion may have far-reaching consequences for the proper functioning of the system, as the *Taxes* module interacts with the *Invoicing* and *Accounting* modules. In case of doubt, contact our customer support.

2. Click the ![Delete](../../Assets/Icons/Trash08.png "[Delete]") (Delete) button next to the tax class to be deleted.  
  The tax class is deleted from the list.

3. Click the [SAVE] button.  
  The changes are saved. The deleted tax class will no longer be displayed in the *Tax class* drop-down list in the *TAX RATES* tab.

  > [Info] It may be necessary to refresh the list view to display the changes made. To do so, click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.

[comment]: <> (SAVE necessary to save changes, that is, for changes to be displayed in the drop-down list in TAX RATES? RS FH/JS. At the moment -01.08.22.- not working.)
