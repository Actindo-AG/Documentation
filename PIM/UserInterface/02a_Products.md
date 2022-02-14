# List

*PIM > Products > Tab LIST*

![Products](/Assets/Screenshots/PIM/Products/List/Products.png "[Products]")

- *View*   
  Click the drop-down list to select the view. All created views are displayed in the drop-down list. For detailed information, see [Create a view](to_be_completed).

- *Language*   
  Click the drop-down list to select the language. All active languages are displayed in the drop-down list.

- *Scope*   
  Click the drop-down list to select the scope. All active scopes are displayed in the drop-down list. By default, the scope **Actindo Basic** is preselected.

- *Produktkategorie*   
  Click the drop-down list to select the catalog. All catalogs are displayed in the drop-down list. By default, the catalog **Produktkategorie** is preselected.


**Products**

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a product.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of products.

- *Variants*   
  Click the drop-down list to select the display settings for variants. The following settings are available:
  - **List all products**
  - **Hide child products**


- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter editing bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all products in the table are selected.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected product. This button is only displayed, when the checkbox of a product is selected. Alternatively, you can click directly a row in the table to edit a product.   
  For detailed information, see [Edit a product](to_be_completed).

- [COPY PRODUCT]   
  Click this button to copy the selected product. This button is only displayed, when the checkbox of a single product is selected.
  For detailed information, see [Copy a product](to_be_completed).

- [ARCHIVE PRODUCT] / [ARCHIVE PRODUCTS]   
  Click this button to archive the selected product(s). This button is only displayed, when the checkbox of at least one product is selected.
  For detailed information, see [Archive a product](to_be_completed).

- [MOVE TO RECYCLE BIN]   
  Click this button to move the selected product(s) to recycle bin. This button is only displayed, when the checkbox of at least one product is selected.
  For detailed information, see [Finally delete a product](to_be_completed).

- [START MASS EDITING]   
  Click this button to edit the selected products. This button is only displayed, when the checkbox of at least one product is selected. The mass editing is only recommended if you select more that one product.
  For detailed information, see [Edit multiple products](to_be_completed).

Depending on the selection in the drop-down list *Variants*, the table displays all products or all products except child products. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Bilder*   
  Image of the product.

- *SKU*   
  Stock Keeping Unit. Identification number for the product.  

- *Artikelname*   
  Name of the product.

- *Produktvarianten*   
  Variant type of the product. The following variant types are displayed:
  - Master entity with *x* children (x indicates the number of child entities for the master entity)
  - Child entity *Defining Attribute: Value* (the defining attributes and their values are indicated)
  - no variant type indicated for all products that are neither a master nor a child entity


- *Attribute Set*   
  Assigned attribute set.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system when the product is created.

- *Modified on*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the product.

- *Created on*   
  Date and time of the creation.

- *Created by*   
  Name and username of the user who created the product.

- Attribute    
  You can add a column for each attribute that is assigned to the product. The column displays the attribute name, the row displays the corresponding attribute value.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a product. The *Create new product* window is displayed.   
  For detailed information, see [Create a product](to_be_completed).


## Create new product
*PIM > Products > Tab LIST > Button Add*

![Create new product](/Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[Create new product]")

- *Select attribute set*   
  Click the drop-down list to select the attribute set for the new product. All available attribute sets are displayed in the drop-down list.

- *SKU*   
  Enter the SKU (Stock Keeping Unit) of the new product.


## Create product
*PIM > Products > Tab LIST > Button Add > Button [CREATE]*

![Create Product](/Assets/Screenshots/PIM/Products/List/CreateProduct.png "[Create Product]")

- [CANCEL]   
  Click this button to cancel the creation of a product.

- [SAVE]   
  Click this button to save the new product.

- Image box
  Image of the product. In the *Create product* view, the image box is always empty.

- *SKU*   
  Stock Keeping Unit. Identification number for the product.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the SKU.

- ![Apply](/Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the SKU. This button is only displayed when you are editing the SKU.

- *Scope*   
  Click the drop-down list to select a scope for the product. All available scopes are displayed in the drop-down list. By default, the scope **Actindo Basic** is preselected.

- *Language*   
  Click the drop-down list to select a language for the product. All available languages are displayed in the drop-down list. The default language is preselected.

- [Completeness: Not available]     
  Completeness of the product. In the *Create product* view, the completeness cannot be indicated.


### Create product - Attributes
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Attributes*

![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesCreate.png "[Attributes]")

In the left margin column, all available groups containing attributes are displayed. Click a (sub-)group to display the attributes that are assigned to this (sub-)group on the right side of the tab *Attributes*. If the product contains attributes that are unassigned, the additional group *Unassigned Group* is automatically displayed in the left margin column.

The right side of the tab *Attributes* displays all attributes that are assigned to the selected group in the left margin column. As the attributes are customized, only those attributes that are predefined by default in the attribute set *PIM Basisprodukttyp* are described below:

-- describe attributes PIM Basisprodukttyp --


### Create product - Varianten
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Varianten*

![Varianten](/Assets/Screenshots/PIM/Products/List/Varianten/VariantenCreate.png "[Varianten]")

- *Variant set*   
  Click the drop-down list to select a variant set for the product. All available variant sets are displayed in the drop-down list. The button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) is displayed in the variants box below if a variant set is selected.

**Variants box**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of products.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

The table displays all variants. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Status*  
  Status of the variant. In the *Create product* view, the status **Created after save** is displayed if you have added a variant.

- *SKU*  
  Stock Keeping Unit. Identification number for the variant. The SKU for the variant is created depending on the selected settings.

- *LifeCycle Status*   
  Status of the ???. The LifeCycle Status is created after saving. In the *Create product* view, no LifeCycle Status is displayed.

- *ID*   
  Variant identification number. The ID is created after saving. In the *Create product* view, no ID is displayed.

- Attribute    
  You can add a column for each attribute that is assigned as a defining or differing attribute to the selected variant set. The column displays the attribute name, the row displays the corresponding attribute value.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The two buttons [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ] and [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ] are displayed.


#### Add variant
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Varianten > Select variant set > Button Add*

![Add variant](/Assets/Screenshots/PIM/Products/List/Varianten/AddVariant.png "[Add variant]")

- [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add single variant* window is displayed.

- [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add multiple variant* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the variant creation and exit the current view.

#### Add single variant
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Varianten > Select variant set > Button Add > Button Add single variant*

![Add single variant](/Assets/Screenshots/PIM/Products/List/Varianten/AddSingleVariant.png "[Add single variant]")

**Additional fields**

- *sku*   
  Stock Keeping Unit. Identification number for the variant.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use formula*   
  Activate this toggle to apply the formula defined in the settings for the variant sets to the variant SKU. When the toggle is active, the field *sku* is read-only. Deactivate the toggle to enter a different SKU. By default, this toggle is active.

**Defined values**

All defining attributes of the variant are displayed in this section.

- Defining attribute
  Enter or select the appropriate value for the defining attribute.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Add single variant* window.

- [SAVE]   
  Click this button to save the variant and close the *Add single variant* window.


#### Add multiple variants
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Varianten > Select variant set > Button Add > Button Add multiple variants*

##### Select Values

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants01.png "[Add multiple variants]")

For each defining attribute a single box to define the attribute value is displayed.

> [Info] If more than one defining attribute is assigned to the variant, you have to select a value for each defining attribute to add a variant.

- [ADD ALL VALUES]   
  Click this button to add all available values to the corresponding attribute. This button is only displayed for attributes with the data type *TreeNode*.

- [ADD VALUE]   
  Click this button to add a further value to the corresponding attribute and enter  or select the desired value.

- [ABORT]   
  Click this button to cancel adding variants and close the *Select Values* window.

- [NEXT]   
  Click this button to proceed to the next step of adding variants. The *Summary* window is displayed.


##### Summary

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants02.png "[Add multiple variants]")

**Variants that will be created (ignoring duplicated)**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all variants in the table are selected.

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected variant from the list. This button is only displayed, when the checkbox of a variant is selected.

The table displays all selected variants. Depending on the settings, the displayed columns may vary.

- *sku*      
  Stock Keeping Unit. Identification number for the variant. Click this field to edit the SKU of the selected variant.

- Defining attribute
  You can add a column for each defining attribute. The column displays the attribute name, the row displays the corresponding attribute value. The fields are read-only.

- [< GO BACK]   
  Click this button to go back to the previous step. The *Select Values* window is displayed.

- [ABORT]   
  Click this button to cancel adding variants and close the *Summary* window.

- [FINISH]   
  Click this button to save the listed variants and close the *Summary* window.



### Create product - Dependencies
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Dependencies*

![Dependencies](/Assets/Screenshots/PIM/Products/List/Dependencies/DependenciesCreate.png "[Dependencies]")

 In the *Create product* view, *Information about dependencies are not available* is displayed in this tab. The dependencies are displayed only after saving.  


### Create product - Catalogs
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Catalogs*

![Catalogs](/Assets/Screenshots/PIM/Products/List/Catalogs/CatalogsCreate.png "[Catalogs]")

For each catalog a single box to assign the new product to a category is displayed. You can assign a product to several categories at the same time.

**Catalog Name**

- [EDIT ATTRIBUTE *CATALOG NAME*]   
  Click this button to assign the product to a category or a sub-category in the selected catalog. The categories window is displayed.

The box displays all selected categories and their level. All fields are read-only. If no category is selected, *No nodes selected* is displayed in the box.

- *Level 1*    
  Level 1 category name.

- *Level 2*   
  Level 2 category name. The field is only displayed, if the product is assigned to a category of level 2 or lower.

- *Level x*   
  Level x category name. The field is only displayed, if the product is assigned to a category of level x or lower. The *x* indicates the level number of the assigned category.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected category from the box. This button is only displayed, when you hover over a category in the box.


#### Categories
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Catalogs > Button [EDIT ATTRIBUTE]*

![Categories](/Assets/Screenshots/PIM/Products/List/Catalogs/Categories.png "[Categories]")

- [x]     
  Select a checkbox to assign the product to the selected category. You can select multiple checkboxes.

> [Info] Categories that are containing sub-categories are displayed with the symbol ![Folders](/Assets/Icons/Folders01.png "[Folders]") (Folders), categories without sub-categories with the symbol ![Folder](/Assets/Icons/Folder01.png "[Folder]") (Folder).    
Click the button [>] to the left of a category checkbox to display their sub-categories.

- [CANCEL]   
  Click this button to cancel selecting categories and close the categories window.

- [SAVE]   
  Click this button to save the selected categories and close the categories window.



### Create product - Associations
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Associations*

![Associations](/Assets/Screenshots/PIM/Products/List/Associations/AssociationsCreate.png "[Associations]")

**Cross Selling**

- [ADD]   
  Click this button to add an associated product for cross selling to the list. The *Filter List of Products* window is displayed.

The box displays all associated product for cross selling. All fields are read-only. If no product is selected, *No associated products selected* is displayed in the box.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.

- ![Eye](/Assets/Icons/Eye01.png "[Eye]") (Eye)   
  Click this button to display ????. This button is only displayed, when you hover over a product in the list.
  [comment]: <> (what should be displayed? For me, the loading never ends...)

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected product from the list. This button is only displayed, when you hover over a product in the list.



#### Filter List of Products
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Associations > Button [ADD]*

![Filter List of Products ](/Assets/Screenshots/PIM/Products/List/Associations/FilterListProducts.png "[Filter List of Products]")

- [CANCEL]   
  Click this button to cancel adding products and close the *Filter List of Products* window.

- [SAVE]   
  Click this button to add the selected poducts to the list and close the *Filter List of Products* window.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a product.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of products.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all products in the table are selected.

The table displays all products. All fields are read-only.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.


### Create product - UCS Lager
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab UCS Lager*

![UCS Lager](/Assets/Screenshots/PIM/Products/List/UCSLager/UCSLagerCreate.png "[UCS Lager]")

 In the *Create product* view, *Available after saving the product.* is displayed in this tab. The UCS Lager information is displayed only after saving.  


### Create product - UCS Marktplätze
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab UCS Marktplätze*

![UCS Marktplätze](/Assets/Screenshots/PIM/Products/List/UCSMarktplätze/UCSMarktplätzeCreate.png "[UCS Marktplätze]")

 In the *Create product* view, *Available after saving the product.* is displayed in this tab. The UCS Marktplätze information is displayed only after saving.  


### Create product - Offers
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Offers*

![Offers](/Assets/Screenshots/PIM/Products/List/Offers/OffersCreate.png "[Offers]")

**Channel Offers**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all offers in the table are selected.

The table displays all created offers to this product. All fields are read-only.

- *SKU*   
  Stock Keeping Unit. Identification number of the product. In the *Create product* view, **TO BE GENERATED** is displayed.

- *Status*   
  Connection status of the offer. In the *Create product* view, **Not available** is displayed.

- *Pending status/Errors*   
  Indication of the pending status or an error for this offer. The pending status is displayed if you have changed the offer status via the editing bar. An error is displayed if ???
  [comment]: <> (when is an error displayed here?)

- *Connection*   
  Connection name of the offer.

- *Attribute Set*   
  Attribute set name of the offer.

- *last edited*   
  Date and time of the last modification. In the *Create product* view, no date is displayed.

- *Modified by*   
  Name and username of the user who modified the product. In the *Create product* view, no name is displayed.

- *ChangeTracking*   
  ETL mode of the offer. The following modes are available:
  - **Initial**: Changes in a PIM product must be triggered manually to be applied to the offers.   
  - **Automatic**: Changes in a PIM product are automatically applied to the offers.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *Created*   
  Date and time of the creation. In the *Create product* view, no date is displayed.

- *Creator*   
  Name and username of the user who created the product. In the *Create product* view, no name is displayed.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The two buttons [Add to a single channel ![Document](/Assets/Icons/Document.png "[Document]") ] and [Add to multiple channels ![Documents](/Assets/Icons/Documents.png "[Documents]") ] are displayed.

- *Status*   
  Click the drop-down list to change the offer status. The selected status is displayed in the column *Pending status/Errors*. This drop-down list is only displayed, when the checkbox of an offer is selected. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Not available**: The offer is unknown to the marketplace and therefore cannot be sold there.


- *Change Tracking*   
  Click the drop-down list to change the ETL mode of the offer. The selected ETL mode is displayed in the column *ChangeTracking*. This drop-down list is only displayed, when the checkbox of an offer is selected. The following ETL modes are available:    
  - **manual**: Changes in a PIM product must be triggered manually to be applied to the offers.   
  - **automatic**: Changes in a PIM product are automatically applied to the offers.


- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected offer from the list. This button is only displayed, when the checkbox of an offer is selected.


#### Add channel
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Offers > Button Add*

![Add](/Assets/Screenshots/PIM/Products/List/Offers/AddCreate.png "[Add]")

- [Add to a single channel ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add to a single channel* window is displayed.

- [Add to multiple channels ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add to multiple channels* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the channel creation and exit the current view.


#### Add to a single channel
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Offers > Button Add > Button Add to a single channel*

![Add to a single channel](/Assets/Screenshots/PIM/Products/List/Offers/SingleChannel.png "[Add to a single channel]")

**Create Channels Offer**

- *Select Connection*   
  Click the drop-down list to select a connection for the offer. All available connections are displayed in the list.

- *Select Attribute Set*   
  Click the drop-down list to select an attribute set for the offer. All available attribute sets are displayed in the drop-down list. The drop-down list is locked if no connection is selected.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Generate SKU*   
  Activate this toggle to automatically generate a SKU for the offer. Deactivate the toggle to enter a SKU manually. By default, this toggle is active.

- *SKU*    
  Enter a SKU (Stock Keeping Unit) for the offer.  
    --> offer or product? how does this work? When I enter a different SKU, The SKU is automatically overwritten.

- *ETL mode*   
  Select an ETL mode:    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **N/A**: The offer is unknown to the marketplace and therefore cannot be sold there.


- [CANCEL]   
  Click this button to cancel adding a channel and close the *Create Channels Offer* window.

- [SAVE]   
  Click this button to save the channel and close the *Create Channels Offer* window.


#### Add to multiple channels
*PIM > Products > Tab LIST > Button Add > Button [CREATE] > Tab Offers > Button Add > Button Add to multiple channels*

##### Select Channels and status

![Add to multiple channels](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels1.png "[Add to multiple channels]")

**Select status and change tracking mode**

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Not available**: The offer is unknown to the marketplace and therefore cannot be sold there.


- Select an ETL mode:    
 ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
 ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.


**Select connections**

- [SELECT ALL]   
  Click this button to select all available connections.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Connection name*     
  Activate this toggle to select the channel for creating an offer. All available connections are displayed. By default, all toggles are inactive.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Select Channels and status* window.

- [CONTINUE]   
  Click this button to proceed to the next step for adding channels. The *Select destination attribute sets* window is displayed.


##### Select destination attribute sets

![Add to multiple channels](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels2.png "[Add to multiple channels]")

- *Destination set for connection*   
  Destination set for the selected connection. The destination set is automatically selected. The field is read-only. A destination set is displayed for each selected connection.

- [< BACK]   
  Click this button to go back to the previous step. The *Select Channels and status* window is displayed.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Select destination attribute sets* window.

- [FINISH]   
  Click this button to save the channel(s) and close the *Select destination attribute sets* window.

-------------

## Edit product
*PIM > Products > Tab LIST > Select product*

![Edit Product](/Assets/Screenshots/PIM/Products/List/EditProduct.png "[Edit Product]")

- [CANCEL]   
  Click this button to cancel editing the product.

- [SAVE]   
  Click this button to save the changes to the product.

- Image box
  Image of the product. The image is displayed if an image is selected for the product in the tab *Attributes*.

- *SKU*   
  Stock Keeping Unit. Identification number for the product.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the SKU.

- ![Apply](/Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the SKU. This button is only displayed when you are editing the SKU.

- *Scope*   
  Click the drop-down list to select a scope for the product. All available scopes are displayed in the drop-down list.

- *Language*   
  Click the drop-down list to select a language for the product. All available languages are displayed in the drop-down list.

- [Complete]     
  Completeness of the product for all available scopes and languages. The percentage of completeness is displayed in the button. Click the button to display the *Completeness* window. If the completeness is less than 100%, the number of missing require attributes is displad to the right of the completeness button.
  If the completeness cannot be calculated, *Completeness: Not available* is displayed and the button is not clickable.

  > [Info] The completeness is calculated by considering the number of missing required fields. As the required fields are defined individually for each attribute set set, it can vary from one product to another.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *show empty required attributes only*     
  Activate this toggle to display only the missing required fields in the tab *Attributes* for this product. By default, the toggle is inactive. The toggle is only displayed if at least one required field is missing.

- *Sets*   
  Click the drop-down list to change the attribute set (attribute set) for the product. All available attribute sets are displayed in the drop-down list. The currently selected attribute set is highlighted in bold.

  > [Info] Changing the attribute set can destroy data. Therefore, an additional message is displayed to confirm the attribute set change. Note, that the change cannot be undone once you have saved the changes.


### Edit product - Completeness
*PIM > Products > Tab LIST > Select product > Button Complete*

![Completeness](/Assets/Screenshots/PIM/Products/List/Completeness.png "[Completeness]")

- *Scopes*   
  Click the drop-down list to change the scope for the product completeness calculation. All available scopes, the option **Scopes (All)** and the option **Not multiscope** are displayed in the drop-down list. By default, the option **Scopes (All)** is preselected.

  > [Info] The product completeness for the selected scope is only displayed in the *Completeness* window. The completeness button in the *Edit Product* view is not affected by this change.

- *Languages*   
  Click the drop-down list to change the language for the product completeness calculation. All available languages, the option **Languages (All)** and the option **Not multilanguage** are displayed in the drop-down list. By default, the option **Languages (All)** is preselected.

  > [Info] The product completeness for the selected language is only displayed in the *Completeness* window. The completeness button in the *Edit Product* view is not affected by this change.

- Percentage
  The current percentage for the product completeness of the selected scope and language is displayed. The percentage is automatically updated when you select a different scope or language.


### Edit product - Attributes
*PIM > Products > Tab LIST > Select product > Tab Attributes*

![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesEdit.png "[Attributes]")

In the left margin column, all available groups containing attributes are displayed. Click a (sub-)group to display the attributes that are assigned to this (sub-)group on the right side of the tab *Attributes*. If the product contains attributes that are unassigned, the additional group *Unassigned Group* is automatically displayed in the left margin column.

The right side of the tab *Attributes* displays all attributes that are assigned to the selected group in the left margin column. As the attributes are customized, only those attributes that are predefined by default in the attribute set *PIM Basisprodukttyp* are described below:

-- describe attributes PIM Basisprodukttyp --


### Edit product - Varianten
*PIM > Products > Tab LIST >  Select product > Tab Varianten*

![Varianten](/Assets/Screenshots/PIM/Products/List/Varianten/VariantenEdit.png "[Varianten]")

- *Variant set*   
  Click the drop-down list to select a variant set for the product. All available variant sets are displayed in the drop-down list. The button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) is displayed in the variants box below if a variant set is selected.
  If the product is a master entity, the corresponding variant set is preselected in the drop-down list. The drop-down list is locked. The corresponding child entities  and the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) are displayed in the variants box.
  If the product is a child entity, the drop-down list is not displayed.

- *Child Entity*
  Indication that thee selected product is a child entity. This field is read-only. The value can be changed within the tab *Attributes*. The field is only displayed for variant articles.

-> how is it possible to change the value of a variant defining attribute in the tab Attributes without changing the variant?


**Variants box**

> [Info] If the product is a child entity, the variants box is not displayed.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of products.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

The table displays all variants. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Status*  
  Status of the variant. The following statuses are available:
  - **Created after save**: The added variant is created after saving the product.
  - **Created**: The variant is already created.


- *SKU*  
  Stock Keeping Unit. Identification number for the variant. The SKU for the variant is created depending on the selected settings.

- *LifeCycle Status*   
  Life cycle status of the variant article. The following statuses are available:
  - **active**: The variant is active.
  - **in_archive**: The variant is archived.
  - **in_recycle_bin**: The variant is moved to the recycle bin.


- *ID*   
  Variant identification number. The ID is automatically assigned by the system after saving.

- Attribute    
  You can add a column for each attribute that is assigned as a defining or differing attribute to the selected variant set. The column displays the attribute name, the row displays the corresponding attribute value.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The two buttons [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ] and [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ] are displayed.


#### Add variant
*PIM > Products > Tab LIST > Select product > Tab Varianten > Select variant set > Button Add*

![Add variant](/Assets/Screenshots/PIM/Products/List/Varianten/AddVariantEdit.png "[Add variant]")

- [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add single variant* window is displayed.

- [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add multiple variant* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the variant creation and exit the current view.

#### Add single variant
*PIM > Products > Tab LIST > Select product > Tab Varianten > Select variant set > Button Add > Button Add single variant*

![Add single variant](/Assets/Screenshots/PIM/Products/List/Varianten/AddSingleVariant.png "[Add single variant]")

**Additional fields**

- *sku*   
  Stock Keeping Unit. Identification number for the variant.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use formula*   
  Activate this toggle to apply the formula defined in the settings for the variant sets to the variant SKU. When the toggle is active, the field *sku* is read-only. Deactivate the toggle to enter a different SKU. By default, this toggle is active.

**Defined values**

All defining attributes of the variant are displayed in this section.

- Defining attribute
  Enter or select the appropriate value for the defining attribute.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Add single variant* window.

- [SAVE]   
  Click this button to save the variant and close the *Add single variant* window.


#### Add multiple variants
*PIM > Products > Tab LIST > Select product > Tab Varianten > Select variant set > Button Add > Button Add multiple variants*

##### Select Values

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants01.png "[Add multiple variants]")

For each defining attribute a single box to define the attribute value is displayed.

> [Info] If more than one defining attribute is assigned to the variant, you have to select a value for each defining attribute to add a variant.

- [ADD ALL VALUES]   
  Click this button to add all available values to the corresponding attribute. This button is only displayed for attributes with the data type *TreeNode*.

- [ADD VALUE]   
  Click this button to add a further value to the corresponding attribute and enter  or select the desired value.

- [ABORT]   
  Click this button to cancel adding variants and close the *Select Values* window.

- [NEXT]   
  Click this button to proceed to the next step of adding variants. The *Summary* window is displayed.


##### Summary

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants02.png "[Add multiple variants]")

**Variants that will be created (ignoring duplicated)**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all variants in the table are selected.

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected variant from the list. This button is only displayed when the checkbox of a variant is selected.

The table displays all selected variants. Depending on the settings, the displayed columns may vary.

- *sku*      
  Stock Keeping Unit. Identification number for the variant. Click this field to edit the SKU of the selected variant.

- Defining attribute
  You can add a column for each defining attribute. The column displays the attribute name, the row displays the corresponding attribute value. The fields are read-only.

- [< GO BACK]   
  Click this button to go back to the previous step. The *Select Values* window is displayed.

- [ABORT]   
  Click this button to cancel adding variants and close the *Summary* window.

- [FINISH]   
  Click this button to save the listed variants and close the *Summary* window.



### Edit product - Dependencies
*PIM > Products > Select product > Tab Dependencies*

![Dependencies](/Assets/Screenshots/PIM/Products/List/Dependencies/DependenciesEdit.png "[Dependencies]")

**Dependencies**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of product dependencies.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependent entities in the table are selected.

The table displays all dependencies of the selected product. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Dependent entity id*   
  Identification number of the dependent entity.

- *Dependent entity type*   
  Type of the dependent entity. The following types can be displayed:
  - **Channels Offer**
  - **UCS Artikel**
  [comment]: <> (what else?)


- *Change tracking*   
  ETL mode of the dependent entity. The following modes can be displayed:
  - **manual**: Changes in a PIM product must be triggered manually to be applied to the offers.   
  - **automatic**: Changes in a PIM product are automatically applied to the offers.
  [comment]: <> (is that right?)


- *Dependent entity friendly identifier*   
[comment]: <> (what id number is that? How is it created?)

- [RERUN MAPPING]   
  Click this button to rerun the mapping of the product and the selected entity. This button is only displayed when the checkbox of a dependent entity is selected.



### Edit product - Completeness
*PIM > Products > Select product > Tab Completeness*

![Completeness](/Assets/Screenshots/PIM/Products/List/Completeness/Completeness.png "[Completeness]")

The tab *Completeness* is only displayed if the completeness of the product has been calculated and is displayed in the header section of the *Edit product* view. The tab is never displayed in the *Create product* view.

- *Not scopable*   
  This box displays the percentage for the product completeness of the selected product without any scope dependency.
  - *Single Language*   
    The box displays the percentage for the product completeness of the selected product without any scope dependency and regarding the single default language only.
  [comment]: <> (is that right?)


- Scope name
  This box displays the percentage for the product completeness of the selected product regarding the assigned scope. A single box is displayed for each scope.
  - Language   
    The box displays the percentage for the product completeness of the selected product regarding the assigned scope and language. A single percentage is displayed for each available language.
  [comment]: <> (is that right?)


- ![Info](/Assets/Icons/Info.png "[Info]") (Info)   
  Hover over this icon to display a box that is listing the missing attribute values. This icon is only displayed when required attribute values for the product completeness are missing.


### Edit product - Catalogs
*PIM > Products > Select product > Tab Catalogs*

![Catalogs](/Assets/Screenshots/PIM/Products/List/Catalogs/CatalogsEdit.png "[Catalogs]")

For each catalog a single box to assign the new product to a category is displayed. You can assign a product to several categories at the same time.

**Catalog Name**

- [EDIT ATTRIBUTE *CATALOG NAME*]   
  Click this button to assign the product to a category or a sub-category in the selected catalog. The categories window is displayed.

The box displays all selected categories and their level. All fields are read-only. If no category is selected, *No nodes selected* is displayed in the box.

- *Level 1*    
  Level 1 category name.

- *Level 2*   
  Level 2 category name. The field is only displayed, if the product is assigned to a category of level 2 or lower.

- *Level x*   
  Level x category name. The field is only displayed, if the product is assigned to a category of level x or lower. The *x* indicates the level number of the assigned category.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected category from the box. This button is only displayed, when you hover over a category in the box.


#### Categories
*PIM > Products > Select product > Tab Catalogs > Button [EDIT ATTRIBUTE]*

![Categories](/Assets/Screenshots/PIM/Products/List/Catalogs/Categories.png "[Categories]")

- [x]     
  Select a checkbox to assign the product to the selected category. You can select multiple checkboxes.

> [Info] Categories that are containing sub-categories are displayed with the symbol ![Folders](/Assets/Icons/Folders01.png "[Folders]") (Folders), categories without sub-categories with the symbol ![Folder](/Assets/Icons/Folder01.png "[Folder]") (Folder).    
Click the button [>] to the left of a category checkbox to display their sub-categories.

- [CANCEL]   
  Click this button to cancel selecting categories and close the categories window.

- [SAVE]   
  Click this button to save the selected categories and close the categories window.



### Edit product - Associations
*PIM > Products > Select product > Tab Associations*

![Associations](/Assets/Screenshots/PIM/Products/List/Associations/AssociationsEdit.png "[Associations]")

**Cross Selling**

- [ADD]   
  Click this button to add an associated product for cross selling to the list. The *Filter List of Products* window is displayed.

The box displays all associated product for cross selling. All fields are read-only. If no product is selected, *No associated products selected* is displayed in the box.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.

- ![Eye](/Assets/Icons/Eye01.png "[Eye]") (Eye)   
  Click this button to display ????. This button is only displayed, when you hover over a product in the list.
  [comment]: <> (what should be displayed? For me, the loading never ends...)

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected product from the list. This button is only displayed, when you hover over a product in the list.



#### Filter List of Products
*PIM > Products > Select product > Tab Associations > Button [ADD]*

![Filter List of Products ](/Assets/Screenshots/PIM/Products/List/Associations/FilterListProducts.png "[Filter List of Products]")

- [CANCEL]   
  Click this button to cancel adding products and close the *Filter List of Products* window.

- [SAVE]   
  Click this button to add the selected poducts to the list and close the *Filter List of Products* window.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a product.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of products.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all products in the table are selected.

The table displays all products. All fields are read-only.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.



### Edit product - History
*PIM > Products > Select product > Tab History*

![History](/Assets/Screenshots/PIM/Products/List/History/History.png "[History]")

The tab *History* is only displayed in the *Edit product* view. The tab is never displayed in the *Create product* view.

**History**

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a change.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of changes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter editing bar and customize the active filters. The *x* indicates the number of filters that are currently active.

The table displays the change history of the product. All fields are read-only. Depending on the settings, the displayed columns may vary.

- [x]     
  Select the checkbox to display the editing toolbar.

- *Date*   
  Date and time of the change.

- *Author*   
  Name and username of the user who modified the product.

- *Changed Elements*   
  List of elements that were changed.

- *ID*   
  Identification number of the change. The ID number is automatically assigned by the system.  

- ![Eye](/Assets/Icons/Eye01.png "[Eye02]") (Eye)   
  Click this button to display the *History (Single Entry)* window. This button is only displayed, when the checkbox of a change is selected. Alternatively, you can click directly a row in the table to display the *History (Single Entry)* window.   


#### History (Single Entry)
*PIM > Products > Select product > Tab History > Select checkbox > Button Eye*

![History](/Assets/Screenshots/PIM/Products/List/History/HistorySingleEntry.png "[History]")

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a change entry.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of change entries.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter editing bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all change entries in the table are selected.

- ![Lock](/Assets/Icons/Lock01.png "[Lock]") (Lock)   
  This entry is locked and cannot be undone. It cannot be selected. The corresponding entry row is grayed out.

The table displays the single entries of the selected product change. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Attribute name*   
  Name of the attribute to which the change was made.

- *Scope name*   
  Name of the scope to which the change was made.

- *Language name*   
  Name of the language to which the change was made

- *Old value*   
  Attribute value before change. If the field is empty, no value was set for this attribute before change.  

- *New value*   
  Attribute value after change.  

- *ID*   
  Identification number of the change entry. The ID number is automatically assigned by the system.  

- ![Undo](/Assets/Icons/Undo01.png "[Undo]") (Undo)   
  Click this button to undo the selected change(s). An additional message is displayed to confirm the change reversion. This button is only displayed, when the checkbox of a change entry is selected.


### Edit product - UCS Lager
*PIM > Products > Select product > Tab UCS Lager*

![UCS Lager](/Assets/Screenshots/PIM/Products/List/UCSLager/UCSLagerEdit.png "[UCS Lager]")

This tab displays the sub-tabs *Basisdaten* and *Lager/Lieferanten*. These sub-tabs are excerpts from the tabs in the *Lager* module: *Lager > SCHNELLBUCHEN > Select article*

- [HILFE]   


- [SPEICHERN]



#### UCS Lager - Basisdaten
*PIM > Products > Select product > Tab UCS Lager > Tab Basisdaten*

![UCS Lager Basisdaten](/Assets/Screenshots/PIM/Products/List/UCSLager/Basisdaten.png "[UCS Lager Basisdaten]")

**Artikeldaten**

- *Lageristik für diesen Artikel aktiv:*   
  Click the drop-down list to select an option. The following options are available:    
  - **Ja**:
  - **Nein**:  


- *Streckengeschäft aktiv:*    
  Click the drop-down list to select an option. The following options are available:    
  -  **Nein**:  
  - **Ja**:
  - **Immer**:  


- *Seriennummern-Artikel:*   
  Click the drop-down list to select an option. The following options are available:    
  - **Nein**:
  - **Ja**:  



#### UCS Lager - Lager/Lieferanten
*PIM > Products > Select product > Tab UCS Lager > Tab Lager/Lieferanten*

This tab displays the sub-tabs *Lagerverwaltung*, *Lagerhistorie* and *Lieferantenzuordnung/Bestelloption*. The tab and its sub-tabs are identical to the tab *Lager/Lieferanten* in the *Lager* module: *Lager > SCHNELLBUCHEN > Select article > Tab Lager/Lieferanten*

##### Lagerverwaltung
*PIM > Products > Select product > Tab UCS Lager > Tab Lager/Lieferanten > Tab Lagerverwaltung*

![UCS Lager Lagerverwaltung](/Assets/Screenshots/PIM/Products/List/UCSLager/Lagerverwaltung.png "[UCS Lager Lagerverwaltung]")

**Lagerorte**

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all change entries in the table are selected.

- *Lager-ID.*   

- *Lager-Nr.*    

- *Lager*   

- *Lager-Fach*   

- *ist Primärlager*   

- *(Bestand)*             

- *Sperrlager*   

- [NEU]   

- [LÖSCHEN]   

- ![Refresh](/Assets/Icons/Refresh03.png "[Refresh]") (Refresh)   
  Click this button to update the table of warehouses.

**Hinzufügen**

- *Lager-Nr.*    

- *Lager-Fach*   

- [BAUMANSICHT]

- *Lager-Fach*   

[comment]: <> (Is the second *Lager-Fach* and the button [BAUMANSICHT] a bug? It's hidden when a warehouse is selected in the drop-down list *Lager-Nr.*...)

- *ist Primärlager* ![checkbox](/Assets/Icons/checkbox.png "[checkbox]")        

- [SPEICHERN]

- *Sperrlager*   

- [LEEREN]


**Bestände**

- *Lager*   

- *Bestand*   

- *Reserviert*   

- *Lagerverfügbarkeit*   

- *Bestellt*   

- *Verfügbar*   

- *Gesamt*   

- *Gesamt [SPERRLAGER]*   

- [BESTANDSZUTEILUNG ANZEIGEN]



##### Lagerhistorie
*PIM > Products > Select product > Tab UCS Lager > Tab Lager/Lieferanten > Tab Lagerhistorie*

![UCS Lager Lagerhistorie](/Assets/Screenshots/PIM/Products/List/UCSLager/Lagerhistorie.png "[UCS Lager Lagerhistorie]")

- *Lagerort:*   

- *Buchungstyp:*   

- [EXCEL]   

- *Kd-Nr.*    

- *Kunde*   

- *Beleg*   

- *Menge*   

- *Preis*             

- *Preis ges.*   

- *Datum*    

- *Buchungsart*   

- *Lager*   

- *Fachbez. bei Buchung*   

- *Fachbez. aktuell*             

- *Bewegung*

- *Bestand ges.*    

- *Verfügbar ges.*   

- *Bemerkung*   

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the warehouse history.

- [ZURÜCKSETZEN]   



##### Lieferantenzuordnung/Bestelloption
*PIM > Products > Select product > Tab UCS Lager > Tab Lager/Lieferanten > Tab Lagerverwaltung*

![UCS Lager Lieferantenzuordnung/Bestelloption](/Assets/Screenshots/PIM/Products/List/UCSLager/Lieferantenzuordnung.png "[UCS Lager Lieferantenzuordnung/Bestelloption]")

**Lieferanten**

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all change entries in the table are selected.

- *Lft.-Nr.*   

- *Firma*   

- *Einkaufspreis*    

- *EK-Datum*   

- *Artikel-Nr*   

- *Lieferzeit ⌀*   

- *Lieferbar*             

- *Strecke*   

- *Grundeinkaufspreis*

- [NEU]   

- [LÖSCHEN]   

- ![Refresh](/Assets/Icons/Refresh03.png "[Refresh]") (Refresh)   
  Click this button to update the table of suppliers.


**Hinzufügen**

- *Lieferant:*   

- *Art-Nr. beim Lft:*   

- *Losgröße:*    

- *durchschn. Lieferzeit:*   

- *Datum des EK:*   

- *Lagerstückzahl beim Lft:*   

- *Datum d. LagerstückzahL:*             

- *Nicht lieferbar:*   

- *Lieferbar ab:*   

- *Streckengeschäft möglich:*   

- [SPEICHERN]   

- [LEEREN]   

**Einkaufspreise**

- *EK*   

- *Preisgrp. 1*    

- *Ab Stk*   

- *Preisgrp. 2*    

- *Ab Stk*   

- *Preisgrp. 3*    

- *Ab Stk*   

- *Preisgrp. 4*    

- *Ab Stk*   

**Langtext**

- Schriftart   

- Text vergrößern   

- Text verkleinern   

- Schriftfarbe   

- Text farblich hervorheben   

- Hyperlink   

- Nummerierte Liste   

- Aufzählungsliste   

- Source bearbeiten

- *Als Artikel-Langtext verwenden:*   



**Bestellwesen**

- *Lagerrichweite - Kalkulationsgrundlage:*   

- *Mindestbestand:*             

- *Mindestbestellmenge:*      

- *insges. eingekaufte Menge:*

- *letzte eingekaufte Menge:*   

- *letzter Einkauf:*   


**Offene Bestellungen**

- [EXCEL]   

- *Lft-Nr.*   

- *Lft-Name*             

- *Belegnr*

- *Datum*    

- *Bestellt*   

- *Offen*   

- *Vsl. Lieferdatum*   

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the warehouse history.

- [ZURÜCKSETZEN]   


### Edit product - UCS Marktplätze
*PIM > Products > Select product > Tab UCS Marktplätze*

![UCS Marktplätze](/Assets/Screenshots/PIM/Products/List/UCSMarktplätze/UCSMarktplätzeEdit.png "[UCS Marktplätze]")

 In the *Create product* view, *Available after saving the product.* is displayed in this tab. The UCS Marktplätze information is displayed only after saving.  

- [HILFE]   

- [SPEICHERN]   



#### UCS Marktplätze - Basisdaten
*PIM > Products > Select product > Tab UCS Marktplätze > Tab Basisdaten*

![UCS Marktplätze Basisdaten](/Assets/Screenshots/PIM/Products/List/UCSMarktplätze/Basisdaten.png "[UCS Marktplätze Basisdaten]")

**Artikeldaten**

- *Shop-Artikel:*

[comment]: <> (Shop über Multimarkets muss angebunden sein/Multimarkets-Kanäle müssen angebunden sein)


#### UCS Marktplätze - Webshop
*PIM > Products > Select product > Tab UCS Marktplätze > Tab Webshop*

![UCS Marktplätze Webshop](/Assets/Screenshots/PIM/Products/List/UCSMarktplätze/Webshop.png "[UCS Marktplätze Webshop]")

[comment]: <> (Shop über Multimarkets muss angebunden sein)


### Edit product - Offers
*PIM > Products > Select product > Tab Offers*

![Offers](/Assets/Screenshots/PIM/Products/List/Offers/OffersEdit.png "[Offers]")

**Channel Offers**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all offers in the table are selected.

The table displays all created offers to this product. All fields are read-only.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Status*   
  Connection status of the offer. The following statuses are available:
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Not available**: The offer is unknown to the marketplace and therefore cannot be sold there.

- *Pending status/Errors*   
  Indication of the pending status or an error for this offer. The pending status is displayed if you have changed the offer status via the editing bar. The displayed statuses are identical to the statuses in the column *Status*. An error is displayed if ???
  [comment]: <> (when is an error displayed here?)

- *Connection*   
  Connection name of the offer.

- *Attribute Set*   
  Attribute set name of the offer.

- *last edited*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the product.

- *ChangeTracking*   
  ETL mode of the offer. The following modes are available:
  - **Initial**: Changes in a PIM product must be triggered manually to be applied to the offers.   
  - **Automatic**: Changes in a PIM product are automatically applied to the offers.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *Created*   
  Date and time of the creation.

- *Creator*   
  Name and username of the user who created the product.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The two buttons [Add to a single channel ![Document](/Assets/Icons/Document.png "[Document]") ] and [Add to multiple channels ![Documents](/Assets/Icons/Documents.png "[Documents]") ] are displayed.

- *Status*   
  Click the drop-down list to change the offer status. The selected status is displayed in the column *Pending status/Errors*. This drop-down list is only displayed, when the checkbox of an offer is selected. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Not available**: The offer is unknown to the marketplace and therefore cannot be sold there.


- *Change Tracking*   
  Click the drop-down list to change the ETL mode of the offer. The selected ETL mode is displayed in the column *ChangeTracking*. This drop-down list is only displayed, when the checkbox of an offer is selected. The following ETL modes are available:    
  - **manual**: Changes in a PIM product must be triggered manually to be applied to the offers.   
  - **automatic**: Changes in a PIM product are automatically applied to the offers.


- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected offer from the list. This button is only displayed, when the checkbox of an offer is selected.


#### Add channel
*PIM > Products > Select product > Tab Offers > Button Add*

![Add](/Assets/Screenshots/PIM/Products/List/Offers/AddEdit.png "[Add]")

- [Add to a single channel ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add to a single channel* window is displayed.

- [Add to multiple channels ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add to multiple channels* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the channel creation and exit the current view.


#### Add to a single channel
*PIM > Products > Select product > Tab Offers > Button Add > Button Add to a single channel*

![Add to a single channel](/Assets/Screenshots/PIM/Products/List/Offers/SingleChannel.png "[Add to a single channel]")

**Create Channels Offer**

- *Select Connection*   
  Click the drop-down list to select a connection for the offer. All available connections are displayed in the drop-down list.

- *Select Attribute Set*   
  Click the drop-down list to select an attribute set for the offer. All available attribute sets are displayed in the drop-down list. The drop-down list is locked if no connection is selected.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Generate SKU*   
  Activate this toggle to automatically generate a SKU for the offer. Deactivate the toggle to enter a SKU manually. By default, this toggle is active.

- *SKU*    
  Enter a SKU (Stock Keeping Unit) for the offer.  
[comment]: <> (offer or product? how does this work? When I enter a different SKU, The SKU is automatically overwritten.)

- *ETL mode*   
  Select an ETL mode:    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **N/A**: The offer is unknown to the marketplace and therefore cannot be sold there.


- [CANCEL]   
  Click this button to cancel adding a channel and close the *Create Channels Offer* window.

- [SAVE]   
  Click this button to save the channel and close the *Create Channels Offer* window.


#### Add to multiple channels
*PIM > Products > Select product > Tab Offers > Button Add > Button Add to multiple channels*

##### Select Channels and status

![Add to multiple channels](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels1.png "[Add to multiple channels]")

**Select status and change tracking mode**

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Not available**: The offer is unknown to the marketplace and therefore cannot be sold there.


- Select an ETL mode:    
 ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
 ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.


**Select connections**

- [SELECT ALL]   
  Click this button to select all available connections.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Connection name*     
  Activate this toggle to select the channel for creating an offer. All available connections are displayed. By default, all toggles are inactive.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Select Channels and status* window.

- [CONTINUE]   
  Click this button to proceed to the next step for adding channels. The *Select destination attribute sets* window is displayed.


##### Select destination attribute sets

![Add to multiple channels](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels2.png "[Add to multiple channels]")

- *Destination set for connection*   
  Destination set for the selected connection. The destination set is automatically selected. The field is read-only. A destination set is displayed for each selected connection.

- [< BACK]   
  Click this button to go back to the previous step. The *Select Channels and status* window is displayed.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Select destination attribute sets* window.

- [FINISH]   
  Click this button to save the channel(s) and close the *Select destination attribute sets* window.
