# Create a variant

Create a variant product to create a product with a special characteristic dependent on its master product. The defining attributes for the variant product are preset in its [variant set](ManageVariantSet.md). You can either create a variant directly when you create a master product, or you can create variants subsequently for an existing master product. Further, you can create a single or multiple variants to a master product.


## Create a product with variants

You can create a single or multiple variants to a product directly when you create the master product.

### Prerequisites

- A variant set is created to the attribute set of the product you want to assign the variants to, see [Create an attribute set](ManageAttributeSet.md#create-an-attribute-set)

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

6. Click the tab *Variants* .   
The tab *Variants* is displayed.

![Variants](/Assets/Screenshots/PIM/Products/List/Varianten/VariantenEdit.png "[Variants]")

7. Click the drop-down list *Variant set* and select a variant set. All active variant sets to the corresponding attribute set of the product are displayed in the list.

8. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the variants area.   
The two buttons [Add single variant ![Add single variant](/Assets/Icons/Document.png "[Add single variant]") ] and [Add multiple variants ![Add multiple variants](/Assets/Icons/Documents.png "[Add multiple variants]") ] are displayed.


#### Create a single variant

1. Click the button [Add single variant ![Add single variant](/Assets/Icons/Document.png "[Add single variant]") ].   
The *Add single variant* window is displayed.

  ![Add single variant](/Assets/Screenshots/PIM/Products/List/Varianten/AddSingleVariant.png "[Add single variant]")

2. If desired, deactivate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use formula* and change the SKU in the field *sku*. By default, the toggle is activated and the predefined SKU is displayed.   

3. Select a value for the displayed attributes in the section *Defined values*. The fields differ depending on the selection of defining attributes for the variant set.  

4. Click the button [SAVE] in the bottom right corner.   
  The new variant is added to the product. The *Add single variant* window is closed. The product variant is displayed in the variants list.

5. Click the button [SAVE] in the upper right corner.   
  The variant is saved. The product view is closed. The product variant is displayed in the products list when you enable the **List all products** option in the drop-down list *Variants* at the top of the products list.


#### Create multiple variants

1. Click the button [Add multiple variants ![Add multiple variants](/Assets/Icons/Documents.png "[Add multiple variants]") ].   
The *Select values* wizard window is displayed.

  ![Select values wizard](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants01.png "[Select values wizard]")

2. Select a value for the displayed attributes in the areas. The fields and areas differ depending on the selection of defining attributes for the variant set.

3. Click the button [ADD VALUE] in the upper right corner of an area to add a further variant with another value.   
A further row is displayed in the area.

 > [Info] If you want to add a variant for each existing value, click the button [ADD ALL VALUES] in the area. This button is only available for certain attributes.

4. Click the button [NEXT] in the bottom right corner of the window.   
  The *Summary* wizard window is displayed.

  ![Summary wizard](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants02.png "[Summary wizard]")

5. Check if all variants listed in the area *Variants that will be created (ignoring duplicated)* are correct. If necessary, select the checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the variant you want to remove from the list and click the button ![Delete](/Assets/Icons/Trash03.png "[Delete]") in the editing toolbar.   
  The selected variants are removed from the list.

6. Click the button [FINISH] in the bottom right corner.   
  The new variants are added to the product. The *Summary* wizard window is closed. The product variants are displayed in the variants list.

  ![Summary wizard](/Assets/Screenshots/PIM/Products/List/Varianten/AddMultipleVariants02.png "[Summary wizard]")


7. Click the button [SAVE] in the upper right corner.   
  The variant is saved. The product view is closed. The product variants are displayed in the products list when you enable the **List all products** option in the drop-down list *Variants* at the top of the products list.

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



## Create a variant to a product


### Prerequisites

- At least one product is created, see [Create a product](#create-a-product).
- A variant set is created to the attribute set of the master product, see [Create an attribute set](ManageAttributeSet.md#create-an-attribute-set)

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the product you want to create one or more product variants to.   
  The *Edit Product* view is displayed. The tab *Attributes* is preselected.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesEdit.png "[Attributes]")

2. Click the tab *Variants*.   
  The tab *Variants* is displayed.

  ![Variants](/Assets/Screenshots/PIM/Products/List/Varianten/VariantenEdit.png "[Variants]")

3. Click the drop-down list *Variant set* and select a variant set. All active variant sets to the corresponding attribute set of the product are displayed in the list.

4. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the variants area.   
  The two buttons [Add single variant ![Add single variant](/Assets/Icons/Document.png "[Add single variant]") ] and [Add multiple variants ![Add multiple variants](/Assets/Icons/Documents.png "[Add multiple variants]") ] are displayed.

5. Follow the steps described below:
  - To create a single variant to the product, see [Create a single variant](#create-a-single-variant)
  - To create multiple variants to the product, see [Create multiple variants](#create-multiple-variants)


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
