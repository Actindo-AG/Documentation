[!!Configure the warehouse groups](./01_ConfigureWarehouseGroups.md)
[!!User interface Warehouse](../UserInterface/03a_Warehouse.md)

# Configure the warehouses

A warehouse is a subordinate storage area within a warehouse group. It is used for a specific purpose, such as sales, returns, or blocked stock. A warehouse may or may not be assigned to a specific warehouse group. If a warehouse is not assigned to any warehouse group, it will be listed under the general *No warehouse group* in the left side bar.

Warehouses can be created, edited, and deleted. Bear in mind, though, that you cannot delete a warehouse where stock has already been allocated.

[comment]: <> (Julian: Gibt es eigentlich einen speziellen Grund, warum ich ein Warehouse keiner Warehouse group zuordnen sollte? Was hat das für Auswirkungen?)


## Create a warehouse

Create one or more specific warehouses to store and manage your stock.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the [NEW WAREHOUSE] button.   
    The *Basic data* tab is displayed on the right side.

     ![Warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseBasicData.png "[Warehouse basic data]")

2. Enter a unique number for the warehouse in the *Warehouse* field. This is the warehouse ID.

3. If desired, select a warehouse group in the *Warehouse group* drop-down list.  
    
    > [Info] If you do not select a warehouse group, the warehouse will be included in the **No warehouse group**.

4. Enter a name for the new warehouse in the *Designation* field.

5. Click the *Products per shelf* drop-down list and select the **Different products per storage shelf** option.  
        
[comment]: <> (One product per storage shelf ignorieren; aktuell bei keinem Kunden benutzt und und Probleme beim Anlegen der Lagerfächer. Warehouse planning can be ignored, as it is no longer developed and has no effect.)

6. Click the *Exclude from ordering* drop-down list and select the appropriate option. This setting works together with the *Purchasing* module. The *Purchasing* module can calculate the suggested amount of a product that needs to be purchased from a supplier to replenish the stock level based on the stock value in the selected warehouse. The following options are available: 

    - **Yes**  
        Select this option if you want to exclude the stock amount stored in this warehouse from the calculation, that is, to be ignored by the system.
    - **No**   
        Select this option if you want to include the stock amount stored in this warehouse in the calculation.
   
7. If desired, enter any comments in the *Comment* field.

8. Click the [SAVE] button.  
    The new warehouse has been saved.
    
9. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) button in the upper right corner of the left side bar to update the list of warehouses.   
    The new warehouse is displayed in the list of warehouses.



## Edit a warehouse

Once you have created a warehouse, you can edit it, for instance if you want to assign a warehouse to a different warehouse group. Bear in mind, though, that you cannot edit the warehouse ID if stock has already been allocated.

#### Prerequisites

At least one warehouse has been created, see [Create a warehouse](#create-a-warehouse).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse you want to edit.  
    The *Basic data* tab of the selected warehouse is displayed.

    > [Caution] **Potential loss of data**   
    Editing has the potential to cause loss of data due to overwrite. The overwrite cannot be undone and the overwritten data cannot be restored. Check all your entries before proceeding.

    ![Edit warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/EditWarehouseBasicData.png "[Edit warehouse basic data]")

2. Modify any settings as necessary in the applicable fields.  

3. Click the [SAVE] button.  
    The changes have been saved.

    > [Info] If the warehouse has already stock allocations, the warehouse ID cannot be modified. A window with the following error message is displayed: *Error deleting: There are warehouse allocations in this warehouse*. 

4. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) button in the upper right corner of the left side bar to display certain changes, for example, if the warehouse has been assigned to a different warehouse group.   
    


## Delete a warehouse

After you have created a warehouse, you can delete it if it is no longer needed. Bear in mind, though, that you cannot delete a warehouse where stock has already been allocated.

#### Prerequisites

At least one warehouse has been created, see [Create a warehouse](#create-a-warehouse).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Warehouse master data*

![Warehouse master data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/WarehouseMasterData.png "[Warehouse master data]")

1. Click the warehouse you want to delete.  
    The *Basic data* tab of the selected warehouse is displayed.

    > [Caution] **Loss of data**  
    Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored. Problems may occur due to unresolved dependencies. Make sure you really want to delete the selected data.

    ![Edit warehouse basic data](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/WarehouseMasterData/EditWarehouseBasicData.png "[Edit warehouse basic data]")
    
2. Click the [DELETE] button.  
    The warehouse is deleted and is no longer displayed in the list of warehouses.
    
    > [Info] If the warehouse has already stock allocations, the warehouse cannot be deleted. A window with the following error message is displayed: *Error deleting: There are warehouse allocations in this warehouse*. 
