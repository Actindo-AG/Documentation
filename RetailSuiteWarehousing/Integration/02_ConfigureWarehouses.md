# Configure the warehouses

In contrast to a warehouse group, a warehouse is a specific storage area that can be assigned, or not, to a specific warehouse group. If a warehouse is not assigned to any warehouse group, it will be listed under the general *No warehouse group* in the left side bar. 

Warehouses can be created, edited and deleted.

## Create a warehouse

Create one or more specific warehouses from which the stock is taken.

#### Prerequisites

A warehouse group is created, see [Create a warehouse group](#create-a-warehouse-group).

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the button [NEW WAREHOUSE].   
    The *Basic data* tab is displayed on the right side.

     ![Warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseBasicData.png "[Warehouse basic data]")

2. Enter a number for the warehouse in the *Warehouse* field.

3. Select the warehouse group in the *Warehouse group* drop-down list.  
    
    > [Info] If you do not select a warehouse group, the warehouse will be included in the **No warehouse group**.

[comment]: <> (C&CS Trainig: Heusels Sandbox hat eine zusätzliche Drop-down-Liste Lager-Typ. Trifft die noch zu? Elemente in der Liste: Kommisionierlager, Nachschubslager, Transferlager, Sperrlager)

4. Enter a name for the new warehouse in the *Designation* field.

5. Click the *Products per shelf* drop-down list and select the appropriate option. The following options are available:  
    - **One product per storage shelf**  
        Select this option if you want to store only one product per storage shelf.  
    - **Different products per storage shelf**   
        Select this option if you want to store more than one product per storage shelf.

[comment]: <> (Julian: Warehouse planning, Exclude from ordering -> Warehouse planing can be ignored, as it is no longer developed and has no effect.)

[comment]: <> (C&CS: *Exclude from ordering* drop-down list should be set to **No** to deactivate the purchasing process for this warehouse. The *Purchasing* module can calculate the suggested amount of a product that needs to be purchased from a supplier to replenish the stock level. If this option is activated, that is, set to **Yes**, the stock amount available in this warehouse will not be part of the calculation, that is, it will be ignored by the system.)

6. If desired, enter any comments in the *Comment* field.

7. Click the [SAVE] button.  
    The warehouse has been saved.
    
8. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) button at the top of the left column.   
    The new warehouse is displayed in the left column.



## Edit a warehouse

Once you have created a warehouse, you can edit it. 

#### Prerequisites

At least one warehouse has been created, see [Create a warehouse](#create-a-warehouse).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse you want to edit.  
    The *Basic data* sub-tab of the selected warehouse is displayed.

    ![Edit warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/EditWarehouseBasicData.png "[Edit warehouse basic data]")

2. Modify any settings as necessary in the applicable fields.  

3. Click the [SAVE] button.  
    The changes have been saved.

 > [Info] It may be necessary to click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) button at the top of the left column to display certain changes, for example, if the warehouse has been assigned to a different warehouse group.   
    


## Delete a warehouse

Once you have created a warehouse, you can delete it. 

#### Prerequisites

At least one warehouse has been created, see [Create a warehouse](#create-a-warehouse).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Sub-tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse you want to edit.  
    The *Basic data* sub-tab of the selected warehouse is displayed.

    ![Edit warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/EditWarehouseBasicData.png "[Edit warehouse basic data]")

2. Modify any settings as necessary in the applicable fields.  

3. Click the [DELETE] button.  
    The warehouse is deleted and is no longer displayed in the left side bar in the *Warehouse master data* sub-tab.
    
    > [Info] If the warehouse has already been included in the stock allocation matrix, the warehouse cannot be deleted. A window with the following error message is displayed: *Error deleting: There are warehouse allocations in this warehouse.* In this case, you have to ... first, see [To be determined](#to-be-determined).
