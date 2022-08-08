[!!Accounting](RetailSuiteAccounting)  
[!!Fakturierung](RetailSuiteFaktBase)  
[!!User Interface Tax classes](../UserInterface/01c_TaxClasses.md)  
[!!Manage the tax rates](./01_ManageTaxRates.md)  



# Manage the tax classes

Each product or group of products is assigned a tax class. The tax class is determined by the competent tax authorities of the territory where the product or group of products is to be taxed. Therefore it usually differs from territory to territory.

There are two main tax classes in most territories: the standard and the reduced tax rate class. However, there can also be special taxes, such as super-reduced or zero taxes. Tax classes can be created, edited and deleted if necessary.


## Create a tax class

Create a tax class to be assigned to a product or group of products.

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

5. Refresh the *Tax* module for the *TAX RATES* tab to display the changes made. To do so, click the F5 key.  
The newly created tax class is displayed in the *Tax class* drop-down list in the *TAX RATES* tab.

[comment]: <> (By creating a tax class, SAVE does not show the confirmation message. For changes to be displayed in the drop-down list in TAX RATES, the whole module must be refreshed with F5. Refresh icon does not work in this case, i.e. no changes in the drop-down list Tax class are displayed. Stand 08.08.22)


## Edit a tax class

Edit a tax class to modify its name.

#### Prerequisites

A tax class is created, see [Create a tax class](#create-a-tax-class).

#### Procedures

*Taxes > Settings > Tab TAX CLASSES*

![Tax classes](../../Assets/Screenshots/Taxes/Settings/TaxClasses/TaxClasses.png "[Tax classes]")

1. Click the entry field to be edited.  
  The field becomes active and the cursor is displayed.

2. Edit the tax class name as necessary.

3. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

4. Refresh the *Tax* module for the *TAX RATES* tab to display the changes made. To do so, click the F5 key.
The edited tax class is displayed in the *Tax class* drop-down list in the *TAX RATES* tab.

[comment]: <> (By editing a tax class, SAVE does show the confirmation message. For changes to be displayed in the drop-down list in TAX RATES, the whole module must be refreshed with F5. Refresh icon does not work in this case, i.e. no changes in the drop-down list Tax class are displayed. Stand 08.08.22)


## Delete a tax class

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
  A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

4. Refresh the *Tax* module for the *TAX RATES* tab to display the changes made. To do so, click the F5 key.  
The deleted tax class is no longer displayed in the *Tax class* drop-down list in the *TAX RATES* tab.

[comment]: <> (By deleting a tax class, SAVE does show the confirmation message. For changes to be displayed in the drop-down list in TAX RATES, the whole module must be refreshed with F5. Refresh icon does not work in this case, i.e. no changes in the drop-down list Tax class are displayed. Stand 08.08.22)
