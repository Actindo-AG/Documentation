# Manage a product

A product defines everything that can be offered and purchased on a market. All products are assigned to an attribute set and can be specified by the attributes within this set. You can create master products and product variants, edit products, archive, delete or restore products and copy products. To offer a product on a marketplace you have to create an offer to the product, see [Create an offer](to_be_completed).

## Create a product

Create a product to offer it on a marketplace. You can create a master product or create product variants to an existing master product, see [Create a variant](#create-a-variant-to-a-product).

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

- [Edit an attribute set](#edit-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Import an attribute set](#import-an-attribute-set)
- [Export an attribute set](#export-an-attribute-set)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)


## Edit products


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

  - [To be completed](#to_be_completed)
  - [To be completed](#to_be_completed)

#### See also

  - [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
  - [To be completed](#to_be_completed)


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

  - [To be completed](#to_be_completed)
  - [To be completed](#to_be_completed)

#### See also

  - [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
  - [To be completed](#to_be_completed)


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

- [To be completed](#to_be_completed)
- [To be completed](#to_be_completed)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [To be completed](#to_be_completed)
