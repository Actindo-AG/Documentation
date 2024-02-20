# Posting types 

Below, you can see the list of all posting types with a detailed description. 

- **Manual posting**  
    This posting type is created manually by the user in the *Quick posting* tab. Depending on the movement in the warehouse, it can be positive (stock in) or negative (stock released). Since the posting is manual, no customer/supplier number and name, and no business document number are provided in the posting history.

- **Reservation**   
    This posting type can be created manually or automatically. It represents the stock postings for open customer orders. This posting type does not reduce the actual physical stock in the warehouse but does affect the available stock calculation. A reservation can therefore result in a negative stock level.

- **Reserved for open delivery note**   
    Currently called **Waiting for picking** in the user interface. This posting type can be both manually and automatically created. It represents the stock postings for materials now linked to an open delivery note. This materials are therefore firmly reserved. This posting type reduces the actual physical stock in the warehouse.

[comment]: <> (Terminologie muss angepasst werden)

- **Sale**  
    This posting type can be created manually or automatically.It represents the stock postings for ordered materials that have left the warehouse, that is, when the delivery note has been processed and closed. This posting type reduces the actual physical stock in the warehouse.  

- **Order**   
    This posting type can be created manually or automatically. It represents the stock postings for ordered additional materials from a supplier for restocking purposes. This posting type does not increase the actual physical stock in the warehouse but does affect the available stock calculation.

- **Purchase**  
    This posting type can be created manually or automatically. It represents the stock postings for purchased materials that have been received in the warehouse. This posting type increases the actual physical stock in the warehouse.    

- **Back to supplier**  
    This posting type is created automatically by the system after a supplier order has been cancelled. 

    [comment]: <> (Stimmt das so? Mehr Info dazu?) 
    
- **Stock adjustment posting**  
    This posting type can only be created manually by the user. It represents the stock adjustment postings after stocktaking.   
    
- **Stock transfer**  
    This posting type can be created manually or automatically. It represents the stock postings for materials redistributed from a source storage shelf to a destination storage shelf. This posting type affects the actual stock in both storage shelves.    
    
- **Return**  
    This posting type can be created manually or automatically. It represents the stock postings for returned materials. This posting type affects the actual stock in the respective storage shelf. 

- **Drop shipment**   
    This posting type is created automatically by the system when a dropshipping order is received. It has no effect in the stock.

    [comment]: <> (Stimmt das so? Mehr Info dazu?)

- **Problem**  
    This posting type can only be created manually by the user. Select this option if you want to display the stock postings for materials that cannot be sold for any reason, for instance due to a defect. This posting type affects the actual stock in the respective storage shelf. 

- **Pre-reservation**  
    This posting type can be created manually or automatically. It represents the stock postings for material reserved for orders that have not been received in the system yet, that is, with no business document assigned. This can be the case, for example, when a customer places a product in the shopping cart. This posting type does not affect the actual nor the available stock in the warehouse. 

    > [Info] To be able to use pre-reservation postings in the system, your shop must support this function.  