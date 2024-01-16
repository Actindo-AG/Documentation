[!!Manage the stock](./01_ManageStock.md)
[!!User interface Quick posting](../UserInterface/01_QuickPosting.md)

# Check posting history

You can check all stock postings that have been performed in the *Warehousing* module. Stock postings can be done automatically, that is, by the system, and manually by the user. If a business document number is provided in the *Document no.* column, the stock posting is automatic. If no business document number is displayed, the stock posting is a manual one.

[comment]: <> (Verweis auf Basic OM process in Core1? Oder hier kurz erklären, wie prinzipiell die stock postings vom System/von den Belegen funktionieren?)

It is possible to check all stock postings performed for a specific material and to filter all stock postings according to different criteria.


## Check posting history for a material

*Warehousing > Posting history > Tab POSTING HISTORY*

![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/PostingHistory.png "[Posting history]")

You can check all stock postings performed for a specific material. The list displayed is the same as the one displayed in the *Stock history* sub-tab in the *Warehouse/suppliers* tab for a selected material, although additional information is provided here, such as the order number in shop.

Besides, you can further filter the list of postings for a selected material by different criteria, see [Filter the stock history by different criteria](#filter-stock-history-by-different-criteria).

#### Prerequisites

At least a stock posting has been performed, see [Create a manual posting](./01_ManageStock.md#create-a-manual-stock-posting).  

#### Procedure

1. Enter the product name or SKU to filter the posting history by product. You can find out the product name or SKU in the *Basic data* sub-tab of the respective product.  
    
    > [Info] As soon as you have typed three characters, a context menu with matching suggestions is displayed.

2. Click the [DISPLAY] button to see the posting history for the selected product.  

    ![Material posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/MaterialPostingHistory.png "[Material posting history]")

    > [Info] If a posting is red-colored and crossed out, it indicates that the business document has been cancelled.

3. Check the different posting types performed in the *Posting type* column.

4. Check the quantity of stock posted for the selected material in the *Quantity* column. 

    > [Info] It is important to notice that the signs in this column are reversed, that is, a **Sale** posting is positive, a **Purchase** posting is negative. At this point, you can compare the numbers displayed in the *Quantity* column with those in the *Movement* column. The numbers match but the sign differ.

[comment]: <> (Grund dafür? Vgl. Quantity vs. Movement Spalten! OC macht positive Reservierung, DL macht negative Reservierung, s. NoE Screenshot)

5. Check the physical and the available stock in the *Stock level* and *Available* columns.   

6. Additionally, you can check the order number in shop in the *Project no.* column in case of automatic stock postings.


## Filter stock history by different criteria

*Warehousing > Posting history > Tab POSTING HISTORY*

![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/PostingHistory.png "[Posting history]")

You can filter all stock postings performed using different criteria. You can also combine several criteria to narrow your search results.

#### Prerequisites

At least a stock posting has been performed, see [Create a manual posting](./01_ManageStock.md#create-a-manual-stock-posting).  

#### Procedure

1. Click the *Posting type* drop-down list and select the desired posting type. The following options are available:  

    - **Reservation**   
        Select this option if you want to display only the stock postings for open orders. This posting type does not reduce the actual, physical stock in the warehouse, but does affect the available stock calculation. A reservation can therefore result in a negative stock level.

    - **Sale**  
        Select this option if you want to display only the stock postings for ordered materials that have left the warehouse. This posting type reduces the actual, physical stock in the warehouse.  

    - **Order**   
        Select this option if you want to display only the stock postings for ordered additional materials from a supplier for restocking purposes. This posting type does not increase the actual, physical stock in the warehouse but does affect the available stock calculation.

    - **Purchase**  
        Select this option if you want to display only the stock postings for purchased materials that have been received in the warehouse. This posting type increases the actual, physical stock in the warehouse.    
        
    - **Stock adjustment posting**  
        Select this option to display the stock adjustment postings after stocktaking.   
        
    - **Stock transfer**  
        Select this option if you want to display only the stock postings for materials redistributed from a source storage shelf to a destination storage shelf. This posting type affects the actual stock in both storage shelves.    
        
    - **Return**  
        Select this option if you want to display only the stock postings of returned materials. This posting type affects the actual stock in the respective storage shelf. 

    - **Problem**  
        Select this option if you want to display the stock postings for materials that cannot be sold for any reason, for instance due to a defect. This posting type affects the actual stock in the respective storage shelf. 

    - **Pre-reservation**  
        Select this option if you want to display stock postings for material reserved for orders that have not been received in the system yet, that is, with no business document assigned. This can be the case, for example, when a customer places a product in the shopping cart. This posting type does not affect the actual nor the available stock in the warehouse. 

        > [Info] Pre-reservation postings are not standard and must be additionally configured in the system. If you have not had it configured, this option will not be displayed in the list.

[comment]: <> (Vgl. Manual posting in 01_ManageStock.md. Evtl. Posting type allg. beschrieben, z.B. in UI, und Verweis? So wie es jetzt ist, passt in beiden Kontexten nicht.)

2. Click the *Warehouse* drop-down list and select the desired warehouse. All warehouses available are displayed in the list.

3. Click the *Storage shelf* drop-down list and select the desired storage shelf. All available storage shelves are displayed in the list.

4. Click the *From date* and/or the *Until date* fields to enter the desired date range. Alternatively, click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to select a date.  

5. Click the [DISPLAY] button to see the posting history according to the set filters.  
    In the example below, the *Manual posting* has been selected in the *Posting type* drop-down list.

   ![Filtered posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/CombinedFilterPostingHistory.png "[Filtered posting history]")

    > [Info] If a posting is red-colored and crossed out, it indicates that the business document has been cancelled.
