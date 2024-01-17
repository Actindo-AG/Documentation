[!!Check the posting history](../Operation/02_CheckPostingHistory.md)

# Posting history

*Warehousing > Quick posting > Tab POSTING HISTORY*

![Posting history](../../Assets/Screenshots/RetailSuiteWarehousing/PostingHistory/PostingHistory.png "[Posting history]")

[comment]: <> (No entries shown when clicking the menu entry. Huge amount of postings available in the system for all stock movements and materials; they are not deleted. Therefore, for efficiency reasons/to save resources, nothing is shown first before a filter is set.) 

The *Posting history* tab allows you to check the stock postings for a specific material and to filter all stock postings according to different criteria. The list displayed when filtering by product/material is the same as the one displayed in the *Stock history* sub-tab of the *Warehouse/suppliers* tab in the *Quick posting* menu entry, see [Check posting history for a material](../Operation/02_CheckPostingHistory.md#check-posting-history-for-a-material). 

For detailed information on general UI functions of the CONNECTIONS tab,

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

        > [Info] Pre-reservation postings are not standard and must be additionally configured in the system. If you have not had it configured, this option will not be displayed in the list.

[comment]: <> (Vgl. Manual posting in 01_ManageStock.md. Evtl. Posting type allg. beschrieben, z.B. in UI, und Verweis? So wie es jetzt ist, passt in beiden Kontexten nicht.)

- *Warehouse*  
    Click the drop-down list and select the desired warehouse. All warehouses available are displayed in the list.

- *Storage shelf*  
    Click the drop-down list and select the desired storage shelf. All available storage shelves are displayed in the list.

- *From date* / *Until date*
    Click the field(s) to enter the desired date or date range. Alternatively, click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button to select a date.  

- [DISPLAY]  
    Click this button to display the posting history according to the filter criteria.












- Calender





