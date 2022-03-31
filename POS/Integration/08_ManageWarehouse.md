[!!Warehouse](RetailSuiteWarehousing)

# Manage the POS warehouse

Manage the warehouse settings to assign one or more specific warehouses to the POS from which the stock is taken and booked. The warehouse specifies where exactly the stock is booked out when a product is sold.

## Check the stock allocation

Check if the stock allocation is correctly configured so that the store stock is correctly assigned to the warehouse. The stock source specifies how the stock available in the POS system is calculated. In most cases, the stock source and the warehouse are identical, but they can also differ.   

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- The stock allocation is configured, see [Configure the stock allocation](06_CreateStore.md#configure-the-stock-allocation).

### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock allocation*

![Stock allocation](/Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockAllocation/StockAllocation.png "[Stock allocation]")

1.  Search for the target channel of the appropriate POS store in the *Target channel* column and check the settings in the corresponding row.

2. If necessary, edit the settings as described in the following:
  - Select the **Calculation, Stock** option in the drop-down list in the *Stock calculation* column.   
    The fields in the warehouse columns are unlocked.

  - Double-click the option in a warehouse column to display the drop-down list.

  - Select the **Yes** option in the drop-down list to include the corresponding warehouse in the stock calculation or select the **No** option to exclude it.

  > [Info] Select for each warehouse whether it should be included or not.

3. Click the [SAVE] button in the bottom right corner.   
  The stock allocation is saved. The stock is calculated from all selected warehouses.

### Next steps

- [Check the stock withdrawal matrix](#check-the-stock-withdrawal-matrix)
- [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products)
- [Manage the stock for POS products](#manage-the-stock-for-pos-products)

### See also

- [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)


## Check the stock withdrawal matrix

Check if the stock withdrawal matrix is correctly configured so that a specific warehouse is assigned to a specific store in POS.

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- The stock withdrawal matrix is configured, see [Configure the stock withdrawal matrix](06_CreateStore.md#configure-the-stock-withdrawal-matrix).

### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](/Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Search for the appropriate POS store in the column *Account* and check the settings in the corresponding row.   

2. If necessary, edit the settings as described in the following:

  + Select the option **--all--** in the drop-down list in the *Product group* column.

  + Select the output channel via which you want to create offers in the drop-down list in the *Marketplace* column.

  + Select the option **--all--** in the drop-down list in the *Sub-account* column.

  + Select the option **--all--** in the drop-down list in the *Shipping provider* column.

  + Select the warehouse from which you want to take the stock in the drop-down list in the *Warehouse* column.

3. Click the button [SAVE ASSIGNMENTS] in the bottom right corner.   
  The new assignment in the stock withdrawal matrix is saved.

### Next steps

- [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products)
- [Manage the stock for POS products](#manage-the-stock-for-pos-products)

### See also

- [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Check the stock allocation](#check-the-stock-allocation)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)


## Manage the warehouse logistics for POS products

Manage the warehouse logistics for POS product to ensure that products are active for warehousing.

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- A POS offer is created, see [Create an offer for POS](07_ManageOffers.md#create-an-offer-for-pos).

### Procedure

*Warehouse > Quick Booking > Tab QUICK BOOKING > Tab Product list*

![Product list](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/ProductList.png "[Product list]")

1.  Double click the article in the article list that you want to check. Alternatively, first right click the article and click then the **Open** entry in the displayed context menu.    
  The article details are displayed on several tabs below the article list. The *Basic data* tab is preselected.

  ![Basic data](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/BasicData/BasicData.png "[Basic data]")

2. Click the *Warehouse logistics active for this product* drop-down list on the right side of the *Basic data* tab and select the **YES** option.


3. Click the [Save] button in the bottom right corner of the *Basic data* tab.   
  The *Successfully saved* message is displayed at the top. The active warehouse logistics for this article is saved.

  ![Successfully saved](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/SuccessfullySaved.png "[Successfully saved]")

### Next steps

- [Manage the stock for POS products](#manage-the-stock-for-pos-products)

### See also

- [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Check the stock allocation](#check-the-stock-allocation)
- [Check the stock withdrawal matrix](#check-the-stock-withdrawal-matrix)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)


## Manage the stock for POS products

You can adjust the stock quantity of your POS products, for instance because of a stock, a purchasing or an ordering.

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- A POS offer is created, see [Create an offer for POS](07_ManageOffers.md#create-an-offer-for-pos).
- The warehouse logistics for the POS article is active, see [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products).
- A warehouse with a defined shelf is assigned to the POS product.

### Procedure

*Warehouse > Quick Booking > Tab QUICK BOOKING > Tab Product list*

![Product list](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/ProductList.png "[Product list]")

1.  Double click the article in the article list that you want to check. Alternatively, first right click the article and click then the **Open** entry in the displayed context menu.    

  ![Context menu](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/ContextMenu.png "[Context menu]")   

  The article details are displayed on several tabs below the article list. The tab *Basic data* is preselected.

  ![Basic data](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/BasicData/BasicData.png "[Basic data]")

2. Click the *Warehouse / Suppliers* tab.   
  The the *Warehouse / Suppliers* tab is displayed. The *Warehouse management* sub-tab is preselected.

  ![Warehouse management](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/WarehouseManagement.png "[Warehouse management]")

  > [Info] Check if a warehouse is displayed in the *Storage locations* section. You can only change the stock for the POS article, if a warehouse is assigned.

3. Click the [ADD BOOKING] button at the bottom of the *Stocks* section.   
  A window to enter the booking is displayed.

  ![Add booking](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/AddBooking.png "[Add booking]")

4. Configure the following settings:

  + Click the *Stock location* drop-down list and select the appropriate warehouse from which you want to adjust the stock.

  + Click the *Posting type* drop-down list and select the appropriate reason for the booking. The following options are available:
      - **Reservation**
      - **Sale**
      - **Order**
      - **Purchase**
      - **Stocktaking entry**
      - **Stock transfer**
      - **Return**
      - **Problem**
      - **Pre-reserve**


  + Enter the number by which the stock should be changed in the *Change* field.

    > [Info] For a stock increase, enter a positive number. For a stock decrease, enter a negative number with a minus sign as a prefix. In the right column of the window, the old stock and a preview of the new stock are displayed.  

  + If desired, select the date on which the stock change will be booked in the *Posting date* field. By default, the current date is preselected.

  + If desired, enter a comment in the *Comment* field.

5. Click the [SAVE & NEW] button in the bottom right corner of the window.   
  The window is closed. The new stock is displayed in the *Stocks* section.

### Next Steps

- [Open a pay desk](POS/Operation/01_OpenPayDesk.md)

### See also

- [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Check the stock allocation](#check-the-stock-allocation)
- [Check the stock withdrawal matrix](#check-the-stock-withdrawal-matrix)
- [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
