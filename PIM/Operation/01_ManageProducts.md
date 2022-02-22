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
- [Create a single scope offer in PIM](#create-a-single-scope-offer-in-PIM)
- [Create a multi-scope offer in PIM](#create-a-multi-scope-offer-in-PIM)
- [Create a variant](02_CreateVariant.md)
- [Move a product](03_MoveProduct.md)
- [Manage the product view](04_ManageProductView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)



## Edit products

After you have created a product, you can edit it.You can either edit a single product or use the mass editing function to edit the same attribute values in several products using a wizard. Depending on the attribute settings, not all attribute values are editable.

### Edit a single product

Edit one or several attribute values for a single product.

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
- [Create a single scope offer in PIM](#create-a-single-scope-offer-in-PIM)
- [Create a multi-scope offer in PIM](#create-a-multi-scope-offer-in-PIM)
- [Create a variant](02_CreateVariant.md)
- [Move a product](03_MoveProduct.md)
- [Manage the product view](04_ManageProductView.md)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)


### Mass editing

The mass editing function enables to edit different attribute values of multiple products at the same time.

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

  ![Select attributes](/Assets/Screenshots/PIM/Products/List/MassEditingWizard/SelectAttributes.png "[Select attributes]")

4. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes you want to edit and click the button [CONTINUE] in the bottom right corner.   
  The *Select Scopes and Languages* window is displayed.

  ![Select scopes and languages](/Assets/Screenshots/PIM/Products/List/MassEditingWizard/SelectScopesLanguages.png "[Select scopes and languages]")

5. Select the appropriate scopes and languages by selecting the corresponding checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") in the sections *Select Scopes* and *Select Languages* and click the button [CONTINUE] in the bottom right corner.   

  The *Editing* window with the selected products and their attributes to be edited is displayed.

  ![Editing](/Assets/Screenshots/PIM/Products/List/MassEditingWizard/Editing.png "[Editing]")

6. Edit the desired data of the products in the corresponding fields and click the button [CONTINUE] in the bottom right corner.   
The *Applying Changes* window and the message *Mass editing has been triggered* are displayed.

  ![Mass editing triggered](/Assets/Screenshots/PIM/Products/List/MassEditingWizard/MassEditingTriggered.png "[Mass editing triggered]")

  The progress bar in the *Applying Changes* window displays **100%** when the changes has been applied.

  ![Applying changes](/Assets/Screenshots/PIM/Products/List/MassEditingWizard/ApplyingChanges.png "[Applying changes]")

7. Click the button [FINALIZE] in the bottom right corner.   
  The changes are saved. The editing wizard window is closed.

#### Next steps

- [Copy a product](#copy-a-product)
- [Create an offer in PIM](#create-an-offer-in-PIM)
- [Create a single scope offer in PIM](#create-a-single-scope-offer-in-PIM)
- [Create a multi-scope offer in PIM](#create-a-multi-scope-offer-in-PIM)
- [Create a variant](02_CreateVariant.md)
- [Move a product](03_MoveProduct.md)
- [Manage the product view](04_ManageProductView.md)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)


## Copy a product

Use the copy function to duplicate a product and its properties to create a similar product where you only have to adjust individual attributes.

### Prerequisites

At least one product is created, see [Create a product](#create-a-product).

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

4. Enter a new product name for the product in the field *Product Name*.

5. Add or edit the data for the product in the tab *Attributes*. You must at least complete the fields *Product Name*, *Price* and *Tax class*.   

  > [Info] All fields marked with the note *(required)* are used for the completeness calculation of product attributes. You can activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *show empty required attributes only* to display only the incomplete required attribute fields for the selected product.

6. Click the button [SAVE] in the upper right corner.   
  The product is saved. The *Edit Product (Copy)* view is closed. The product list with the new product is displayed.

### Next steps

- [Create an offer in PIM](#create-an-offer-in-PIM)
- [Create a single scope offer in PIM](#create-a-single-scope-offer-in-PIM)
- [Create a multi-scope offer in PIM](#create-a-multi-scope-offer-in-PIM)
- [Create a variant](02_CreateVariant.md)
- [Move a product](03_MoveProduct.md)
- [Manage the product view](04_ManageProductView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)


## Create an offer in PIM

Create an offer to a product so you can sell the product in a selected connection. In the *PIM* module you can  create offers to all PIM products. You can either create an offer for a single scope or a multi-scope offer.

### Create a single scope offer in PIM

#### Prerequisites

- At least one product is created, see [Create a product](#create-a-product).    
- At least one scope is created, see [Create a scope](/DataHub/Integration/CreateScope.md).

> [Info] By default, the scope *Actindo Basic* is created and activated in the *PIM* module.

#### Procedure
*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the product you want to create an offer to in the product list.    
  The *Edit Product* view is displayed.

2. Click the tab *Offers* in the product view.   
  The tab *Offers* with a list of all existing offers to the product in all scopes is displayed.

   ![PIM Offers](/Assets/Screenshots/PIM/Products/List/Offers/Offers.png "[PIM Offers]")

3. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
   The two buttons [Add to a single scope ![Add to a single scope](/Assets/Icons/Document.png "[Single scope]") ] and [Add to multiple scopes ![Multiple scopes](/Assets/Icons/Documents.png "[Multiple scopes]") ] are displayed.

  ![Add Offer](/Assets/Screenshots/PIM/Products/List/Offers/AddEdit.png "[Add Offer]")

4. Click the button [Add to a single scope ![Add to a single scope](/Assets/Icons/Document.png "[Single scope]") ] to create an offer from the selected PIM product to a single scope.   
   The *Create Offer* window is displayed.

   ![Single scope offer](/Assets/Screenshots/PIM/Products/List/Offers/SingleScope.png "[Single scope offer]")

5. Configure the following settings:

  + Click the drop-down list *Select Scope* and select the scope for which you want to create the offer. All active scopes are displayed in the list.    
  The drop-down list *Select Attribute Set* is unlocked.

  + Click the drop-down list *Select Attribute Set* and select the appropriate attribute set for the offer. All active attribute sets are displayed in the list.   

  + Activate the toggle *![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Generate SKU* to automatically create a SKU for the product offer.   

  + Select the appropriate option for change tracking in the section *Change Tracking Mode* :   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-scope* module. The initial offer is automatically applied without confirmation.   
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic, changes must be confirmed by another user*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.    
   ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

  + Click the drop-down list *Offer Status* and select the initial offer status. The statuses below are available:   
    + *Active*: The offer is active. It is displayed in the selected scope and can be sold there.   
    + *Inactive*: The offer is inactive. It is not displayed in the selected scope and cannot be sold there.   
    + *N/A*: The offer is unknown to the selected scope and cannot be sold there.   


6. Click the button [SAVE] in the bottom right corner of the *Create Offer* window.   
The single offer is added to the list of offers. The *Create Offer* window is closed.

  > [Info] The product must be saved to start the creation process of the offer.


7. Click the button [SAVE] in the upper right corner.   
  The *Edit Product* view is closed. The tab *LIST* with the product list is displayed again. The new offer is being created.

  > [Info] It may take some time until the offer is finally created.

#### Next steps

- [Create a multi-scope offer in PIM](#create-a-multi-scope-offer-in-PIM)
- [Create a variant](02_CreateVariant.md)
- [Move a product](03_MoveProduct.md)
- [Manage the product view](04_ManageProductView.md)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)
- [Copy a product](#copy-a-product)
- [Create an offer in Omni-Channel](to_be_completed)


### Create a multi-scope offer in PIM

#### Prerequisites

- At least one product is created, see [Create a product](#create-a-product).    
- At least two scopes are created, see [Create a scope](/DataHub/Integration/CreateScope.md).

#### Procedure
*PIM > Products > Tab LIST*

![PIM Products](/Assets/Screenshots/PIM/Products/List/Products.png "[PIM Products]")

1. Click the product you want to create an offer to in the product list.    
  The *Edit Product* view is displayed.

2. Click the tab *Offers* .   
  The tab *Offers* with a list of all existing offers of the product in all scopes is displayed.

   ![PIM Offers](/Assets/Screenshots/PIM/Products/List/Offers/Offers.png "[PIM Offers]")

3. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
   The two buttons [Add to a single scope ![Add to a single scope](/Assets/Icons/Document.png "[Single scope]") ] and [Add to multiple scopes ![Multiple scopes](/Assets/Icons/Documents.png "[Multiple scopes]") ] are displayed.

  ![Add Offer](/Assets/Screenshots/PIM/Products/List/Offers/AddEdit.png "[Add Offer]")

4. Click the button [Add to multiple scopes ![Multiple scopes](/Assets/Icons/Documents.png "[Multiple scopes]") ] to create an offer from the selected PIM product to multiple scopes.   
  The wizard window *Select scopes and status* is displayed.

   ![Select scopes and status](/Assets/Screenshots/PIM/Products/List/Offers/MultipleScopes01.png "[Select scopes and status]")

5. Configure the following settings:

  + Click the drop-down list *Offer Status* and select the initial offer status. The statuses below are available:   
    + *Active*: The offer is active. It is displayed in the selected scope and can be sold there.   
    + *Inactive*: The offer is inactive. It is not displayed in the selected scope and cannot be sold there.   
    + *N/A*: The offer is unknown to the selected scope and cannot be sold there.   

  + Select the appropriate option for the change tracking mode:   
     ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *manual*: Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.   
     ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module. The initial offer is automatically applied without confirmation.   
     ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *semi-automatic, changes must be confirmed by another user*: Changes in a PIM product are automatically applied to the offer after confirmation in the *Omni-Channel* module by another user. The initial offer is only applied after confirmation by another user.    
     ![Radionbutton](/Assets/Icons/Radiobutton.png "[Radiobutton]") *automatic*: Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

  + Activate the toggles ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") of the scopes for which you want to create offers in the section *Select connections*. If you want to create an offer for all displayed scopes, click the button [SELECT ALL] to activate all toggles. All active scopes are displayed in the list.    

6. Click the button [CONTINUE] in the bottom right corner of the window.   
  The *Select destination attribute sets* wizard window is displayed.

   ![Select destination attribute sets](/Assets/Screenshots/PIM/Products/List/Offers/MultipleScopes02.png "[Select destination attribute sets]")

   > [Info] The attribute destination sets for the selected scopes are automatically selected. You cannot edit the selection.

  [comment]: <> (Is that correct? Why does this window exist when I cannot make any changes?)

7. Click the button [FINISH] in the bottom right corner of the window.   
  The new offers are added to the list of offers. The *Select destination attribute sets* wizard window is closed.

  > [Info] The product must be saved to start the creation process of the offers.

8. Click the button [SAVE] in the upper right corner.   
The *Edit Product* view is closed. The tab *LIST* with the product list is displayed again. The new offers are being created.

  > [Info] It may take some time until the offers are finally created.

#### Next steps

- [Create a variant](02_CreateVariant.md)
- [Move a product](03_MoveProduct.md)
- [Manage the product view](04_ManageProductView.md)

#### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a product](#create-a-product)
- [Edit products](#edit-products)
- [Edit a single product](#edit-a-single-product)
- [Mass editing](#mass-editing)
- [Copy a product](#copy-a-product)
- [Create a single scope offer in PIM](#create-a-single-scope-offer-in-PIM)
