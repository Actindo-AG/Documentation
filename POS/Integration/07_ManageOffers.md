[!!PIM](PIM)
[!!Venduo POS](POS)
[!!DataHub](DataHub)
[!!Omni-Channel](Channels)


# Manage offers for POS

To to offer products in Venduo POS, it is recommended to create the products in advance and create the corresponding offers afterwards in order to be able to distribute them properly in the system.

## Create products for POS

To create an offer for POS, it is recommended to create products for which you can make an offer.

### Prerequisites

No prerequisites to fulfill.

### Procedure

*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create new product* window is displayed.

   ![New Product](/Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[New Product]")

2. Click the *Select product type* drop-down list and select the appropriate product type.

  > [Info] If you have not created a new product type, the only available product type is **PIM Basic Product** .   
    For detailed information on how to create a product type for POS, see [Create a product type](#create-a-product-type).

3. Enter a SKU in the *SKU* field.

  > [Info] The SKU (Stock Keeping Unit) is an identification number for the article. Therefore, it has to be uniquely assigned to a single article and should not be changed once assigned.

4. Click the button [CREATE] in the bottom right corner.   
  The *Create new product* window is closed. The *Create product* view is displayed in the *List* tab. The sub  *Attributes* tab is preselected.

   ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesCreate.png "[Attributes]")

5. Enter the article data in the fields of the tab *Attributes*. You must at least enter an article name, a price and a tax class.

  > [Info] If you want to create a variant article you have to specify it in the *Variants* tab.   
  For detailed information on how to create a variant article, see [Create a variant article](/PIM/Integration/Manage_VariantSet.md#create-a-variant-set).

6. Click the button [SAVE] in the upper right corner.   
  The new article is saved. The *Create product* view is closed. The *List* tab with the new article in the article list is displayed.

[comment]: <> (Please explain the difference between product and article!)

### Next steps

- [Create a product type](#create-a-product-type)
- [Map a new product type in POS](#map-a-new-product-type-in-pos)
- [Create a QuickSelect Category](#create-a-quickselect-category)
- [Create a voucher](#create-a-voucher)
- [Create an offer for POS](#create-an-offer-for-pos)
- [Activate a POS offer](#activate-a-pos-offer)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)


## Create a product type

To improve the product classification, you can create a product type and use it in POS.   
For detailed information on how to create a product type, see [Create a product type](/PIM/Integration/Manage_AttributeSet.md#create-an-attribute-set)

### Next steps

- [Map a new product type in POS](#map-a-new-product-type-in-pos)
- [Create a QuickSelect Category](#create-a-quickselect-category)
- [Create a voucher](#create-a-voucher)
- [Create an offer for POS](#create-an-offer-for-pos)
- [Activate a POS offer](#activate-a-pos-offer)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create products for POS](#create-products-for-pos)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)


## Map a new product type in POS

When a new product type is created, it must be mapped before offers with this product type can be created for the POS.

### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos).

### Procedure

*Venduo POS > Management > Tab MAPPING FROM PIM*

![Mapping from PIM](/Assets/Screenshots/POS/Management/MappingFromPIM/MappingFromPIM01.png "[Mapping from PIM]")

1. Click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner.   
All not mapped PIM product types are displayed in the list.

   ![Mapping from PIM](/Assets/Screenshots/POS/Management/MappingFromPIM/MappingFromPIM02.png "[Mapping from PIM]")

2. Select the checkboxes of the product types you want to map.   
A toolbar is displayed at the bottom.

3. Click the [CREATE MAPPINGS] button in the toolbar.    
The selected mappings are removed from the list when the mappings are created.

### Next steps

- [Create a QuickSelect Category](#create-a-quickselect-category)
- [Create a voucher](#create-a-voucher)
- [Create an offer for POS](#create-an-offer-for-pos)
- [Activate a POS offer](#activate-a-pos-offer)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Create products for POS](#create-products-for-pos)
- [Create a product type](#create-a-product-type)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)


## Create a QuickSelect Category

Create a QuickSelect Category for POS for faster access to favorite products.

### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos)

### Procedure

#### Create a QuickSelect attribute
*DataHub > Settings > Tab ATTRIBUTES*

![DataHub Attributes](/Assets/Screenshots/DataHub/Settings/Attributes/Attributes.png "[DataHub Attributes]")

1. Enter **QuickSelect** in the search bar and click the ![Search](/Assets/Icons/Search.png "[Search]") (Search) button.   
  The matching attributes are displayed in the attributes list.

2. Click the appropriate *QuickSelect Category* attribute in the attributes list.  
  The *Edit Attribute* view is diplayed.

   ![Edit Attribute](/Assets/Screenshots/DataHub/Settings/Attributes/EditAttribute.png "[Edit Attribute]")

3. Scroll down to the *CONFIGURATION* section and click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner of the *Edit tree* table.
  A plus sign is displayed in the left column of the *Edit tree* table.

   ![Edit Tree](/Assets/Screenshots/DataHub/Settings/Attributes/EditTree.png "[Edit Tree]")

4. Click the plus sign in the left column of the *Edit tree* table.   
  The *Add Element* window is displayed.

   ![Add Element](/Assets/Screenshots/DataHub/Settings/Attributes/AddElement.png "[Add Element]")

5. Enter a name in the *Name* field.

  > [Info] The entered name equals the name of the QuickSelect element that will be displayed in Venduo POS.

6. If desired, enter a key in the *Key* field.

  > [Info] By entering a key, you can define an icon for the QuickSelect element.   
    For detailed information on the icon list, see [QuickSelect Icon List](to_be_completed).

7. Click the [SAVE] button in the bottom right corner of the *Add Element* window.   
  The *Add Element* window is closed. The element is displayed in the left column of the *Edit tree* table.

    > [Info] If you want to create further QuickSelect elements, repeat step **3** to **6**.

8. Click the button [SAVE] in the upper right corner.   
  The *Edit Attribute* view is closed. The QuickSelect element is saved.

9. Press **F5** to initialize the Core1 Platform.

10. Switch to the *Omni-Channel* module.

#### Select the QuickSelect attribute
*Omni-Channel > Offers > Tab OFFERS* .   

![Offers](/Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

1. Click the offer you want to create the QuickSelect element to.   
  The *Edit offer* view of the selected offer is displayed. The *Attributes* tab is preselected.

   ![Edit offer](/Assets/Screenshots/Channels/Offers/Offers/EditOffer.png "[Edit offer]")

2. Scroll down in the *Attribute* tab and select the QuickSelect element in the *QuickSelect Category* drop-down list.

3. Click the [SAVE] button in the upper right corner.    
  The *Edit offer* view is closed. The offer with the QuickSelect element is saved.

> [Info] You have to repeat this procedure for each offer you want to assign the QuickSelect Category to. Alternatively, you can ------

[comment]: <> (JULIAN: Hier könnten man noch unterbringen wie man zusätzliche Felder mapped ausm PIM raus oder Felder ausm Omni-Channel ins PIM übernimmt)

### Next steps

- [Create a voucher](#create-a-voucher)
- [Create an offer for POS](#create-an-offer-for-pos)
- [Activate a POS offer](#activate-a-pos-offer)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [User Interface Omni-Channel](/Channels/UserInterface/00_UserInterface.md)
- [Map a new product type in POS](#map-a-new-product-type-in-pos)
- [Create products for POS](#create-products-for-pos)
- [Create a product type](#create-a-product-type)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)


## Create a voucher

If you want to sell vouchers in your POS system, you have to create them first.

### Prerequisites

No prerequisites to fulfill.

### Procedure

#### Create a voucher product
*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create new product* window is displayed.

   ![New Product](/Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[New Product]")

2. Click the *Select product type* drop-down list and select the appropriate product type.

  > [Info] If you have not created a new product type, the only available product type is **PIM Basic Data** .   
  For detailed information on how to create a product type for POS, see [Create a product type](#create-a-product-type).

3. Enter a SKU in the *SKU* field, for instance **Voucher**.

> [Info] The SKU (Stock Keeping Unit) is an identification number for the article. Therefore, it has to be uniquely assigned to a single article and should not be changed once assigned.

4. Click the button [CREATE] in the bottom right corner of the *Create new product* window.   
  The *Create new product* window is closed. The *Create product* view is displayed in the *List* tab. The *Attributes* tab is preselected.

   ![Attribute](/Assets/Screenshots/PIM/Products/List/CreateProduct.png "[Attributes]")

5. Enter the article data in the fields of the *Attributes* tab. You must at least enter an article name, a price and a tax class.

6. Click the button [SAVE] in the upper right corner.   
  The new article is saved. The *Create product* view is closed. The *List* tab with the new article in the article list is displayed.

7. Create an offer for the voucher article, see [Create an offer for POS](#create-an-offer-for-pos)

8. Switch to the *Omni-Channel* module.


#### Activate the voucher attribute setting
*Omni-Channel > Offers > Tab OFFERS*

![Offers](/Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

1. Click the offer to the voucher.   
  The *Edit offer* view is displayed. The *Attributes* tab is preselected.

   ![Edit offer](/Assets/Screenshots/Channels/Offers/Offers/EditOffer.png "[Edit offer]")

2. Scroll down in the attributes and activate the *Voucher* toggle.

3. Click the [SAVE] button in the upper right corner.
The voucher is saved. The *Edit offer* view is closed.

  > [Info] When a voucher-offer is sold, a voucher code is created and printed on the receipt. The value of the voucher corresponds to the price of the voucher before discounts are applied.

### Next steps

- [Create an offer for POS](#create-an-offer-for-pos)
- [Activate a POS offer](#activate-a-pos-offer)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface)
- [Create a QuickSelect Category](#create-a-quickselect-category)
- [Map a new product type in POS](#map-a-new-product-type-in-pos)
- [Create products for POS](#create-products-for-pos)
- [Create a product type](#create-a-product-type)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)


## Create an offer for POS

Create an offer in Omni-Channel so you can offer and select the products in Venduo POS. You can either create an offer from a PIM product or create a manual offer.

### Prerequisites

At least one product has been created, see [Create products for POS](#create-products-for-pos)

### Procedure

#### Create an offer from a PIM product in Omni-Channel

*Omni-Channel > Offers > Tab OFFERS*

![Offers](/Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The ![Manual Offer](/Assets/Icons/Document.png "[Manual Offer]") (Manual Offer) button and the ![PIM Offer](/Assets/Icons/Package.png "[PIM Offer]") (aus PIM-Produkt erstellen) button are displayed.

  > [Info] If the product you want to create an offer for exists in PIM, it is recommended to create the offer from the PIM product instead of creating a manual offer.

2. Click the ![PIM Offer](/Assets/Icons/Package.png "[PIM Offer]") (aus PIM-Produkt erstellen) button to create an offer from a PIM product.   
  The *Select Marketplace* wizard window is displayed.

   ![Select Marketplace](/Assets/Screenshots/Channels/Offers/Offers/PIMOffer/PO01.png "[Select Marketplace]")

3. Configure the following settings:

  + Select one of the radio buttons:
    + **All products**:  Offers for all existing PIM products are created.
    + **Select Products**: Select manually the products you want to create an offer for.    

  + Select the marketplace for which you want to create the offers in the *Connection* drop-down list, for instance the appropriate POS Store.

    > [Info] A POS Store is handled like a marketplace in Omni-Channel.

  + Activate the *Do not create duplicates* toggle to automatically exclude offers that already exist from the creation process.  

    > [Info] Be aware that, if you deactivate the *Do not create duplicates* toggle, existing offers are created again, an automatically generated SKU is assigned to them and they exist in addition to the original offers.


4. Click the button [CONTINUE] in the bottom right corner.    
  If you have selected the *All products* radio button, continue with step **8** .   
  If you have selected the *Select Products* radio button, the *Select Products* wizard window is displayed.

   ![Select Products](/Assets/Screenshots/Channels/Offers/Offers/PIMOffer/PO02.png "[Select Products]")

5. Select the checkboxes of all products to which you want to create an offer for.   
  A toolbar is displayed above the product list.

6. Click the [ADD TO SELECTION >] button in the toolbar.   
  The selected products are added to the *Add to selection Products* section on the right side of the wizard window.

7. Click the [CONTINUE] button in the upper right corner.   
  The *Review and finalize* wizard window is displayed.

   ![Review and finalize](/Assets/Screenshots/Channels/Offers/Offers/PIMOffer/PO03.png "[Review and finalize]")

8. Configure the following settings:

  + Select one of the radio buttons for the *ETL mode* section:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.

  + Select one of the radio buttons for the *Initial offer status* section:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *Active*: The offer is active. It is displayed on the marketplace and can be sold there.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *Inactive*: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *Offline*: The offer is unknown to the marketplace and therefore cannot be sold there.

[comment]: <> (Note for reuse: In case of webshops the procedure can be little bit more complicated because there are potential conflicts to be resolved)

9. Click the button [CREATE OFFERS] in the upper right corner.   
   The *Product import from PIM scheduled* message is displayed. The offers will be created. The creation process starts asynchronously, so that it may take some time until the offer creation starts.

   ![Import scheduled](/Assets/Screenshots/Channels/Offers/Offers/ProductImportScheduled.png "[Import scheduled]")

   > [Info] It may take some time until all offers are created. Click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner to update the offer list.

#### Create a manual offer in Omni-Channel

*Omni-Channel > Offers > Tab OFFERS*

![OC Offers](/Assets/Screenshots/Channels/Offers/Offers/Offers.png "[OC Offers]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The ![Manual Offer](/Assets/Icons/Document.png "[Manual Offer]") (Manual Offer) button and the ![PIM Offer](/Assets/Icons/Package.png "[PIM Offer]") (aus PIM-Produkt erstellen) button are displayed.

   > [Info] If the product you want to create an offer for exists in PIM, it is recommended to create the [offer from the PIM product](#create-an-offer-from-a-pim-product-in-Omni-Channel) instead of creating a manual offer.

2. Click the ![Manual Offer](/Assets/Icons/Document.png "[Manual Offer]") (Manual Offer) button to create a manual offer.   
  The *Create Offer* window is displayed.

   ![Create Offer](/Assets/Screenshots/Channels/Offers/Offers/Create.png "[Create Offer]")

3. Enter a SKU in the *SKU* field.

> [Info] The SKU (Stock Keeping Unit) is an identification number for the article. Therefore, it has to be uniquely assigned to a single article and should not be changed once assigned.

4. Click the *Select Connection* drop-down list and select the marketplace for which you want to create the offers, for instance the appropriate POS Store.   
  The *Select Attribute Set* drop-down list is unlocked.

5. Click the *Select Attribute Set* drop-down list and select the appropriate attribute set for the offer.

6. Click the [SAVE] button in the bottom right corner of the *Create Offer* window.   
  The *Create Offer* window is closed. The *Create Offer* view is displayed. The *Attributes* tab is preselected.

   ![Create Offer](/Assets/Screenshots/Channels/Offers/Offers/CreateOffer.png "[Create Offer]")

7. Enter the article data in the fields of the *Attributes* tab. You must at least enter an article name, an EAN code, a price, a tax class and a tax rate.

  > [Info] If you want to create a variant article you have to specify it in the *Variants* tab.   
  For detailed information on how to create a variant article, see [Create a variant article](to_be_completed).

8. Click the [SAVE] button in the upper right corner.   
  The new offer is created. The *Create Offer* view is closed. The *Offers* tab with the new offer in the offer list is displayed.

  > [Info] By default, the initial offer status of the new offer is **Not available**. You have to activate the offer to sell it on the marketplace, see [Activate a POS offer](#activate-a-pos-offer).

#### Create a single channel offer in PIM

*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the article you want to create an offer to in the article list.    
  The *Edit Product* view is displayed.

2. Click the *OFFERS* tab.   
  The *OFFERS* tab with a list of all existing offers of the product in all channels is displayed.

   ![PIM Offers](/Assets/Screenshots/PIM/Products/List/Offers/Offers.png "[PIM Offers]")

3. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
   The ![Single Channel](/Assets/Icons/Document.png "[Single Channel]") (Single Channel) button and the ![Multiple Channels](/Assets/Icons/Documents.png "[Multiple Channels]") (Multiple Channels) button are displayed.

4. Click the ![Single Channel](/Assets/Icons/Document.png "[Single Channel]") (Single Channel) button to create an offer from the selected PIM product to a single channel.   
   The *Create Channels Offer* window is displayed.

   ![Single Channel Offer](/Assets/Screenshots/PIM/Products/List/Offers/SingleChannel.png "[Single Channel Offer]")

5. Configure the following settings:

  + Select the marketplace for which you want to create the offers in the *Connection* drop-down list, for instance the appropriate POS Store.   
  The *Select Attribute Set* drop-down list is unlocked.

  + Select the appropriate attribute set for the offer in the *Select Attribute Set* drop-down list.

  + Activate the toggle to automatically generate a SKU for the product in the offer.   

  + Select one of the radio buttons for the ETL mode:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.

  + Select initial offer status in the *Status* drop-down list:   
    + *Active*: The offer is active. It is displayed on the marketplace and can be sold there.   
    + *Inactive*: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
    + *N/A*: The offer is unknown to the marketplace and therefore cannot be sold there.   


6. Click the button [SAVE] in the bottom right corner of the *Create Channels Offer* window.   
  The new offer will be created. The *Create Channels Offer* window is closed. The *OFFERS* tab with the new offer in the *Channel Offers* list is displayed.

  > [Info] It may take some time until the channel offer is created.

7. Click the button [SAVE] in the upper right corner.   
  The *Edit Product* view is closed. The *LIST* tab with the product list is displayed again.


#### Create a multiple channels offer in PIM

*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the article you want to create an offer to in the article list.    
  The *Edit Product* view is displayed.

2. Click the *Offers* tab.   
  The *Offers* tab with a list of all existing offers of the product in all channels is displayed.

   ![PIM Offers](/Assets/Screenshots/PIM/Products/List/Offers/Offers.png "[PIM Offers]")

3. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
   The ![Single Channel](/Assets/Icons/Document.png "[Single Channel]") (Single Channel) button and the ![Multiple Channels](/Assets/Icons/Documents.png "[Multiple Channels]") (Multiple Channels) button are displayed.

4. Click the ![Multiple Channels](/Assets/Icons/Documents.png "[Multiple Channels]") (Multiple Channels) button to create an offer from the selected PIM product to multiple channels.   
  The *Select Channels and status* wizard window is displayed.

   ![Select Channels and status](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels1.png "[Select Channels and status]")

5. Configure the following settings:

  + Select initial offer status in the *Status* drop-down list:
    + **Active**: The offer is active. It is displayed on the marketplace and can be sold there.
    + **Inactive**: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.
    + **Not available**: The offer is unknown to the marketplace and therefore cannot be sold there.   

  + Select one of the radio buttons for the ETL mode:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.


  + Activate the toggles of the marketplaces for which you want to create the offers in the *Select connections* section. If you want to create an offer for all channels, click the [SELECT ALL] button to activate all toggles.

6. Click the [FINISH] button in the bottom right corner of the window.   
  The *Select destination attribute sets* wizard window is displayed.

   ![Select destination attribute sets](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels2.png "[Select destination attribute sets]")

   > [Info] The attribute destination sets for the selected channels are automatically selected. You cannot edit the selection.

  [comment]: <> (Is that correct? Why does this window exist when I cannot make any changes?)

7. Click the [FINISH] button in the upper right corner of the window.   
  The new offers will be created. The *Select destination attribute sets* wizard window is closed. The *OFFERS* tab with the new offers in the *Channel Offers* list is displayed.

    > [Info] It may take some time until the channel offer is created.

8. Click the [SAVE] button in the upper right corner.   
The *Edit Product* view is closed. The *LIST* tab with the product list is displayed again.

### Next steps

- [Activate a POS offer](#activate-a-pos-offer)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface Omni-Channel](/Channels/UserInterface/00_UserInterface.md)
- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a voucher](#create-a-voucher)
- [Create a QuickSelect Category](#create-a-quickselect-category)
- [Map a new product type in POS](#map-a-new-product-type-in-pos)
- [Create products for POS](#create-products-for-pos)
- [Create a product type](#create-a-product-type)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)


## Activate a POS offer

An offer has to be active so that it is displayed in the selected marketplace and can be sold there.

### Prerequisites

At least one offer has been created, see [Create an offer for POS](#create-an-offer-for-pos)

### Procedure

*Omni-Channel > Offers > Tab OFFERS*

![OC Offers Inactive](/Assets/Screenshots/Channels/Offers/Offers/OffersInactive.png "[OC Offers Inactive]")

1. Select the checkboxes of the offers you want to activate.   
  A toolbar is displayed above the offer list.

2. Click the *Change Status to* drop-down list  in the right side of the toolbar and select the **Active** option.   
  The **Active** status is displayed in the *Pending stauts/Errors* column of the selected offers.    

   ![OC Offers Pending](/Assets/Screenshots/Channels/Offers/Offers/OffersPending.png "[OC Offers Pending]")

   When the offers are active, the status in the *Pending stauts/Errors* column is no longer displayed, but the status in the *Status* column has changed to **Active**.

   > [Info] It may take some time until all offers are activated. Click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner to update the offer list.

### Next Steps

[Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface Omni-Channel](/Channels/UserInterface/00_UserInterface.md)
- [Create an offer for POS](#create-an-offer-for-pos)
- [Create a voucher](#create-a-voucher)
- [Create a QuickSelect Category](#create-a-quickselect-category)
- [Map a new product type in POS](#map-a-new-product-type-in-pos)
- [Create products for POS](#create-products-for-pos)
- [Create a product type](#create-a-product-type)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
