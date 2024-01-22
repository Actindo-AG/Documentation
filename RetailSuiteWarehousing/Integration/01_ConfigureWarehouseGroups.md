[!!Configure the warehouses](./02_ConfigureWarehouses.md)
[!!Check the posting history](../Operation/02_CheckPostingHistory.md)
[!!User interface Warehouse](../UserInterface/03a_Warehouse.md)

# Configure the warehouse groups

A warehouse group is a higher-level classification of storage facilities according to customer-defined criteria, for example location or type of product. Warehouse groups are physically and conceptually separated from each other and therefore one delivery note must be issued for each warehouse group. A warehouse group can contain an unlimited number of warehouses.  

Warehouses can be created, edited, and deleted. Bear in mind, though, that you cannot delete a warehouse group where postings have been made in the past, as all posting information is kept in the system. For detailed information, see [Check posting history](../Operation/02_CheckPostingHistory.md).



## Create a warehouse group

Create a warehouse group to which you can assign any number of specific warehouses, for example a sales warehouse, a returns warehouse, or a storage area for blocked stock.

### Add a warehouse group

Add a new warehouse group to the warehouse group list and define its name and identification number.

#### Prerequisites

The following plugins must be installed:   
- *Warehouse groups*  
- *Calculation of the range of storage and ordering by range of storage*  
- *Warehouse planning*  

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the [NEW GROUP] button in the *Warehouse master data* tab.  
    The *Basic data* sub-tab is displayed.

    ![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseGroupBasicData.png "[Warehouse group basic data]")

2. Enter a unique number for the warehouse group in the *Warehouse group* field. This is the warehouse group ID.

3. Enter a description for the warehouse group in the *Designation* field. This description will be displayed later on in the left side bar in the *Warehouse master data* tab.

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

Create an own warehouse group, that is, a warehouse group managed by yourself. 

#### Prerequisites

- A warehouse group has been added, see [Add a warehouse group](#add-a-warehouse-group).
- The **Own warehouse group** option has been selected in the *Group type* field.

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data > Select Own warehouse group*

![Own warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseGroupBasicData.png "[Own warehouse group basic data]")

1. If necessary, click the *Fulfill orders from other warehouse groups* drop-down list and select a warehouse group. All available warehouse groups are displayed in the list. The **No warehouse group** option includes all warehouses that have not been assigned to any warehouse group.
        
2. If desired, enter any comments in the *Comment* field.

3. Click the [SAVE] button.  
    The warehouse group has been saved.

4. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner of the left side bar to update the list of warehouses.  
The new warehouse group is displayed in the list of warehouses.


### Create an externally controlled warehouse group

Create an externally controlled warehouse group, that is, a warehouse group managed by a third party, such as a fulfillment partner.

#### Prerequisites

- A warehouse group has been added, see [Add a warehouse group](#add-a-warehouse-group).
- The **Externally controlled warehouse group** option has been selected in the *Group type* field.
- At least one connection has been established in the *Fulfillment* module, see [Create a connection](../../Fulfillment/Integration/01_ManageConnections.md#create-a-connection).

[comment]: <> (Evtl. auf Create connection in OC verweisen, wenn vereinheitlicht) 

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data > Select Externally controlled warehouse group*

![External warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/ExternalWarehouseGroupBasicData.png "[External warehouse group basic data]")

1. If necessary, click the *Fulfill orders from other warehouse groups* drop-down list and select a warehouse group. All available warehouse groups are displayed in the list. The **No warehouse group** option includes all warehouses that have not been assigned to any warehouse group.
       
2. Click the *External warehouse type* drop-down list and select the **Fulfillment module** option.  
    The applicable fields and drop-down lists are displayed.

    > [Info] The **Legacy** option in the *External warehouse type* drop-down list is no longer supported. Therefore, it is not described in this documentation.

3. Click the *Connection* drop-down list and select the applicable connection. All connections established in the *Fulfillment* module are displayed in the list.

4. Click the *Return to this location possible* drop-down list and select **Yes** to allow returned materials to be sent to this warehouse group. 

5. Click the *Country* drop-down list and select the country where the warehouse is located.

6. Click the *Zip* field and enter the applicable zip code.
    
    > [Info] Both country and zip code are needed to determine where the materials are shipped from, which is relevant to define the applicable tax regime. Any other address-related fields are optional.

7. If desired, enter any comments in the *Comment* field.

8. Click the [SAVE] button.  
    The warehouse group has been saved.

9. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner of the left side bar to update the list of warehouses.  
The new warehouse group is displayed in the list of warehouses.



## Edit a warehouse group

Once you have created a warehouse group, you can edit it. 

#### Prerequisites

At least one warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse group you want to edit.  
    The *Basic data* sub-tab of the selected warehouse group is displayed.

    ![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/EditWarehouseGroupBasicData.png "[Warehouse group basic data]")

    > [Caution] **Potential loss of data**    
    Editing has the potential to cause loss of data due to overwrite. The overwrite cannot be undone and the overwritten data cannot be restored. Check all your entries before proceeding.

2. Modify any settings as necessary in the applicable fields.  

    > [Info] If the warehouse group already contains warehouses, the warehouse group number cannot be modified. A window with the following error message is displayed: *Error while saving: There are warehouses in this warehouse group.*

3. Click the [SAVE] button.  
    The changes have been saved.



## Delete a warehouse group

After you have created a warehouse group, you can delete it if it is no longer needed. 

Bear in mind, though, that you cannot delete a warehouse group where postings have been made in the past, as all posting information is kept in the system.

#### Prerequisites

At least one warehouse group has been created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse group you want to delete.  
    The *Basic data* sub-tab of the selected warehouse group is displayed.

    ![Warehouse group basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/EditWarehouseGroupBasicData.png "[Warehouse group basic data]")

    > [Caution] **Loss of data**  
        Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored. Problems may occur due to unresolved dependencies. Make sure you really want to delete the selected data.

2. Click the [DELETE] button.   
    The warehouse group is deleted and is no longer displayed in the list of warehouses.
    
    > [Info] If the warehouse group already contains warehouses, the warehouse group number cannot be deleted. A window with the following error message is displayed: *Error while deleting: There are warehouses in this warehouse group.* In this case, you have to delete the warehouses included in the warehouse group first, see [Delete a warehouse](#delete-a-warehouse).