[!!Accounting](RetailSuiteAccounting)  
[!!Fakturierung](RetailSuiteFaktBase)  
[!!User Interface Tax zones](../UserInterface/XX_DecisionMatrix.md)  
[!!Manage the tax rates](../Integration/01_ManageTaxRates.md)  
[!!Manage the tax classes](../Integration/01_ManageTaxClasses.md)  
[!!Manage the tax zones](../Integration/01_ManageTaxZones.md)  


# Manage the decision matrix

The decision tax matrix is designed to help the system decide which tax zone, and therefore which tax rate, is to be applied to an order. The decision matrix consists of a list of decision-making criteria based on the information provided by the *Invoicing* module.

Taking into account the order confirmation and the delivery note, the *Invoicing* module provides the *Taxes* module with following details:

- Country of origin
- Ship-to country
- Ship-to postcode
- VAT ID

Using this information, the decision matrix is able to determine the tax zone. Once the tax zone has been determined, the *Taxes* module can provide the *Invoicing* module with this information, as well as with the applicable tax key and tax rate.  

The order of the decision-making criteria is essential, as the system goes through the criteria in the order they are listed, starting from the top, and stops checking them as soon as a matching criterion is found. This means, that the criteria must be organized from specific to general to cover all possible relevant cases.


## Create an entry

Create an entry to define a new tax zone.

#### Prerequisites  

- An applicable tax class is created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone is created, see [Create a tax zone](../Integration/02_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line is displayed.

2. Click the *VAT ID* drop-down list and select the appropriate option. The following options are available:

  - **Yes**: The end customer is a company and, therefore, has a VAT ID number (business-to-business transaction).
  - **No**: The end customer is a private individual and, therefore, has no VAT ID number (business-to-customer transaction).
  - **Any**: Wildcard; any value is accepted.


3. Click the *Country of origin* drop-down list(s) and select the appropriate option(s). Use the left drop-down list to select a group of countries and the right one to select an individual country.

  > {Info] The current version only provides the option **EU - European Union** as a group of countries. When a group of countries is selected, the right drop-down list is grayed out.

4. Click the *Ship-to country* drop-down list(s) and select the appropriate option(s). Use the left drop-down list to select a group of countries and the right one to select an individual country.

  > {Info] The current version only provides the option **EU - European Union** as a group of countries. When a group of countries is selected, the right drop-down list is grayed out.

5. Click the *Ship-to postcode* drop-down list and select the appropriate option. The following options are available:

  - **Range**: Enter a postcode range, for example, 27498-27498 to limit the criterion to a specific target area.
  - **Regex**: Use regular expressions to specify postcodes containing alphanumeric characters, for example /^BT.*/. There are many regular expressions testing tools available free of charge in the Internet, such as [Regex101](https://regex101.com/).

For detailed information, see [Define tax exceptions on ZIP code level](#define-tax-exceptions-on-ZIP-code-level).

6. Click the *Net value of goods smaller than* drop-down list and select the applicable currency. If necessary, specify an amount using the keyboard or the increase and decrease arrows on the right.

7. Click the *Tax zone* drop-down list to select a different tax zone if necessary.

8. Click the [SAVE] button.  
A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

[comment]: <> (Vermutetes Verhalten. SAVE not working -> Method not found message. 02.08.22)


## Edit an entry

Edit an entry to modify any of the configured parameters or to change its position in the decision matrix.

#### Prerequisites  

An entry in the decision matrix is created, see [Create an entry](#create-an-entry).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the drop-down list(s) to be edited.  
The selected field becomes active and the corresponding drop-down list is displayed.

2. Select a different option from the drop-down list.  
The newly selected option is displayed in the field.

3. If an option from a drop-down list is already selected, click the selected option again to deselect it.  
The option **Any** (wildcard) is displayed in the field.

4. Click the *Ship-to postcode* right field to modify the range or the regular expression if necessary. Use the keyboard to enter a different value.

5. Click the *Net value of goods smaller than* right field to modify the net value amount entered. You can use the keyboard or the increase and decrease arrows.

6. Click the *Tax zone* drop-down list to select a different applicable tax zone.

7. To modify the entry position in the matrix, click the  

8. Click the [SAVE] button.  
A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

[comment]: <> (Vermutetes Verhalten. SAVE not working -> Method not found message. 02.08.22)


## Delete an entry

Delete a entry that is no longer applicable.  

> [Warning] Be aware that any deletion is permanent and cannot be undone.

#### Prerequisites  

An entry in the decision matrix is created, see [Create an entry](#create-an-entry).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Select the entry you want to delete.

  > [Warning] Be aware that the deletion may have far-reaching consequences for the proper functioning of the system, as the *Taxes* module interacts with the *Invoicing* and *Accounting* modules. In case of doubt, contact our customer support.

2. Click the ![Delete](../../Assets/Icons/Trash08.png "[Delete]") (Delete) button to the right of the entry to be deleted.  
  The entry is deleted from the list.

3. Click the [SAVE] button.  
  A pop-up window confirms that the changes have been saved.

  ![Changes saved](../../Assets/Screenshots/Taxes/Settings/TaxClasses/ChangesSaved.png "[Changes saved]")

[comment]: <> (Vermutetes Verhalten. SAVE not working -> Method not found message. 02.08.22)


## Define a tax delivery threshold



#### Prerequisites  

- An applicable tax class is created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone is created, see [Create a tax zone](../Integration/02_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")




## Define tax exceptions on ZIP code level

Some areas within a territory have special tax regulations. This is case, for example, of Helgoland in Germany or Northern Ireland in the United Kingdom.

This tax exceptions can be defined using the *Ship-to postcode* fields.

#### Prerequisites  

- An applicable tax class is created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone is created, see [Create a tax zone](../Integration/02_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the *Ship-to postcode* drop-down list and select the appropriate option. The following options are available:

  - **Range**: Enter a postcode range, for example, 27498-27498 to limit the criterion to a specific target area.
  - **Regex**: Use regular expressions to specify postcodes containing alphanumeric characters, for example /^BT.*/. There are many regular expressions testing tools available free of charge in the Internet, such as [Regex101](https://regex101.com/).
