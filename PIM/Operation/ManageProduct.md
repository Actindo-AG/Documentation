# Manage a product

A product defines everything that can be offered and purchased on a market. All products are assigned to an attribute set and can be specified by the attributes within this set. You can create master products and [product variants](CreateVariant.md), edit products, archive, delete or restore products and copy products. To offer a product on a marketplace you have to create an offer to the product, see [Create an offer in PIM](#create-an-offer-in-PIM).

## Create a product

Create a product to offer it on a marketplace. You can create a master product or create product variants, see [Create a variant](CreateVariant.md#create-a-variant-to-a-product). In the following, the procedure to create a master product is described.

### Prerequisites

An attribute set is created, see [Create an attribute set](ManageAttributeSet.md#Create-an-attribute-set).

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  The *Create new product* window is displayed.

  ![Create new product](/Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[Create new product]")

2. Select a attribute set in the drop-down list *Select attribute set*. All active attribute sets are displayed in the drop-down list.

3. Enter a SKU for the product in the field *SKU*.

  > [Info] The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.

4. Click the button [CREATE].   
  The *Create Product* view is displayed. The tab *Attributes* is preselected.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesCreate.png "[Attributes]")

5. Enter the data for the product in the tab *Attributes*. You must at least complete the fields *Product Name*, *Price* and *Tax class*.   

  > [Info] All fields marked with the note *(required)* are used for the completeness calculation of product attributes. You can activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *show empty required attributes only* to display only the incomplete required attribute fields for the selected product.

6. Click the button [SAVE] in the upper right corner.   
  The new product is saved. The *Create product* view is closed. The product list with the new product is displayed.

### Next steps

- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)
- [Copy a product](#copy-a-product)
- [Create an offer in PIM](#create-an-offer-in-PIM)
- [Create a single channel offer in PIM](#create-a-sinlge-channel-offer-in-PIM)
- [Create a multiple channels offer in PIM](#create-a-multiple-channels-offer-in-PIM)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)



## Edit products

After you have created a product, you can edit it. Depending on the attribute settings, not all attribute values are editable.

### Edit a single product

-> what are the typical changes I make for a product?

#### Prerequisites

At least one product is created, see [Create a product](#create-a-product).

#### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the product you want to edit in the list of products.   
  The *Edit Product* view is displayed. The tab *Attributes* is preselected.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesEdit.png "[Attributes]")

2. Edit the desired data of the product in the corresponding fields and tabs.

3. Click the button [SAVE] in the upper right corner.   
  The changes are saved. The *Edit Product* view is closed.  

#### Next steps

- [Mass editing](#mass-editing)
- [Copy a product](#copy-a-product)
- [Create an offer in PIM](#create-an-offer-in-PIM)
- [Create a single channel offer in PIM](#create-a-sinlge-channel-offer-in-PIM)
- [Create a multiple channels offer in PIM](#create-a-multiple-channels-offer-in-PIM)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)


### Mass editing

The mass editing option enables to edit different attributes of multiple products at the same time.

#### Prerequisites

Several products are created, see [Create a product](#create-a-product).

#### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the products you want to edit.   
  The editing toolbar is displayed above the products list.

2. Click the button [START MASS EDITING] in the toolbar.   
  The *Mass Editing* window is displayed on the right side.

  ![Mass editing](/Assets/Screenshots/PIM/Products/List/MassEditing.png "[Mass editing]")

  > [Info] You can still add products to the mass editing process when the window is displayed. Just select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the products in the list and click the button [MASS EDITING >] in the editing toolbar to add the selected products to the mass editing list.    
  To remove a product from the mass editing list, click the button ![Remove](/Assets/Icons/Trash01.png "[Remove]") (Remove) right to the respective product. The button ![Remove](/Assets/Icons/Trash01.png "[Remove]") (Remove) is only displayed if you hover over a product in the list.

3. Click the button [START] to start the editing wizard.
  The *Select Attributes* window is displayed.

  ![Select attributes](/Assets/Screenshots/PIM/Products/List/SelectAttributes.png "[Select attributes]")

4. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes you want to edit and click the button [CONTINUE] in the bottom right corner.   
  The *Select Scopes and Languages* window is displayed.

  ![Select scopes and languages](/Assets/Screenshots/PIM/Products/List/SelectScopesLanguages.png "[Select scopes and languages]")

5. Select the appropriate scopes and languages by selecting the corresponding checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") in the sections *Select Scopes* and *Select Languages* and click the button [CONTINUE] in the bottom right corner.   

  The *Editing* window with the selected products and their attributes to be edited is displayed.

  ![Editing](/Assets/Screenshots/PIM/Products/List/Editing.png "[Editing]")

6. Edit the desired data of the products in the corresponding fields and click the button [CONTINUE] in the bottom right corner.   
The *Applying Changes* window and the message *Mass editing has been triggered* are displayed.

  ![Mass editing triggered](/Assets/Screenshots/PIM/Products/List/MassEditingTriggered.png "[Mass editing triggered]")

  The progress bar in the *Applying Changes* window displays **100%** when the changes has been applied.

  ![Applying changes](/Assets/Screenshots/PIM/Products/List/ApplyingChanges.png "[Applying changes]")

7. Click the button [FINALIZE] in the bottom right corner.   
  The changes are saved. The editing wizard window is closed.

#### Next steps

- [Copy a product](#copy-a-product)
- [Create an offer in PIM](#create-an-offer-in-PIM)
- [Create a single channel offer in PIM](#create-a-sinlge-channel-offer-in-PIM)
- [Create a multiple channels offer in PIM](#create-a-multiple-channels-offer-in-PIM)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)


## Copy a product

### Prerequisites

No prerequisites to fulfill.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Select the checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the product you want to copy.   
  The editing toolbar is displayed above the products list.

2. Click the button [COPY PRODUCT] in the toolbar.   
  The *Edit Product (Copy)* view is displayed. The tab *Attributes* is preselected. All attribute values from the selected product are adopted to the copied product.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesCopy.png "[Attributes]")

3. Enter a new SKU for the product in the field *SKU*.

  > [Info] The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.

4. Enter a new article name for the product in the field *Artikelname*.

5. Add or edit the data for the product in the tab *Attributes*. You must complete at least all mandatory fields.

  > [Info] All mandatory fields are marked with the note *(required)*.

6. Click the button [SAVE] in the upper right corner.   
  The product is saved. The *Edit product (Copy)* view is closed. The product list with the new product is displayed.

### Next steps

- [Create an offer in PIM](#create-an-offer-in-PIM)
- [Create a single channel offer in PIM](#create-a-sinlge-channel-offer-in-PIM)
- [Create a multiple channels offer in PIM](#create-a-multiple-channels-offer-in-PIM)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)


## Create an offer in PIM

### Create a single channel offer in PIM

#### Prerequisites


#### Procedure
*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the article you want to create an offer to in the article list.    
  The *Edit Product* view is displayed.

2. Click the tab *OFFERS*.   
  The tab *OFFERS* with a list of all existing offers of the product in all channels is displayed.

   ![PIM Offers](/Assets/Screenshots/PIM/Products/List/Offers/Offers.png "[PIM Offers]")

3. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
   The two buttons ![Single Channel](/Assets/Icons/Document.png "[Single Channel]") (Single Channel) and ![Multiple Channels](/Assets/Icons/Documents.png "[Multiple Channels]") (Multiple Channels) are displayed.

4. Click the button ![Single Channel](/Assets/Icons/Document.png "[Single Channel]") (Single Channel) to create an offer from the selected PIM product to a single channel.   
   The *Create Channels Offer* window is displayed.

   ![Single Channel Offer](/Assets/Screenshots/PIM/Products/List/Offers/SingleChannel.png "[Single Channel Offer]")

5. Configure the following settings:

  + Select the marketplace for which you want to create the offers in the drop-down list *Connection*, e. g. the appropriate POS Store.   
  The drop-down list *Select Attribute Set* is unlocked.

  + Select the appropriate attribute set for the offer in the drop-down list *Select Attribute Set*.

  + Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") to automatically generate a SKU for the product in the offer.   

  + Select one of the radio buttons for the *ETL mode* :   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.

  + Select initial offer status in the drop-down list *Status* :   
    + *Active*: The offer is active. It is displayed on the marketplace and can be sold there.   
    + *Inactive*: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.   
    + *N/A*: The offer is unknown to the marketplace and therefore cannot be sold there.   


6. Click the button [SAVE] in the bottom right corner of the *Create Channels Offer* window.   
  The new offer will be created. The *Create Channels Offer* window is closed. The tab *OFFERS* with the new offer in the *Channel Offers* list is displayed.

  > [Info] It may take some time until the channel offer is created.

7. Click the button [SAVE] in the upper right corner.   
  The *Edit Product* view is closed. The tab *LIST* with the product list is displayed again.

#### Next steps

- [Create a multiple channels offer in PIM](#create-a-multiple-channels-offer-in-PIM)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)
- [Copy a product](#copy-a-product)
- [Create an offer in Omni-Channel](to_be_completed)


### Create a multiple channels offer in PIM

#### Prerequisites


#### Procedure
*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the article you want to create an offer to in the article list.    
  The *Edit Product* view is displayed.

2. Click the tab *Offers*.   
  The tab *Offers* with a list of all existing offers of the product in all channels is displayed.

   ![PIM Offers](/Assets/Screenshots/PIM/Products/List/Offers/Offers.png "[PIM Offers]")

3. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
   The two buttons ![Single Channel](/Assets/Icons/Document.png "[Single Channel]") (Single Channel) and ![Multiple Channels](/Assets/Icons/Documents.png "[Multiple Channels]") (Multiple Channels) are displayed.

4. Click the button ![Multiple Channels](/Assets/Icons/Documents.png "[Multiple Channels]") (Multiple Channels) to create an offer from the selected PIM product to multiple channels.   
  The wizard window *Select Channels and status* is displayed.

   ![Select Channels and status](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels1.png "[Select Channels and status]")

5. Configure the following settings:

  + Select initial offer status in the drop-down list *Status*:
    + *Active*: The offer is active. It is displayed on the marketplace and can be sold there.
    + *Inactive*: The offer is inactive. It is not displayed on the marketplace and cannot be sold there.
    + *Not available*: The offer is unknown to the marketplace and therefore cannot be sold there.   

  + Select one of the radio buttons for the ETL mode:   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offers.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offers.


  + Activate the toggles ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") of the marketplaces for which you want to create the offers in the section *Select connections*. If you want to create an offer for all channels, click the button [SELECT ALL] to activate all toggles.

6. Click the button [FINISH] in the bottom right corner of the window.   
  The *Select destination attribute sets* wizard window is displayed.

   ![Select destination attribute sets](/Assets/Screenshots/PIM/Products/List/Offers/MultipleChannels2.png "[Select destination attribute sets]")

   > [Info] The attribute destination sets for the selected channels are automatically selected. You cannot edit the selection.

  [comment]: <> (Is that correct? Why does this window exist when I cannot make any changes?)

7. Click the button [FINISH] in the upper right corner of the window.   
  The new offers will be created. The *Select destination attribute sets* wizard window is closed. The tab *OFFERS* with the new offers in the *Channel Offers* list is displayed.

    > [Info] It may take some time until the channel offer is created.

8. Click the button [SAVE] in the upper right corner.   
The *Edit Product* view is closed. The tab *LIST* with the product list is displayed again.

#### Next steps


#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)
- [Copy a product](#copy-a-product)
- [Create a single channel offer in PIM](#create-a-sinlge-channel-offer-in-PIM)
- [Create an offer in Omni-Channel](to_be_completed)
