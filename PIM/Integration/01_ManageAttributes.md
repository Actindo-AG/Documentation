[!!PIM](Actindo/PIM)
[!!DataHub](Actindo/DataHub)

# Manage an attribute

An attribute defines a characteristic to describe a product. By default, the *PIM Basic Set* attribute set with the following attributes is predefined:
- Additional terms for search
- Customs Tariff Number
- Completeness
- Sale Unit
- Country of Origin
- Depth		
- Tags / Keywords
- Bundle		
- Product Variants
- Product Categories
- Price
- PIM Omni-Channel Connection
- Meta Title		
- Meta Keywords		
- Meta Description		
- Long Text
- Length
- Stock		
- Supplier Link		
- 18+
- EAN-Code		
- Digital Item
- Files
- Product relations
- Width		
- Images		
- Baseunit (Basic price)
- Expiration Date
- Product Name
- Weight		
- Product short description		
- Product Description
- Sale Item

You can create attributes, edit existing attributes and deactivate or delete attributes that are not in use. Further, you can add attributes to an attribute set or remove them from an attribute set.
In the *PIM* module, only PIM attributes are displayed.


## Create an attribute

Create an attribute to specify a new property for a product.

### Prerequisites

An attribute set is created, see [Create an attribute set](02_ManageAttributeSets.md#Create-an-attribute-set).

### Procedure
*PIM > Settings > Tab ATTRIBUTES*

![Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[Attributes]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create Attribute* view is displayed.

  ![Create attribute](/Assets/Screenshots/PIM/Settings/Attributes/CreateAttribute.png "[Create attribute]")

2. Enter a name for the attribute in the *Name* field and, if desired, add an attribute description in the  *Description* field.

3. Select a data type in the *Data type* drop-down list.   
 For detailed information about all data types, see [Data type list](/PIM/UserInterface/04_DataTypeList.md).

   > [Info] The settings displayed in the *CONFIGURATION* section depend on the selected data type.

4. Enter a key for the attribute in the *Key* field. The key is required for API access and must be system wide unique.

  > [Info] In order to facilitate the assignment of attributes in the further process (for instance in the ETL mapping), it is recommended to add the prefix **pim_** to all attributes created in the *PIM* module.     

5. If desired, activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi-language* toggle to assign values in multiple languages to the attribute or activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi-channel* toggle to assign different attribute values in different channels.

  > [Info] Be aware that only attributes which are neither multi-language nor multi-channel can be used as defining attributes for variants. For detailed information, see [Create a variant set](07_ManageVariantSets.md#create-a-variant-set).

6. Click the ![Add](/Assets/Icons/Plus05.png "[Add]") (Add) button in the *Assigned Sets* field. The button is locked if you have not yet selected a data type.   
  A drop-down list with all active attribute sets is displayed.

7. Select an attribute set in the *Assigned Sets* drop-down list.

  > [Info] You can assign the attribute to multiple sets. Repeat the steps **7** to **8** to assign the attribute to a further attribute set. To delete the assignment to a selected set, click the ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete) button right to the set.

8. If required, configure the settings in the *CONFIGURATION* section. For detailed information about the different configuration settings, see [Data type list](/PIM/UserInterface/04_DataTypeList.md).

9. Click the [SAVE] button in the upper right corner.   
  The new attribute is saved. The *Create Attribute* view is closed.  

### Next steps

- [Edit an attribute](#edit-an-attribute)
- [Deactivate an attribute](#deactivate-an-attribute)
- [Delete an attribute](#delete-an-attribute)
- [Recover an attribute](#recover-an-attribute)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the variant sets](07_ManageVariantSets.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)
- [Data type list](/PIM/UserInterface/04_DataTypeList.md)


## Edit an attribute

After you have created an attribute, you can edit it. However, only some attribute properties are editable. For instance, the data type and the attribute key cannot be subsequently modified. The assignment of an attribute to an attribute set must be changed in the [attribute set](ManageAttributeSet.md) itself.   
There are also some attributes that are automatically created by the system, for instance when installing a plugin or module. These system attributes are read-only and cannot be edited. It is highly recommended not to deactivate these attributes to avoid interfering with the functioning of the Core1 Platform.

### Prerequisites

At least one attribute is created, see [Create an attribute](#create-an-attribute).

### Procedure
*PIM > Settings > Tab ATTRIBUTES*

![Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[Attributes]")

1. Click the attribute you want to edit in the list of attributes.   
  The *Edit Attribute* view is displayed. The *Data* tab is preselected.

  ![Edit attribute data](/Assets/Screenshots/PIM/Settings/Attributes/EditAttribute_Data.png "[Edit attribute data]")

  > [Info] Be aware that you can only edit the attribute name, description, its status and configuration. All other fields and toggles are locked.

2. Edit the desired data of the attribute in the corresponding fields in the *Data* tab.

3. If desired, click the *Attribute Set Assignments* tab to check to which sets the selected attribute is assigned.

  ![Edit attribute assignments](/Assets/Screenshots/PIM/Settings/Attributes/EditAttribute_Assignments.png "[Edit attribute assignments]")

   > [Info] If you want to change the attribute set assignments of the selected attribute, you have to modify the corresponding attribute set.

4. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Edit Attribute* view is closed.  

### Next steps

- [Deactivate an attribute](#deactivate-an-attribute)
- [Delete an attribute](#delete-an-attribute)
- [Recover an attribute](#recover-an-attribute)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the variant sets](07_ManageVariantSets.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create an attribute](#create-an-attribute)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)



## Deactivate an attribute

It is recommended to deactivate an attribute instead of deleting it to prevent any problems because of existing dependencies. If you deactivate an attribute, it is no longer available for new attribute sets and it is hidden in existing products with this attribute.

### Prerequisites

At least one attribute is created, see [Create an attribute](#create-an-attribute).

### Procedure
*PIM > Settings > Tab ATTRIBUTES*

![Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[Attributes]")

1. Click the attribute you want to deactivate in the list of attributes.   
  The *Edit Attribute* view is displayed. The *Data* tab is preselected.

  ![Edit attribute data](/Assets/Screenshots/PIM/Settings/Attributes/EditAttribute_Data.png "[Edit attribute data]")

2. Deactivate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active* toggle in the *Data* tab.

   > [Info] If you want to reactivate an attribute, activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active* toggle.

3. Click the [SAVE] button in the upper right corner.   
  The attribute is deactivated. The *Edit Attribute* view is closed.

4. Press **F5** to initialize the Core1 Platform and to apply the changes.   

### Next steps

- [Delete an attribute](#delete-an-attribute)
- [Recover an attribute](#recover-an-attribute)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the variant sets](07_ManageVariantSets.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create an attribute](#create-an-attribute)
- [Edit an attribute](#edit-an-attribute)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)




## Delete an attribute

You can delete an attribute from the *PIM* module and move it to the *DELETED ATTRIBUTES* tab in the *DataHub* module if it is no longer needed. As there are usually dependencies on an attribute, for example through an attribute set or created products, it is strongly recommended not to delete an attribute. Instead, you can deactivate an attribute and thus prevent its use.

### Prerequisites

At least one attribute is created, see [Create an attribute](#create-an-attribute).

### Procedure
*PIM > Settings > Tab ATTRIBUTES*

![Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[Attributes]")

1. Select the checkbox of the attribute you want to delete in the list of attributes.   
  The editing toolbar is displayed above the attributes list.

2. Click the ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete) button in the toolbar. The *Confirm deletion of attribute?* window is displayed.

  > [Info] In the window all dependencies to attribute sets, ETL-mappings and entity entries are displayed. Be aware that problems may occur if you delete an attribute with existing dependencies.

3. Click the [CONFIRM] button in the bottom right corner.   
  The attribute is deleted and moved to the *DELETED ATTRIBUTES* tab in the *DataHub* module. The *Confirm deletion of attribute?* window is closed.

  > [Warning] Problems may occur if you delete an attribute with existing dependencies.  

> [Info] The attribute is deleted in the PIM product, but it can still be recovered. To irretrievably delete the attribute, see [Finally delete an attribute](#finally-delete-an-attribute).


### Next steps

- [Recover an attribute](#recover-an-attribute)
- [Manage the attribute sets](02_ManageAttributeSets.md)
- [Manage the attribute groups](03_ManageGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the channel settings](05_ConfigureChannels.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the variant sets](07_ManageVariantSets.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute](#create-an-attribute)
- [Edit an attribute](#edit-an-attribute)
- [Deactivate an attribute](#deactivate-an-attribute)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)


## Recover an attribute

If you delete an attribute in the *PIM* module, it is not irretrievably deleted. You can still recover the attribute and make the deletion undone.

The procedure to recover a deleted attribute is described in the *DataHub* module [Recover an attribute](/DataHub/Integration/01_ManageAttribute.md#recover-an-attribute)


## Finally delete an attribute

You can finally delete an attribute that has been deleted in the *PIM* module. As there are usually dependencies on an attribute, for example through an attribute set or created products, it is strongly recommended not to delete an attribute irretrievably. Finally deleted attributes cannot be recovered.

The procedure to recover a deleted attribute is described in the *DataHub* module [Finally delete an attribute](/DataHub/Integration/01_ManageAttributes.md#finally-delete-an-attribute)
