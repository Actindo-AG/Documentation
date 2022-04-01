[!!DataHub](DataHub)

# Manage the attribute groups

The attribute groups serve the logical organization of the product attributes. You can create groups, edit groups and the sorting of the groups themselves as well as the sorting of the attributes within a group.

## Create an attribute group

Create an attribute group for new attributes you want to assign to a certain group.

### Prerequisites

The attributes for the attribute set are created, see [Create an attribute](01_ManageAttributes.md#create-an-attribute).

### Procedure
*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Groups* section in the left column.   
  The *Edit groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  A plus sign is displayed in the group column.

  ![Add attribute group](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributeGroup.png "[Add attribute group]")

3. Click the plus sign in the group column.    
  The *Add Element* window is displayed in the group column.

  ![Add element](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddElement.png "[Add element]")

4. Enter a name for the group in the *Name* field.

5. Enter a key for the group in the *Key* field.

6. Click the [SAVE] button.   
  The group is created. The *Add Element* window is closed. The new group is displayed in the group column.

  ![Attribute group created](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroupCreated.png "[Attribute group created]")

  > [Info] If you want to change the order of the groups in the list, see [Change the order of groups](#change-the-order-of-groups).

7. Click the [SAVE] button in the upper right corner.  
  The new group is saved. The *Edit groups* view is closed.

### Next steps

- [Edit an attribute group](#edit-an-attribute-group)
- [Create an attribute sub-group](#create-an-attribute-sub-group)
- [Change the order of attribute groups](#change-the-order-of-attribute-groups)
- [Delete an attribute group](#delete-an-attribute-group)
- [Add attributes to a group](#add-attributes-to-a-group)
- [Change the order of attributes within a group](#change-the-order-of-attributes-within-a-group)
- [Remove attributes from a group](#remove-attributes-from-a-group)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the attributes](01_ManageAttributes.md)
- [Manage the attribute sets](02_ManageAttributeSets.md)


## Edit an attribute group

After you have created an attribute group, you can edit it. You can create sub-groups, change the order of groups, add attributes to a group, change the order of attributes within a group, remove attributes from a group or delete groups.

### Prerequisites

At least one group is created, see [Create an attribute group](#create-an-attribute-group).

### Procedure

#### Create an attribute sub-group

Create a sub-group to organize the attributes in special groups, for instance depending on product-related categories.

*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Groups* section in the left column.   
  The *Edit groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click the group to which you want to create a sub-group.   
  The existing sub-groups are displayed in the column to the right of the group column.

  ![Attribute sub-groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeSubGroups.png "[Attribute sub-groups]")

3. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  Plus signs are displayed in the group and the sub-group column.

  ![Add attribute sub-group](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributeSubGroups.png "[Add attribute sub-group]")

4. Click the plus sign in the sub-group column.    
  The *Add Element* window is displayed in the sub-group column.

  ![Add element](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddElement.png "[Add element]")

5. Enter a name for the sub-group in the *Name* field.

6. Enter a key for the sub-group in the *Key* field.

7. Click the [SAVE] button.   
  The sub-group is created. The *Add Element* window is closed. The new sub-group is displayed in the sub-group column.

  ![Attribute sub-group created](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeSubGroupCreated.png "[Attribute sub-group created]")

  > [Info] If you want to change the order of the sub-groups in the list, see [Change the order of groups](#change-the-order-of-groups).

8. Click the [SAVE] button in the upper right corner.  
  The new sub-group is saved. The *Edit groups* view is closed.


#### Change the order of attribute groups

The order of attribute groups in the *GROUPS* tab equals to the order of attributes groups in the product view. You can change the order to display an attribute group in a different place when creating or editing a product.   
The procedure to change the order of groups and sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Groups* section in the left column.   
  The *Edit groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click and hold the ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort) button to the left of the group you want to move to another position in the list.

3. By using drag and drop, move the selected group to the desired position in the list.

4. Click the [SAVE] button in the upper right corner.  
  The new group order is saved. The *Edit groups* view is closed.


#### Delete an attribute group

You can delete an attribute group if it is no longer in use. Note, that you just delete the group but not the attributes within a group. All active attributes that are no longer assigned to a group are automatically assigned to a group with the name *Unassigned Group* which is only displayed in the product view. If you delete an attribute group with sub-groups, also the sub-groups are deleted. The procedure to delete groups and sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button to the right of the *Groups* section in the left column.   
  The *Edit groups* view is displayed.

  ![Edit attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

2. Click the ![Edit](/Assets/Icons/Edit03.png "[Edit]") (Edit) button to the right of the group you want to delete.   
  The group data is displayed in a window in the group column.

  ![Edit attribute group data](/Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroupData.png "[Edit attribute group data]")

3. Click the ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete) button in the bottom left corner of the group data window.    
  The selected group is removed from the group column. The group data window is closed.

4. Click the [SAVE] button in the upper right corner.  
  The group is deleted. The *Edit groups* view is closed.


#### Add attributes to a group

You can add attributes to a group or sub-group. Note that you can add an attribute only to a group without sub-groups. Otherwise, you have to add the attribute to a sub-group. Be aware, that an attribute can be assigned to one group or sub-group only. When you add an attribute to a group that is already added to another group, it is automatically removed from the former group.

*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the group or sub-group to which you want to add an attribute.   
  The selected group is highlighted. The attributes assigned to the group are displayed on the right side.

  > [Info] If an attribute group has at least one sub-group, you can only add an attribute to the sub-group.

  ![Group attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

2. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Add Attributes To Group* view is displayed.

  ![Add attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributesGroup.png "[Add attributes]")

3. Select the checkboxes of the attributes in the list, you want to add to the selected group.   
  A toolbar is displayed above the list.

  > [Info] Activate the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Only Unassigned Attributes* toggle above the list to hide all attributes that are already assigned to a group.

4. Click the [ADD] button in the toolbar.
  The *Add Attributes To Group* view is closed. The selected attributes are added to the group.

  > [Info] The new attributes are always added at the end of the attribute list. If you want to change the position of an attribute in the list, see [Change the order of attributes within a group](#change-the-order-of-attributes-within-a-group).


#### Change the order of attributes within a group

The order of attributes within a group in the *GROUPS* tab equals to the order of attributes within a group in the product view. You can change the order to display a certain attribute in a different place in the group when creating or editing a product.   
The procedure to change the order of attributes within groups and sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*DataHub > Settings > Tab GROUPS*

![Attribute groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Attribute groups]")

1. Click the group or sub-group where you want to change the order of attributes.   
  The selected group is highlighted. The attributes assigned to the group are displayed on the right side.

  ![Group attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

2. Click the ![Sort attributes](/Assets/Icons/Sort02.png "[Sort attributes]") (Sort attributes) button above the list.   
  The *Assigned Attributes (Sorting Mode)* view is displayed on the right side.

  ![Assigned attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AssignedAttributes.png "[Assigned attributes]")

3. Click and hold the ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort) button to the left of the attribute you want to move to another position in the list.

4. By using drag and drop, move the selected attribute to the desired position in the list.

  > [Info] Repeat the steps **3** and **4** for all attributes whose position in the list you want to change.

5. Click the [SAVE] button in the upper right corner.
  The new order of attributes within the selected group is saved. The *Assigned Attributes (Sorting Mode)* view is closed.


#### Remove attributes from a group

You can remove an attribute from a group if it is no longer in use. Note, that you just remove the attribute from the group but you do not delete the attribute itself. The procedure to remove attributes from groups or sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*DataHub > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/DataHub/Settings/AttributeGroups/AttributeGroups.png "[Groups]")

1. Click the group or sub-group where you want to remove an attribute from.   
  The selected group is highlighted. The attributes assigned to the group are displayed on the right side.

  ![Group attributes](/Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

2. Select the checkboxes of the attributes in the list, you want to remove from the selected group.   
  A toolbar is displayed above the list.

3. Click the ![Remove](/Assets/Icons/Trash03.png "[Remove]") (Remove) button in the toolbar.   
  The selected attributes are removed from the list.


### Next steps



### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create an attribute group](#create-an-attribute-group)
- [Manage the attributes](01_ManageAttributes.md)
- [Manage the attribute sets](02_ManageAttributeSets.md)
