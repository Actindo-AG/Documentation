[!!Create a store in POS](./06_CreateStore.md)
[!!Manage the POS warehouse](./08_ManageWarehouse.md)
[!!Handle an out-of-stock order](../Troubleshooting/01_OutOfStockOrder.md)

[comment]: <> (add link to Warehouse module if available)

# Configure the warehouse for POS

As a POS system usually has its own warehouse and is separated from the main warehouse, a new POS warehouse should be created in advance.
Therefore, it is recommended to create a new warehouse group and integrate all warehouses made specifically for POS into this group.


## Create a warehouse group

Create a warehouse group to which you can assign all specific warehouses for your POS store, for instance a sales warehouse, a returns warehouse and a quarantine warehouse.

#### Prerequisites

The *Warehouse groups* plugin must be installed.

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/GroupBasicData.png "[Warehouse group basic data]")

1. Click the button [NEW GROUP].   
    The *Basic data* tab is displayed on the right side.

2. Enter a unique number for the warehouse group in the *Warehouse group* field.

3. Enter a name for the new warehouse group in the *Designation* field.

4. Click the *Group type* drop-down list and select a group type.  

[comment]: <> (add link to Warehouse UI if available)

5. Click the [SAVE] button.

6. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button at the top of the left column.   
    The new warehouse group is displayed in the left column.



## Create a warehouse

Create one or more specific warehouses for your POS store from which the stock is taken.

#### Prerequisites

A warehouse group is created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseBasicData.png "[Warehouse basic data]")

1. Click the button [NEW WAREHOUSE].   
    The *Basic data* tab is displayed on the right side.

2. Enter a number for the warehouse in the *Warehouse* field.

    > [Info] If the warehouse is part of a warehouse group, it is recommended to enter a number corresponding to the number range of the warehouse group.

3. Select the warehouse group in the *Warehouse group* drop-down list.

4. Enter a name for the new warehouse in the *Designation* field.

5. Select the products per shelf in the *Products per shelf* drop-down list.

    > [Info] If you create a warehouse for POS, it is recommended to select the option **Multiple items per shelf**.   
    
[comment]: <> (add link to Warehouse UI if available)

6. Click the [SAVE] button.

7. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) button at the top of the left column.   
    The new warehouse is displayed in the left column.
