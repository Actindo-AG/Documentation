
[!!User interface Stock withdrawal matrix](../UserInterface/to-be-determined)
[!!Configure the warehouse groups](./01_ConfigureWarehouseGroups.md)
[!!Configure the warehouses](./02_ConfigureWarehouses.md)
[!!](../Integration/.md)


# Check the stock withdrawal matrix

The stock withdrawal matrix is designed to determine automatically from which warehouse and under which conditions stock is withdrawn. The usual parameters are country of delivery and sales channel, although the following parameters can also be configured:

- Country of delivery: where the shipment has to be delivered
- Product group: if desired
- Sales channel: e.g. Omni-Channel
- Account: connection, e.g. Commerce Cloud 
- Sub account: Shop, e.g. DE, EN, FR...
- Shipping provider: e.g. if Express take it from one warehouse, if Standard, from a different one
- Warehouse: specific warehouse where it should be withdrawn
- Warehouse group: you can also specify the warehouse group only  
(Obviously, when both warehouse and warehouse group are specified, the warehouse should be included in the warehouse group)

The stock withdrawal matrix consists of a list of decision-making criteria. The correct order of these criteria is crucial, as the system goes through them in the order they are listed, starting from the top, and stops checking them as soon as a matching criterion is found.
This means, that the criteria must be organized from specific to general to cover all possible relevant cases.


## Create an entry

Create an entry to ...

#### Prerequisites  

- At least one warehouse has been created, see [Create a warehouse](./02_ConfigureWarehouses.md#create-a-warehouse).
- Product group
- Sales channel
- Warehouse group?

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Click the [ADD] button in the bottom left corner.   
    A new data input line is displayed.

2. Double-click the **Delivery address country** field and select the applicable country from the drop-down list.  
    
3. 


2. If necessary, edit the settings as described in the following:

    + Select the option **--all--** in the drop-down list in the *Product group* column.

    + Select the output channel via which you want to create offers in the drop-down list in the *Marketplace* column.

    + Select the option **--all--** in the drop-down list in the *Sub-account* column.

    + Select the option **--all--** in the drop-down list in the *Shipping provider* column.

    + Select the warehouse from which you want to take the stock in the drop-down list in the *Warehouse* column.

3. Click the button [SAVE ASSIGNMENTS] in the bottom right corner.   
    The new assignment in the stock withdrawal matrix is saved.


---




