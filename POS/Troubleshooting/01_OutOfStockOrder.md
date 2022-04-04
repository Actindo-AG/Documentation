[!!Warehouse](RetailSuiteWarehousing)
[!!Omni-Channel](Channels)

# Handle an out-of-stock order

## Error Message

Error booking bill: [stage: lager_book] Fehler beim Erzeugen der Lagerbuchungen: Der Bestand für Artikel *x* im Lager *x* ist nur 0.00, benötigt würden *x*.

Follow the instructions below if this error message is displayed.

## Procedure
*Warehouse > Quick Booking > Tab QUICK BOOKING > Tab Product list*

![Product list](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/ProductList.png "[Product list]")

1.  Double click the article in the article list that you want to check. Alternatively, first right click the article and click then the **Open** entry in the displayed context menu.    
    The article details are displayed on several tabs below the article list. The *Basic data* tab is preselected.

  ![Basic data](/Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/BasicData/BasicData.png "[Basic data]")

2. Click the *Warehouse / Supplier* tab.   
  The *Warehouse / Supplier* tab is displayed. The *Warehouse management* sub-tab is preselected.

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

      > [Info] For detailed information, see [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md).

  + Enter the number by which the stock should be changed in the *Change* field.

    > [Info] For a stock increase, enter a positive number. For a stock decrease, enter a negative number with a minus sign as a prefix. In the right column of the window, the old stock and a preview of the new stock are displayed.  

  + If desired, select the date on which the stock change will be booked in the *Posting date* field. By default, the current date is preselected.

  + If desired, enter a comment in the *Comment* field.

5. Click the [SAVE & NEW] button in the bottom right corner of the window.   
  The window is closed. The new stock is displayed in the *Stocks* section.

6. Switch to the *Omni-Channel* module: *Omni-Channel > Orders and Returns > Tab ORDERS* .    
  The *ORDERS* tab is displayed.

  ![Orders](/Assets/Screenshots/Channels/OrdersReturns/Orders/Orders.png "[Orders]")

7. Select the checkbox of the order that was out-of-order and click the [EXPORT TO OMS] button in the editing toolbar at the top.     
  The order export is restarted. During the export, the **Being exported** status is displayed in the *Status of Export to OMS* column.

  > [Info] The export can take several minutes. Click the ![Process](/Assets/Icons/Process.png "[Process]") (Process) button in the upper right corner to display the process window with the current state of export.

8. Click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner to update the order list.   
  The order status in the *Status of Export to OMS* column changed to **Exported**. The order is correctly exported.

## See also

- [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md)
- [User Interface Omni-Channel](/Channels/UserInterface/00_UserInterface.md)

## Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
