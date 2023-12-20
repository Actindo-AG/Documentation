

# Manage the stock

The main purpose of the *Warehousing* module is to manage the stock, that is post stock in and release stock from the warehouse. You can do this manually, see...

[comment]: <> (In Overview: The *Warehousing* module is undergoing a major redesigning process and, therefore, only the most important features are described in this documentation. Oder Diese Funktion wird in absehbarer Zeit sich ändern oder wegfallen und daher wird aktuell nicht beschrieben.)


## Activate the warehouse logistics for a material

All materials created in the *Actindo Core1 Platform* are displayed in the *Article list* in the *Warehousing* module. However, a material is not relevant for the warehouse logistics by default. To be able to post stock of a specific material in the *Warehousing* module, you have to activate the warehouse logistics for that material. 

Once you have activated the warehouse logistics, the sub-tab  *Warehouse/suppliers* is displayed. As soon as a material stock has been posted, the warehouse logistics cannot be deactivated for this material. 

[comment]: <> (Artikel im Lager kommen aus Artikelverwaltung oder aus PIM kommen? Terminologie problematisch: hier ist immer die Rede von Artikel oder Produkt,  nicht Material... Sollen wir das schon mal trotz Abweichungen im UI ändern?)

Warehouse logistics cannot be activated for the following materials:  

- Master material  
    A master material is a superordinate (parent) entity that has subordinate (child) entities, that is, the material variants. A master material is an abstract entity that represents an object; the material variants, on the other hands, are the actual materials, in all its variants, that are on sale. For example, the master material "t-shirt" can have the different material variants, for instance a red t-shirt in M size and blue t-shirt in L size.

- Bundle ("soft bundle") 
    A bundle is a set of materials that are sold together. However, they are individual materials that are managed independently in the *Warehouse* module. Actually, bundle availability depends on the stock of the individual products that form the bundle. If one of them is not in stock any more, the bundle cannot be sold. 



[comment]: <> (Begriffe zu erklären: Verpackungseinheiten/packaging unit, hard bundle?)



[comment]: <> (Zur Terminologie: hier Material statt Produkt / Artikel verwenden? In UI gemischt. Master material, variant material auch ok?)

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Warehousing > Quick posting > Tab QUICK POSTING*

![Product list](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/ProductList.png "[Product list]")

1. Double-click the material for which you want to activate the warehouse logistics. Alternatively, you can right-click and select the [![Open](../../Assets/Icons/Open.png "[Open]") Open] button in the context menu.  
    The *Basic data* view is displayed.

    ![Product list](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/BasicData/BasicData.png "[Product list]")

2. Click the *Warehouse logistics active for this product* drop-down list and select **Yes** to activate the selected material.

3. Click the [SAVE] button.  
    The notice *Please wait... Saving...* is displayed while saving. The setting has been saved. The *Successfully saved** pop-up window is displayed. 

    ![Product list](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/SuccessfullySaved.png "[Product list]")

    
## Add a manual stock posting

#### Prerequisites

The warehouse logistics has been activated for the selected material, see [Activate the warehouse logistics for a material](../Operation/01_ManageStock.md#activate-warehouse-logistics-for-a-material).

#### Procedure

*Warehousing > Quick posting > Tab QUICK POSTING > Select a material > Tab Warehouse/suppliers > Sub-tab Warehouse management*

![Warehouse management](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/WarehouseManagement.png "[Warehouse management]")

1. Click the [ADD POSTING] button in the bottom left corner of the *Stocks* sections.  
    The *Add posting* window is displayed.

    ![Add posting](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/WarehouseSuppliers/WarehouseManagement/AddBooking.png "[Add posting]") 

2. Click the *Stock location* drop-down list and select the storage shelf where you want to post the stock. All available storage shelves for this material are displayed in the list.

3. Click the *Posting type* drop-down list and select the desired posting type. The following options are available:

    - **Reservation**   
        Select this option if you want to reserve a material for an open order. This reservation does not reduce the real, physical stock, only the available stock. A negative stock level can therefore result from a reservation.

    - **Sale**  
        Select this option if the ordered material has left the warehouse. This posting reduces the real, physical stock in the warehouse.

    - **Order**   
        Select this option if you want to ... This reservation ...

    - **Purchase**  
        Select this option if you want to add any purchased material to the warehouse. This posting increases the real, physical stock in the warehouse.

        [comment]: <> (physical oder available stock?)

    - **Stock adjustment posting**  
        Stock in, release from lager

    - **Stock transfer**  
        Select this option if you want to post a redistribution of a material from a source storage shelf to a destination storage shelf. If you select this posting type, the *New stock location* drop-down list is displayed.

    - **Return**  
        Select this option if you want to post a returned material. If a material is available in more than one storage shelf, the returned material will be always posted to the primary storage shelf.

    - **Problem**  
        Select this option if you want to post ...

    - **Pre-reservation**  
        Select this option if you want to post a reservation for an order that has not been received in the system yet, that is, there is no business document assigned to it yet. This can be the case, for example, when a customer places a product in the shopping cart.

3.  If you have selected the *Stock transfer* posting type, click the *New stock location* drop-down list and select the destination storage shelf. Otherwise, proceed to next step.

4. Check the material amount in the *Change* field and enter a different material amount if necessary. 

    > [Info] Bear in mind that, depending of the posting type, the sign changes. A positive value means a receipt of materials, whereas a negative value means the dispatch of materials.

5. 


## Check the stock allocation for a product 


#### Prerequisites


#### Procedure


[comment]: <> (Stock allocation for bundles: was wird im PIM zurückgespielt? Es richtet sich nach dem am Wenigsten verfügbaren Material im Lager, von den Materialien, die im Bundle hingehören. Es wird logischerweise abgerundet: wenn im Lager 3 items auf Lager sind und ein Bundle davon 2 enthält, ist Bundle stock nicht 2, sondern 1.) 