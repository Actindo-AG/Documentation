[!!Accounting](RetailSuiteAccounting)  
[!!Fakturierung](RetailSuiteFaktBase)  
[!!User Interface tax zones](../UserInterface/XX_DecisionMatrix.md)  
[!!Manage the tax rates](../Integration/01_ManageTaxRates.md)  
[!!Manage the tax classes](../Integration/01_ManageTaxClasses.md)  
[!!Manage the tax zones](../Integration/01_ManageTaxZones.md)  


# Manage the decision matrix

The decision tax matrix is designed to help the system decide which tax zone is to be applied. The decision matrix consist of a list of decision-making criteria based on the information provided by the *Invoicing* module.

Based on the order confirmation and the delivery note, the *Invoicing* module provides the *Taxes* module with following information:

- Country of origin
- Ship-to country
- Ship-to postcode
- VAT ID

Based on this criteria, the decision matrix is able to determine the applicable tax zone, subsequently providing the *Invoicing* module with the tax zone, the tax key and the tax rate.  

The order of the decision-making criteria is essential, as the system goes through the criteria in the order they are given, starting from the top, and stops checking as soon as a matching criteria is found. This means, that the criteria must be organized from the most specific to the most general to cover all possible relevant cases.


## Create an entry

Create a

#### Prerequisites  

- An applicable tax class is created, see [Create a tax class](../Integration/02_ManageTaxClasses.md#create-a-tax-class).
- An applicable tax zone is created, see [Create a tax zone](../Integration/02_ManageTaxZones.md#create-a-tax-zone).

#### Procedures

*Taxes > Settings > Tab DECISION MATRIX*




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
