[!!User interface Product list](../UserInterface/02a_List.md)
[!!Manage the products](./01_ManageProducts.md)
[!!Manage a variant set](../Integration/07_ManageVariantSets.md)

# Manage a variant

A variant is a product with a special characteristic dependent on its master product. The defining attributes for the variants are predefined in their variant sets, see [Manage a variant set](../Integration/07_ManageVariantSets.md). You can create a variant directly when you create a master product, or you can add variants subsequently for an existing master product. Further, you can create a single variant or multiple variants to a master product.


## Create variants

You can create a single or multiple variants to a product directly when you create the master product. To add variants to an existing product, see [Add variants](#add-variants).

### Define the variants basic data

Define the basic inputs, such as name and description, for the variant.

#### Prerequisites

A variant set has been created to the attribute set of the product you want to assign the variants to, see [Create a variant set](../Integration/07_ManageVariantSets.md#create-a-variant-set).

#### Procedure

*PIM > Products > Tab LIST*

![Product list](../../Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create new product* window is displayed.

    ![Create new product](../../Assets/Screenshots/PIM/Products/List/CreateNewProduct.png "[Create new product]")

2. Select an attribute set in the *Attribute set* drop-down list. All active attribute sets are displayed in the drop-down list.

3. Enter a SKU for the product in the *SKU* field.

    > [Info] The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be unique within the *PIM* module.

4. Click the [CREATE] button.   
    The *Create product* view is displayed. The *Attributes* tab is preselected.

    ![Attributes](../../Assets/Screenshots/PIM/Products/List/Attributes/AttributesCreate.png "[Attributes]")

5. Enter the data for the product in the *Attributes* tab. It is recommended to complete at least the *Product name*, *Price* and *Tax class* fields.   

    > [Info] All fields marked with the note *(required)* are used for the completeness calculation of product attributes. When editing a product, you can enable the *Show empty required attributes only* toggle to display only the incomplete required attribute fields for the selected product.

6. Click the *Variants* tab.   
    The *Variants* tab is displayed.

    ![Variants](../../Assets/Screenshots/PIM/Products/List/Variants/VariantsCreate.png "[Variants]")

7. Click the *Variant set* drop-down list and select a variant set. All variant sets to the corresponding attribute set of the product are displayed in the list.   
    A single ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button is displayed in each variants  box.

8. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the variants box.   
    The [Add single variant ![Add single variant](../../Assets/Icons/Document.png "[Add single variant]") ] button and the [Add multiple variants ![Add multiple variants](../../Assets/Icons/Documents.png "[Add multiple variants]") ] button are displayed.

9. Follow one of the described procedures:
    - To create a single variant to the product, see [Create a single variant](#create-a-single-variant).
    - To create multiple variants to the product, see [Create multiple variants](#create-multiple-variants).


### Create a single variant

Create a single variant to a product.

#### Prerequisites

A variant set has been created to the attribute set of the product you want to assign the variants to, see [Create a variant set](../Integration/07_ManageVariantSets.md#create-a-variant-set).

#### Procedure

*PIM > Products > Tab LIST > Button Add > Tab Variants > Select variant set > Button Add*   
*PIM > Products > Tab LIST > Select Product > Tab Variants > Button Add*

![Add variants](../../Assets/Screenshots/PIM/Products/List/Variants/AddVariantCreate.png "[Add variants]")

1. Click the [Add single variant ![Add single variant](../../Assets/Icons/Document.png "[Add single variant]") ] button.   
    The *Add single variant* window is displayed.

    ![Add single variant](../../Assets/Screenshots/PIM/Products/List/Variants/AddSingleVariant.png "[Add single variant]")

2. If desired, disable the *Use formula* toggle and change the SKU in the *SKU* field. By default, the toggle is enabled and the predefined SKU is displayed.   

3. Select a value for the displayed attributes in the *Defined values* section. The fields differ depending on the selection of defining attributes for the variant set.  
    The selected attribute value is displayed in the box.

4. Click the [SAVE] button in the bottom right corner.   
    The new variant has been added to the product. The *Add single variant* window is closed. The variant is displayed in the variants list.

    ![Variant added](../../Assets/Screenshots/PIM/Products/List/Variants/VariantAddedCreate.png "[Variant added]")

5. Click the [SAVE] button in the upper right corner.   
    The variant has been saved. The product view is closed. The variant is displayed in the product list when you enable the **All products** option in the *Variants* drop-down list at the top of the product list.


### Create multiple variants

Create multiple variants at once for the same master product.

#### Prerequisites

A variant set has been created to the attribute set of the product you want to assign the variants to, see [Create a variant set](../Integration/07_ManageVariantSets.md#create-a-variant-set).

#### Procedure

*PIM > Products > Tab LIST > Button Add > Tab Variants > Select variant set > Button Add*   
*PIM > Products > Tab LIST > Select Product > Tab Variants > Button Add*

![Add variants](../../Assets/Screenshots/PIM/Products/List/Variants/AddVariantCreate.png "[Add variants]")

1. Click the [Add multiple variants ![Add multiple variants](../../Assets/Icons/Documents.png "[Add multiple variants]") ] button.   
    The *Select values* wizard window is displayed.

    ![Select values wizard](../../Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants01.png "[Select values wizard]")

2. Select a value for the displayed attributes in the box(es). The fields and the box(es) differ depending on the selection of defining attributes for the variant set.   
    The selected attribute value is displayed in the box(es).

3. Click the [ADD VALUE] button in the upper right corner of the box to add a further variant with another value.   
    A further row is displayed in the box.

    > [Info] If you want to add a variant for each existing value, click the [ADD ALL VALUES] button in the box. This button is only available for certain attributes.

4. Select a value for the attribute in the new row.
    The selected attribute value is displayed in the box.

    > [Info] Repeat the steps **3** and **4** to add further variants.

5. Click the [NEXT] button in the bottom right corner of the window.   
    The *Summary* wizard window is displayed.

    ![Summary wizard](../../Assets/Screenshots/PIM/Products/List/Variants/AddMultipleVariants02.png "[Summary wizard]")

6. Check if all variants listed in the *Variants that will be created (ignoring duplicated)* box are correct.

    > [Info] To remove a variant from the list, select the checkbox of the variant and click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button in the editing toolbar displayed above the list.

7. Click the [FINISH] button in the bottom right corner.   
    The new variants have been added to the product. The *Summary* wizard window is closed. The variants are displayed in the variants list.

    ![Variants added](../../Assets/Screenshots/PIM/Products/List/Variants/VariantsAddedCreate.png "[Variants added]")

8. Click the [SAVE] button in the upper right corner.   
    The variants have been saved. The product view is closed. The variants are displayed in the product list when you enable the **All products** option in the *Variants* drop-down list at the top of the product list.

    > [Info] For detailed information about the different views, see [Manage the view](./04_ManageView.md).



## Add variants

You can add a single or multiple variants to an existing product.

#### Prerequisites

- At least one product has been created, see [Create a product](./01_ManageProducts.md#create-a-product).
- A variant set has been created to the attribute set of the master product, see [Create a variant set](../Integration/07_ManageVariantSets.md#create-a-variant-set).

#### Procedure

*PIM > Products > Tab LIST*

![Product list](../../Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the product you want to create one or more variants to.   
    The *Edit product* view is displayed. The *Attributes* tab is preselected.

    ![Attributes](../../Assets/Screenshots/PIM/Products/List/Attributes/AttributesEdit.png "[Attributes]")

2. Click the *Variants* tab.   
    The *Variants* tab is displayed.

    ![Variants](../../Assets/Screenshots/PIM/Products/List/Variants/VariantsEdit.png "[Variants]")

3. Click the *Variant set* drop-down list and select a variant set. All active variant sets to the corresponding attribute set of the product are displayed in the list.

    > [Info] If the selected master product has already one ore more variants, the variant set is selected and read-only. It cannot be edited subsequently.

4. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the variants box.   
    The [Add single variant ![Add single variant](../../Assets/Icons/Document.png "[Add single variant]") ] button and the [Add multiple variants ![Add multiple variants](../../Assets/Icons/Documents.png "[Add multiple variants]") ] button are displayed.

5. Follow one of the described procedures:
    - To add a single variant to the product, see [Create a single variant](#create-a-single-variant).
    - To add multiple variants to the product, see [Create multiple variants](#create-multiple-variants).



## Edit a variant

After you have created a variant, you can edit it. Note that only defining and changeable attribute values are editable. All other attribute values are defined by the master product and can only be edited within the master product. Be careful when editing defining attribute values as you are also affecting the variant settings of the master product.

#### Prerequisites

At least one variant has been created, see [Create variants](#create-variants) or [Add variants](#add-variants).

#### Procedure

*PIM > Products > Tab LIST*

![Product list](../../Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the *Variants* drop-down list at the top of the product list and select the **All products** option.   
    All products including the variants are displayed in the product list.

    ![All products](../../Assets/Screenshots/PIM/Products/List/AllProducts.png "[All products]")

2. Click the variant you want to edit.   
    The *Edit product* view is displayed. The *Attributes* tab is preselected.

    ![Attributes](../../Assets/Screenshots/PIM/Products/List/Attributes/AttributesVariant.png "[Attributes]")

3. Go to the attributes that are not defined by the master product and edit the desired data of the variant.

    > [Info] Note that changes of the defining attributes are also applied to the variant settings of the master product. Especially if you are using a SKU with the defining attribute values as a placeholder, it is not recommended to modify a defining attribute value.

4. Click the [SAVE] button in the upper right corner.   
    The changes have been saved. The *Edit product* view is closed.
