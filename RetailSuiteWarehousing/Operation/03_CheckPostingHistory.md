[!!Manage the stock](./02_ManageStock.md)
[!!User interface Quick posting](../UserInterface/01_QuickPosting.md)

# Check posting history

You can check all stock postings that have been performed in the *Warehousing* module. Stock postings can be done automatically, that is, by the system, and manually by the user. If the business document number and customer/supplier details are provided in the corresponding columns, the stock posting is automatic. If this information is not displayed, the stock posting is a manual one. For a detailed description of all posting types, see [Posting types](#posting-types). 

The system performs the postings automatically when an order is received in the *Order Management* module. In the case of customer orders, the automatic posting process works as follows:

Every order that is imported into the system is linked to a business document, the head document. The head document, regardless of the business document it is, as this can be determined by the customer, creates a reservation posting in the *Warehousing* module. The ordered material is then reserved. This reservation has no effect on the actual physical stock, but it reduces the available material stock, that is, the number of units that are available to be sold.

When a delivery head, usually the delivery note, is created, this business document creates two postings in the stock history. The first one is a reserved for open delivery note posting (also known as waiting for picking) to withdraw the physical stock in the system, thus reducing the physical stock in the warehouse. The second one is a reservation posting with a negative sign to clear the initial reservation. The result of all materials processed in the order must always be 0.

Once the material has left the warehouse, that is, the delivery note has been closed, the reserved for open delivery note posting is updated into a sale posting.

[comment]: <> (Evtl. Verweis auf Basic OM process in Core1, wenn veröffentlicht)

The *Posting history* tab allows you to check all stock postings performed for a specific material and to filter all stock postings according to different criteria.



## Posting types 

Below, you can see the list of all posting types with a detailed description. 

- **Manual posting**  
    This posting type is performed manually by the user in the *Quick posting* tab. Depending on the movement in the warehouse, it can be positive (stock in) or negative (stock released). Since the posting is manual, no customer/supplier number and name, and the business document number is provided in the posting history.

- **Reservation**   
    This posting type can be both manual and automatic. It represents the stock postings for open customer orders. This posting type does not reduce the actual, physical stock in the warehouse but does affect the available stock calculation. A reservation can therefore result in a negative stock level.

- **Reserved for open delivery note**   
    Also known as **Waiting for picking**. This posting type can be both manual and automatic. It represents the stock postings for materials now linked to an open delivery note. This materials are therefore firmly reserved. This posting type reduces the actual, physical stock in the warehouse.

[comment]: <> (Reserved for open delivery note vs. Sale)

- **Sale**  
    This posting type can be both manual and automatic. It represents the stock postings for ordered materials that have left the warehouse, that is, when the delivery note has been processed and closed. This posting type reduces the actual, physical stock in the warehouse.  

- **Order**   
    This posting type can be both manual and automatic. It represents the stock postings for ordered additional materials from a supplier for restocking purposes. This posting type does not increase the actual, physical stock in the warehouse but does affect the available stock calculation.

- **Purchase**  
    This posting type can be both manual and automatic. It represents the stock postings for purchased materials that have been received in the warehouse. This posting type increases the actual, physical stock in the warehouse.    

- **Back to supplier**  
    This posting type is performed automatically by the system after a supplier order has been cancelled. 

    [comment]: <> (Stimmt das so? Mehr Info dazu?) 
    
- **Stock adjustment posting**  
    This posting type can only be performed manually by the user. It represents the stock adjustment postings after stocktaking.   
    
- **Stock transfer**  
    This posting type can be both manual and automatic. It represents the stock postings for materials redistributed from a source storage shelf to a destination storage shelf. This posting type affects the actual stock in both storage shelves.    
    
- **Return**  
    This posting type can be both manual and automatic. It represents the stock postings of returned materials. This posting type affects the actual stock in the respective storage shelf. 

- **Drop shipment**   
    This posting type is performed automatically by the system when a dropshipping order is received. It has no effect in the stock.

    [comment]: <> (Stimmt das so? Mehr Info dazu?)

- **Problem**  
    This posting type can only be performed manually by the user. Select this option if you want to display the stock postings for materials that cannot be sold for any reason, for instance due to a defect. This posting type affects the actual stock in the respective storage shelf. 

- **Pre-reservation**  
    This posting type can be both manual and automatic. It represents the stock postings for material reserved for orders that have not been received in the system yet, that is, with no business document assigned. This can be the case, for example, when a customer places a product in the shopping cart. This posting type does not affect the actual nor the available stock in the warehouse. 

    > [Info] To be able to use pre-reservation posting in the system, your shop must support this function.  



## Check the posting history for a material

You can check all stock postings performed for a specific material. The list displayed is the same as the one displayed in the *Stock history* sub-tab in the *Warehouse/suppliers* tab for a selected material, although additional information is provided here, such as the order number in shop.

Besides, you can further filter the list of postings for a selected material by different criteria, see [Filter the posting history by different criteria](#filter-the-posting-history-by-different-criteria).

#### Prerequisites

At least a stock posting has been performed, see [Create a manual posting](./01_ManageStock.md#create-a-manual-stock-posting).  

#### Procedure

*Warehousing > Posting history > Tab POSTING HISTORY*

![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/PostingHistory.png "[Posting history]")

1. Enter the product name or SKU to filter the posting history by product. You can find out the product name or SKU in the *Basic data* sub-tab of the respective product.  
    
    > [Info] As soon as you have typed three characters, a context menu with matching suggestions is displayed.

2. Click the [DISPLAY] button to see the posting history for the selected product.  

    ![Material posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/MaterialPostingHistory.png "[Material posting history]")

    > [Info] If a posting is red-colored and crossed out, it indicates that the business document has been cancelled.

3. Check the different posting types performed in the *Posting type* column.

4. Check the quantity of stock posted for the selected material in the *Quantity* column. 

    > [Info] Notice that the number signs in this column are reversed with regards to the *Movement* column. 
    
5. Check the physical and the available stock in the *Stock level* and *Available* columns.   

6. Additionally, you can check the order number in shop in the *Project no.* column in case of automatic stock postings.



## Filter the posting history by different criteria

You can filter all stock postings performed using different criteria. You can also combine several criteria to narrow your search results.

#### Prerequisites

At least a stock posting has been performed, see [Create a manual posting](./01_ManageStock.md#create-a-manual-stock-posting).  

#### Procedure

*Warehousing > Posting history > Tab POSTING HISTORY*

![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/PostingHistory.png "[Posting history]")

1. Click the *Posting type* drop-down list and select the desired posting type. The following options are available:  

    - **Manual posting**
    - **Reservation**   
    - **Waiting for picking**
    - **Sale**  
    - **Order**   
    - **Purchase**  
    - **Back to supplier**
    - **Stock adjustment posting**  
    - **Stock transfer**  
    - **Return**  
    - **Drop shipment** 
    - **Problem**  
    - **Pre-reservation**  

    For a detailed description of the posting types, see [Posting types](#posting-types). 
    
[comment]: <> (Vgl. Manual posting in 01_ManageStock.md. Evtl. Posting type allg. beschrieben, z.B. in UI, und Verweis? So wie es jetzt ist, passt in beiden Kontexten nicht.)

2. Click the *Warehouse* drop-down list and select the desired warehouse. All warehouses available are displayed in the list.

3. Click the *Storage shelf* drop-down list and select the desired storage shelf. All available storage shelves are displayed in the list.

4. Click the *From date* and/or the *Until date* fields to enter the desired date range. Alternatively, click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to select a date.  

5. Click the [DISPLAY] button to see the posting history according to the set filters.  
    In the example below, the *Manual posting* has been selected in the *Posting type* drop-down list.

   ![Filtered posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/CombinedFilterPostingHistory.png "[Filtered posting history]")

    > [Info] If a posting is red-colored and crossed out, it indicates that the business document has been cancelled.
