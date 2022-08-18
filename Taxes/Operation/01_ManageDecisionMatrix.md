[!!Accounting](RetailSuiteAccounting)  
[!!User Interface Decision matrix](../UserInterface/01b_DecisionMatrix.md)  
[!!Manage the tax rates](../Integration/01_ManageTaxRates.md)  
[!!Manage the tax classes](../Integration/02_ManageTaxClasses.md)  
[!!Manage the tax zones](../Integration/03_ManageTaxZones.md)  


# Manage the decision matrix

The decision matrix is designed to determine which tax zone, and therefore which tax rate, is applicable to an order. The decision matrix consists of a list of decision-making criteria based on the information provided by the *Order management* module.

Taking into account the order confirmation and the delivery note, the *Order management* module provides the *Taxes* module with the following details: country of origin, ship-to country, ship-to postcode, and VAT ID. Using this information, the decision matrix is able to determine the tax zone. Once the tax zone has been determined, the *Taxes* module can provide the *Order management* module with this information, as well as with the applicable tax key and tax rate.  

The correct order of the decision-making criteria is crucial, as the system goes through the criteria in the order they are listed, starting from the top, and stops checking them as soon as a matching criterion is found. This means, that the criteria must be organized from specific to general to cover all possible relevant cases.


## Create an entry

Create an entry to determine a new tax zone.

#### Prerequisites  

- An applicable tax class has been created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone has been created, see [Create a tax zone](../Integration/03_ManageTaxZones.md#create-a-tax-zone).
- An applicable tax rate has been created, see [Create a tax rate](../Integration/01_ManageTaxRates.md#create-a-tax-rate).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line is displayed.

2. Click the *VAT ID* drop-down list and select the appropriate option. The following options are available:

  - **Yes**  
  Select this option if the end customer is a company and, therefore, has a VAT ID number (business-to-business transaction).
  - **No**  
  Select this option if the end customer is a private individual and, therefore, has no VAT ID number (business-to-customer transaction).


3. Click the *Country of origin* drop-down list and select the appropriate option. Use the drop-down list on the left to select a group of countries or the one on the right to select an individual country. As a group of countries, only the **EU - European Union** option is available. In the drop-down list of individual countries, all available countries in the system are displayed. When a group of countries is selected, the drop-down list on the right is locked.

4. Click the *Ship-to country* drop-down list and select the appropriate option. Use the drop-down list on the left to select a group of countries or the one on the right to select an individual country. As a group of countries, only the **EU - European Union** option is available. In the drop-down list of individual countries, all available countries in the system are displayed. When a group of countries is selected, the drop-down list on the right is locked.

5. If necessary, click the *Ship-to postcode* drop-down list and select the appropriate option. The following options are available:

  - **Range**  
  Select this option to specify a numeric postcode range, for example 27498 or 52001-52006.
  - **Regex**  
  Select this option to specify a postcode containing alphanumeric characters with regular expressions, for example /^BT.*/. For detailed information about regular expressions, see https://regex101.com/.

> [Info] This feature can be used to define special tax regimes within a territory, such as that of Northern Ireland in the United Kingdom or Helgoland in Germany. For detailed information, see [Define tax exceptions on ZIP code level](#define-tax-exceptions-on-ZIP-code-level).

6. Enter the applicable postcode range or regular expression in the *Ship-to postcode* field on the right.

7. If necessary, click the *Net value of goods smaller than* drop-down list and select the applicable currency.

8. Enter the applicable amount using the keyboard or the increase and decrease arrows in the *Net value of goods smaller than* field on the right.

9. Click the *Tax zone* drop-down list and select the applicable tax zone. All available tax zones are displayed in the list.

10. Click the [SAVE] button.  
The new tax rule has been saved. The *Success* pop-up window is displayed.

  ![Decision matrix saved](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrixSaved.png "[Decision matrix saved]")


## Edit an entry

Edit an entry to modify any of the configured parameters.

#### Prerequisites  

An entry has been created in the decision matrix, see [Create an entry](#create-an-entry).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the *VAT ID* drop-down list and select a different option, if necessary.

2. Click the *Country of origin* drop-down list on the left and deselect the selected group of countries, if necessary. As a group of countries, only the **EU - European Union** option is available. When no group of countries is selected, the drop-down list on the right is unlocked. Click the drop-down list on the right to select an individual country.

3. Click the *Ship-to county* drop-down list on the left to deselect the selected group of countries, if necessary. As a group of countries, only the **EU - European Union** option is available. When no group of countries is selected, the drop-down list on the right is unlocked. Click the drop-down list on the right to select an individual country.

4. Click the *Ship-to postcode* drop-down list on the left and select a different option, if necessary. Click the field on the right to modify the range or the regular expression entered. Use the keyboard to enter a different value.

5. Click the *Net value of goods smaller than* drop-down list on the left to select a different currency, if necessary. Click the field on the right to modify the net value amount entered. You can use the keyboard or the increase and decrease arrows.

6. Click the *Tax zone* drop-down list to select a different applicable tax zone.

7. Click the [SAVE] button.  
The edited tax rule has been saved. The *Success* pop-up window is displayed

  ![Decision matrix saved](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrixSaved.png "[Decision matrix saved]")

8. If it is necessary to change the position of an entry in the decision matrix, see [Change the order of entries](#change-the-order-of-entries).


## Change the order of entries

Modify the position of one or more entries to organize them from specific to general and cover all possible tax scenarios.

> [Info] The correct order of the decision-making criteria is crucial, as the system goes through the criteria in the order they are listed.

#### Prerequisites  

At least two entries have been created in the decision matrix, see [Create an entry](#create-an-entry).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")


1. Click the ![Drag](../../Assets/Icons/Points03.png "[Drag]") (Drag) button to the left of the entry line, move the entry to a different position with the left mouse button pressed and drop it in the desired position by releasing the mouse button.   

2. Click the [SAVE] button.  
The entry position has been saved. The *Success* pop-up window is displayed.

  ![Decision matrix saved](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrixSaved.png "[Decision matrix saved]")

3. If necessary, repeat the steps **1** and **2** with all entries that need to be repositioned.


## Delete an entry

Delete an entry that is no longer applicable.  

> [Warning] Be aware that any deletion is permanent and cannot be undone.

#### Prerequisites  

An entry has been created in the decision matrix, see [Create an entry](#create-an-entry).

  > [Warning] Be aware that the deletion may have far-reaching consequences for the proper functioning of the system, as the *Taxes* module interacts with the *Invoicing* and *Accounting* modules.

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")


1. Click the ![Delete](../../Assets/Icons/Trash08.png "[Delete]") (Delete) button to the right of the entry to be deleted.  
  The entry is removed from the list.

2. Click the [SAVE] button.  
The entry has been deleted. The *Success* pop-up window is displayed.  

  ![Decision matrix saved](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrixSaved.png "[Decision matrix saved]")


## Define a tax delivery threshold

[comment]: <> (Configure the decision matrix with tax delivery thresholds)

All applicable tax scenarios can be configured using the decision matrix.

[comment]: <> (Lieferschwelle muss man über Tax rates start/end date konfigurieren, also gehört nicht ganz in der Decision Matrix. Einstellung ist trotzdem etwas besonders... Evtl. 2 Subprocedures: Subprocedure 1 Decision matrix configuration, Subprocedure 2 Update the tax rate validity, oder Verweis auf "Standardeinstellung", i.e. Create an entry + Einstellung des Datums des Tax rates?)

#### Prerequisites  

- All applicable tax rates have been defined for delivery thresholds, see [Define the tax rates for delivery thresholds](#define-the-tax-rates-for-delivery-thresholds).
- All applicable entries have been created, see [Create an entry](#create-an-entry).
- All entries are in the right order, see [Change the order of entries](#change-the-order-of-entries).


[comment]: <> (Entweder prereq + nur Einstellung in TAX RATES oder Subprocedure 1 + Subprocedure 2)

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line is displayed.

2. Click the *VAT ID* drop-down list and select **No**, as the end customer must be a private individual.

3. Click the *Country of origin* drop-down list on the right and select the country where the product is shipped from.

4. Click the *Ship-to country* drop-down list on the right to select the country where the product is to be shipped to.  

5. If necessary, click the *Ship-to postcode* drop-down list on the left and select the appropriate option. Specify a postcode in the field on the right. For detailed information, see [Define tax exceptions on ZIP code level](#define-tax-exceptions-on-ZIP-code-level).

6. If necessary, click the *Net value of goods smaller than* drop-down list and select the applicable currency, and enter the applicable net value in the field on the right.   

7. Click the *Tax zone* drop-down list and select the applicable tax zone.

8. Click the [SAVE] button.  
A pop-up window confirms that the decision matrix has been saved. The new entry has been saved.

  ![Decision matrix saved](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrixSaved.png "[Decision matrix saved]")

9. Repeat this procedure to configure one by one all the applicable tax scenarios depending on your business needs.




## Define tax exceptions on ZIP code level

Some areas within a territory have special tax regulations. This is the case, for example, of Helgoland in Germany or Northern Ireland in the United Kingdom.

These tax exceptions can be defined using the *Ship-to postcode* fields.

#### Prerequisites  

- An applicable tax class has been created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone has been created, see [Create a tax zone](../Integration/03_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line is displayed.

2. Click the *VAT ID* drop-down list and select the appropriate option. The following options are available:

  - **Yes**: The end customer is a company and, therefore, has a VAT ID number (business-to-business transaction).
  - **No**: The end customer is a private individual and, therefore, has no VAT ID number (business-to-customer transaction).
  - **Any**: Wildcard; any value is accepted.


3. Click the *Country of origin* drop-down list(s) and select the appropriate option(s). Use the drop-down list on the left to select a group of countries and the one on the right to select an individual country.

  > {Info] The current version only provides the option **EU - European Union** as a group of countries. When a group of countries is selected, the right drop-down list is grayed out.

4. Click the *Ship-to country* drop-down lists and select **Any** on the left and the country where the product is to be shipped to on the right.  

5. Click the *Ship-to postcode* drop-down list and select the appropriate option. The following options are available:

  - **Range**: Enter a postcode range, for example, 27498-27498 to limit the criterion to a specific target area.
  - **Regex**: Use regular expressions to specify postcodes containing alphanumeric characters, for example /^BT.*/.

  > [Info] There are many regular expressions testing tools available free of charge in the Internet, such as [Regex101](https://regex101.com/).

6. Enter a postcode range or a regular expression to define a specific tax exception area in the selected country.

7. Click the *Net value of goods smaller than* drop-down list and select the applicable currency. If necessary, specify an amount using the keyboard or the increase and decrease arrows on the right.

8. Click the *Tax zone* drop-down list to select the applicable tax zone.

9. Click the [SAVE] button.  
A pop-up window confirms that the decision matrix has been saved.  

  ![Decision matrix saved](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrixSaved.png "[Decision matrix saved]")
