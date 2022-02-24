# Manage the variants

A product variant is product with a special characteristic dependent on its master product. The defining attributes for the product variants are preset in their [variant set](/PIM/Integration/07_ManageVariantSets.md). You can create a variant directly when you create a master product, or you can add variants subsequently for an existing master product. Further, you can create a single variant or multiple variants to a master product.


## Create product variants

You can create a single or multiple product variants to a product directly when you create the master product. To add variants to an existing product, see [Add product variants](#add-product-variants).

### Prerequisites

A variant set is created to the attribute set of the product you want to assign the variants to, see [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set).

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
The *Create new product* window is displayed.

  ![Create new product](/Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[Create new product]")

2. Select an attribute set in the drop-down list *Select attribute set*. All active attribute sets are displayed in the drop-down list.

3. Enter a SKU for the product in the field *SKU*.

  > [Info] The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.

4. Click the button [CREATE].   
The *Create Product* view is displayed. The tab *Attributes* is preselected.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesCreate.png "[Attributes]")

5. Enter the data for the product in the tab *Attributes*. You must at least complete the fields *Product Name*, *Price* and *Tax class*.   

  > [Info] All fields marked with the note *(required)* are used for the completeness calculation of product attributes. You can activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *show empty required attributes only* to display only the incomplete required attribute fields for the selected product.

6. Click the tab *Variants* .   
The tab *Variants* is displayed.

  ![Variants](/Assets/Screenshots/PIM/Products/List/Variants/VariantsCreate.png "[Variants]")

7. Click the drop-down list *Variant set* and select a variant set. All active variant sets to the corresponding attribute set of the product are displayed in the list.

8. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the variants area.   
The two buttons [Add single variant ![Add single variant](/Assets/Icons/Document.png "[Add single variant]") ] and [Add multiple variants ![Add multiple variants](/Assets/Icons/Documents.png "[Add multiple variants]") ] are displayed.

9. Follow one of the described sub-procedures:
  - To create a single variant to the product, see [Create a single variant](#create-a-single-variant).
  - To create multiple variants to the product, see [Create multiple variants](#create-multiple-variants).


#### Create a single variant

*PIM > Products > Tab LIST > Button Add > Tab Variants > Select variant set > Button Add*   
*PIM > Products > Tab LIST > Select Product > Tab Variants > Button Add*

![Add variants](/Assets/Screenshots/PIM/Products/List/Variants/AddVariantCreate.png "[Add variants]")

1. Click the button [Add single variant ![Add single variant](/Assets/Icons/Document.png "[Add single variant]") ].   
  The *Add single variant* window is displayed.

  ![Add single variant](/Assets/Screenshots/PIM/Products/List/Variants/AddSingleVariant.png "[Add single variant]")

2. If desired, deactivate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use formula* and change the SKU in the field *sku*. By default, the toggle is activated and the predefined SKU is displayed.   

3. Select a value for the displayed attributes in the section *Defined values*. The fields differ depending on the selection of defining attributes for the variant set.  
  The selected attribute value is displayed in the area.

4. Click the button [SAVE] in the bottom right corner.   
  The new variant is added to the product. The *Add single variant* window is closed. The product variant is displayed in the variants list.

  ![Variant added](/Assets/Screenshots/PIM/Products/List/Variants/VariantAddedCreate.png "[Variant added]")

5. Click the button [SAVE] in the upper right corner.   
  The variant is saved. The product view is closed. The product variant is displayed in the products list when you enable the **List all products** option in the drop-down list *Variants* at the top of the products list.


#### Create multiple variants

*PIM > Products > Tab LIST > Button Add > Tab Variants > Select variant set > Button Add*   
*PIM > Products > Tab LIST > Select Product > Tab Variants > Button Add*

![Add variants](/Assets/Screenshots/PIM/Products/List/Variants/AddVariantCreate.png "[Add variants]")

1. Click the button [Add multiple variants ![Add multiple variants](/Assets/Icons/Documents.png "[Add multiple variants]") ].   
  The *Select Values* wizard window is displayed.

  ![Select values wizard](/Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants01.png "[Select values wizard]")

2. Select a value for the displayed attributes in the areas. The fields and areas differ depending on the selection of defining attributes for the variant set.   
  The selected attribute value is displayed in the area.

3. Click the button [ADD VALUE] in the upper right corner of the area to add a further variant with another value.   
  A further row is displayed in the area.

  > [Info] If you want to add a variant for each existing value, click the button [ADD ALL VALUES] in the area. This button is only available for certain attributes.

4. Select a value for the attribute in the new row.
  The selected attribute value is displayed in the area.

  > [Info] Repeat the steps **3** and **4** to add further variants.

5. Click the button [NEXT] in the bottom right corner of the window.   
  The *Summary* wizard window is displayed.

  ![Summary wizard](/Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants02.png "[Summary wizard]")

6. Check if all variants listed in the area *Variants that will be created (ignoring duplicated)* are correct.

  > [Info] To remove a variant from the list, select the checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the variant and click the button ![Delete](/Assets/Icons/Trash03.png "[Delete]") in the editing toolbar displayed above the list.

7. Click the button [FINISH] in the bottom right corner.   
  The new variants are added to the product. The *Summary* wizard window is closed. The product variants are displayed in the variants list.

  ![Variants added](/Assets/Screenshots/PIM/Products/List/Variants/VariantsAddedCreate.png "[Variants added]")

8. Click the button [SAVE] in the upper right corner.   
  The variant is saved. The product view is closed. The product variants are displayed in the products list when you enable the **List all products** option in the drop-down list *Variants* at the top of the products list.

  > [Info] For detailed information about the different views, see [Manage the view](04_ManageView.md).

### Next steps

- [Add product variants](#add-product-variants)    
- [Edit a variant](#edit-a-variant)
- [Move a product](03_MoveProduct.md)
- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the products](01_ManageProducts.md)
- [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set)



## Add product variants

You can add a single or multiple variants to a product directly when you create the master product.

### Prerequisites

- At least one product is created, see [Create a product](01_ManageProducts.md#create-a-product).
- A variant set is created to the attribute set of the master product, see [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set).

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the master product you want to create one or more product variants to.   
  The *Edit Product* view is displayed. The tab *Attributes* is preselected.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesEdit.png "[Attributes]")

2. Click the tab *Variants* .   
  The tab *Variants* is displayed.

  ![Variants](/Assets/Screenshots/PIM/Products/List/Variants/VariantsEdit.png "[Variants]")

3. Click the drop-down list *Variant set* and select a variant set. All active variant sets to the corresponding attribute set of the product are displayed in the list.

  > [Info] If the selected master product has already one ore more product variants, the variant set is selected and read-only. It cannot be edited subsequently.

4. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the variants area.   
  The two buttons [Add single variant ![Add single variant](/Assets/Icons/Document.png "[Add single variant]") ] and [Add multiple variants ![Add multiple variants](/Assets/Icons/Documents.png "[Add multiple variants]") ] are displayed.

5. Follow one of the described sub-procedures:
  - To add a single variant to the product, see [Create a single variant](#create-a-single-variant).
  - To add multiple variants to the product, see [Create multiple variants](#create-multiple-variants).

### Next steps

- [Edit a variant](#edit-a-variant)
- [Move a product](03_MoveProduct.md)
- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create product variants](#create-product-variants)
- [Manage the products](01_ManageProducts.md)
- [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set)


## Edit a variant

After you have created a product variant, you can edit it. Note that only defining and differing attribute values are editable. All other attribute values are defined by the master product and can only be edited within the master product. Be careful when editing defining attribute values as you are also affecting the variant settings of the master product.

### Prerequisites

At least one product variant is created, see [Create product variants](#create-product-variants) or [Add product variants](#add-product-variants).

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Variants* at the top of the products list and select the option **List all products** .   
  All products including the product variants are displayed in the products list.

  ![All products](/Assets/Screenshots/PIM/Products/List/AllProducts.png "[All products]")

2. Click the product variant you want to edit.   
  The *Edit Product* view is displayed. The tab *Attributes* is preselected.

  ![Attributes](/Assets/Screenshots/PIM/Products/List/Attributes/AttributesVariant.png "[Attributes]")

3. Go to the attributes that are not defined by the master product and edit the desired data of the product variant.

  > [Info] Note that changes of the defining attributes are also applied to the variant settings of the master product. Especially when you are using a SKU with the defining attribute values as a placeholder, it is not recommended to modify a defining attribute value.

4. Click the button [SAVE] in the upper right corner.   
  The changes are saved. The *Edit Product* view is closed.

### Next steps

- [Move a product](03_MoveProduct.md)
- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create product variants](#create-product-variants)
- [Add product variants](#add-product-variants)
- [Create a single variant](#create-a-single-variant)
- [Create multiple variants](#create-multiple-variants)
- [Manage the products](01_ManageProducts.md)
