[!!User Interface DataHub](/DataHub/UserInterface/02c_AttributeGroups.md)
[!!Manage the attributes](01_ManageAttributes.md)
[!!Manage the attribute sets](02_ManageAttributeSets.md)


# Manage the attribute groups

The attribute groups serve the logical organization of the product attributes. You can create attribute groups, edit attribute groups and the sorting of the attribute groups themselves as well as the sorting of the attributes within a group.

## Create an attribute group

Create an attribute group for new attributes you want to assign to a certain group.

#### Prerequisites

The attributes for the attribute set are created, see [Create an attribute](01_ManageAttributes.md#create-an-attribute).

#### Procedure
*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Attribute groups* section in the left column.   
  The *Edit attribute groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  A plus sign is displayed in the attribute group column.

  ![Add attribute group](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributeGroup.png "[Add attribute group]")

3. Click the plus sign in the attribute group column.    
  The *Add element* window is displayed in the attribute group column.

  ![Add element](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddElement.png "[Add element]")

4. Enter a name for the attribute group in the *Name* field.

5. Enter a key for the attribute group in the *Key* field.

6. Click the [SAVE] button.   
  The attribute group is created. The *Add element* window is closed. The new attribute group is displayed in the attribute group column.

  ![Attribute group created](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroupCreated.png "[Attribute group created]")

  > [Info] If you want to change the order of the attribute groups in the list, see [Change the order of attribute groups](#change-the-order-of-attribute-groups).

7. Click the [SAVE] button in the upper right corner.  
  The new attribute group is saved. The *Edit attribute groups* view is closed.



## Edit an attribute group

After you have created an attribute group, you can edit it. You can create attribute sub-groups, change the order of attribute groups, add attributes to a group, change the order of attributes within a group, remove attributes from an attribute group or delete attribute groups.

### Create an attribute sub-group

Create an attribute sub-group to organize the attributes in special groups, for instance depending on product-related categories.

#### Prerequisites

At least one attribute group is created, see [Create an attribute group](#create-an-attribute-group).

#### Procedure
*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Attribute groups* section in the left column.   
  The *Edit attribute groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click the attribute group to which you want to create a sub-group.   
  The existing attribute sub-groups are displayed in the column to the right of the attribute group column.

  ![Attribute sub-groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeSubGroups.png "[Attribute sub-groups]")

3. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  Plus signs are displayed in the attribute group and the attribute sub-group column.

  ![Add attribute sub-group](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributeSubGroups.png "[Add attribute sub-group]")

4. Click the plus sign in the attribute sub-group column.    
  The *Add element* window is displayed in the attribute sub-group column.

  ![Add element](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddElement.png "[Add element]")

5. Enter a name for the attribute sub-group in the *Name* field.

6. Enter a key for the attribute sub-group in the *Key* field.

7. Click the [SAVE] button.   
  The attribute sub-group is created. The *Add element* window is closed. The new attribute sub-group is displayed in the attribute sub-group column.

  ![Attribute sub-group created](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeSubGroupCreated.png "[Attribute sub-group created]")

  > [Info] If you want to change the order of the attribute sub-groups in the list, see [Change the order of attribute groups](#change-the-order-of-attribute-groups).

8. Click the [SAVE] button in the upper right corner.  
  The new attribute sub-group is saved. The *Edit attribute groups* view is closed.


### Change the order of attribute groups

The order of attribute groups in the *ATTRIBUTE GROUPS* tab equals to the order of attributes groups in the product view. You can change the order to display an attribute group in a different place when creating or editing a product.   
The procedure to change the order of attribute groups and sub-groups is identical. Just select the attribute sub-group instead of the group and follow the steps described below.

#### Prerequisites

At least two attribute groups are created, see [Create an attribute group](#create-an-attribute-group).

#### Procedure
*DataHub > Settings > Tab ATTRIBUTE GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Attribute groups* section in the left column.   
  The *Edit attribute groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click and hold the ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort) button to the left of the attribute group you want to move to another position in the list.

3. By using drag and drop, move the selected attribute group to the desired position in the list.

4. Click the [SAVE] button in the upper right corner.  
  The new attribute group order is saved. The *Edit attribute groups* view is closed.


### Delete an attribute group

You can delete an attribute group if it is no longer in use. Note, that you just delete the attribute group but not the attributes within a group. All active attributes that are no longer assigned to an attribute group are automatically assigned to a new attribute group with the name *Unassigned group* which is only displayed in the product view. If you delete an attribute group with sub-groups, also the attribute sub-groups are deleted. The procedure to delete attribute groups and sub-groups is identical. Just select the attribute sub-group instead of the group and follow the steps described below.

#### Prerequisites

At least one attribute group is created, see [Create an attribute group](#create-an-attribute-group).

#### Procedure
*DataHub > Settings > Tab ATTRIBUTE GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Attribute groups* section in the left column.   
  The *Edit attribute groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click the ![Edit](/Assets/Icons/Edit03.png "[Edit]") (Edit) button to the right of the attribute group you want to delete.   
  The attribute group data is displayed in a window in the attribute group column.

  ![Edit attribute group data](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroupData.png "[Edit attribute group data]")

3. Click the ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete) button in the bottom left corner of the attribute group data window.    
  The selected attribute group is removed from the attribute group column. The attribute group data window is closed.

4. Click the [SAVE] button in the upper right corner.  
  The attribute group is deleted. The *Edit attribute groups* view is closed.


### Add attributes to a group

You can add attributes to an  group or sub-group. Note that you can add an attribute only to an attribute group without sub-groups. Otherwise, you have to add the attribute to an attribute sub-group. Be aware, that an attribute can be assigned to one attribute group or sub-group only. When you add an attribute to an attribute group that is already added to another group, it is automatically removed from the former attribute group.

#### Prerequisites

- At least one attribute group is created, see [Create an attribute group](#create-an-attribute-group).
- At least one attribute is created that is not yet assigned to a group, see [Create an attribute](01_ManageAttributes.md#create-an-attribute).

#### Procedure
*DataHub > Settings > Tab ATTRIBUTE GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the attribute group or sub-group to which you want to add an attribute.   
  The selected attribute group is highlighted. The attributes assigned to the group are displayed on the right side.

  > [Info] If an attribute group has at least one attribute sub-group, you can only add an attribute to the sub-group.

  ![Group attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

2. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Add attributes to attribute group* view is displayed.

  ![Add attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributes.png "[Add attributes]")

3. Select the checkboxes of the attributes in the list, you want to add to the selected attribute group.   
  A toolbar is displayed above the list.

  > [Info] Enable the *Only Unassigned Attributes* toggle above the list to hide all attributes that are already assigned to an attribute group.

4. Click the [ADD] button in the toolbar.
  The *Add attributes to attribute group* view is closed. The selected attributes are added to the attribute group.

  > [Info] The new attributes are always added at the end of the attribute list. If you want to change the position of an attribute in the list, see [Change the order of attributes within a group](#change-the-order-of-attributes-within-a-group).


### Change the order of attributes within a group

The order of attributes within an attribute group in the *ATTRIBUTE GROUPS* tab equals to the order of attributes within a group in the product view. You can change the order to display a certain attribute in a different place in the attribute group when creating or editing a product.   
The procedure to change the order of attributes within attribute groups and sub-groups is identical. Just select the attribute sub-group instead of the group and follow the steps described below.

#### Prerequisites

- At least one attribute group is created, see [Create an attribute group](#create-an-attribute-group).
- At least two attributes are added to the attribute group, see [Add attributes to a group](#add-attributes-to-a-group).

#### Procedure
*DataHub > Settings > Tab ATTRIBUTE GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the attribute group or sub-group where you want to change the order of attributes.   
  The selected attribute group is highlighted. The attributes assigned to the group are displayed on the right side.

  ![Group attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

2. Click the ![Sort attributes](/Assets/Icons/Sort02.png "[Sort attributes]") (Sort attributes) button above the list.   
  The *Assigned attributes (Sorting mode)* view is displayed on the right side.

  ![Assigned attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AssignedAttributes.png "[Assigned attributes]")

3. Click and hold the ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort) button to the left of the attribute you want to move to another position in the list.

4. By using drag and drop, move the selected attribute to the desired position in the list.

  > [Info] Repeat the steps **3** and **4** for all attributes whose position in the list you want to change.

5. Click the [SAVE] button in the upper right corner.
  The new order of attributes within the selected attribute group is saved. The *Assigned attributes (Sorting mode)* view is closed.


### Remove attributes from a group

You can remove an attribute from an attribute group if it is no longer in use. Note, that you just remove the attribute from the attribute group but you do not delete the attribute itself. Alternatively, you can [deactivate an attribute](01_ManageAttributes.md#deactivate-an-attribute) so it is no longer displayed in the product view. The procedure to remove attributes from attribute groups or sub-groups is identical. Just select the attribute sub-group instead of the group and follow the steps described below.

#### Prerequisites

- At least one attribute group is created, see [Create an attribute group](#create-an-attribute-group).
- At least one attribute is added to the attribute group, see [Add attributes to a group](#add-attributes-to-a-group).

#### Procedure
*DataHub > Settings > Tab ATTRIBUTE GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the attribute group or sub-group where you want to remove an attribute from.   
  The selected attribute group is highlighted. The attributes assigned to the attribute group are displayed on the right side.

  ![Group attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

2. Select the checkboxes of the attributes in the list, you want to remove from the selected attribute group.   
  A toolbar is displayed above the list.

3. Click the ![Remove](/Assets/Icons/Trash03.png "[Remove]") (Remove) button in the toolbar.   
  The selected attributes are removed from the list.
