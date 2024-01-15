[!!Configure warehouses](./01_ConfigureWarehouseGroups.md)
[!!User interface to be completed](../UserInterface/XX_tobecompleted.md)
[!!Manage the attributes](../../PIM/Integration/01_ManageAttributes.md)

# Configure the stock allocation

The stock allocation function allows you to update the stock levels automatically across all your sales channels. In the stock allocation table, you can define which value should be indicated as available stock in each sales channel. There are different methods you can choose from to calculate the available stock. The calculated stock amount is then transferred to the *PIM* product, where it is displayed in the *Stock level* field. From the *PIM* module, the calculated stock amount is transferred via ETL to the *Omni-Channel* module, and from there to the corresponding sales channel via driver. 

Every time a posting is made in the *Warehousing* module, the stock value in the *PIM* module is updated. This process occurs asynchronously and may take a few moments. The stock value is transferred in turn to the sale channel via the *Omni-Channel* module.

The stock allocation table includes automatically all warehouses you have created. You can decide any time if you want to include the stock stored in a specific warehouse in the stock calculation. For detailed information to create a warehouse, see [Create a warehouse](./02_ConfigureWarehouses.md#create-a-warehouse). 

Depending on the configured target channels and warehouses, the displayed columns and rows will vary. 

#### Prerequisites

- At least a warehouse has been created, see [Create a warehouse](./02_ConfigureWarehouses.md#create-a-warehouse).
- The necessary attributes of the *Stock value* data type have been created in the *PIM* module, see [Create an attribute](../../PIM/Integration/01_ManageAttributes.md#create-an-attribute). 
- The *Stock value* attribute has been assigned to the relevant attribute sets, see [Add an attribute to the set](../../DataHub/Integration/02_ManageAttributeSets.md#add-an-attribute-to-the-set). 
- The necessary mappings between the corresponding *PIM* attribute sets and the *Omni-Channel* attribute sets have been created, see [Manage the ETL mappings](../../DataHub/Operation/01_ManageETLMappings.md#manage-the-etl-mappings). 

[comment]: <> (Stimmt der letzte Punkt? Trotzdem funktioniert bei mir nicht. Warum? Was fehlt?)

#### Procedure 

*Warehousing > Settings > Tab WAREHOUSE > Tab Stock allocation*

![Stock allocation](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockAllocation/StockAllocation.png "[Stock allocation]")

1. Select the row with the stock allocation attribute name corresponding to the desired target channel in the *Target channel* column.

2. Double-click the field with the **Default setting** option in the *Stock calculation* column.   
    A drop-down list is displayed.

[comment]: <> (Ist Default setting tatsächlich ein Setting? Wo wird es eingestellt, wenn überhaupt?)

3. Click the drop-down list and select the appropriate option. The following options are available:  
      
    - **Fixed value**  
        Select this option to transfer a fixed stock amount.   
        The corresponding field in the *Fixed value* column is unlocked. 

    - **Formula**  
        Select this option to create your own formula to calculate the stock amount. For this purpose, Actindo implements php formulas using the different posting types, for example GET_BESTAND(50)+GET_RESERVED(50)+GET_PRE_RESERVED(50)+GET_SELL(50).  
        The corresponding field in the *Formula* column is unlocked. 

        > [Info] Bear in mind that all outgoing postings, such as pre-reservations, reservations or sales, are negative, and therefore they must be added to the formula with a plus sign, not a minus. 

        Below, you can a table containing the php commands used in the *Actindo Core1 Platform* and their meaning:

        | php commands | Meaning |
        | ------------ | ---------------- |
        | GET_BESTAND | Physical stock |
        | GET_RESERVED | Reserved material |
        | GET_PRE_RESERVED | Pre-reserved material |
        | GET_ RESERVED_SPECIAL | Material waiting for picking |
        | GET_SELL | Material sold |
        | GET_COUNT | Physical stock minus material waiting for picking |
        | GET_COUNTAVAIL | Physical stock minus reserved material |
        
        [comment]: <> (Oder nur COUNT? Gibt es andere Methoden?)

        [comment]: <> (Vorreservierung hat keine Auswirkung auf dem Bestand, auch wenn bei Lager/Lieferanten > Bestände das Vorzeichen negativ ist. Die muss man extra abziehen. Vorreservierungen sind auch nicht Standard; man muss die im Shop einstellen. Sonderfall von NoE: Shop muss mit dem Core1 "reden".)

    - **Calculation, stock level**  
        Select this option to transfer the physical stock stored in the warehouse.  
        The fields in the warehouse columns are unlocked.
        
    - **Calculation, stock availability (stock level - reserved)**  
        Select this option to transfer the stock amount resulting from the physical stock stored in the warehouse minus the reservations (open customer orders). This is done to prevent overselling.  
        The fields in the warehouse columns are unlocked.

    - **Calculation, availability (stock level + ordered - reserve)**   
        Select this option to transfer the stock amount resulting from the physical stock stored in the warehouse, plus the stock ordered from the supplier (open supplier orders, even if the materials have not yet arrived in the warehouse), minus the reservations (open customer orders).  
        The fields in the warehouse columns are unlocked.

4. Depending of the option you have selected in the previous step, proceed as follows:

    - If you have selected the **Fixed value** option, double-click the applicable field and enter the desired value.  

    - If you have selected the **Formula** option, double-click the applicable field and enter the desired formula. See the table in step **3** for the php commands and their meaning. 

    - If you have selected one of the predefined calculation formulas, double-click the field corresponding to the desired warehouse to display the drop-down list. Then, select the **Yes** option in the drop-down list to include the warehouse in the stock allocation calculation or select the **No** option to exclude it.

    > [Info] The small red triangle in the left upper corner of the field indicates that the marked field has been changed.  

5. If desired, the supplier stock can also be included in the calculation. To do so, click the drop-down list of the field corresponding to the desired target channel in the *Supplier stock* column and select the appropriate option. The following options are available:

    - **No**  
        Select this option to exclude stock from all suppliers.
    - **Yes, all**  
        Select this option to include stock from all suppliers.
    - **Yes, only dropship suppliers**    
        Select this option to include stock only from dropship suppliers.
    - **Yes, only normal suppliers**  
        Select this option to include stock only from normal suppliers.

[comment]: <> (Was ist damit gemeint? Wo kann ich diese voreinstellen? What is actually meant? Does it include the stock at the supplier? Or just the ordered supplier stock? That is, btw, already included in one of the calculation formulas To add a plug-in supplier, see... Achtung! Fixed value und Formel erlauben nicht, hier Nein/Ja einzustellen!)

5. Click the [SAVE] button in the bottom right corner.   
    The stock allocation is saved. 
    





