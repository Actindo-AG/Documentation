[!!DataHub](DataHub)

# Manage an attribute set

An attribute set consists of a group of attributes to classify certain products according to demand or production contexts. By default, the *PIM Basic Set* attribute set is predefined.

[comment]: <> (Are there any other sets outside PIM predefined?)

You can create attribute sets, edit existing attribute sets and deactivate attribute sets that are not in use. You can add attributes to or remove attributes from an attribute set and change the required attributes within an attribute set.
Further, you can import or export attribute sets.


## Create an attribute set

Create an attribute set to define a new product type with different attributes to the predefined attribute sets.
In contrast to attribute sets created in the *PIM* module, you have to select an entity type for the attribute set.

[comment]: <> (What does that mean -> what consequences has the entity type? All pim attribute sets = entity type  PIM product?)

### Prerequisites

The attributes for the attribute set are created, see [Create an attribute](01_ManageAttributs.md#create-an-attribute).

### Procedure
*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attribute sets](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attribute sets]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create Attribute Set* view is displayed.

  ![Create attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/CreateAttributeSet.png "[Create attribute set]")

2. Enter a name for the attribute set in the *Name* field and, if desired, add an attribute set description in the *Description* field.

3. Enter a key for the attribute set in the *Key* field. The key is required for API access and must be system wide unique.

  > [Info] In order to facilitate the assignment of sets in the further process, it is recommended to add the prefix **datahubset_** to all attribute sets created in the *DataHub* module.

4. Click the *Entity Type* drop-down list and select the appropriate entity type. The list of options may differ depending on the system configuration.

[comment]: <> (More information about the entity type!)

5. For the next steps to create an attribute set, follow the appropriate sub-procedure:   
    - [Create an attribute set without attribute inheritance](#create-an-attribute-set-without-attribute-inheritance)
    - [Create an attribute set with attribute inheritance](#create-an-attribute-set-with-attribute-inheritance)
    - [Create an attribute set with attribute copying](#create-an-attribute-set-with-attribute-copying)


#### Create an attribute set without attribute inheritance

> [Info]  When you create an attribute set without inheritance, you have to add all attributes manually to the created attribute set. Neither attributes nor configurations are applied from another attribute set. In exchange, you can define individually which attributes are required and customize their configuration.

1. Select the **no inheritance** option in the *Inherit/Copy Values from* drop-down list.   
  The ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration* toggle and the *Inherit/Copy Values* drop-down list are locked.

2. Click the [SAVE] button.   
  The new attribute set is saved. The *Edit Attribute Set* view is displayed.  

3. Click the ![Back](/Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).


#### Create an attribute set with attribute inheritance

> [Info] When you create an attribute set with attribute inheritance, you adopt all attributes from the selected attribute set. The inherited attributes cannot be changed. Further, all changes in the inheritance attribute set are also applied to the linked attribute set. Each time a change is made in the inheritance attribute set, the linked attribute sets are updated.  

1. Select an attribute set in the *Inherit/Copy Values from* drop-down list.

2. Activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration* toggle if you also want to adopt the configuration to the new attribute set.

3. Select the **Inherit** option in the *Inherit/Copy Values* drop-down list.

4. Click the [SAVE] button.   
  The new attribute set is saved. The *Edit Attribute Set* view is displayed.  

5. Click the ![Back](/Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).


#### Create an attribute set with attribute copying

> [Info] When you create an attribute set with attribute copying, you copy all attributes from the selected attribute set once. After copying, the attribute set behaves like an attribute set without attribute inheritance. Further changes in the copied attribute set or not affecting the created attribute set.   

1. Select an attribute set in the *Inherit/Copy Values from* drop-down list.

2. Activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration* toggle if you also want to adopt the configuration to the new attribute set.

3. Select the **Copy once** option in the *Inherit/Copy Values* drop-down list.

4. Click the [SAVE] button.   
  The new attribute set is saved. The *Edit Attribute Set* view is displayed.  

5. Click the ![Back](/Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).


### Next steps

- [Edit an attribute set](#edit-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Import an attribute set](#import-an-attribute-set)
- [Export an attribute set](#export-an-attribute-set)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage the attributes](01_ManageAttributes.md)



## Edit an attribute set

After you have created an attribute set, you can edit it. Depending on the selected inheritance type, only a certain number of attributes may be editable. However, you can add further attributes to an attribute set or remove unmapped attributes from an attribute set.

### Add an attribute to the set

Add a new attribute to an attribute set to define any further specifications.

#### Prerequisites

- An attribute set is created, see [Create an attribute set](#create-an-attribute-set).
- At least one additional attribute is created, see [Create an attribute](01_ManageAttributes.md#create-an-attribute).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to edit in the list of attribute sets.   
  The *Edit Attribute Set* view is displayed.

  ![Edit attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the *Assigned Attributes* section.   
  The *Add attributes* view is displayed. All active attributes that are not yet included in the selected attribute set are displayed in the list.

  ![Add attribute](/Assets/Screenshots/DataHub/Settings/AttributeSets/AddAttributes.png "[Edit attribute set]")

  > [Info] If the message **There are no unassigned attributes.** is displayed in the *Add attributes* view, all active attributes are already included in the selected attribute set. Check if you have selected the appropriate attribute set, click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list or [create a new attribute](01_ManageAttributes.md#create-an-attribute).

3. Select the checkboxes of the attributes in the list, you want to add to the attribute set.   
  The editing toolbar is displayed above the list.

4. Click the [ADD] button in the editing toolbar.   
  The selected attributes are added to the attribute set. The *Add attributes* view is closed. The *Edit Attribute Set* view is displayed again. The added attributes are displayed in the *Assigned Attributes* section.

5. Click the [SAVE] button.   
  The changes are saved. The *Edit Attribute Set* view is closed.

#### Next steps

- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Import an attribute set](#import-an-attribute-set)
- [Export an attribute set](#export-an-attribute-set)
- [Manage the attribute groups](03_ManageAttributeGroups.md)


#### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute set](#create-an-attribute-set)
- [Manage the attributes](01_ManageAttributes.md)



### Remove an attribute from the set

Remove an attribute from an attribute set to limit the specifications. Inherited attributes or mapped attributes cannot be removed from an attributes set.

#### Prerequisites

- An attribute set is created, see [Create an attribute set](#create-an-attribute-set).
- At least one attribute is added to the attribute set, see [Add an attribute to the set](#add-an-attribute-to-the-set).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to edit in the list of attribute sets.   
  The *Edit Attribute Set* view is displayed.

  ![Edit attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. In the *Assigned Attributes* section, select the checkboxes of the attributes, you want to remove from the attribute set.   
  The editing toolbar is displayed above the list.

3. Click the ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete) button in the editing toolbar.   
  The selected attributes are removed from the attribute set. The list of attributes is updated.

  > [Info] If the selected attributes cannot be removed from the attribute set, an error message is displayed in the upper right corner.

4. Click the [SAVE] button.   
  The changes are saved. The *Edit Attribute Set* view is closed.

#### Next steps

- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Import an attribute set](#import-an-attribute-set)
- [Export an attribute set](#export-an-attribute-set)
- [Manage the attribute groups](03_ManageAttributeGroups.md)
- [Configure the language settings](04_ConfigureLanguages.md)
- [Configure the scope settings](05_ConfigureScopes.md)
- [Manage the catalogs](06_ManageCatalogs.md)
- [Manage the variant sets](07_ManageVariantSets.md)

#### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute set](#create-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Manage the attributes](01_ManageAttributes.md)
- [Manage the products](/PIM/Operation/01_ManageProducts.md)



### Change the required attributes in the set

The product completeness is calculated depending on the required attributes within an attribute set. You can define whether an attribute should be required or not. Note that inherited attributes can only be changed in the origin attribute set and the required status is also inherited to the linked attribute sets. All required attributes are marked with a *(required)* indication in the product view.     
Be aware that the activation or deactivation of languages affects the completeness calculation.

#### Prerequisites

An attribute set is created, see [Create an attribute set](#create-an-attribute-set).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to edit in the list of attribute sets.   
  The *Edit Attribtue Set* view is displayed.

  ![Edit attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. Click the ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) button in the *Assigned Attributes* section.   
  The *required* column in the list of attributes is unlocked. The color of the ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) button switches to blue.

  ![Required](/Assets/Screenshots/DataHub/Settings/AttributeSets/Required.png "[Required]")

3. Activate or deactivate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *required* toggle in the *required* column to define whether or not an attribute value should be required in the selected attribute set.

  > [Info] Be aware that you can only edit the *required* option for attributes that are not inherited.

4. Click the ![Settings](/Assets/Icons/Settings02.png "[Settings]") (Settings) button in the *Assigned Attributes* section.       
  The *required* column in the list of attributes is locked. All changes in the attribute list are saved.

5. Click the ![Back](/Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).

#### Next steps

- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Import an attribute set](#import-an-attribute-set)
- [Export an attribute set](#export-an-attribute-set)
- [Manage the attribute groups](03_ManageAttributeGroups.md)

#### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute set](#create-an-attribute-set)
- [Edit an attribute set](#edit-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Manage the attributes](01_ManageAttributes.md)



## Deactivate an attribute set

If an attribute set is no longer used, it is recommended to deactivate the attribute set to prevent any problems because of existing dependencies. If you deactivate an attribute set, it is no longer available when creating attributes or products.

### Prerequisites

At least one attribute set is created, see [Create an attribute set](#create-an-attribute-set).

### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to deactivate in the list of attribute sets.   
  The *Edit Attribute Set* view is displayed.

  ![Edit attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. Deactivate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active* toggle.

     > [Info] If you want to reactivate an attribute set, activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active* toggle.

3. Click the [SAVE] button.   
  The attribute set is deactivated. The *Edit Attribute Set* view is closed.

4. Press **F5** to initialize the Core1 Platform and to apply the changes.


### Next steps

- [Import an attribute set](#import-an-attribute-set)
- [Export an attribute set](#export-an-attribute-set)
- [Manage the attribute groups](03_ManageAttributeGroups.md)


### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute set](#create-an-attribute-set)
- [Edit an attribute set](#edit-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Manage the attributes](01_ManageAttributes.md)



--------
[comment]: <> (Import/Export will be changed)

## Import an attribute set

### Prerequisites
No prerequisites to fulfill.

### Procedure
*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the [IMPORT] button in the upper left corner.   
  The *Upload file* window of the import wizard is displayed.

  ![Upload file](/Assets/Screenshots/DataHub/Settings/AttributeSets/Import01.png "[Upload file]")

2. Drag the import file from your local folder and drop it in the dashed box ![Upload](/Assets/Icons/Upload.png "[Upload]") *Drop file here...*. Alternatively, click the [SELECT FILE] button and select a file from your local folder in the displayed Explorer window.   
  The selected file is displayed in the dashed box.

  > [Info] What file types are supported? What requirements?

3. Activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Move existing attributes into attribute groups specified in the file* toggle if you want to ???

[comment]: <> (---> what is this setting doing?)

4. Click the [CONTINUE] button in the bottom right corner. The button is unlocked if an appropriate file is uploaded.   
  The *Summary* window of the import wizard is displayed.

  ![Summary](/Assets/Screenshots/DataHub/Settings/AttributeSets/Import02.png "[Summary]")

5. Click the [FINALIZE] button in the bottom right corner.
  The import is completed.

### Next steps

- [Export an attribute set](#export-an-attribute-set)
- [Manage the attribute groups](03_ManageAttributeGroups.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute set](#create-an-attribute-set)
- [Edit an attribute set](#edit-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Manage the attributes](01_ManageAttributes.md)



## Export an attribute set

### Prerequisites
At least one attribute set is created, see [Create an attribute set](#create-an-attribute-set).

### Procedure
*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Select the checkboxes of the attribute sets you want to export.   
  The editing toolbar is displayed above the attribute sets list.

2. Click the [EXPORT] button in the toolbar.  
  The *Step 1* window of the export wizard is displayed.

  ![Export Step 1](/Assets/Screenshots/DataHub/Settings/AttributeSets/Export01.png "[Export Step 1]")

3. Select the checkboxes of the attributes you want to exclude from the export.   

4. Click the [CONTINUE] button in the bottom right corner.  
  The *Step 2* window of the export wizard is displayed.

  ![Export Step 2](/Assets/Screenshots/DataHub/Settings/AttributeSets/Export02.png "[Export Step 2]")

  > [Info] If the attributes selected for export are not assigned to an attribute set, the *Step 2* window of the export wizard is skipped and the *Step 3* window is immediately displayed.

5. Select the checkboxes of the variant sets you want to exclude from the export.   

6. Click the [CONTINUE] button in the bottom right corner.  
  The *Step 3* window of the export wizard is displayed.

  ![Export Step 3](/Assets/Screenshots/DataHub/Settings/AttributeSets/Export03.png "[Export Step 3]")

7. Click the [EXPORT] button in the bottom right corner.
  The export is started. By default, the export file is saved in the local download folder.

### Next steps

- [Manage the attribute groups](03_ManageAttributeGroups.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an attribute set](#create-an-attribute-set)
- [Edit an attribute set](#edit-an-attribute-set)
- [Add an attribute to the set](#add-an-attribute-to-the-set)
- [Remove an attribute from the set](#remove-an-attribute-from-the-set)
- [Change the required attributes in the set](#change-the-required-attributes-in-the-set)
- [Deactivate an attribute set](#deactivate-an-attribute-set)
- [Import an attribute set](#import-an-attribute-set)
- [Manage the attributes](01_ManageAttributes.md)
