[!!Configure warehouses](./02_ConfigureWarehouses.md)
[!!Check the stock](../Operation/02_ManageStock.md)
[!!Check the posting history](../Operation/03_CheckPostingHistory.md)
[!!User interface Quick posting](../UserInterface/01a_QuickPosting.md)


# Configure the storage shelves 

Warehouses are subdivided into storage shelves, from which stock is actually posted. A storage shelf is, therefore, a subordinate storage area within a warehouse that can contain one or several materials. This depends on the warehouse settings. Currently, the recommended setting is to allow several materials per storage shelf. To modify the amount of materials per shelf, see [Edit a warehouse](./02_ConfigureWarehouses.md#edit-a-warehouse). 

Each material can be stored in several storage shelves and different warehouses, but they can only have one primary storage shelf, that is, one main storage location. When an order is received, stock is taken from the primary storage shelf automatically, as long as the ordered material is in stock, no other configuration is stored in the stock withdrawal matrix, or no configuration matches the criteria.

The first storage shelf that is created for a material is automatically set as primary. You can subsequently create another storage shelf and set it as primary by clicking the *is primary storage* checkbox. 

Storage shelves can be created, edited, and deleted. Bear in mind, though, that you cannot delete a storage shelf where postings have been made in the past, as all posting information is kept in the system. For detailed information, see [Check the posting history](../Operation/03_CheckPostingHistory.md).



## Create a storage shelf  

You can create an unlimited number of storage shelves in your warehouses to specify exactly where your materials are stored.

#### Prerequisites

- At least one warehouse has been created, see [Create a warehouse](./02_ConfigureWarehouses.md#create-a-warehouse).
- The warehouse logistics must be active for the selected material, see [Activate the warehouse logistics for a material](../Operation/01_ManageWarehouse.md#activate-the-warehouse-logistics-for-a-material).

#### Procedure

*Warehousing > Quick posting > Tab QUICK POSTING > Select a material > Tab Warehouse/suppliers > Sub-tab Warehouse management*

![Warehouse management](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/WarehouseManagement.png "[Warehouse management]")

1. Click the [CREATE] button in the bottom left corner of the *Storage locations* section.  
    The *Add* section is displayed.

    ![Add storage shelf](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/AddStorageShelf.png "[Add storage shelf]")

2. Click the *Warehouse ID* drop-down list and select the warehouse where you want to create the storage shelf.  
    All available warehouses are displayed in the list.

3. Click the *Storage shelf* field and enter a unique number. This is the storage shelf ID.  

4. If desired, click the *is primary storage shelf* checkbox to set the storage shelf as primary for the selected material.  

    > [Info] The primary storage shelf is then marked with **1** in the **is primary storage shelf** column in the *Storage locations* section.  

5. If you want to create a storage shelf for blocked storage, click the *Blocked storage* drop-down list and select the applicable material conditions. The following options are available:  
    - **ALL CONDITIONS**  
    - **NO ORIGINAL PACKAGING**  
    - **Incomplete**
    - **Defective item**
    - **Defective item, to be repaired**
    - **Out of withdrawal period**
    - **Out of warranty**
    - **Used**
    - **Wrong serial number**

    > [Info] You can create different blocked storage shelves for different material conditions. 
    
6. Click the [SAVE] button to save the storage shelf.  
    The notice *Please wait... Saving...* is displayed. The new storage shelf is displayed in the list of storage locations. 



## Edit a storage shelf  

Once you have created a storage shelf, you can edit it.

#### Prerequisites

A storage shelf has been created, see [Create a storage shelf](#create-a-storage-shelf).

#### Procedure

*Warehousing > Quick posting > Tab QUICK POSTING > Select a material > Tab Warehouse/suppliers > Sub-tab Warehouse management*

![Warehouse management](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/WarehouseManagement.png "[Warehouse management]")

1. Select the storage shelf you want to edit from the list in the *Storage locations* section.  
    The *Edit* section is displayed.

    ![Edit storage shelf](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/EditStorageShelf.png "[Edit storage shelf]")  

    > [Caution] **Potential loss of data**   
    Editing has the potential to cause loss of data due to overwrite. The overwrite cannot be undone and the overwritten data cannot be restored. Check all your entries before proceeding.

2. If desired, modify the storage shelf ID.  

[comment]: <> (Ist dies überhaupt möglich bzw. vernünftig, wenn Buchungen schon gemacht worden sind?)

3. Select or deselect the **is primary storage shelf** checkbox as necessary to change the storage shelf setting. 
    
    > [Info] The *Warehouse ID* und the *Blocked storage* settings cannot be changed for already existing warehouse storage shelves. In this case, you have to create a new warehouse shelf with the desired settings.   

4. Click the [SAVE] button.  
    The notice *Please wait... Saving...* is displayed. The changes are displayed in the list of storage locations. 



## Delete a storage shelf   

After you have created a storage shelf, you can delete it.  

Bear in mind, though, that you cannot delete a storage shelf where postings have been made in the past, as all posting information is kept in the system.

#### Prerequisites

A storage shelf has been created, see [Create a storage shelf](#create-a-storage-shelf).

#### Procedure

*Warehousing > Quick posting > Tab QUICK POSTING > Select a material > Tab Warehouse/suppliers > Sub-tab Warehouse management*

![Warehouse management](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/WarehouseManagement.png "[Warehouse management]")

1. Select the storage shelf you want to delete from the list in the *Storage locations* section.  
    The *Edit* section is displayed.

    ![Edit storage shelf](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/EditStorageShelf.png "[Edit storage shelf]")

    > [Caution] **Loss of data**  
    Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored. Problems may occur due to unresolved dependencies. Make sure you really want to delete the selected data.

2. Click the [DELETE] button.  
    The notice *Please wait... Saving...* is displayed. The deleted storage shelf is no longer displayed in the list of storage locations.  




