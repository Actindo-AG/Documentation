[!!Accounting](RetailSuiteAccounting)  
[!!Fakturierung](RetailSuiteFaktBase)  
[!!User Interface tax zones](../UserInterface/XX_DecisionMatrix.md)  
[!!Manage the tax rates](../Integration/01_ManageTaxRates.md)  
[!!Manage the tax classes](../Integration/01_ManageTaxClasses.md)  
[!!Manage the tax zones](../Integration/01_ManageTaxZones.md)  


# Manage the decision matrix

The decision tax matrix is designed to help the system decide which tax zone, and therefore which tax rate, is to be applied. The decision matrix consist of a list of decision-making criteria based on the information provided by the *Invoicing* module.

Taking into account the order confirmation and the delivery note, the *Invoicing* module provides the *Taxes* module with following details:

- Country of origin
- Ship-to country
- Ship-to postcode
- VAT ID

Using this information, the decision matrix is able to determine the tax zone, subsequently providing the *Invoicing* module with the applicable tax key and tax rate as well.  

The order of the decision-making criteria is essential, as the system goes through the criteria in the order they are listed, starting from the top, and stops checking them as soon as a matching criterion is found. This means, that the criteria must be organized from specific to general to cover all possible relevant cases.


## Create an entry

Create an entry to define a new tax zone.

#### Prerequisites  

- An applicable tax class is created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone is created, see [Create a tax zone](../Integration/02_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the upper left corner.   
  A new data entry line is displayed.

2. Click the *VAT ID* drop-down list and select the appropriate option (**Yes/No**).

  > [Info] This field refers to the end customer VAT ID. If the end customer is a private individual, no VAT ID is needed (business-to-customer transaction). If the end customer is a company (business-to-business transaction), the VAT ID number is needed. 


## Edit an entry

Edit a

#### Prerequisites  

No prerequisites to fulfill.

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*



## Delete an entry

Delete a

#### Prerequisites  

No prerequisites to fulfill.

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*



## Define a tax delivery threshold

Delete a

#### Prerequisites  

No prerequisites to fulfill.

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*




## Define a tax exceptions on ZIP code level

Delete a

#### Prerequisites  

No prerequisites to fulfill.

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*
