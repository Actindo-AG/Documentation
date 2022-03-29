# List

*PIM > Products > Tab LIST*

![Products](/Assets/Screenshots/PIM/Products/List/Products.png "[Products]")

- *View*   
  Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu and create or edit a view. For detailed information, see [Create a view](/PIM/Operation/04_ManageView.md#create-a-view).

  - View context menu   
    Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![Create](/Assets/Icons/Plus06.png "[Create]") create   
      Click this entry to create a view. The *Create view* window is displayed.

    - ![Rename](/Assets/Icons/Edit02.png "[Rename]") rename    
      Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed when a view is selected.

    - ![Reset](/Assets/Icons/Reset.png "[Reset]") reset    
      Click this entry to reset the view to the selected views settings. This menu entry is only displayed when a view is selected and any changes are made to the views settings.

    - ![Publish](/Assets/Icons/Publish.png "[Publish]") publish    
      Click this entry to publish the view. This menu entry is only displayed when a view is selected and unpublished.

    - ![Unpublish](/Assets/Icons/Unpublish.png "[Unpublish]") unpublish    
      Click this entry to unpublish the view. This menu entry is only displayed when a view is selected and published.

    - ![Save](/Assets/Icons/Save.png "[Save]") save    
      Click this entry to save the current view settings in the selected view. This menu entry is only displayed when a view is selected.

      > [Info] When the settings of a view have been changed, an asterisk is displayed behind the views name. The asterisk is hidden as soon as the changes have been saved saved.

    - ![Delete](/Assets/Icons/Trash01.png "[Delete]") delete    
      Click this entry to delete the selected view. The A confirmation window to confirm the deletion is displayed. This menu entry is only displayed when a view is selected.

[comment]: <> (when can I reset a view? -> cannot track when this entry is displayed; where is a view published?)

- *Language*   
  Click the drop-down list to select the language. All languages, that are active in *PIM* are displayed in the drop-down list. For detailed information, see [Select a language](/PIM/Operation/04_ManageView.md#select-a-language).

- *Channel*   
  Click the drop-down list to select the channel. All channels that are active in *PIM* are displayed in the drop-down list. By default, the **Actindo Basic** channel is preselected. For detailed information, see [Select a channel](/PIM/Operation/04_ManageView.md#select-a-channel).

[comment]: <> (List needs title)

- *Catalog*   
  Click the drop-down list to select the catalog. All catalogs are displayed in the drop-down list. After having selected a catalog, all categories and sub-categories of the selected catalog are displayed. Click a category or sub-category to limit the product list to those products that are assigned to the selected category. By default, the **Product Categories** catalog is preselected. For detailed information, see [Select a product category](/PIM/Operation/04_ManageView.md#select-a-product-category).


**Products**

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a product.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of products.

- *Variants*   
  Click the drop-down list to select the display settings for variants. The following settings are available:
  - **All products**: All products and their variants are displayed in the product list.   
  - **Hide variants**: No variants are displayed in the product list.
  For detailed information, see [Select a variant view](/PIM/Operation/04_ManageView.md#select-a-variant-view).


- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all products in the list are selected.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected product(s). This button is only displayed, when the checkbox of at least one product is selected. Alternatively, you can click directly a row in the list to edit a product.   
  For detailed information, see [Edit a product](/PIM/Operation/01_ManageProducts.md#edit-a-single-product).

- [COPY PRODUCT]   
  Click this button to copy the selected product. This button is only displayed, when the checkbox of a single product is selected.
  For detailed information, see [Copy a product](/PIM/Operation/01_ManageProducts.md#copy-a-product).

- [ARCHIVE PRODUCT] / [ARCHIVE PRODUCTS]   
  Click this button to archive the selected product(s). This button is only displayed, when the checkbox of at least one product is selected.
  For detailed information, see [Archive a product](/PIM/Operation/03_MoveProducts.md#archive-a-product).

- [MOVE TO RECYCLE BIN]   
  Click this button to move the selected product(s) to the recycle bin. This button is only displayed, when the checkbox of at least one product is selected.
  For detailed information, see [Delete a product](/PIM/Operation/03_MoveProducts.md#delete-a-product).

- [START MASS EDITING]   
  Click this button to edit the selected products. This button is only displayed, when the checkbox of at least one product is selected. The mass editing is only recommended if you select more that one product.
  For detailed information, see [Mass editing](/PIM/Operation/01_ManageProducts.md#mass-editing).

Depending on the selection in the *Variants* drop-down list, the product list displays all products or just the master products without their variants. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Images*   
  Image of the product.

- *SKU*   
  Stock Keeping Unit. Identification number for the product.  

- *Product Name*   
  Name of the product.

- *Product Variants*   
  Variant type of the product. The following variant types are displayed:
  - **Master product with *x* variants** (x indicates the number of variants for the master product)
  - **Variant *Defining Attribute: Value*** (the defining attributes and their values are indicated)
  - no variant type indicated for all products that are neither a master product nor a variant


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
  You can add a column for each attribute that is assigned to the product. The column displays the attribute name, the row displays the corresponding attribute value of the product.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a product. The *Create new product* window is displayed.   
  For detailed information, see [Create a product](/PIM/Operation/01_ManageProducts.md#create-a-product).


## Create view
*PIM > Products > Tab LIST > Button Points > Menu entry create*

![Create view](/Assets/Screenshots/PIM/Products/List/CreateView.png "[Create view]")

- *Name*   
  Enter a name for the view.

- [CANCEL]   
  Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]   
  Click this button to save the new view. The *Create view* window is closed. The view is saved and displayed in the *View* drop-down list.


## Rename view
*PIM > Products > Tab LIST > Button Points > Menu entry rename*

![Rename view](/Assets/Screenshots/PIM/Products/List/RenameView.png "[Rename view]")

- *Name*   
  Click this field to edit the views name.

- [CANCEL]   
  Click this button to cancel renaming the view. The *Rename view* window is closed.

- [SAVE]   
  Click this button to save the changes to the views name. The *Rename view* window is closed. The new name for the view is saved and displayed in the *View* drop-down list.


## Create new product
*PIM > Products > Tab LIST > Button Add*

![Create new product](/Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[Create new product]")

- *Select attribute set*   
  Click the drop-down list to select the attribute set for the new product. All available attribute sets are displayed in the drop-down list.

- *SKU*   
  Enter the SKU of the new product. The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.


## Create product
*PIM > Products > Tab LIST > Button Add > Button CREATE*

![Create Product](/Assets/Screenshots/PIM/Products/List/CreateProduct.png "[Create Product]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create product* view and return to the product list. All changes are rejected.

- [CANCEL]   
  Click this button to cancel the creation of a product.

- [SAVE]   
  Click this button to save the new product.

- Image box   
  Image of the product. In the *Create product* view, the image box is always empty. When an image is assigned in the corresponding attribute and the product is saved, this image is displayed next time opening the product view.

- *SKU*   
  Stock Keeping Unit. Identification number for the product. The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.   
  Click the button ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the SKU to edit it.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the SKU.

- ![Apply](/Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the SKU. This button is only displayed when you are editing the SKU.

- *Channel*   
  Click the drop-down list to select a channel for the product. All active channels are displayed in the drop-down list. By default, the **Actindo Basic** channel is preselected.

- *Language*   
  Click the drop-down list to select a language for the product. All active languages are displayed in the drop-down list. The default language is preselected.

- [Completeness: Not available]     
  Completeness of the product. In the *Create product* view, the completeness cannot be indicated. The completeness is indicated once the product have been saved.


### Create product - Attributes
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Attributes*

![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesCreate.png "[Attributes]")

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the product contains attributes that are unassigned, the *Unassigned Group* group is automatically displayed in the left margin column.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. As the attributes are customized, only those attributes that are predefined by default in the *PIM Basic Set* attribute set are described below:

[comment]: <> (should we describe all attributes of the PIM Basic Set?)


- ![Fade in/out](/Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
  Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed an you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


### Create product - Variants
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Variants*

![Variants](/Assets/Screenshots/PIM/Products/List/Variants/VariantsCreate.png "[Variants]")

- *Variant set*   
  Click the drop-down list to select a variant set for the product. All variant sets to the corresponding attribute set of the product are displayed in the drop-down list. The ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button is displayed in the variants box below if a variant set is selected.

**Variants box**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of variants.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

The list displays all variants of the selected product. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Status*  
  Status of the variant. In the *Create product* view, the **Created after save** status is displayed if you have added a variant.

- *SKU*  
  Stock Keeping Unit. Identification number for the variant. The SKU for the variant is created depending on the selected settings.

- *LifeCycle Status*   
  Lifecycle status of the variant The status is created after saving. In the *Create product* view, no lifecycle status is displayed.

- *ID*   
  Variant identification number. The ID is created after saving. In the *Create product* view, no ID is displayed.

- Defining/changeable attribute    
  You can add a column for each attribute that is assigned as a defining or changeable attribute to the selected variant set. The column displays the attribute name, the row displays the attribute value.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ] button and the [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ] button are displayed.


#### Add variant
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Variants > Select variant set > Button Add*

![Add variant](/Assets/Screenshots/PIM/Products/List/Variants/AddVariantCreate.png "[Add variant]")

- [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant. The *Add single variant* window is displayed.

- [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants. The *Select Values* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to hide the buttons and return to the *Variants* tab.

#### Add single variant
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Variants > Select variant set > Button Add > Button Add single variant*

![Add single variant](/Assets/Screenshots/PIM/Products/List/Variants/AddSingleVariant.png "[Add single variant]")

**Additional fields**

- *SKU*   
  Identification number for the variant. The SKU (Stock Keeping Unit) is an identification number and should be assigned only once. This field is read-only as long as the *Use formula* toggle is active. Deactivate the toggle to edit the SKU.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use formula*   
  Activate this toggle to apply the formula defined in the settings for the variant sets to the variant SKU. When the toggle is active, the *SKU* field is read-only. Deactivate the toggle to enter a different SKU. By default, this toggle is active.

**Defined values**

For each defining attribute a single field or box to define the attribute value is displayed.

> [Info] If more than one defining attribute is assigned to the variant, you have to select a value for each defining attribute to add a variant.

- Defining attribute(s)   
  Enter or select the appropriate value for the defining attribute(s).

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Add single variant* window.

- [SAVE]   
  Click this button to save the variant and close the *Add single variant* window.


#### Add multiple variants
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Variants > Select variant set > Button Add > Button Add multiple variants*

##### Select Values

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants01.png "[Add multiple variants]")

For each defining attribute a single box to define the attribute value is displayed.

> [Info] If more than one defining attribute is assigned to the variant, you have to select a value for each defining attribute to add a variant.

- [ADD ALL VALUES]   
  Click this button to add all available values in the box for the corresponding defining attribute. This button is only displayed for attributes with the *TreeNode* data type.

- [ADD VALUE]   
  Click this button to add a further row to the corresponding attribute where you can enter or select the desired value.

- [ABORT]   
  Click this button to cancel adding variants and close the *Select Values* wizard window.

- [NEXT]   
  Click this button to proceed to the next step of adding variants. The *Summary* wizard window is displayed.


##### Summary

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants02.png "[Add multiple variants]")

The box displays all variants that will be created from the selected attribute values. For each possible combination of the selected attributes, a new variant is created. Variants that already exist will not be created even when they are listed in the box.

**Variants that will be created (ignoring duplicated)**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all variants in the list are selected.

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected variant from the list. This button is only displayed, when the checkbox of a variant is selected.

The list displays all selected variants. Depending on the settings, the displayed columns may vary.

- *SKU*      
  Stock Keeping Unit. Identification number for the variant. Click this field to edit the SKU of the selected variant.

- Defining attribute     
  You can add a column for each defining attribute. The column displays the attribute name, the row displays the corresponding attribute value. The fields are read-only.

- [< GO BACK]   
  Click this button to go back to the previous step of adding variants. The *Select Values* wizard window is displayed.

- [ABORT]   
  Click this button to cancel adding variants and close the *Summary* wizard window.

- [FINISH]   
  Click this button to save the listed variants and close the *Summary* wizard window.



### Create product - Dependencies
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Dependencies*

![Dependencies](/Assets/Screenshots/PIM/Products/List/Dependencies/DependenciesCreate.png "[Dependencies]")

 In the *Create product* view, the notice *Information about dependencies are not available* is displayed in this tab. Dependencies are displayed only after saving.  


### Create product - Catalogs
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Catalogs*

![Catalogs](/Assets/Screenshots/PIM/Products/List/Catalogs/CatalogsCreate.png "[Catalogs]")

For each catalog a single box to assign the new product to a category is displayed. You can assign a product to several catalogs and categories at the same time.

**Catalog Name**

- [EDIT ATTRIBUTE *CATALOG NAME* ]   
  Click this button to assign the product to a category or a sub-category in the selected catalog. The categories window is displayed.

The catalog box displays all selected categories and their level. All fields are read-only. If no category is selected, the notice *No nodes selected* is displayed in the box.

- *Level 1*    
  Level 1 category name.

- *Level 2*   
  Level 2 category name. The field is only displayed, if the product is assigned to a category of level 2 or lower.

- *Level x*   
  Level x category name. The field is only displayed, if the product is assigned to a category of level x or lower. The *x* indicates the level number of the assigned category.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the category next to the button from the box. This button is only displayed, when you hover over a category in the box.


#### Categories

[comment]: <> (window needs title!)

*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Catalogs > Button EDIT ATTRIBUTE*

![Categories](/Assets/Screenshots/PIM/Products/List/Catalogs/Categories.png "[Categories]")

- [x]     
  Select a checkbox to assign the product to the selected category. You can select multiple checkboxes.

  > [Info] Categories that are containing sub-categories are displayed with the symbol ![Folders](/Assets/Icons/Folders01.png "[Folders]") (Folders), categories without sub-categories with the symbol ![Folder](/Assets/Icons/Folder01.png "[Folder]") (Folder). Click the [>] button to the left of a category checkbox to display all sub-categories.

- [CANCEL]   
  Click this button to cancel selecting categories and close the *Categories* window.

- [SAVE]   
  Click this button to save the selected categories and close the *Categories* window.



### Create product - Associations
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Associations*

![Associations](/Assets/Screenshots/PIM/Products/List/Associations/AssociationsCreate.png "[Associations]")

In this tab, boxes of all attributes with the *Related products* data type are displayed. The box titles differ depending on the corresponding attribute names, but the structure of all boxes is identical.   

> [Info] For detailed information about the data types, see [Data type list](04_DataTypeList.md).

- [ADD]   
  Click this button to add an associated product to the list. The *Filter List of Products* window is displayed.

The box displays all associated products. All fields are read-only. If no product is selected, the notice *No associated products selected* is displayed in the box.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.

- ![Eye](/Assets/Icons/Eye01.png "[Eye]") (Eye)   
  The button is only displayed, when you hover over a product in the list.  

  [comment]: <> (what should be displayed? loading never ends...)

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected product from the list. The button is only displayed, when you hover over a product in the list.



#### Filter list of products
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Associations > Button ADD*

![Filter List of Products ](/Assets/Screenshots/PIM/Products/List/Associations/FilterListProducts.png "[Filter List of Products]")

- [CANCEL]   
  Click this button to cancel adding products and close the *Filter List of Products* window.

- [SAVE]   
  Click this button to add the selected products to the list and close the *Filter List of Products* window.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a product.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of products.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all products in the list are selected.

The list displays all products. All fields are read-only.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.


### Create product - UCS Warehouse
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab UCS Warehouse*

![UCS Warehouse](/Assets/Screenshots/PIM/Products/List/UCSWarehouse/UCSWarehouseCreate.png "[UCS Warehouse]")

 In the *Create product* view, the notice *Available after saving the product.* is displayed in this tab. The warehouse information is displayed only after saving.  


### Create product - UCS Marketplaces
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab UCS Marketplaces*

![UCS Marketplaces](/Assets/Screenshots/PIM/Products/List/UCSMarketplaces/UCSMarketplacesCreate.png "[UCS Marketplaces]")

 In the *Create product* view, the notice *Available after saving the product.* is displayed in this tab. The marketplaces information is displayed only after saving.  


### Create product - Offers
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Offers*

![Offers](/Assets/Screenshots/PIM/Products/List/Offers/OffersCreate.png "[Offers]")

**Offers**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all offers in the list are selected.

- *Status*   
  Click the drop-down list to change the offer status. The selected status is displayed in the *Pending status/Errors* column. This drop-down list is only displayed, when the checkbox of at least one offer is selected. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.


- *Change tracking mode*   
  Click the drop-down list to change the change tracking mode (ETL mode) of the offer. The selected change tracking mode is displayed in the *Change tracking mode* column. This drop-down list is only displayed, when the checkbox of one offer is selected. The following change tracking modes are available:    
  - **manual**: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.
  - **semi-automatic**: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
  - **semi-automatic, changes must be confirmed by another user**: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.       
  - **automatic**: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.



- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected offer from the list. This button is only displayed, when the checkbox of at least one offer is selected.

[comment]: <> (not working -> if I want to edit an offer, a window is displayed loading all the time...)

The list displays all created offers to this product. All fields are read-only.

- *SKU*   
  Stock Keeping Unit. Identification number of the product. In the *Create product* view, **TO BE GENERATED** is displayed.

- *Status*   
  Connection status of the offer. In the *Create product* view, **Offline** is displayed.

- *Pending status/Errors*   
  Indication of the pending status or an error for this offer. The selected status (**Active**/**Inactive**/**Offline**) is displayed if you have changed the offer status via the editing toolbar.

  [comment]: <> (when is an error displayed here? what is displayed? The Error code or message?)

- *Connection*   
  Selected connection for the offer.

- *Attribute Set*   
  Selected attribute set for the offer.

- *Last edited*   
  Date and time of the last modification. In the *Create product* view, no date is displayed.

- *Modified by*   
  Name and username of the user who modified the product. In the *Create product* view, no name is displayed.

- *Change tracking mode*   
  Change tracking mode (ETL mode) of the offer. The following modes can be displayed:
  - **manual**
  - **semi-automatic**
  - **semi-automatic, changes must be confirmed by another user**   
  - **automatic**


- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *Created*   
  Date and time of the creation. In the *Create product* view, no date is displayed.

- *Creator*   
  Name and username of the user who created the product. In the *Create product* view, no name is displayed.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a new offer. The [Add to a single connection ![Add to a single connection](/Assets/Icons/Document.png "[Single connection]") ] button and the [Add to multiple connections ![Multiple connections](/Assets/Icons/Documents.png "[Multiple connections]") ] button are displayed.


#### Add an offer in PIM
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Offers > Button Add*

![Add](/Assets/Screenshots/PIM/Products/List/Offers/AddCreate.png "[Add]")

- [Add to a single connection ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add to a single connection* window is displayed.

- [Add to multiple connections ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add to multiple connections* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the connection creation and close the current view.


#### Add to a single connection
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Offers > Button Add > Button Add to a single connection*

![Add to a single connection](/Assets/Screenshots/PIM/Products/List/Offers/SingleConnection.png "[Add to a single connection]")

**Create Offer**

- *Select Connection*   
  Click the drop-down list to select a connection for the offer. All available connections are displayed in the list.

- *Select Attribute Set*   
  Click the drop-down list to select an attribute set for the offer. All active attribute sets are displayed in the drop-down list. The drop-down list is locked if no connection is selected.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Generate SKU*   
  Activate this toggle to automatically generate a SKU for the offer. Deactivate the toggle to enter a SKU manually. By default, this toggle is active.

- *SKU*    
  Enter an individual SKU for the offer. The SKU (Stock Keeping Unit) is an identification number and should be assigned only once.

[comment]: <> (offer or product? how does this work? When I enter a different SKU, The SKU is automatically overwritten)

- *Change Tracking mode*   
  Select the appropriate option for change tracking (ETL mode). The following options are available:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic, changes must be confirmed by another user*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

[comment]: <> (adjust field name!)

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.


- [CANCEL]   
  Click this button to cancel adding an offer and close the *Create Offer* window.

- [SAVE]   
  Click this button to save the offer and close the *Create Offer* window.


#### Add to multiple connections
*PIM > Products > Tab LIST > Button Add > Button CREATE > Tab Offers > Button Add > Button Add to multiple connections*

##### Select connections and status

![Add to multiple connections](/Assets/Screenshots/PIM/Products/List/Offers/MultipleConnections01.png "[Add to multiple connections]")

**Select status and change tracking mode**

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.


- Select the appropriate change tracking mode. The following options are available:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic, changes must be confirmed by another user*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.


**Select connections**

- [SELECT ALL]   
  Click this button to select all available connections.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Connection name     
  Activate a toggle to select the corresponding connection to create an offer to. All available connections are displayed. By default, all toggles are inactive.

- [CANCEL]   
  Click this button to cancel adding multi-connection offers and close the *Select Connections and status* wizard window.

- [CONTINUE]   
  Click this button to proceed to the next step to add multi-connection offers. The *Select destination attribute sets* wizard window is displayed.


##### Select destination attribute sets

![Add to multiple connections](/Assets/Screenshots/PIM/Products/List/Offers/MultipleConnections02.png "[Add to multiple connections]")

- *Destination set for connection*   
  Destination attribute set for the selected connection. The attribute set is automatically selected. The field is read-only. An own attribute set is assigned to each selected connection.

- [< BACK]   
  Click this button to go back to the previous step. The *Select Connections and status* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel adding multi-connection offers and close the *Select destination attribute sets* wizard window.

- [FINISH]   
  Click this button to save the multi-connection offers and close the *Select destination attribute sets* wizard window.



## Edit product
*PIM > Products > Tab LIST > Select product*

![Edit Product](/Assets/Screenshots/PIM/Products/List/EditProduct.png "[Edit Product]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit product* view and return to the product list. All changes are rejected.

- [CANCEL]   
  Click this button to cancel editing the product.

- [SAVE]   
  Click this button to save the changes to the product.

- Image box
  Image of the product. The image is displayed when an image is assigned in the corresponding attribute.

- *SKU*   
  Stock Keeping Unit. Identification number for the product.  he SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.   
  Click the button ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the SKU to edit it.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the SKU.

- ![Apply](/Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the SKU. This button is only displayed when you are editing the SKU.

- *Channel*   
  Click the drop-down list to select a channel for the product. All active channels are displayed in the drop-down list. By default, the **Actindo Basic** channel is preselected.

- *Language*   
  Click the drop-down list to select a language for the product. All active languages are displayed in the drop-down list. The default language is preselected.


- [Complete]     
  Completeness of the product for all available channels and languages. The percentage of completeness is displayed in the button. Click the button to display the *Completeness* window. If the completeness is less than 100%, the number of missing require attributes is displayed to the right of the completeness button.
  If the completeness cannot be calculated, *Completeness: Not available* is displayed and the button is not clickable.

  > [Info] The completeness is calculated by considering the number of missing required fields. As the required fields are defined individually for each attribute set set, it can vary from one product to another.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *show empty required attributes only*     
  Activate this toggle to display only the missing required fields in the *Attributes* tab for this product. By default, the toggle is inactive. The toggle is only displayed if at least one required field is missing.

- *Sets*   
  Click the drop-down list to change the attribute set (attribute set) for the product. All available attribute sets are displayed in the drop-down list. The currently selected attribute set is highlighted in bold.

  > [Info] Changing the attribute set can destroy data. Therefore, a confirmation window is displayed to confirm the attribute set change. Note, that the change cannot be undone once you have saved the changes.


### Completeness
*PIM > Products > Tab LIST > Select product > Button Complete*

![Completeness](/Assets/Screenshots/PIM/Products/List/Completeness.png "[Completeness]")

- *Channels*   
  Click the drop-down list to change the channel for the product completeness calculation. All available channels, the **Channels (All)** option and the **Not multi-channel** option are displayed in the drop-down list. By default, the **Channels (All)** option is preselected.

  > [Info] The product completeness for the selected channel is only displayed in the *Completeness* window. The completeness button in the *Edit Product* view is not affected by this change.

- *Languages*   
  Click the drop-down list to change the language for the product completeness calculation. All available languages, the **Languages (All)** option and the **Not multi-language** option are displayed in the drop-down list. By default, the **Languages (All)** option is preselected.

  > [Info] The product completeness for the selected language is only displayed in the *Completeness* window. The completeness button in the *Edit Product* view is not affected by this change.

- Percentage   
  The current percentage for the product completeness of the selected channel and language is displayed. The percentage is automatically updated when you select a different channel or language.


### Edit product - Attributes
*PIM > Products > Tab LIST > Select product > Tab Attributes*

![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesEdit.png "[Attributes]")

In the left margin column, all available groups containing attributes are displayed. Click a (sub-)group to display the attributes that are assigned to this (sub-)group on the right side of the *Attributes* tab. If the product contains attributes that are unassigned, the *Unassigned Group* group is automatically displayed in the left margin column.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. As the attributes are customized, only those attributes that are predefined by default in the *PIM Basic Set* attribute set are described below:

[comment]: <> (describe attributes in PIM Basic Set?!)


### Edit product - Variants
*PIM > Products > Tab LIST >  Select product > Tab Variants*

![Variants](/Assets/Screenshots/PIM/Products/List/Variants/VariantsEdit.png "[Variants]")

- *Variant set*   
  Click the drop-down list to select a variant set for the product. All available variant sets are displayed in the drop-down list. The ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button is displayed in the variants box below if a variant set is selected.
  If the product is a master product, the corresponding variant set is preselected in the drop-down list. The drop-down list is locked. The corresponding variants and the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button are displayed in the variants box.
  If the product is a variant, the *Variant set* drop-down list is not displayed, but the *Variant* field.

- *Variant*   
  Indication that the selected product is a variant. This field is read-only. The value can be changed within the *Attributes* tab. The field is only displayed for variants.


**Variants box**

> [Info] If the product is a variant, the variants box is not displayed.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of variants.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

The list displays all variants. All fields are read-only. Depending on the settings, the displayed columns may vary.

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

- Defining/changeable attribute    
  You can add a column for each attribute that is assigned as a defining or changeable attribute to the selected variant set. The column displays the attribute name, the row displays the attribute value.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ] button and the [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ] button are displayed.


#### Add variant
*PIM > Products > Tab LIST > Select product > Tab Variants > Select variant set > Button Add*

![Add variant](/Assets/Screenshots/PIM/Products/List/Variants/AddVariantEdit.png "[Add variant]")

- [Add single variant ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add single variant* window is displayed.

- [Add multiple variants ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add multiple variant* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the variant creation and exit the current view.


#### Add single variant
*PIM > Products > Tab LIST > Select product > Tab Variants > Select variant set > Button Add > Button Add single variant*

![Add single variant](/Assets/Screenshots/PIM/Products/List/Variants/AddSingleVariant.png "[Add single variant]")

**Additional fields**

- *SKU*   
  Identification number for the variant. The SKU (Stock Keeping Unit) is an identification number and should be assigned only once. This field is read-only as long as the *Use formula* toggle is active. Deactivate the toggle to edit the SKU.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use formula*   
  Activate this toggle to apply the formula defined in the settings for the variant sets to the variant SKU. When the toggle is active, the *SKU* field is read-only. Deactivate the toggle to enter a different SKU. By default, this toggle is active.

**Defined values**

All defining attributes of the variant are displayed in this section.

- Defining attribute   
  Enter or select the appropriate value for the defining attribute.

- [CANCEL]   
  Click this button to cancel adding a variant and close the *Add single variant* window.

- [SAVE]   
  Click this button to save the variant and close the *Add single variant* window.


#### Add multiple variants
*PIM > Products > Tab LIST > Select product > Tab Variants > Select variant set > Button Add > Button Add multiple variants*

##### Select values

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants01.png "[Add multiple variants]")

For each defining attribute a single box to define the attribute value is displayed.

> [Info] If more than one defining attribute is assigned to the variant, you have to select a value for each defining attribute to add a variant.

- [ADD ALL VALUES]   
  Click this button to add all available values in the box for the corresponding defining attribute. This button is only displayed for attributes with the *TreeNode* data type.

- [ADD VALUE]   
  Click this button to add a further row to the corresponding attribute where you can enter or select the desired value.

- [ABORT]   
  Click this button to cancel adding variants and close the *Select Values* wizard window.

- [NEXT]   
  Click this button to proceed to the next step of adding variants. The *Summary* wizard window is displayed.


##### Summary

![Add multiple variants](/Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants02.png "[Add multiple variants]")

The box displays all variants that will be created from the selected attribute values. For each possible combination of the selected attributes, a new variant is created. Variants that already exist will not be created even when they are listed in the box.

**Variants that will be created (ignoring duplicated)**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all variants in the list are selected.

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected variant from the list. This button is only displayed when the checkbox of a variant is selected.

The list displays all selected variants. Depending on the settings, the displayed columns may vary.

- *SKU*      
  Stock Keeping Unit. Identification number for the variant. Click this field to edit the SKU of the selected variant.

- Defining attribute   
  You can add a column for each defining attribute. The column displays the attribute name, the row displays the corresponding attribute value. The fields are read-only.

- [< GO BACK]   
  Click this button to go back to the previous step of adding variants. The *Select Values* wizard window is displayed.

- [ABORT]   
  Click this button to cancel adding variants and close the *Summary* wizard window.

- [FINISH]   
  Click this button to save the listed variants and close the *Summary* wizard window.



### Edit product - Dependencies
*PIM > Products > Select product > Tab Dependencies*

![Dependencies](/Assets/Screenshots/PIM/Products/List/Dependencies/DependenciesEdit.png "[Dependencies]")

**Dependencies**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of product dependencies.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependent entities in the list are selected.

The list displays all dependencies of the selected product. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Dependent entity id*   
  Identification number of the dependent entity.

- *Dependent entity type*   
  Type of the dependent entity. The following types can be displayed:
  - **Omni-Channel Offer**
  - **UCS Product**

  [comment]: <> (what else?)


- *Change tracking mode*   
  Change tracking mode (ETL mode) of the dependent entity. The following modes can be displayed:
  - **manual**
  - **semi-automatic**
  - **semi-automatic, changes must be confirmed by another user**   
  - **automatic**


- *Dependent entity friendly identifier*   

[comment]: <> (what id number is that? How is it created?)

- [RERUN MAPPING]   
  Click this button to rerun the mapping of the selected entity. This button is only displayed when the checkbox of at least one dependency is selected.



### Edit product - Completeness
*PIM > Products > Select product > Tab Completeness*

![Completeness](/Assets/Screenshots/PIM/Products/List/Completeness/Completeness.png "[Completeness]")

The *Completeness* tab displays the completeness of the product for the different languages and channels. A single box is displayed for each active channel. The tab is only displayed if the completeness of the product has been calculated and is displayed in the header section of the *Edit product* view. Consequently, the tab is never displayed in the *Create product* view.

- Channel name   
  This box displays the percentage for the product completeness of the selected product regarding the assigned channel.
  - Language   
    The box displays the percentage for the product completeness of the selected product regarding the assigned channel and language. A single percentage is displayed for each available language for one channel.

  - ![Info](/Assets/Icons/Info.png "[Info]") (Info)   
    Hover over this icon to display a box that is listing the missing attribute values. This icon is only displayed when at least one required attribute value for the product completeness is missing.


### Edit product - Catalogs
*PIM > Products > Select product > Tab Catalogs*

![Catalogs](/Assets/Screenshots/PIM/Products/List/Catalogs/CatalogsEdit.png "[Catalogs]")

For each catalog a single box to assign the new product to a category is displayed. You can assign a product to several categories at the same time.

**Catalog Name**

- [EDIT ATTRIBUTE *CATALOG NAME*]   
  Click this button to assign the product to a category or a sub-category in the selected catalog. The categories window is displayed.

The box displays all selected categories and their level. All fields are read-only. If no category is selected, the notice *No nodes selected* is displayed in the box.

- *Level 1*    
  Level 1 category name.

- *Level 2*   
  Level 2 category name. The field is only displayed, if the product is assigned to a category of level 2 or lower.

- *Level x*   
  Level x category name. The field is only displayed, if the product is assigned to a category of level x or lower. The *x* indicates the level number of the assigned category.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected category from the box. This button is only displayed, when you hover over a category in the box.


#### Categories
*PIM > Products > Select product > Tab Catalogs > Button EDIT ATTRIBUTE*

![Categories](/Assets/Screenshots/PIM/Products/List/Catalogs/Categories.png "[Categories]")

- [x]     
  Select a checkbox to assign the product to the selected category. You can select multiple checkboxes.

> [Info] Categories that are containing sub-categories are displayed with the symbol ![Folders](/Assets/Icons/Folders01.png "[Folders]") (Folders), categories without sub-categories with the symbol ![Folder](/Assets/Icons/Folder01.png "[Folder]") (Folder).    
Click the [>] button to the left of a category checkbox to display their sub-categories.

- [CANCEL]   
  Click this button to cancel selecting categories and close the *Categories* window.

- [SAVE]   
  Click this button to save the selected categories and close the *Categories* window.



### Edit product - Associations
*PIM > Products > Select product > Tab Associations*

![Associations](/Assets/Screenshots/PIM/Products/List/Associations/AssociationsEdit.png "[Associations]")

In this tab, boxes of all attributes with the *Related products* data type are displayed. The box titles differ depending on the corresponding attribute names, but the structure of all boxes is identical.

> [Info] For detailed information about the data types, see [Data type list](04_DataTypeList.md).

- [ADD]   
  Click this button to add an associated product to the list. The *Filter List of Products* window is displayed.

The box displays all associated product for cross selling. All fields are read-only. If no product is selected, *No associated products selected* is displayed in the box.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.

- ![Eye](/Assets/Icons/Eye01.png "[Eye]") (Eye)   
  The button is only displayed, when you hover over a product in the list.

  [comment]: <> (what should be displayed? loading never ends...)

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected product from the list. This button is only displayed, when you hover over a product in the list.



#### Filter list of products
*PIM > Products > Select product > Tab Associations > Button ADD*

![Filter List of Products ](/Assets/Screenshots/PIM/Products/List/Associations/FilterListProducts.png "[Filter List of Products]")

- [CANCEL]   
  Click this button to cancel adding products and close the *Filter List of Products* window.

- [SAVE]   
  Click this button to add the selected poducts to the list and close the *Filter List of Products* window.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a product.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of products.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all products in the list are selected.

The list displays all products. All fields are read-only.

- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Attribute Set*   
  Assigned attribute set.



### Edit product - History
*PIM > Products > Select product > Tab History*

![History](/Assets/Screenshots/PIM/Products/List/History/History.png "[History]")

The *History* tab is only displayed in the *Edit product* view. The tab is never displayed in the *Create product* view.

**History**

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a change.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of changes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

The list displays the change history of the product. All fields are read-only. Depending on the settings, the displayed columns may vary.

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
  Click this button to display the *History (Single Entry)* window. This button is only displayed, when the checkbox of a change entry is selected. Alternatively, you can click directly a row in the list to display the *History (Single Entry)* window.   


#### History (Single Entry)
*PIM > Products > Select product > Tab History > Select checkbox > Button Eye*

![History](/Assets/Screenshots/PIM/Products/List/History/HistorySingleEntry.png "[History]")

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a change entry.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of change entries.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all change entries in the list are selected.

- ![Lock](/Assets/Icons/Lock01.png "[Lock]") (Lock)   
  This entry is locked and cannot be undone. It cannot be selected. The corresponding entry row is grayed out.

The list displays the single entries of the selected product change. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Attribute name*   
  Name of the attribute to which the change was made.

- *Channel name*   
  Name of the channel to which the change was made.

- *Language name*   
  Name of the language to which the change was made

- *Old value*   
  Attribute value before change. If the field is empty, no value was set for this attribute before change.  

- *New value*   
  Attribute value after change.  

- *ID*   
  Identification number of the change entry. The ID number is automatically assigned by the system.  

- ![Undo](/Assets/Icons/Undo01.png "[Undo]") (Undo)   
  Click this button to undo the selected change(s). A confirmation window is displayed to confirm the change reversion. This button is only displayed, when the checkbox of a change entry is selected.


### Edit product - UCS Warehouse
*PIM > Products > Select product > Tab UCS Warehouse*

![UCS Warehouse](/Assets/Screenshots/PIM/Products/List/UCSWarehouse/UCSWarehouseEdit.png "[UCS Warehouse]")

This tab displays the *Basic data* and *Warehouse / Suppliers* sub-tabs. These sub-tabs are excerpts from the tabs in the *Warehouse* module: *Warehouse > Quick Booking > QUICK BOOKING > Select product*

[comment]: <> (link to the Corresponding warehouse documentation? What about the buttons [HILFE] and [SPEICHERN]?)


### Edit product - UCS Marketplaces
*PIM > Products > Select product > Tab UCS Marketplaces*

![UCS Marketplaces](/Assets/Screenshots/PIM/Products/List/UCSMarketplaces/UCSMarketplacesEdit.png "[UCS Marketplaces]")

This tab displays the *Basic data* and *webshop* sub-tabs. These sub-tabs are excerpts from the tabs in the *Material Management* module: *Material Management > Product > PRODUCT > Select product*

[comment]: <> (link to the Corresponding material management/Artikelverwaltung documentation? What about the buttons [HILFE] and [SPEICHERN]?)


### Edit product - Offers
*PIM > Products > Select product > Tab Offers*

![Offers](/Assets/Screenshots/PIM/Products/List/Offers/OffersEdit.png "[Offers]")

**Offers**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all offers in the list are selected.

- *Status*   
  Click the drop-down list to change the offer status. The selected status is displayed in the *Pending status/Errors* column. This drop-down list is only displayed, when the checkbox of at least one offer is selected. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.


- *Change tracking mode*   
  Click the drop-down list to change the change tracking mode (ETL mode) of the offer. The selected change tracking mode is displayed in the *Change tracking mode* column. This drop-down list is only displayed, when the checkbox of one offer is selected. The following change tracking modes are available:    
  - **manual**: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.
  - **semi-automatic**: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
  - **semi-automatic, changes must be confirmed by another user**: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.       
  - **automatic**: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.



- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected offer from the list. This button is only displayed, when the checkbox of at least one offer is selected.

[comment]: <> (not working -> if I want to edit an offer, a window is displayed loading all the time...)

The list displays all created offers to this product. All fields are read-only.

- *SKU*   
  Stock Keeping Unit. Identification number of the product.

- *Status*   
  Connection status of the offer. The following statuses are available:
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.

- *Pending status/Errors*   
  Indication of the pending status or an error for this offer. The selected status (**Active**/**Inactive**/**Offline**) is displayed if you have changed the offer status via the editing toolbar.

  [comment]: <> (when is an error displayed here?)

- *Connection*   
  Selected connection for the offer.

- *Attribute Set*   
  Selected attribute set for the offer.

- *last edited*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the product.

- *Change tracking mode*   
  Change tracking mode (ETL mode) of the offer. The following modes can be displayed:
  - **manual**
  - **semi-automatic**
  - **semi-automatic, changes must be confirmed by another user**   
  - **automatic**


- *ID*   
  Product identification number. The ID number is automatically assigned by the system.

- *Created*   
  Date and time of the creation.

- *Creator*   
  Name and username of the user who created the product.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new variant to the product. The [Add to a single connection ![Document](/Assets/Icons/Document.png "[Document]") ] button and the [Add to multiple connections ![Documents](/Assets/Icons/Documents.png "[Documents]") ] button are displayed.


#### Add an offer in PIM
*PIM > Products > Select product > Tab Offers > Button Add*

![Add](/Assets/Screenshots/PIM/Products/List/Offers/AddEdit.png "[Add]")

- [Add to a single connection ![Document](/Assets/Icons/Document.png "[Document]") ]    
  Click this button to add a single variant to the product. The *Add to a single connection* window is displayed.

- [Add to multiple connections ![Documents](/Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to add multiple variants to the product. The *Add to multiple connections* wizard window is displayed.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the connection creation and exit the current view.


#### Add to a single connection
*PIM > Products > Select product > Tab Offers > Button Add > Button Add to a single connection*

![Add to a single connection](/Assets/Screenshots/PIM/Products/List/Offers/SingleConnection.png "[Add to a single connection]")

**Create Offer**

- *Select Connection*   
  Click the drop-down list to select a connection for the offer. All available connections are displayed in the list.

- *Select Attribute Set*   
  Click the drop-down list to select an attribute set for the offer. All active attribute sets are displayed in the drop-down list. The drop-down list is locked if no connection is selected.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Generate SKU*   
  Activate this toggle to automatically generate a SKU for the offer. Deactivate the toggle to enter a SKU manually. By default, this toggle is active.

- *SKU*    
  Enter an individual SKU for the offer. The SKU (Stock Keeping Unit) is an identification number and should be assigned only once.

[comment]: <> (offer or product? how does this work? When I enter a different SKU, The SKU is automatically overwritten)

- *Change Tracking mode*   
  Select the appropriate option for change tracking (ETL mode). The following options are available:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic, changes must be confirmed by another user*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

[comment]: <> (adjust field name!)

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.


- [CANCEL]   
  Click this button to cancel adding an offer and close the *Create Offer* window.

- [SAVE]   
  Click this button to save the offer and close the *Create Offer* window.


#### Add to multiple connections
*PIM > Products > Select product > Tab Offers > Button Add > Button Add to multiple connections*

##### Select connections and status

![Add to multiple connections](/Assets/Screenshots/PIM/Products/List/Offers/MultipleConnections01.png "[Add to multiple connections]")

**Select status and change tracking mode**

- *Status*    
  Click the drop-down list to select the connection status. The following statuses are available:    
  - **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
  - **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
  - **Offline**: The offer is unknown to the marketplace and therefore cannot be sold there.


- Select the appropriate change tracking mode. The following options are available:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic, changes must be confirmed by another user*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.


**Select connections**

- [SELECT ALL]   
  Click this button to select all available connections.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Connection name     
  Activate a toggle to select the corresponding connection to create an offer to. All available connections are displayed. By default, all toggles are inactive.

- [CANCEL]   
  Click this button to cancel adding multi-connection offers and close the *Select Connections and status* wizard window.

- [CONTINUE]   
  Click this button to proceed to the next step to add multi-connection offers. The *Select destination attribute sets* wizard window is displayed.


##### Select destination attribute sets

![Add to multiple connections](/Assets/Screenshots/PIM/Products/List/Offers/MultipleConnections02.png "[Add to multiple connections]")

- *Destination set for connection*   
  Destination attribute set for the selected connection. The attribute set is automatically selected. The field is read-only. An own attribute set is assigned to each selected connection.

- [< BACK]   
  Click this button to go back to the previous step. The *Select Connections and status* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel adding multi-connection offers and close the *Select destination attribute sets* wizard window.

- [FINISH]   
  Click this button to save the multi-connection offers and close the *Select destination attribute sets* wizard window.
