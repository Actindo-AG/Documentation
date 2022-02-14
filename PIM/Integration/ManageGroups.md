[!!PIM](Actindo/PIM)

# Manage a group

The attribute groups serve the logical organization of the product attributes. You can create groups, edit groups and the sorting of the groups themselves as well as the sorting of the attributes within a group.

## Create a group

Create a group for new attributes you want to assign to a certain group.

### Prerequisites

The attributes for the attribute set are created, see [Create an attribute](ManageAttribut.md#create-an-attribute).

### Procedure
*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the button ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the section *Groups* in the left column.   
  The *Edit groups* view is displayed.

  ![Edit groups](/Assets/Screenshots/PIM/Settings/Groups/EditGroups.png "[Edit groups]")

2. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  A plus sign is displayed in the group column.

  ![Add group](/Assets/Screenshots/PIM/Settings/Groups/AddGroup.png "[Add group]")

3. Click the plus sign in the group column.    
  The *Add Element* window is displayed in the group column.

  ![Add element](/Assets/Screenshots/PIM/Settings/Groups/AddElementTop.png "[Add element]")

4. Enter a name for the group in the field *Name*.

5. Enter a key for the group in the field *Key*.

6. Click the button [SAVE].   
  The group is created. The *Add Element* window is closed. The new group is displayed in the group column.

  ![Group created](/Assets/Screenshots/PIM/Settings/Groups/GroupCreated.png "[Group created]")

  > [Info] If you want to change the order of the groups in the list, see [Change the order of groups](#change-the-order-of-groups).

7. Click the button [SAVE] in the upper right corner.  
  The new group is saved. The *Edit groups* view is closed.

### Next steps

- [Edit a group](#edit-a-group)
- [Create a sub-group](#create-a-sub-group)
- [Change the order of groups](#change-the-order-of-groups)
- [Delete a group](#delete-a-group)
- [Add attributes to a group](#add-attributes-to-a-group)
- [Change the order of attributes within a group](#change-the order-of-attributes-within-a-group)
- [Remove attributes from a group](#remove-attributes-from-a-group)
- [Configure the language settings](ConfigureLanguages.md)
- [Configure the scope settings](ConfigureScopes.md)
- [Manage a catalog](ManageCatalog.md)
- [Manage a variant set](ManageVariantSet.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage an attribute](ManageAttribute.md)
- [Manage an attribute set](ManageAttributeSet.md)
- [Manage a product](/PIM/Operation/ManageProduct.md)


## Edit a group

After you have created an attribute group, you can edit it. You can create sub-groups, change the order of groups, add attributes to a groups, change the order of attributes within a group, remove attributes from a group or delete groups.

### Prerequisites

At least one group is created, see [Create a group](#create-a-group).

### Procedure

#### Create a sub-group

Create a sub-group to  organize the attributes in special groups, e.g. depending on product-related categories.

*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the button ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the section *Groups* in the left column.   
  The *Edit groups* view is displayed.

  ![Edit groups](/Assets/Screenshots/PIM/Settings/Groups/EditGroups.png "[Edit groups]")

2. Click the group to which you want to create a sub-group.   
  The existing sub-groups are displayed in the column to the right of the group column.

  ![Sub groups](/Assets/Screenshots/PIM/Settings/Groups/SubGroups.png "[Sub groups]")

3. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  Plus signs are displayed in the group and the sub-group column.

  ![Add sub-group](/Assets/Screenshots/PIM/Settings/Groups/AddSubGroup.png "[Add sub-group]")

4. Click the plus sign in the sub-group column.    
  The *Add Element* window is displayed in the sub-group column.

  ![Add element sub](/Assets/Screenshots/PIM/Settings/Groups/AddElementSub.png "[Add element sub]")

5. Enter a name for the sub-group in the field *Name*.

6. Enter a key for the sub-group in the field *Key*.

7. Click the button [SAVE].   
  The sub-group is created. The *Add Element* window is closed. The new sub-group is displayed in the sub-group column.

  ![Sub-group created](/Assets/Screenshots/PIM/Settings/Groups/SubGroupCreated.png "[Sub-group created]")

  > [Info] If you want to change the order of the sub-groups in the list, see [Change the order of groups](#change-the-order-of-groups).

8. Click the button [SAVE] in the upper right corner.  
  The new sub-group is saved. The *Edit groups* view is closed.


#### Change the order of groups

The order of attribute groups in the tab *GROUPS* equals to the order of attributes groups in the product view. You can change the order to display a group in a different place when creating or editing a product.   
The procedure to change the order of groups and sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the button ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the section *Groups* in the left column.   
  The *Edit groups* view is displayed.

  ![Edit groups](/Assets/Screenshots/PIM/Settings/Groups/EditGroups.png "[Edit groups]")

2. Click and hold the button ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort) to the left of the group you want to move to another position in the list.

3. By using drag and drop, move the selected group to the desired position in the list.

4. Click the button [SAVE] in the upper right corner.  
  The new group order is saved. The *Edit groups* view is closed.


#### Delete a group

You can delete an attribute group if it is no longer in use. Note, that you just delete the group but not the attributes within a group. All active attributes that are no longer assigned to a group are automatically assigned to a group with the name *Unassigned Group* which is only displayed in the product view. If you delete a group with sub-groups, also the sub-groups are deleted. The procedure to delete groups and sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the button ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the section *Groups* in the left column.   
  The *Edit groups* view is displayed.

  ![Edit groups](/Assets/Screenshots/PIM/Settings/Groups/EditGroups.png "[Edit groups]")

2. Click the button ![Edit](/Assets/Icons/Edit03.png "[Edit]") (Edit) to the right of the group you want to delete.   
  The group data is displayed in a window in the group column.

  ![Edit group data](/Assets/Screenshots/PIM/Settings/Groups/EditGroupData.png "[Edit group data]")

3. Click the button ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete) in the bottom left corner of the group data window.    
  The selected group is removed from the group column. The group data window is closed.

4. Click the button [SAVE] in the upper right corner.  
  The group is deleted. The *Edit groups* view is closed.


#### Add attributes to a group

You can add attributes to a group or sub-group. Note that you can add an attribute only to a group without sub-groups. Otherwise, you have to add the attribute to a sub-group. Be aware, that an attribute can be assigned to one group or sub-group only. When you add an attribute to a group that is already added to another group, it is automatically removed from the former group.

*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the group or sub-group to which you want to add an attribute.   
  The selected group is highlighted. The attributes assigned to the group are displayed on the right side.

  > [Info] If a group has at least one sub-group, you can only add an attribute to the sub-group.

  ![Group attributes](/Assets/Screenshots/PIM/Settings/Groups/GroupAttributes.png "[Group attributes]")

2. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  The *Add Attributes To Group* view is displayed.

  ![Add attributes](/Assets/Screenshots/PIM/Settings/Groups/AddAttributes.png "[Add attributes]")

3. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes in the list, you want to add to the selected group.   
  A toolbar is displayed above the list.

  > [Info] Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Only Unassigned Attributes* above the list to hide all attributes that are already assigned to a group.

4. Click the button [ADD] in the toolbar.
  The *Add Attributes To Group* view is closed. The selected attributes are added to the group.

  > [Info] The new attributes are always added at the end of the attribute list. If you want to change the position of an attribute in the list, see [Change the order of attributes within a group](#change-the-order-of-attributes-within-a-group).


#### Change the order of attributes within a group

The order of attributes within a group in the tab *GROUPS* equals to the order of attributes within a group in the product view. You can change the order to display a certain attribute in a different place in the group when creating or editing a product.   
The procedure to change the order of attributes within groups and sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the group or sub-group where you want to change the order of attributes.   
  The selected group is highlighted. The attributes assigned to the group are displayed on the right side.

  ![Group attributes](/Assets/Screenshots/PIM/Settings/Groups/GroupAttributes.png "[Group attributes]")

2. Click the button ![Sort attributes](/Assets/Icons/Sort02.png "[Sort attributes]") (Sort attributes) above the list.   
  The *Assigned Attributes (Sorting Mode)* view is displayed on the right side.

  ![Assigned attributes](/Assets/Screenshots/PIM/Settings/Groups/AssignedAttributes.png "[Assigned attributes]")

3. Click and hold the button ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort) to the left of the attribute you want to move to another position in the list.

4. By using drag and drop, move the selected attribute to the desired position in the list.

  > [Info] Repeat the steps **3** and **4** for all attributes whose position in the list you want to change.

5. Click the button [SAVE] in the upper right corner.
  The new order of attributes within the selected group is saved. The *Assigned Attributes (Sorting Mode)* view is closed.


#### Remove attributes from a group

You can remove an attribute from a group if it is no longer in use. Note, that you just remove the attribute from the group but you do not delete the attribute itself. Alternatively, you can [deactivate an attribute]((ManageAttribute.md#deactivate-an-attribute)) so it is no longer displayed in the product view. The procedure to remove attributes from groups or sub-groups is identical. Just select the sub-group instead of the group and follow the steps described below.

*PIM > Settings > Tab GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/Groups/Groups.png "[Groups]")

1. Click the group or sub-group where you want to remove an attribute from.   
  The selected group is highlighted. The attributes assigned to the group are displayed on the right side.

  ![Group attributes](/Assets/Screenshots/PIM/Settings/Groups/GroupAttributes.png "[Group attributes]")

2. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the attributes in the list, you want to remove from the selected group.   
  A toolbar is displayed above the list.

3. Click the button ![Remove](/Assets/Icons/Trash03.png "[Remove]") (Remove) in the toolbar.   
  The selected attributes are removed from the list.


### Next steps

- [Configure the language settings](ConfigureLanguages.md)
- [Configure the scope settings](ConfigureScopes.md)
- [Manage a catalog](ManageCatalog.md)
- [Manage a variant set](ManageVariantSet.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a group](#create-a-group)
- [Manage an attribute](ManageAttribute.md)
- [Manage an attribute set](ManageAttributeSet.md)
- [Manage a product](/PIM/Operation/ManageProduct.md)
