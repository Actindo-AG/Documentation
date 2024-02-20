# Activate the warehouse logistics for a product

All products created in the *Actindo Core1 Platform* are displayed in the *Product list* in the *Warehousing* module. However, a product is not relevant for the warehouse logistics by default. To be able to manage the stock for a material corresponding to a specific product in the *Warehousing* module, you have to activate the warehouse logistics for that individual product first. 

Once you have activated the warehouse logistics for a selected product, the *Warehouse/suppliers* sub-tab is displayed. As soon as a stock amount has been posted, the warehouse logistics cannot be deactivated for this product anymore. 

Not all products displayed in the product list are actual items kept in stock. The warehouse logistics cannot be activated for the following products:  

- Master product  
    A master product is a superordinate (parent) entity that has subordinate (child) entities, that is, the product variants. A master product is an abstract entity that represents an object; the product variants, on the other hand, are the actual products, in all its variants, that are on sale. For example, the master product "T-shirt" can have different product variants, for instance a red T-shirt in M size, a blue T-shirt in L size, and so on.

- Product bundle  
    A bundle is a set of products that are sold together. However, these are individual products that are managed independently in the *Warehouse* module. The bundle stock depends, therefore, on the stock of the individual products included in the bundle. If one of the products is not in stock any more, the bundle cannot be sold. 

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Warehousing > Quick posting > Tab QUICK POSTING*

![Product list](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/ProductList.png "[Product list]")

1. Double-click the product for which you want to activate the warehouse logistics. Alternatively, you can right-click and select the [![Open](../../Assets/Icons/Open.png "[Open]") Open] button in the context menu.  
    The *Basic data* sub-tab is displayed.

    ![Basic data](../../Assets/Screenshots/RetailSuiteWarehousing/QuickBooking/BasicData/BasicData.png "[Basic data]")

2. Click the *Warehouse logistics active for this product* drop-down list and select **Yes** to activate the selected product.  

3. Click the [SAVE] button.  
    The notice *Please wait... Saving...* is displayed while saving. The setting has been saved. A confirmation message is displayed. 

