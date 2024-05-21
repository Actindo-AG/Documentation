[!!Record the purchase](../Operation/02_SelectOffer.md)
[!!Edit the bill list](../Operation/03_EditBillList.md)
[!!Complete a purchase](../Operation/04_CompletePurchase.md)
[!!User interface Mapping from PIM](../UserInterface/02c_MappingFromPIM.md)
[!!User interface Omni-Channel Offers](../../Channels/UserInterface/02a_Offers.md)
[!!User interface DataHub Attributes](../../DataHub/UserInterface/01a_Attributes.md)
[!!User interface PIM List](../../PIM/UserInterface/02a_List.md)

# Manage offers for POS

To offer products in POS, it is recommended to create the products in advance in the *PIM* module and create the corresponding offers afterwards in order to be able to distribute them properly in the system.
<!---Ich glaube das versteht man so nicht. Vorschlag:
To offer products in POS, it is recommended to create the products in the *PIM* module first and then import them later into the *Omni-Channel* module. From there, the *POS* module receives its offers.-->


## Create products for POS

To create an offer for POS, it is recommended to create products in the *PIM* module for which you can make an offer.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

Create the product in the *PIM* module. For detailed information, see [Create a product](../../PIM/Operation/01_ManageProducts.md#create-a-product) in the *PIM* documentation.



## Create a product type

To improve the product classification, you can create a product type and use it in POS. To do this, you create an attribute set in the *PIM* module.  
For detailed information on how to create an attribute set, see [Create an attribute set](../../PIM/Integration/02_ManageAttributeSets.md#create-an-attribute-set) in the *PIM* documentation.
<!---Product type= Attribute set?-->



## Map a new product type in POS

When a new product type is created, it must be mapped before offers with this product type can be created for the POS.

#### Prerequisites

At least one new product type has been created, see [Create an attribute set](../../PIM/Integration/02_ManageAttributeSets.md#create-an-attribute-set) in the *PIM* documentation.

#### Procedure

*POS > Management > Tab MAPPING FROM PIM*

![Mapping from PIM](../../Assets/Screenshots/POS/Management/MappingFromPIM/MappingFromPIM01.png "[Mapping from PIM]")

1. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.   
    All not mapped PIM product types are displayed in the list.

    ![Mapping from PIM](../../Assets/Screenshots/POS/Management/MappingFromPIM/MappingFromPIM02.png "[Mapping from PIM]")

2. Select the checkboxes of the product types you want to map.   
    A toolbar is displayed at the bottom.

3. Click the [CREATE MAPPINGS] button in the toolbar.    
    The selected mappings are removed from the list when the mappings are created.



## Create an offer for POS

Create an offer in the *Omni-Channel* module or a product in the *PIM* module, so you can offer and select the products/offers in the *POS* store.

If you have the *PIM* module in use, it is recommended to create/edit the products in the *PIM* module. Changes to the *PIM* product are automatically transferred (via ETL) to the offers available in the *Omni-Channel* module.  
Especially if you want to exchange your product data available in the *PIM* module with your stores, you must additionally create the ETL mappings and processes for the data transfer between the PIM product data and the Omni-Channel offer data.



### Create an offer from a PIM product in Omni-Channel

You can create an offer from a PIM product in the *Omni-Channel* module if the corresponding product exists in the *PIM* module.

> [Info] If the product you want to create an offer for exists in the *PIM* module, it is recommended to create the offer from the PIM product instead of creating a manual offer.

#### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos).

#### Procedure

For detailed information, see [Create an offer from a PIM product](../../Channels/Operation/01_ManageOffers.md#create-an-offer-from-a-pim-product) in the *Omni-Channel* documentation.



### Create a manual offer in Omni-Channel

You can create a manual offer in the *Omni-Channel* module for all products regardless of whether they exist in the *PIM* module or not.

#### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos).

#### Procedure

Create an offer manually. For detailed information, see [Create a manual offer](../../Channels/Operation/01_ManageOffers.md#create-a-manual-offer) in the *Omni-Channel* documentation.



### Create a single channel offer in PIM

You can create an offer for a single sales channel for the selected product in the *PIM* module.
<!---Warum würde ich das tun wollen? Use case?-->


#### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos).

#### Procedure

Create a single channel offer in the *PIM* module. For detailed information, see [Create a single connection offer in PIM](../../PIM/Operation/01_ManageProducts.md#create-a-single-connection-offer-in-pim) in the *PIM* documentation.




### Create a multiple channels offer in PIM

You can create an offer for multiple channels to the selected product in the *PIM* module.

#### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos).

#### Procedure

Create an offer for multiple sales channels to the selected product in the *PIM* module. For detailed information, see [Create a multi-connection offer in PIM](../../PIM/Operation/01_ManageProducts.md#create-a-multi-connection-offer-in-pim) in the *PIM* documentation.


## Activate a POS offer

An offer has to be active so that it is displayed in the selected sales channel and can be sold there.

#### Prerequisites

At least one offer has been created, see [Create an offer for POS](#create-an-offer-for-pos).

#### Procedure

*Omni-Channel > Offers > Tab OFFERS*

![OC Offers Inactive](../../Assets/Screenshots/Channels/Offers/Offers/OffersInactive.png "[OC Offers Inactive]")

1. Select the checkboxes of the offers you want to activate.   
    The editing toolbar is displayed.

2. Click the *Change status to* drop-down list in the editing toolbar and select the **Active** option.   
    The **Active** status is displayed in the *Pending status/Errors* column of the selected offers.    

    ![OC Offers Pending](../../Assets/Screenshots/Channels/Offers/Offers/OffersPending.png "[OC Offers Pending]")

    When the offers are active, the status in the *Pending status/Errors* column is no longer displayed, but the status in the *Status* column has changed to **Active**.

    > [Info] It may take some time until all offers are activated. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner to update the offer list.



## Create a QuickSelect category

Create a QuickSelect category for POS for faster access to favorite offers at the cashpoint.  

The following image shows how QuickSelects can organize the most requested offers:
<!---Marina, ich habe hier ein Bild eingefügt, damit die Kunden überhaupt wissen, worum es sich bei dieser Funktion handelt-->
![QuickSelect in the cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/QuickSelect.png "[QuickSelect in the cashpoint]")

### Define a QuickSelect attribute

When creating a POS store, a QuickSelect attribute is automatically created in the *DataHub* module. Edit the QuickSelect attribute to specify the different QuickSelect elements for a *POS* offer.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*DataHub > Data model > Tab ATTRIBUTES*

![DataHub Attributes](../../Assets/Screenshots/DataHub/Settings/Attributes/Attributes.png "[DataHub Attributes]")

1. Enter **QuickSelect** in the search bar and click the ![Search](../../Assets/Icons/Search.png "[Search]") (Search) button.   
  The matching attributes are displayed in the attributes list.

2. Click the appropriate *QuickSelect Category* attribute in the attributes list.  
    The *Edit attribute* view is diplayed.

    ![Edit attribute](../../Assets/Screenshots/DataHub/Settings/Attributes/EditAttribute.png "[Edit attribute]")

3. Scroll down to the *CONFIGURATION* section and click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner of the *Edit tree* table.
    A plus sign is displayed in the left column of the *Edit tree* table.

    ![Edit Tree](../../Assets/Screenshots/DataHub/Settings/Attributes/EditTree.png "[Edit Tree]")

4. Click the plus sign in the left column of the *Edit tree* table.   
    The *Add element* window is displayed.

    ![Add element](../../Assets/Screenshots/DataHub/Settings/Attributes/AddElement.png "[Add element]")

5. Enter a name in the *Name* field.

    > [Info] The entered name equals the name of the QuickSelect element that will be displayed in POS.

6. If desired, enter a key in the *Key* field.
<!---Link war tot. Gibt es das noch?
    > [Info] By entering a key, you can define an icon for the QuickSelect element.   
      For detailed information on the icon list, see [QuickSelect Icon List](to_be_completed).-->

[comment]: <> (Add list of icon keys for Quickselect)

7. Click the [SAVE] button in the bottom right corner of the *Add element* window.   
    The *Add element* window is closed. The element is displayed in the left column of the *Edit tree* table.

    > [Info] If you want to create further QuickSelect elements, repeat step **3** to **6**.

8. Click the [SAVE] button in the upper right corner.   
    The *Edit attribute* view is closed. The QuickSelect element is saved.

9. Press the **F5** key to initialize the *Core1 Platform*.



### Assign the QuickSelect attribute

An offer is assigned to a certain QuickSelect category when you assign the created QuickSelect elements to the corresponding offer.

#### Prerequisites

- At least one QuickSelect attribute has been created, see [Define a QuickSelect attribute](#define-a-quickselect-attribute).
- At least one offer is created for *POS*, see [Create an offer for POS](#create-an-offer-for-pos).

#### Procedure

*Omni-Channel > Offers > Tab OFFERS*

![Offers](../../Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

1. Click the offer you want to create the QuickSelect element to.   
    The *Edit offer* view of the selected offer is displayed. The *Attributes* tab is preselected.

    ![Edit offer](../../Assets/Screenshots/Channels/Offers/Offers/EditOffer.png "[Edit offer]")

2. Scroll down in the *Attribute* tab and select the QuickSelect element in the *QuickSelect Category* drop-down list.

    ![Define QuickSelect](../../Assets/Screenshots/POS/Sales/Cashpoint/OfffersQuickSelectAttribute.png "[Define Quickselect]")


3. Click the [SAVE] button in the upper right corner.    
    The *Edit offer* view is closed. The offer with the QuickSelect element is saved.

> [Info] You have to repeat this procedure for each offer you want to assign the QuickSelect Category to.

[comment]: <> (Is there an alternative to manually assign each offer?)
[comment]: <> (JULIAN: Hier könnten man noch unterbringen wie man zusätzliche Felder mapped aus PIM raus oder Felder aus Omni-Channel ins PIM übernimmt)



## Create a voucher 

If you want to sell vouchers in your POS system, you have to create them first.

### Create a voucher product

To create a voucher, you need to create a product that you define as a voucher.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*PIM > Products > Tab LIST*

![PIM Products](../../Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create new product* window is displayed.

    ![New Product](../../Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[New Product]")

2. Click the *Select attribute set* drop-down list and select the appropriate attribute set.

    > [Info] If you have not created a new attribute set, the only available attribute set is **PIM Basic Data**.   

    For detailed information on how to create an attribute set for POS, see [Create a product type](#create-a-product-type).

3. Enter an SKU in the *SKU* field, for instance **Voucher**.

    > [Info] The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it has to be uniquely assigned to a single product and should not be changed once assigned.

4. Click the [CREATE] button in the bottom right corner of the *Create new product* window.   
    The *Create new product* window is closed. The *Create product* view is displayed in the *List* tab. The *Attributes* tab is preselected.

    ![Attribute](../../Assets/Screenshots/PIM/Products/List/CreateProduct.png "[Attributes]")

5. Enter the product data in the fields of the *Attributes* tab. You must at least enter a product name, a price and a tax class.

6. Click the [SAVE] button in the upper right corner.   
    The new product is saved. The *Create product* view is closed. The *List* tab with the new product in the product list is displayed.

7. Create an offer for the voucher product, see [Create an offer for POS](#create-an-offer-for-pos).



### Define the voucher setting

You need to define the created product as a voucher to use it in the *POS* store.

#### Prerequisites

- At least one product to be defined as a voucher has been created in the *PIM* module, see [Create a voucher product](#create-a-voucher-product).
- The voucher product has been transferred to the *Omni-Channel* module. For detailed information, see [Create an offer from a PIM product](../../Channels/Operation/01_ManageOffers.md#create-an-offer-from-a-pim-product) in the *Omni-Channel* documentation.

#### Procedure

*Omni-Channel > Offers > Tab OFFERS*

![Offers](../../Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

1. Click the offer to the voucher.   
    The *Edit offer* view is displayed. The *Attributes* tab is preselected.

    ![Edit offer](../../Assets/Screenshots/Channels/Offers/Offers/EditOffer.png "[Edit offer]")

2. Scroll down in the attributes and enable the *Voucher* toggle.

3. Click the [SAVE] button in the upper right corner.
    The voucher is saved. The *Edit offer* view is closed.

    > [Info] When a voucher-offer is sold, a voucher code is created and printed on the receipt. The value of the voucher corresponds to the price of the voucher before discounts are applied.


<!---NEU-->
### Create an offer for pre&dash;printed vouchers

A *Knistr&trade;* integration is available for vouchers, with which pre-printed voucher cards can be used. The codes of these vouchers can be entered via barcode scan or manually. For detailed information, see the [Knistr](https://www.knistr.com "[//https:knistr.com]") website.   

Pre-printed vouchers have the following special features:

- The voucher cards can be used as refill cards, so that you do not need to define a fixed price for the voucher. When it is created, the cashier can individually load the voucher card with any amount.
- The amount entered when creating the voucher is added to the amount already existing on the voucher card.
- The voucher is created store-specific in the *Omni-Channel* module.

Note that the *Set for POS Store "Name of the store"* attribute set, which is inherited from the *POS base set*, contains the *Voucher* attribute, which allows you to classify an offer as a voucher. Since the voucher is store-specific, create the voucher offer in the *Omni-Channel* module.

#### Prerequisites

- The credentials for the Knistr&trade;connection have been specified. For detailed information, see [KNISTR credentials](../UserInterface/02a_GlobalSettings.md#knistr-credentials).
- The *Voucher* attribute is added to the *Set for POS Store "Name of the store"* attribute set.

#### Procedure

*Omni-Channel > Offers > Tab OFFERS*

![Offers](../../Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The [Manual offer ![Manual offer](../../Assets/Icons/Document.png "[Manual offer]") ] button and the [Create from PIM product ![Create from PIM product](../../Assets/Icons/Package.png "[Create from PIM product]") ] button are displayed.

    ![Add offer](../../Assets/Screenshots/Channels/Offers/Offers/AddOffer.png "[Add offer]")

2. Click the [Manual offer ![Manual offer](../../Assets/Icons/Document.png "[Manual offer]") ] button.   
    The *Create offer* window is displayed.

    ![Create manual offer](../../Assets/Screenshots/Channels/Offers/Offers/CreateManualOffer.png "[Create manual offer]")

3. Enter the desired SKU in the *SKU* field.

4. Click the *Select connection* drop-down list and select the connection for the store for which you want to create the voucher. All available connections are displayed in the list.   

5. Click the *Select attribute set* dropdown-list and select the *Set for POS Store "Name of the store"* for your store.

6. Click the [SAVE] button.   
     The *Edit offer "Name of the voucher"* view is displayed.

7. Define the voucher. Note the following:

    > [Info] This description relates to the *POS base set*. 

    - Enter **voucher** in the *Barcode* field.
    - Enter a default value in the *Price* field. This value can be overwritten individually when selling the voucher.
    - Enter the tax rate value in the *Tax rate* field and select the required tax class in the *Tax class* drop-down field.
    - Enable the *Voucher* toggle to classify the offer as a voucher.

8. Click the [SAVE] button.

9. Activate the new offer.
    


<!---NEU-->
## Add an age rating to a product

If you want to use the *Age rating* feature, the attribute set assigned to the PIM product should contain an age rating attribute in which the required minimum age of a buyer is specified. Refer to the *PIM Basic set* attribute set for this.     
For detailed information on configuring this feature, see [Display age rating](../UserInterface/02a_GlobalSettings.md#display-age-rating).

<!---NEU-->
## Create a price group for POS

Price groups are used to classify different prices that apply to customers to whom the same pricing criteria are applied, for example members or business partners.

### Create attributes for the POS price group

Define the attribute that is assigned to the customer master data later and in which the price group of the customer is stored. Assign this attribute to the customer master data attribute set. In addition, define the attribute that contains the POS price group. Assign this attribute to the related store-specific attribute set.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*DataHub > Settings > Tab ATTRIBUTES*

![Attributes](../../Assets/Screenshots/DataHub/Settings/Attributes/Attributes.png "[Attributes]")

1. Create the attribute that represent the POS price group, for example the *pos_price_group* attribute. It must be of the *string* data type. 

2. Assign this attribute to the *RetailSuite Customer* attribute set. 

3. Create the attribute(s), with which you define the price group itself, for example the *pos_member_price* attribute. You can assign this price group to offers later to be able to define a special price for customers assigned to this price group. It must be of the *Floating point number* data type. 

3. Assign this attribute to the *POS base set* attribute set.

For detailed information, see [Create an attribute](../../DataHub/Integration/01_ManageAttributes.md#create-an-attribute) in the *DataHub* documentation.


### Declare the price group attribute for customer master data

Declare the field in which the price group is stored in the customer master data. 

#### Prerequisites

*POS > Management > General setting > Entry Field for price group*

![Field for price group](../../Assets/Screenshots/POS/Management/GlobalSettings/FieldForPriceGroup.png "[Field for price group]")

Click the *Price group* drop-down list and select the field you want to use for storing the price group in the customer master data.


### Activate the price groups

Activate the price groups you want to use in your stores. You can also activate the price groups store-specific.

*POS > Management > Tab GLOBAL SETTINGS > Entry Active price group*   
*POS > Management > Tab STORES > Tab Admin settings > Entry Active price group*

![Active price groups](../../Assets/Screenshots/POS/Management/GlobalSettings/ActivePriceGroups.png "[Active price groups]")

Enable the toggles next to the desired price groups.



### Add the price group price to offers

 Assign the attribute for defining the price group-related price, for example the *pos_member_price* attribute, to each offer, to which a price group-specific price should apply.   

 Because you added the price group attribute to the *POS base set*, the attribute is automatically inherited by all *Set for POS "Name of the store"* attribute groups. This means that it is available for all of your store-specific offers.

#### Prerequisites

The attribute for defining the price group-related price has been defined in the *DataHub* module.

#### Procedure

*Omni-Channel > Offers*

![Offers](../../Assets/Screenshots/Channels/Offers/Offers/Offers.png)

1. Click the *Connections* drop-down list and select the connection to the store, for which you want to assign the price group price to the offers.

2. Select an offer, for which a special price group price should apply. If the offer has a master offer with variants, select this one. This allows that the price is automatically inherited by all variants.    
    The *Edit offer "offer name"* view is displayed. The *Attributes* tab is displayed by default. Only the *Unassigned Group* is available.

    ![Edit offer](../../Assets/Screenshots/POS/Management/Customizing/PriceGroupOffer.png "[Edit offer]")

3. Scroll down to the attribute you have created, see [Create the POS price group attributes](#create-the-pos-price-group-attributes).

4. Enter the price.

5. Click the [SAVE] button.



<!---NEU-->
## Create a product option 

You might want to associate additional services to an offer. If your store has the appropriate technical capabilities, you might want to offer shirts with an optional flocking, or photos with an optional printing on cups and other objects. In these cases, a specific service is associated to an offer.   

From a technical point of view, you have to associate a product/service to an existing product.



### Define a product option
Define a product option that describes the additional service to an offer, for example, photo print or flocking.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*POS > Management > Tab PRODUCT OPTIONS*

![Product options](../../Assets/Screenshots/POS/Management/Customizing/ProductOptions.png "[Product options]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create option attribute* window is opened.

2. Enter a name for the product option in the *Name* field.

3. Enter a key for the product option in the *Key* field.

4. Click the [SAVE] button.    
    The new attribute is saved. It is automatically saved in the *DataHub* module with the *Related offers* data type and added to the *Set for POS Store ("Name of the store")* and the *POS base set* attribute sets. Since the *POS base set* attribute set is inherited automatically to the *Set for POS Store ("Name of the store")* attribute sets, it is also available for each newly created store.

5. If desired, add additional product options.


### Add additional attributes

You might want to have the possibility to specify a product option more precisely. For example, you want to offer to print a text on a shirt or a cup. In this case, you must create one or more attributes, in which the cashiers can enter a text or select a predefined text. 

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

Create the additional attributes you require. For detailed information, see [Manage an attribute](../../PIM/Integration/01_ManageAttributes.md) in the *PIM* documentation.

Test option zu Set for Actindo2 hinzugefügt


### Create an offer option set for store

In addition to the store-specific variant set you must create an offer option variant set for the product option. 
Here you can add additional attributes, for example, attributes for editing a text to be printed on an item.
> [Info] The variant set for your store has been automatically created when creating the store. It is inherited from the  

