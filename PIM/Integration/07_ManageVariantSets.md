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

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create variant set* view is displayed.

  ![Create variant set](/Assets/Screenshots/PIM/Settings/VariantSets/CreateVariantSet.png "[Create variant set]")

2. Enter a name for the variant set in the *Name* field.

3. Select an attribute set in the *Attribute Set* drop-down list. All active attribute sets are displayed in the list.   

  > [Info] You need to specify defining and differing attributes for the variant set at a later step. Be aware that only those attributes assigned to the selected attribute set will be available.

  The *Formulas* section with the *Formula for SKU* field is displayed.

  ![Formulas](/Assets/Screenshots/PIM/Settings/VariantSets/Formulas.png "[Formulas]")

4. Enter a formula for the variants SKU in the *Formula for SKU* field using the displayed placeholders. By default, you can enter the formula **{master}-{L}**.   

  > [Info] The value of the defining attributes can be included into the SKU formula. When you have added a defining attribute, the corresponding placeholder for this attribute is displayed in the *Formulas* section.

5. For the next steps to create a variant set, follow the sub-procedures below:   
      - [Add defining attributes](#add-defining-attributes)
      - [Add differing attributes](#add-differing-attributes)


#### Add defining attributes

> [Info] You have to select at least one defining attribute to create a variant set. You can only select attributes as defining attributes, that are neither multilingual nor multi-channel and assigned to the selected attribute set.

1. In the *Defining attributes* box click the ![Add](/Assets/Icons/Plus01.png "[Add]") button. This button is only displayed when an attribute set is selected.       
  The *Add defining attributes* view is displayed.

  ![Add defining attributes](/Assets/Screenshots/PIM/Settings/VariantSets/AddDefiningAttributes.png "[Add defining attributes]")

2. Select the checkboxes of the attributes you want to be a defining attribute for the selected variant.   
  The editing toolbar is displayed above the attribute list.

  > [Info] The defining attributes are those attributes that characterize the variant, so those attributes that are defining the variants of the master product.

3. Click the [ADD AND GO BACK] button.     
    The *Add defining attributes* view is closed. The selected attributes are displayed in the *Defining attributes* box. A placeholder for the added attribute is displayed in the *Formulas* section.   

    ![Defining attributes added](/Assets/Screenshots/PIM/Settings/VariantSets/DefiningAttributesAdded.png "[Defining attributes added]")

    > [Info] You can edit the formula in the *Formula for SKU* field and include the defining attribute placeholder.

4. If desired, add differing attributes to the variant set, see [Add differing attributes](#add-differing-attributes) .   
Otherwise, click the [SAVE] button in the upper right corner.   
  The *Create variant set* view is closed. The new variant set is saved and displayed in the list of variant sets.


#### Add differing attributes

> [Info] You can select differing attributes for a variant set. If you want to define an attribute for the variants which value may differ from its master product value, you have to define this attribute as a differing attribute.

1. In the *Differing Attributes* box click the ![Add](/Assets/Icons/Plus01.png "[Add]") button. This button is only displayed when an attribute set is selected.         
  The *Add differing attributes* view is displayed.

  ![Add differing attributes](/Assets/Screenshots/PIM/Settings/VariantSets/AddDifferingAttributes.png "[Add differing attributes]")

2. Select the checkboxes of the attributes you want to be a differing attribute for the selected variant.   
  The editing toolbar is displayed above the attribute list.

  > [Info] Generally, a variant inherits all attribute values from its master product. These attribute values are locked in the variant and can only be edited in the master product. Attribute values that differ from the master product and must be maintained individually in the variant itself must be added to the list of differing attributes.

3. Click the [ADD AND GO BACK] button.   
  The *Add differing attributes* view is closed. The selected attributes are displayed in the *Differing Attributes* box.

  ![Differing attributes added](/Assets/Screenshots/PIM/Settings/VariantSets/DifferingAttributesAdded.png "[Differing attributes added]")

4. Click the [SAVE] button in the upper right corner.   
  The *Create variant set* view is closed. The new variant set is saved and displayed in the list of variant sets.

### Next steps

- [Edit a variant set](#edit-a-variant-set)
- [Remove an attribute from the variant set](#remove-an-attribute-from-the-variant-set)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the attributes](01_ManageAttributes.md)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)



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

3. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Edit variant set* view is closed.

[comment]: <> (I have to refresh the list to apply the changes - is that a bug?)

### Next steps

- [Remove an attribute from the variant set](#remove-an-attribute-from-the-variant-set)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a variant set](#create-a-variant-set)
- [Manage the attributes](01_ManageAttributes.md)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)



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

2. In the *Defining attributes* box or *Differing attributes* box, select the checkboxes of the attributes you want to remove.     
  The [DELETE] button is displayed in the editing toolbar above the attribute list.

3. Click the [DELETE] button in the toolbar.   
  The attribute is removed from the list.

4. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Edit variant set* view is closed.

  [comment]: <> (I have to refresh the list to apply the changes - is that a bug?)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a variant set](#create-a-variant-set)
- [Edit a variant set](#edit-a-variant-set)
- [Manage the attributes](01_ManageAttributes.md)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)
