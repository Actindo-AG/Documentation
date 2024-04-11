[!!Create a manual stock posting](../Operation/02_ManageStock.md)
[!!Check the posting history](../Operation/03_CheckPostingHistory.md)


# Posting types

The *Warehousing* module allows you to manage the stock manually through the *Quick posting* menu entry. For detailed information, see [Create a manual stock posting](../Operation/02_ManageStock.md#create-a-manual-stock-posting).

However, stock postings are usually created automatically by the system, triggered by the creation and processing of business documents as configured in your workflow. The system performs the postings automatically when an order is received in the *Order Management* module. In the case of customer orders, the automatic posting process works as follows:

Every order that is imported into the system is linked to a business document, the head document. The head document, regardless of what business document it is, creates a reservation posting in the *Warehousing* module. The ordered material is then reserved. This reservation has no effect on the actual physical stock, but it reduces the available material stock, that is, the number of units that are available to be sold.

When the so-called delivery head, usually the delivery note, is created, this business document creates two postings in the stock history. The first one is a reserved for open delivery note posting (also known as waiting for picking) to withdraw the physical stock in the system, thus reducing the physical stock in the warehouse. The second one is a reservation posting with a negative sign to clear the initial reservation. The result of all materials processed in the order must always be 0.

Once the material has left the warehouse, that is, the delivery note has been closed, the reserved for open delivery note posting is updated into a sale posting.

Below, you can see the list of all posting types with a detailed description. 

- **Manual posting**  
    This posting type is created manually by the user in the *Quick posting* tab. Depending on the movement in the warehouse, it can be positive (stock in) or negative (stock released). Since the posting is manual, no customer/supplier number and name, and no business document number are provided in the posting history.

- **Reservation**   
    This posting type can be created manually or automatically. It represents the stock postings for open customer orders. This posting type does not reduce the actual physical stock in the warehouse but does affect the available stock calculation. A reservation can therefore result in a negative stock level.

- **Reserved for open delivery note**   
    Also called **Waiting for picking**. This posting type can be both manually and automatically created. It represents the stock postings for materials now linked to an open delivery note. These materials are therefore firmly reserved. This posting type reduces the actual physical stock in the warehouse.

[comment]: <> (Terminologie muss noch im UI angepasst werden; dementsprechend hier aktualisieren, wenn erledigt)

- **Sale**  
    This posting type can be created manually or automatically. It represents the stock postings for ordered materials that have left the warehouse, that is, when the delivery note has been processed and closed. This posting type reduces the actual physical stock in the warehouse.  

- **Order**   
    This posting type can be created manually or automatically. It represents the stock postings for ordered additional materials from a supplier for restocking purposes. This posting type does not increase the actual physical stock in the warehouse but does affect the available stock calculation.

- **Purchase**  
    This posting type can be created manually or automatically. It represents the stock postings for purchased materials that have been received in the warehouse. This posting type increases the actual physical stock in the warehouse.    

- **Back to supplier**  
    This posting type is created automatically when a customer return is processed in the *Returns* module and the follow-up action "Send to supplier and ship to customer after stock receipt" is triggered.
    
- **Stock adjustment posting**  
    This posting type can only be created manually by the user. It represents the stock adjustment postings after stocktaking.   
    
- **Stock transfer**  
    This posting type can be created manually or automatically. It represents the stock postings for materials redistributed from a source storage shelf to a destination storage shelf. This posting type affects the actual stock in both storage shelves.    
    
- **Return**  
    This posting type can be created manually or automatically. It represents the stock postings for returned materials. This posting type affects the actual stock in the respective storage shelf. 

- **Drop shipment**   
    This posting type is created automatically by the system when a dropshipping order is received. It has no effect on the stock.

- **Problem**  
    This posting type can only be created manually by the user. Select this option if you want to display the stock postings for materials that cannot be sold for any reason, for instance due to a defect. This posting type affects the actual stock in the respective storage shelf. 

- **Pre-reservation**  
    This posting type can be created manually or automatically. It represents the stock postings for material reserved for orders that have not been received in the system yet, that is, with no business document assigned. This can be the case, for example, when a customer places a product in the shopping cart. This posting type does not affect the actual nor the available stock in the warehouse. 

    > [Info] To be able to use pre-reservation postings in the system, your shop must support this function.  