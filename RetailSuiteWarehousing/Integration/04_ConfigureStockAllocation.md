[!!Configure warehouses](./01_ConfigureWarehouseGroups.md)
[!!User interface to be completed](../UserInterface/XX_tobecompleted.md)
[!!Manage the attributes](../../PIM/Integration/01_ManageAttributes.md)

# Stock allocation

The stock allocation function serves the purpose to update stock levels automatically across all your sales channels. The stock allocation table allows you to define which value should be indicated as available stock in each sales channel. There are different methods you can choose from to calculate the available stock. The calculated stock amount is then transferred to the *PIM* product, where it is displayed in the *Stock level* field. From the *PIM* module, the calculated stock amount is transferred via ETL to the *Omni-Channel* module, and then there via driver to the corresponding sales channel. 

The *Target channel* column displays all target "locations" where the calculated stock value is transferred in the *PIM* module. 

[comment]: <> (Include following columns: target channel, where the calculated value is transferred to, and supplier stock, if you want to include it in the calculation. What is actually meant? Does it include the stock at the supplier? Or just the ordered supplier stock? That is, btw, already included in one of the calculation formulas)

The stock allocation table integrates all the warehouse groups that have been created. For detailed information to create a warehouse group, see [Create a warehouse group](./01_ConfigureWarehouseGroups.md#create-a-warehouse-group). You can decide if you want to include the stock in those warehouse group in the stock calculation.

You can set up a calculation of the stock that will be updated from the *Warehousing* module to PIM product. Attribute: stock/Lagerbestand: Number (calculated result of the settings in the stock allocation table)

Depending on the preconfigured target channels and warehouse groups, the displayed columns and rows will vary. 

#### Prerequisites

- At least a warehouse group has been created.
- The necessary attributes of the *Stock value* data type have been created in the *PIM* module, see [Create an attribute](../../PIM/Integration/01_ManageAttributes.md#create-an-attribute). 
- The *Stock value* attribute has been assigned to the relevant attribute sets, see [Add an attribute to the set](../../DataHub/Integration/02_ManageAttributeSets.md#add-an-attribute-to-the-set). 
- Add to variant set, changeable attribute?
- The necessary mappings between the corresponding *PIM* attribute sets and the *Omni-Channel* attribute sets have been created, see [Manage the ETL mappings](../../DataHub/Operation/01_ManageETLMappings.md#manage-the-etl-mappings). 

[comment]: <> (Prekonfiguration nötig bei Target channel und Supplier stock - plugins?)

[comment]: <> (*Multimarkets* module is now obsolete.)

#### Procedure 

1. In the *Supplier stock* column, click the drop-down list of the cell corresponding to the desired target channel and select the appropriate option. The following options are available:

    - **No**  
        Select this option to exclude stock from all suppliers.
    - **Yes, all**  
        Select this option to include stock from all suppliers.
    - **Yes, only dropship suppliers**    
        Select this option to include stock only from dropship suppliers.
    - **Yes, only normal suppliers**  
        Select this option to include stock only from normal suppliers.

[comment]: <> (Was ist damit gemeint? Wo kann ich diese voreinstellen? What is actually meant? Does it include the stock at the supplier? Or just the ordered supplier stock? That is, btw, already included in one of the calculation formulas To add a plug-in supplier, see...)

2. In the *Stock calculation* column, click the drop-down list of the cell corresponding to the desired target channel and select the appropriate option. The following calculation options are available:  
    
    - **Default setting**   
        Select this option to ... 

        [comment]: <> (Wo voreinsgestellt? Was bewirkt dies? Keine weitere Felder in der Tabelle anklickbar)
      
    - **Fixed value**  
        Select this option to transfer a fixed stock amount to the *PIM* module and subsequently, via the *Omni-Channel* module, to the sales channel. The fixed value can be entered in the corresponding cell in the *Fixed value* column. 

    - **Formula**  
        Select this option to create your own formula to calculate the stock amount. For this purpose, Actindo implements php formulas using the different posting types, for example GET_BESTAND(50)+GET_BESTAND(51)+GET_RESERVED(50)+GET_PRE_RESERVED(50). The formula can be entered in the corresponding cell in the *Formula* column.

        [comment]: <> (Mehr info über die Formulas? Externes Link?)

    - **Calculation, stock level**  
        Select this option to transfer the physical stock amount in the warehouse. 

    - **Calculation, stock availability (stock level - reserved)**  
        Select this option to transfer the stock amount resulting from the physical stock in the warehouse minus the reservations (open customer orders). This is done to prevent overselling.

    - **Calculation, availability (stock level + ordered - reserve)**   
        Select this option to transfer the stock amount resulting from the physical stock in the warehouse, plus the stock ordered from the supplier (open supplier orders, even if it has not arrived yet in the warehouse), minus the reservations (open customer orders).

4. Bestandsberechnung

1-Eigenlager - Ja
2-Außenlager - Ja

This means the amount of stock available in those warehouses are included in the calculation.



