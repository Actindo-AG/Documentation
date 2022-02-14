[!!PIM](Actindo/PIM)

# Manage a variant set

You can create a variant set for a product. A variant is a special characteristics of a product, for instance the size or the color.

## Create a variant set

Create a variant set to be able to create variants to products. A variant set is always assigned to a certain attribute set. When a variant set is created to an attribute set, you can create variants to all products with this attribute set. You must assign at least one defining attribute to a variant set. Further, you can assign more defining as well as differing attributes.   

### Prerequisites

An attribute set is created, see [Create an attribute set](ManageAttributeSet.md#create-an-attribute-set).

### Procedure
*PIM > Settings > Tab VARIANT SETS*

![Variant sets](/Assets/Screenshots/PIM/Settings/VariantSets/VariantSets.png "[Variant sets]")

1. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  The *Create variant set* view is displayed.

  ![Create variant set](/Assets/Screenshots/PIM/Settings/VariantSets/CreateVariantSet.png "[Create variant set]")

2. Enter a name for the variant set in the field *Name*.

3. Select an attribute set in the drop-down list *Attribute Set*. All active attribute sets are displayed in the list.   

  > [Info] You need to specify defining and differing attributes for the variant set at a later step. Be aware that only those attributes assigned to the selected attribute set will be available.

  The section *Formulas* with the field *Formula for sku* is displayed.

  ![Formulas](/Assets/Screenshots/PIM/Settings/VariantSets/Formulas.png "[Formulas]")

4. Enter a formula for the product variants SKU in the field *Formula for sku* using the displayed placeholders. By default, you can enter the formula **{master}-{L}**.   

  > [Info] The value of the defining attributes can be included into the SKU formula. When you have added a defining attribute, the corresponding placeholder for this attribute is displayed in the section *Formulas*.

5. For the next steps to create a variant set, follow the sub-procedures below:   
      - [Add defining attributes](#add-defining-attributes)
      - [Add differing attributes](#add-differing-attributes)


#### Add defining attributes

> [Info] You have to select at least one defining attribute to create a variant set. You can only select attributes as defining attributes, that are neither multilingual nor multi-scope and assigned to the selected attribute set.

1. In the area *Defining attributes* click the button ![Add](/Assets/Icons/Plus01.png "[Add]"). This button is only displayed when an attribute set is selected.       
  The *Add defining attributes* view is displayed.

  ![Add defining attributes](/Assets/Screenshots/PIM/Settings/VariantSets/AddDefiningAttributes.png "[Add defining attributes]")

2. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes you want to be a defining attribute for the selected variant.   
  The editing toolbar is displayed above the attribute list.

  > [Info] The defining attributes are those attributes that characterize the variant article, so those attributes that are defining the variants of the master article.

3. Click the button [ADD AND GO BACK].     
    The *Add defining attributes* view is closed. The selected attributes are displayed in the area *Defining attributes*. A placeholder for the added attribute is displayed in the section *Formulas*.   

    ![Defining attributes added](/Assets/Screenshots/PIM/Settings/VariantSets/DefiningAttributesAdded.png "[Defining attributes added]")

    > [Info] You can edit the formula in the field *Formula for sku* and include the defining attribute placeholder.

4. If desired, add differing attributes to the variant set, see [Add differing attributes](#add-differing-attributes) .   
Otherwise, click the button [SAVE] in the upper right corner.   
  The *Create variant set* view is closed. The new variant set is saved and displayed in the list of variant sets.


#### Add differing attributes

> [Info] You can select differing attributes for a variant set. If you want to define an attribute for the variants which value may differ from its master product value, you have to define this attribute as a differing attribute.

1. In the area *Differing Attributes* click the button ![Add](/Assets/Icons/Plus01.png "[Add]"). This button is only displayed when an attribute set is selected.         
  The *Add differing attributes* view is displayed.

  ![Add differing attributes](/Assets/Screenshots/PIM/Settings/VariantSets/AddDifferingAttributes.png "[Add differing attributes]")

2. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes you want to be a differing attribute for the selected variant.   
  The editing toolbar is displayed above the attribute list.

  > [Info] Generally, a variant article inherits all attribute values from its master article. These attribute values are locked in the variant article and can only be edited in the master article. Attribute values that differ from the master article and must be maintained individually in the variant article itself must be added to the list of differing attributes.

3. Click the button [ADD AND GO BACK].   
  The *Add differing attributes* view is closed. The selected attributes are displayed in the area *Differing Attributes*.

  ![Differing attributes added](/Assets/Screenshots/PIM/Settings/VariantSets/DifferingAttributesAdded.png "[Differing attributes added]")

4. Click the button [SAVE] in the upper right corner.   
  The *Create variant set* view is closed. The new variant set is saved and displayed in the list of variant sets.

### Next steps

- [Edit a variant set](#edit-a-variant-set)
- [Remove an attribute from the variant set](#remove-an-attribute-from-the-variant-set)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage an attribute](ManageAttribute.md)
- [Manage an attribute set](ManageAttributeSet.md)
- [Manage an attribute group](ManageGroups.md)
- [Configure the language settings](ConfigureLanguages.md)
- [Configure the scope settings](ConfigureScopes.md)
- [Manage a catalog](ManageCatalog.md)
- [Manage a product](/PIM/Operation/ManageProduct.md)



## Edit a variant set

After you have created a variant set, you can edit it. However, only some fields are editable. The assigned attribute set cannot be subsequently modified.

### Prerequisites

At least one variant set is created, see [Create a variant set](#create-a-variant-set).

### Procedure
*PIM > Settings > Tab VARIANT SETS*

![Variant sets](/Assets/Screenshots/PIM/Settings/VariantSets/VariantSets.png "[Variant sets]")

1. Click the variant set you want to edit in the list of variant sets.   
  The *Edit variant set* view is displayed.

  ![Edit variant set](/Assets/Screenshots/PIM/Settings/VariantSets/EditVariantSet.png "[Edit variant set]")

2. Edit the desired data of the variant set in the corresponding fields.

3. Click the button [SAVE] in the upper right corner.   
  The changes are saved. The *Edit variant set* view is closed.

[comment]: <> (I have to refresh the list to apply the changes - is that a bug?)

### Next steps

- [Remove an attribute from the variant set](#remove-an-attribute-from-the-variant-set)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a variant set](#create-a-variant-set)
- [Manage an attribute](ManageAttribute.md)
- [Manage an attribute set](ManageAttributeSet.md)
- [Manage an attribute group](ManageGroups.md)
- [Configure the language settings](ConfigureLanguages.md)
- [Configure the scope settings](ConfigureScopes.md)
- [Manage a catalog](ManageCatalog.md)
- [Manage a product](/PIM/Operation/ManageProduct.md)



## Remove an attribute from the variant set

You can remove defining and differing attributes from the variant set. Note, that at least one defining attribute is assigned. If one or more differing attributes has been assigned to the variant set, also at least one differing attribute must be assigned.

[comment]: <> (is that a bug?)

### Prerequisites

A variant set is created, see [Create a variant set](#create-a-variant-set).

### Procedure
*PIM > Settings > Tab VARIANT SETS*

![Variant sets](/Assets/Screenshots/PIM/Settings/VariantSets/VariantSets.png "[Variant sets]")

1. Click the variant set you want to edit in the list of variant sets.   
  The *Edit variant set* view is displayed.

  ![Edit variant set](/Assets/Screenshots/PIM/Settings/VariantSets/EditVariantSet.png "[Edit variant set]")

2. In the area *Defining attributes* or *Differing attributes*, select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes you want to remove.     
  The button [DELETE] is displayed in the editing toolbar above the attribute list.

3. Click the button [DELETE] in the toolbar.   
  The attribute is removed from the list.

4. Click the button [SAVE] in the upper right corner.   
  The changes are saved. The *Edit variant set* view is closed.

  [comment]: <> (I have to refresh the list to apply the changes - is that a bug?)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a variant set](#create-a-variant-set)
- [Edit a variant set](#edit-a-variant-set)
- [Manage an attribute](ManageAttribute.md)
- [Manage an attribute set](ManageAttributeSet.md)
- [Manage an attribute group](ManageGroups.md)
- [Configure the language settings](ConfigureLanguages.md)
- [Configure the scope settings](ConfigureScopes.md)
- [Manage a catalog](ManageCatalog.md)
- [Manage a product](/PIM/Operation/ManageProduct.md)
