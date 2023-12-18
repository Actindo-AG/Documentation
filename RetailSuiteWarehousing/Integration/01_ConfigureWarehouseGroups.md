[!!Configure warehouses](./02_ConfigureWarehouses.md)
[!!User interface to be completed](../UserInterface/XX_tobecompleted.md)

# Configure the warehouse groups

A warehouse group is a higher-level classification of storage facilities according to customer-defined criteria, for example location or type of product. Warehouse groups are physically separated from each other and, therefore, one delivery note must be issued for each warehouse group. A warehouse group can contain an unlimited number of warehouses.  

Warehouses can be created, edited and deleted.



## Create a warehouse group

Create a warehouse group to which you can assign any number of specific warehouses, for instance a sales warehouse, a returns warehouse, or a storage area for blocked stock.

#### Prerequisites

No prerequisites to fulfill.

The *Warehouse groups* plugin must be installed.

[comment]: <> (Diese Info in General? Stimmt das? Lagergruppe-, Lager-, Lagerplanung- und Lagerreichweiten...- Plugins müssen generell zusammen mit Lager installiert sein? Oder passiert das beim Installation von Lager-Modul?)

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the [NEW GROUP] button in the *Warehouse master data* sub-tab.  
    The *Basic data* sub-tab is displayed.

    ![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseGroupBasicData.png "[Warehouse group basic data]")

2. Enter a unique number for the warehouse group in the *Warehouse group* field.

3. Enter a description for the warehouse group in the *Designation* field. This description will be displayed later on in the left side bar in the *Warehouse master data* sub-tab.

4. Click the *Group type* drop-down list and select the appropriate option. The following options are available:
    - **Own warehouse group**  
        Select this option if the warehouse group is managed by yourself.
    - **Externally controlled warehouse group**  
        Select this option if the warehouse group is managed by a third party. 

    Depending on the selected option, the fields displayed differ. 

5. For the next steps to create a warehouse group, follow the appropriate procedure:

    - [Create an own warehouse group](#create-an-own-warehouse-group)
    - [Create an externally controlled warehouse group](#create-an-externally-controlled-warehouse-group)


### Create an own warehouse group

#### Prerequisites

- A warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).
- The **Own warehouse group** option has been selected in the *Group type* field.

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data > Select Own warehouse group*

![Own warehouse group master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseGroupBasicData.png "[Own warehouse group master data]")

1. If necessary, click the *Fulfill orders from other warehouse groups* drop-down list and select the appropriate option. All available warehouse groups are displayed in the list. The **No warehouse group** option includes all warehouses that have not been assigned to any warehouse group.

[Comment]: <> (Tooltip: If orders cannot be completely fulfilled from the warehouse groups selected here, the missing products are taken from this warehouse group. The delivery note is printed in this storage group and contains all items. -> Frage: "from the warehouse groups selected here" oder "warehouse group"? Man kann nur eine Gruppe wählen, oder? Julian: Offenbar kann man nur eine Lagergruppe wählen. So gewollt oder Bug?)
        
2. If desired, enter any comments in the *Comment* field.

3. Click the [SAVE] button.  
    The warehouse group has been saved.

4. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner of the left side bar to update the list of warehouses.  
The new warehouse group is displayed in the list of warehouses.


### Create an externally controlled warehouse group

#### Prerequisites

- A warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).
- The **Externally controlled warehouse group** option has been selected in the *Group type* field.
- At least one connection has been established in the *Fulfillment* module, see [Create a connection](../../Fulfillment/Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data > Select Externally controlled warehouse group*

![External warehouse group master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/ExternalWarehouseGroupBasicData.png "[External warehouse group master data]")

1. If necessary, click the *Fulfill orders from other warehouse groups* drop-down list and select the appropriate option. All available warehouse groups are displayed in the list. The **No warehouse group** option includes all warehouses that have not been assigned to any warehouse group.

[comment]: <> (Tooltip: If orders cannot be completely fulfilled from the warehouse groups selected here, the missing products are taken from this warehouse group. The delivery note is printed in this storage group and contains all items. -> Frage: "from the warehouse groups selected here" oder "warehouse group"? Man kann nur eine Gruppe wählen, oder? Julian: Offenbar kann man nur eine Lagergruppe wählen. So gewollt oder Bug?)
        
2. Click the *External warehouse type* drop-down list and select the appropriate option. The following options are available:
    - **Legacy (obsolete)**  
        Select this option if ...
    - **Fulfillment module**  
        Select this option if the external warehouse is accessed via a connection in the *Fulfillment* module. 

[comment]: <> (Julian: bedeutet obsolete, dass diese Option nicht mehr zutrifft, also kann man ignorieren? Gibt es andere mögliche Optionen, außer Fulfillment? --> C&CS Training: Bezieht sich diese Funktion nur auf das alte Amazon-Verbindung Import-Funktion, also dass der Kunde den Bestand bei Amazon-fulfilled Bestellungen sehen und ggf. aufstocken kann?)

3. Click the *Connection* drop-down list and select the applicable connection. All connections established in the *Fulfillment* module are displayed in the list.

[comment]: <> (Julian: *Return to this location possible* obsolete?)

4. If desired, enter the address details in the corresponding fields.

5. If desired, enter any comments in the *Comment* field.

6. Click the [SAVE] button.  
    The warehouse group has been saved.

7. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner of the left side bar to update the list of warehouses.  
The new warehouse group is displayed in the list of warehouses.



## Edit a warehouse group

Once you have created a warehouse group, you can edit it. 

#### Prerequisites

At least one warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse group you want to edit.  
    The *Basic data* sub-tab of the selected warehouse group is displayed.

    ![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseGroupBasicData.png "[Warehouse group basic data]")

2. Modify any settings as necessary in the applicable fields.  

    > [Info] If the warehouse group already contains warehouses, the warehouse group number cannot be modified. A window with the following error message is displayed: *Error while saving: There are warehouses in this warehouse group.*

3. Click the [SAVE] button.  
    The changes have been saved.



## Delete a warehouse group

Once you have created a warehouse group, you can delete it. 

#### Prerequisites

At least one warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse group you want to delete.  
    The *Basic data* sub-tab of the selected warehouse group is displayed.

    ![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseGroupBasicData.png "[Warehouse group basic data]")

2. Click the [DELETE] button.
    The warehouse group is deleted and is no longer displayed in the left side bar in the *Warehouse master data* sub-tab.
    
    > [Info] If the warehouse group already contains warehouses, the warehouse group number cannot be modified. A window with the following error message is displayed: *Error while deleting: There are warehouses in this warehouse group.* In this case, you have to delete the warehouses included in the warehouse group first, see [Delete a warehouse](#delete-a-warehouse).