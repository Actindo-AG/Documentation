[!!Check the posting history](../Operation/03_CheckPostingHistory.md)

# Posting history

*Warehousing > Quick posting > Tab POSTING HISTORY*

![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/PostingHistory.png "[Posting history]")

The *Posting history* tab allows you to check the stock postings for a specific material and to filter all stock postings according to different criteria. Since all stock postings ever performed are stored in the system, a huge number of entries is available. Therefore, to reduce system overload and improve performance, no posting is displayed before setting a filter.

The list displayed when filtering by product is similar to the one displayed in the *Stock history* sub-tab of the *Warehouse/suppliers* tab in the *Quick posting* menu entry, see [Check the posting history for a material](../Operation/03_CheckPostingHistory.md#check-the-posting-history-for-a-material). 


[comment]: <> (For detailed information on general UI functions, see... -> Link to Core1 UI)

- *Product*  
    Enter the product SKU or name to search for the stock posting for a specific material. 

- *Posting type*  
    Click the drop-down list and select the posting type you would like to display. The following options are available: 
    
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

        > [Info] To be able to use pre-reservation postings in the system, your shop must support this function.  

[comment]: <> (Vgl. Manual posting in 02_ManageStock.md. Evtl. Posting type allg. beschrieben, z.B. in UI, und Verweis? So wie es jetzt ist, passt in beiden Kontexten nicht.)

- *Warehouse*  
    Click the drop-down list and select the desired warehouse. All warehouses available are displayed in the list.

- *Storage shelf*  
    Click the drop-down list and select the desired storage shelf. All available storage shelves are displayed in the list.

- *From date* / *Until date*  
    Click the field(s) to enter the desired date or date range. Alternatively, click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to select a date.  

- [DISPLAY]  
    Click this button to display the posting history according to the filter criteria.


![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/CombinedFilterPostingHistory.png "[Posting history]")

The results list displays all posting according to the selected criteria, including the following details:

- *Date*  
    Posting date.

- *Posting type*  
    Type of posting.

- *Customer no.*  
    Customer or supplier number.

- *Customer name*  
    Customer or supplier name.

- *Document no.*  
    Business document number. This detail is only displayed in case of automatic postings. 

- *SKU*  
    Product SKU.

- *Product name*  
    Product name.

- *Quantity*  
    Number of units posted. 

[comment]: <> (Vorzeichen erklären)

- *Unit price*  
    Price per unit for the material posted.

- *Total price*  
    Price of all units posted.

- *Warehouse*   
    Warehouse ID and name.

- *Storage shelf*   
    Storage shelf number.

- *Movement*  
    Units added or reduced (minus sign).

- *Stock*  
    Actual physical number of units stored.

- *Available*  
    Number of units available to be sold (actual stock minus reserved units).

- *Comment*  
    Comments added to the posting.

- *Time of posting*  
    Date and time of posting.

- *Project no.*  
    Order number in shop.






