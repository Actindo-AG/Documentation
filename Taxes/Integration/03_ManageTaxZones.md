[!!Accounting](RetailSuiteAccounting)  
[!!Fakturierung](RetailSuiteFaktBase)  
[!!User Interface Tax zones](../UserInterface/01d_TaxZones.md)  
[!!Manage the tax rates](./01_ManageTaxRates.md)  
[!!Manage the tax classes](./02_ManageTaxClasses.md)  
[!!Manage the decision matrix](../Operation/01_ManageDecisionMatrix.md)  


# Manage the tax zones

Tax zones are essential to determine where a specific tax rate is to be applied. The applicable tax zone depends on several factors, such as the country where the selling company is based, the country where the product is shipped from, and the country where the product is shipped to.

The default configuration includes three tax zones:

  - Domestic, that is, where the selling company is based

  - EU (European Union)  

  - Third country, that is, any territory other than the two specified above  

Next to the configured tax zone, a VAT ID (value-added-tax identification number) can be added. The VAT ID number is an identifier used by companies operating in the European Union for value-added-tax purposes. VAT ID numbers can be verified at the EU's [VIES](https://ec.europa.eu/taxation_customs/vies/) (VAT Information Exchange System) official website.

Tax zones can be created, edited and deleted to configure the automatic taxation feature according to the customer's business needs.


## Create a tax zone

Create a tax zone to define a territory where a specific tax rate is to be applied.

#### Prerequisites  

No prerequisites to fulfill.

#### Procedures

*Taxes > Settings > Tab TAX ZONES*

![Tax zones](../../Assets/Screenshots/Taxes/Settings/TaxZones/TaxZones.png "[Tax zones]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line with two fields is displayed.  

2. Click the entry field in the *Tax zones* column.  
  The field becomes active and the cursor is displayed.

3. Enter the desired tax zone name in the field.  

4. Click the entry field in the *VAT ID* column.  
  The field becomes active and the cursor is displayed.

5. Enter the relevant VAT ID number in the field.  

6. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

7. Refresh the *Tax* module for the *TAX RATES* tab to display the changes made. To do so, click the F5 key.  
The newly created tax zone is displayed in the *Tax zone* drop-down list in the *TAX RATES* tab.

[comment]: <> (By creating a tax zone, SAVE shows the confirmation message. For changes to be displayed in the drop-down list in TAX RATES, the whole module must be refreshed with F5. Refresh icon does not work in this case, i.e. no changes in the drop-down list Tax zone are displayed. Stand 08.08.22)


## Edit a tax zone

Edit a tax zone name or its configured VAT ID number if necessary.

#### Prerequisites

A tax zone is created, see [Create a tax zone](#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab TAX ZONES*

![Tax zones](../../Assets/Screenshots/Taxes/Settings/TaxZones/TaxZones.png "[Tax zones]")

1. Click the entry field to be edited.  
  The field becomes active and the cursor is displayed.

2. Edit the tax zone name and/or its VAT ID number as necessary.

3. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

4. Refresh the *Tax* module for the *TAX RATES* tab to display the changes made. To do so, click the F5 key.  
The edited tax zone is displayed in the *Tax zone* drop-down list in the *TAX RATES* tab.

[comment]: <> (By editing a tax zone, SAVE shows the confirmation message. For changes to be displayed in the drop-down list in TAX RATES, the whole module must be refreshed with F5. Refresh icon does not work in this case, i.e. no changes in the drop-down list Tax zone are displayed. Stand 08.08.22)


## Delete a tax zone

Delete a tax zone that is no longer applicable.  

> [Warning] Be aware that any deletion is permanent and cannot be undone.

#### Prerequisites

A tax zone is created, see [Create a tax zone](#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab TAX ZONES*

![Tax zones](../../Assets/Screenshots/Taxes/Settings/TaxZones/TaxZones.png "[Tax zones]")

1. Select the tax zone you want to delete.

  > [Warning] Be aware that the deletion may have far-reaching consequences for the proper functioning of the system, as the *Taxes* module interacts with the *Invoicing* and *Accounting* modules. In case of doubt, contact our customer support.

2. Click the ![Delete](../../Assets/Icons/Trash08.png "[Delete]") (Delete) button next to the tax zone to be deleted.  
  The tax zone is deleted from the list.

3. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

4. Refresh the *Tax* module for the *TAX RATES* tab to display the changes made. To do so, click the F5 key.  
The deleted tax zone is no longer displayed in the *Tax zone* drop-down list in the *TAX RATES* tab.

[comment]: <> (By deleting a tax zone, SAVE shows the confirmation message. For changes to be displayed in the drop-down list in TAX RATES, the whole module must be refreshed with F5. Refresh icon does not work in this case, i.e. no changes in the drop-down list Tax zone are displayed. Stand 08.08.22)
