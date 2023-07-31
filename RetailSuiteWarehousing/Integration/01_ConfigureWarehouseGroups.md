# Configure the warehouse groups

Warehouse group explanation

Warehouse group vs. Warehouse -> Link auf Warehouse


## Add a warehouse group

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the [NEW GROUP] button in the *Warehouse master data* sub-tab.  
    The *Basic data* sub-tab is displayed.

    ![Group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/GroupBasicData.png "[Group basic data]")

2. Enter a number in the *Warehouse group* field.

3. Enter a description for the warehouse group in the *Designation* field. This description will be displayed later on in the left menu in the *Warehouse master data* sub-tab.

4. Click the *Group type* drop-down list and select the appropriate option. The following options are available:
    - **Own warehouse**  
        Select this option if the warehouse group is managed by yourself.
    - **Externally controlled warehouse**  
        Select this option if the warehouse group is managed by a third party. 

    Depending on the selected option, the fields displayed differ. 

5. For the next steps to create a warehouse, follow the appropriate procedure:

    - [Create an own warehouse group](#create-an-own-warehouse-group)
    - [Create an externally controlled warehouse group](#create-an-externally-controlled-warehouse-group)


### Create an own warehouse group

#### Prerequisites

- A warehouse group has been added, see [Add a warehouse group](#add-a-warehouse-group).
- The *Own warehouse* option has been selected in the *Group type* field.

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data > Select own warehouse*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/GroupBasicData.png "[Warehouse master data]")

1. If necessary, click the *Fulfill orders from other warehouse groups* drop-down list and select the appropriate option. All available warehouse groups are displayed in the list. The **No warehouse group** option includes all warehouses that have not been assigned to any warehouse group.

[comment]: <> (Tooltip: If orders cannot be completely fulfilled from the warehouse groups selected here, the missing products are taken from this warehouse group. The delivery note is printed in this storage group and contains all items. -> Frage: "from the warehouse groups selected here" oder "warehouse group"? Man kann nur eine Gruppe wählen, oder?)
        
2. If desired, enter any comments in the *Comment* field.

3. Click the [SAVE] button.  
    The warehouse group has been saved.

4. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner of the left menu to update the list of warehouses. The new warehouse group is displayed in the list of warehouses.


### Create an externally controlled warehouse group

#### Prerequisites

- A warehouse group has been added, see [Add a warehouse group](#add-a-warehouse-group).
- The *Externally controlled warehouse* option has been selected in the *Group type* field.
- At least one connection has been established in the *Fulfillment* module, see [Create a connection](../../Fulfillment/Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data > Select externally controlled warehouse*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/ExternalWarehouseBasicData.png "[Warehouse master data]")

1. If necessary, click the *Fulfill orders from other warehouse groups* drop-down list and select the appropriate option. All available warehouse groups are displayed in the list. The **No warehouse group** option includes all warehouses that have not been assigned to any warehouse group.

[comment]: <> (Tooltip: If orders cannot be completely fulfilled from the warehouse groups selected here, the missing products are taken from this warehouse group. The delivery note is printed in this storage group and contains all items. -> Frage: "from the warehouse groups selected here" oder "warehouse group"? Man kann nur eine Gruppe wählen, oder?)
        
2. *External warehouse type*

3. *Connection*

4. *Return to this location possible*

5. If desired, enter the address details in the corresponding fields.

6. If desired, enter any comments in the *Comment* field.

7. Click the [SAVE] button.  
    The warehouse group has been saved.

8. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner of the left menu to update the list of warehouses. The new warehouse group is displayed in the list of warehouses.


[comment]: <> (Evtl. zwei komplett separate procedures mit H2?)


## Edit a warehouse group

#### Prerequisites

At least one warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse group you want to edit.  
    The *Basic data* sub-tab of the selected warehouse group is displayed.

    ![Group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/GroupBasicData.png "[Group basic data]")


## Delete a warehouse group

#### Prerequisites


#### Procedure

