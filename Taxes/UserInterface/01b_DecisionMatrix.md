# Decision matrix

*Taxes > Settings > Tab DECISION MATRIX*

![Decision matrix](../../Assets/Screenshots/Taxes/Settings/DecisionMatrix/DecisionMatrix.png "[Decision matrix]")

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
Click this button to create an entry. A new entry line is displayed.

- ![Drag](../../Assets/Icons/Points03.png "[Drag]") (Drag)  
Click this button to move the entry to a different position with the left mouse button pressed. Drop it in the desired position by releasing the mouse button.

- *VAT ID*  
Value-added tax identification number. Click the drop-down list to select the appropriate option. The following options are available:

  - **Yes**  
  Select this option if the end customer is a company and, therefore, has a VAT ID number (business-to-business transaction).
  - **No**  
  Select this option if the end customer is a private individual and, therefore, has no VAT ID number (business-to-customer transaction).
  - **Any**  
Select this option to use a wildcard; any value is accepted.


- *Country of origin*  
Country where the product is shipped from.

  - Click the drop down-list on the left to select a group of countries. The following options are available:

    - **EU - European Union**  
    Select this option to include all EU member states. When selecting this option, the drop-down list on the right is grayed out.
    - **Any**  
    Select this option if you want to specify an individual country in the drop-down list on the right.

  - Click the drop-down list on the right to select a specific country.  

- *Ship-to country*  
Country where the product is shipped to.

  - Click the drop down-list on the left to select a group of countries. The following options are available:

    - **EU - European Union**  
    Select this option to include all EU member states. When selecting this option, the drop-down list on the right is grayed out.
    - **Any**  
    Select this option if you want to specify an individual country in the drop-down list on the right.

  - Click the drop-down list on the right to select a specific country.  

- *Ship-to postcode*  
Specific area within a country or territory where the product is shipped to.

  - Click the drop down-list on the left and select the appropriate option. The following options are available:

    - **Range**: Select this option to enter a postcode range, for example, 27498-27498 to limit the criterion to a specific postcode area.
    - **Regex**: Select this option to use regular expressions to specify postcodes containing alphanumeric characters, for example /^BT.*/.  

  - Enter the applicable range or regular expression in the field on the right.

- *Net value of goods smaller than*  

  - Click the drop-down list on the left to select the applicable currency.   
  - Enter a maximum net value amount if necessary. You can use the keyboard or the increase and decrease arrows on the right.


- *Tax zone*  
Click the drop-down list and select the applicable tax zone. By default, the following options are available:

  - **Domestic**  
  Select this option if the product is to be taxed according to the country of origin, that is, the dealer country.
  - **EU**  
  Select this option if the product is to be taxed according to EU regulations.
  - **Third country**  
  Select this option if the product is to be taxed outside the EU.

[comment]: <> (Check with FS if this is correct!)

Tax zones can be created, edited and deleted, see [Manage the tax zones](../Integration/03_ManageTaxZones.md). Any additionally created tax zones are displayed in the *Tax zone* drop-down list. 

- ![Delete](../../Assets/Icons/Trash08.png "[Delete]") (Delete)  
Click this button to delete the corresponding entry.  

- [SAVE]  
Click this button to save any changes made.
