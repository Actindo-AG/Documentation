[!!Manage the attributes](./01_ManageAttributes.md)
[!!User interface Attribute sets](../UserInterface/02b_AttributeSets.md)

# Manage an attribute set

An attribute set consists of multiple attributes to classify certain products according to demand or production contexts.
Several plugins may bring their own attribute sets as a starting point for the tenant's configuration, such as the *PIM* module.

You can create attribute sets, edit existing attribute sets and deactivate attribute sets that are not in use.
You can add attributes to or remove attributes from an attribute set and change the required attributes within an attribute set.


## Create an attribute set

Create an attribute set to define a new attribute set with different attributes to the predefined attribute sets.

Several plugins have their own configuration user interface, where only those attributes and attribute sets are listed that belong to the specific plugin.
When using the plugin-specific user interface, several options may be restricted or not available.


### Define the attribute set basic data

Define the basic inputs, such as name and description, for the attribute set.

#### Prerequisites

Additional attributes for the attribute set have been created, see [Create an attribute](./01_ManageAttributes.md#create-an-attribute).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attribute sets](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attribute sets]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create attribute set* view is displayed.

    ![Create attribute set](../../Assets/Screenshots/DataHub/Settings/AttributeSets/CreateAttributeSet.png "[Create attribute set]")

2. Enter a name for the attribute set in the *Name* field and, if desired, add an attribute set description in the *Description* field.

3. Enter a key for the attribute set in the *Key* field. The key is required for API access and must be system wide unique. An attribute set key must fulfill the following criteria:
    - valid characters are **a-z** (upper and lower case), **0-9** and the underscore ( **_** )
    - the key must not start with a number
    - a double underscore ( **___** ) and a trailing underscore are forbidden

    > [Info] In order to facilitate the assignment of sets in the further process, it is recommended to add the prefix **datahubset_** to all attribute sets created in the *DataHub* module.

4. Click the *Entity type* drop-down list and select the appropriate entity type. The list of options may differ depending on the system configuration.

    > Entity types are all classes interacting with the *DataHub* module.

5. For the next steps to create an attribute set, follow the appropriate procedure:   
    - [Create an attribute set without attribute inheritance](#create-an-attribute-set-without-attribute-inheritance)
    - [Create an attribute set with attribute inheritance](#create-an-attribute-set-with-attribute-inheritance)
    - [Create an attribute set with attribute copying](#create-an-attribute-set-with-attribute-copying)


### Create an attribute set without attribute inheritance

When you create an attribute set without inheritance, you have to add all attributes manually to the created attribute set.
Neither attributes nor configurations are applied from another attribute set.
In exchange, you can define individually which attributes are required and customize their configuration.

#### Prerequisites

The basic data of the attribute set has been completed, see [Define the attribute set basic data](#define-the-attribute-set-basic-data).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS > Button Add*

![Create attribute set inheritance](../../Assets/Screenshots/DataHub/Settings/AttributeSets/CreateAttributeSetInheritance.png "[Create attribute set inheritance]")

1. Select the **No inheritance** option in the *Inherit/Copy values from* drop-down list.   
    The *Inherit configuration* toggle and the *Inherit/Copy values* drop-down list are locked.

2. Click the [SAVE] button.   
    The new attribute set has been saved. The *Create attribute set* view changes to the *Edit attribute set* view. The *Attribute set created* pop-up window is displayed.   

    ![Attribute set created](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSetCreated.png "[Attribute set created]")   

3. Click the ![Back](../../Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).


### Create an attribute set with attribute inheritance

When you create an attribute set with attribute inheritance, you adopt all attributes from the selected attribute set.
The inherited attributes cannot be changed.
Further, all changes in the inheritance attribute set are also applied to the linked attribute set.
Each time a change is made in the inheritance attribute set, the linked attribute sets are updated.  

#### Prerequisites

The basic data of the attribute set has been completed, see [Define the attribute set basic data](#define-the-attribute-set-basic-data).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS > Button Add*

![Create attribute set inheritance](../../Assets/Screenshots/DataHub/Settings/AttributeSets/CreateAttributeSetInheritance.png "[Create attribute set inheritance]")

1. Select an attribute set in the *Inherit/Copy values from* drop-down list.

2. Enable the *Inherit configuration* toggle if you also want to adopt the configuration to the new attribute set.

3. Select the **Inherit** option in the *Inherit/Copy values* drop-down list.

4. Click the [SAVE] button.   
    The new attribute set has been saved. The *Create attribute set* view changes to the *Edit attribute set* view. The *Attribute set created* pop-up window is displayed.   

    ![Attribute set created](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSetCreated.png "[Attribute set created]")     

5. Click the ![Back](../../Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).


### Create an attribute set with attribute copying

When you create an attribute set with attribute copying, you copy all attributes from the selected attribute set once.
After copying, the attribute set behaves like an attribute set without attribute inheritance.
Further changes in the copied attribute set or not affecting the created attribute set.   

#### Prerequisites

The basic data of the attribute set has been completed, see [Define the attribute set basic data](#define-the-attribute-set-basic-data).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS > Button Add*

![Create attribute set inheritance](../../Assets/Screenshots/DataHub/Settings/AttributeSets/CreateAttributeSetInheritance.png "[Create attribute set inheritance]")

1. Select an attribute set in the *Inherit/Copy values from* drop-down list.

2. Enable the *Inherit configuration* toggle if you also want to adopt the configuration to the new attribute set.

3. Select the **Copy once** option in the *Inherit/Copy values* drop-down list.

4. Click the [SAVE] button.   
    The new attribute set has been saved. The *Create attribute set* view changes to the *Edit attribute set* view. The *Attribute set created* pop-up window is displayed.   

    ![Attribute set created](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSetCreated.png "[Attribute set created]")     

5. Click the ![Back](../../Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).



## Edit an attribute set

After you have created an attribute set, you can edit it.
Depending on the selected inheritance type, only a certain number of attributes may be editable.
However, you can add further attributes to an attribute set or remove unmapped attributes from an attribute set.


### Add an attribute to the set

Add a new attribute to an attribute set to define any further specifications.
In the *DataHub* module all available attributes can be added to the different attribute sets.

#### Prerequisites

- An attribute set has been created, see [Create an attribute set](#create-an-attribute-set).
- At least one additional attribute that is not yet assigned to the attribute set has been created, see [Create an attribute](./01_ManageAttributes.md#create-an-attribute).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to edit in the list of attribute sets.   
    The *Edit attribute set* view is displayed.

    ![Edit attribute set](../../Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the *Assigned attributes* section.   
    The *Add attributes* view is displayed. All active attributes that are not yet included in the selected attribute set are displayed in the list.

    ![Add attribute](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AddAttributes.png "[Edit attribute set]")

    > [Info] If the *There are no unassigned attributes.* notice is displayed in the *Add attributes* view, all active attributes are already included in the selected attribute set. Check if you have selected the appropriate attribute set, click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list or [create a new attribute](./01_ManageAttributes.md#create-an-attribute).

3. Select the checkboxes of the attributes you want to add to the attribute set.   
    The editing toolbar is displayed above the list.

4. Click the [ADD] button in the editing toolbar.   
    The selected attributes have been added to the attribute set. The *Add attributes* view is closed. The *Edit attribute set* view is displayed again. The added attributes are displayed in the *Assigned attributes* section.

> [Info] Any changes to the assigned attributes are automatically saved in the attribute set.


### Remove an attribute from the set

Remove an attribute from an attribute set to limit the specifications.
Inherited attributes or mapped attributes cannot be removed from an attribute set.

#### Prerequisites

- An attribute set has been created, see [Create an attribute set](#create-an-attribute-set).
- At least one additional attribute that is not yet assigned to the attribute set has been created, see [Create an attribute](./01_ManageAttributes.md#create-an-attribute).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to edit in the list of attribute sets.   
    The *Edit attribute set* view is displayed.

    ![Edit attribute set](../../Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. In the *Assigned attributes* section, select the checkboxes of the attributes you want to remove from the attribute set.   
    The editing toolbar is displayed above the list.

3. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button in the editing toolbar.   

    > [Info] If the selected attributes cannot be removed from the attribute set, an error message is displayed in the upper right corner.

    The selected attributes have been removed from the attribute set. The list of attributes is updated.

> [Info] Any changes to the assigned attributes are automatically saved in the attribute set.


### Change the required attributes in the set

The product completeness is calculated depending on the required attributes within an attribute set.
All required attributes are marked with a *(required)* indication in the product view.
Note that entities can be saved even if not all *(required)* attributes are completed.   

You can define whether an attribute should be required or not.
Note that inherited attributes can only be changed in the origin attribute set and the required status is also inherited to the linked attribute sets.   

Be aware that the activation or deactivation of languages affects the completeness calculation.
Further, deactivated attributes are not included in the completeness calculation even if they are required.

#### Prerequisites

An attribute set has been created, see [Create an attribute set](#create-an-attribute-set).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to edit in the list of attribute sets.   
    The *Edit attribute set* view is displayed.

    ![Edit attribute set](../../Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. Click the ![Settings](../../Assets/Icons/Settings01.png "[Settings]") (Settings) button in the *Assigned attributes* section.   
    The *Required* column in the list of attributes is unlocked. The color of the ![Settings](../../Assets/Icons/Settings01.png "[Settings]") (Settings) button switches to blue.

    ![Required](../../Assets/Screenshots/DataHub/Settings/AttributeSets/Required.png "[Required]")

3. Enable or disable the *Required* toggle in the *Required* column to define whether or not an attribute value should be required in the selected attribute set.

    > [Info] Be aware that you can only edit the *Required* option for attributes that are not inherited.

4. Click the ![Settings](../../Assets/Icons/Settings02.png "[Settings]") (Settings) button in the *Assigned attributes* section.       
    The *Required* column in the list of attributes is locked. All changes in the attribute list have been saved.

5. Click the ![Back](../../Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the list of attribute sets or proceed to [edit the attribute set](#edit-an-attribute-set).



## Deactivate an attribute set

If an attribute set is no longer used, it is recommended to deactivate the attribute set to prevent any problems because of existing dependencies.
If you deactivate an attribute set, it is no longer available when creating attributes or products.

#### Prerequisites

At least one attribute set has been created, see [Create an attribute set](#create-an-attribute-set).

#### Procedure

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attributes](../../Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attributes]")

1. Click the attribute set you want to deactivate in the list of attribute sets.   
    The *Edit attribute set* view is displayed.

    ![Edit attribute set](../../Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

2. Disable the *Active* toggle.

    > [Info] If you want to reactivate an attribute set, enable the *Active* toggle.

3. Click the [SAVE] button.   
    The attribute set has been deactivated. The *Edit attribute set* view is closed.

4. Press the **F5** key to initialize the *Core1 Platform* and to apply the changes.
