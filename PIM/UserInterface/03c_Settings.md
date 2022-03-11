# Attribute Groups

*PIM > Settings > Tab ATTRIBUTE GROUPS*

![Groups](/Assets/Screenshots/PIM/Settings/AttributeGroups/Groups.png "[Groups]")

**Groups**

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the attribute groups. The *Edit groups* view is displayed.   
  For detailed information, see [Edit an attribute group](/PIM/Integration/03_ManageGroups.md#edit-an-attribute-group).

- ![Folders](/Assets/Icons/Folders01.png "[Folders]") (Folders)  
  Attribute group that contains sub-groups. Click the group or the arrow *>* left to the group to unfold the group and display the sub-groups.

- ![Folder](/Assets/Icons/Folder01.png "[Folder]") (Folder)  
  Attribute group. Click the group to display all attributes that are assigned to the selected group in the *Assigned Attributes* list.

**Assigned Attributes**

- ![Sort](/Assets/Icons/Sort02.png "[Sort]") (Sort)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active. The button is only displayed when an attribute group is selected.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute. The button is only displayed when an attribute group is selected.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of assigned attributes. The button is only displayed when an attribute group is selected.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the list are selected.

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to remove the selected attribute from the group. The button is only displayed when the checkbox of an attribute is selected.       

  > [Info] If you remove an attribute from the group, the attribute itself is not deleted, but it is unassigned to the selected group.  

The list displays all attributes assigned to the selected attribute group. All fields are read-only. Depending on the settings, the displayed columns may vary. When no attribute is assigned to the selected group, the notice *No attribute assigned. Use + button to assign one* is displayed.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Description*   
  Description to the attribute.

- *Plugin*   
  Module or plugin from which the attribute is created. In the *PIM* module, only PIM attributes are displayed.
  [comment]: <> (Is that correct?)


- *Read-only*   
  Indication whether the attribute is read-only or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is read-only.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute can be edited.


- *ID*   
  Attribute identification number. The ID number is automatically assigned by the system.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add an attribute to the selected group. The *Add Attributes to Group* view is displayed.   


## Add attributes to group
*PIM > Settings > Tab ATTRIBUTE GROUPS > Button Add*

![Add attributes](/Assets/Screenshots/PIM/Settings/AttributeGroups/AddAttributes.png "[Add attributes]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to cancel adding an attribute to the selected attribute group and close the *Add Attribute to Group* view.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Only Unassigned Attributes*   
  Activate this toggle to display only the attributes that are not yet assigned to any group. Deactivate the toggle to display all attributes. By default, this toggle is inactive.

  > [Info] An attribute can be assigned to one attribute group or sub-group only. When you add an attribute to a group that is already added to another group, it is automatically removed from the former group.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the list are selected. Alternatively, you can click directly a row in the list to select the attribute.

- [ADD]   
  Click this button to add the selected attribute to the group. The *Add Attributes to Group* view is closed.

The list displays all attributes that are not assigned to the selected group. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Current Group*   
  Group to which the attribute is currently assigned.

- *Description*   
  Description to the attribute.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Read-only*   
  Indication whether the attribute is read-only or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is read-only.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute can be edited.


- *ID*   
  Attribute identification number. The ID number is automatically assigned by the system.

[comment]: <> (Hier weiter)

## Edit attribute groups
*PIM > Settings > Tab ATTRIBUTE GROUPS > Button Edit*

![Edit groups](/Assets/Screenshots/PIM/Settings/AttributeGroups/EditGroups.png "[Edit groups]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit groups* view and return to the *Groups* view. All changes are rejected.

- [CANCEL]   
  Click this button to cancel editing groups and close the *Edit groups* view.

- [SAVE]   
  Click this button to save all changes and close the *Edit groups* view.

- ![Sort](/Assets/Icons/Sort01.png "[Sort]") (Sort)   
  Click and hold this button to move the selected group to another position in the list using drag and drop.

- ![Edit](/Assets/Icons/Edit03.png "[Edit]") (Edit)   
  Click this button to edit the selected group. The group data window is displayed. This button is only displayed, when you hover over the group.

- Attribute group   
  Top attribute group. Click the group to display the sub-group column and all assigned sub-groups. Hover over the group to display the ![Edit](/Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- Attribute sub-group   
  Sub-group to the selected attribute group. Hover over the sub-group to display the ![Edit](/Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add an attribute group or sub-group. A plus sign is displayed in each displayed column. Click the plus sign in the desired column to add a new group or sub-group to the selected group. The *Add Element* window is displayed.    
  For detailed information about creating groups or sub-groups, see [Create an attribute group](/PIM/Integration/03_ManageGroups.md#create-an-attribute-group) or [Create an attribute sub-group](/PIM/Integration/03_ManageGroups.md#create-an-attribute-sub-group).


### Add element
*PIM > Settings > Tab ATTRIBUTE GROUPS > Button Edit > Button Add*

![Add element](/Assets/Screenshots/PIM/Settings/AttributeGroups/AddElement.png "[Add element]")

> [Info] The *Add Element* window for groups and sub-groups is identical.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* field is displayed. The system languages *English (United States)* and *Deutsch (Deutschland)* are available in the drop-down list.
  [comment]: <> (Is that right? -> language question)

- *Name (Language)*   
  Enter an attribute group name in the selected language.

- *Key*   
  Enter an attribute group key. The key is required for API access and must be system wide unique.

- [CANCEL]   
  Click this button to cancel adding an attribute group, close the *Add Element* window and return to the *Edit groups* view.

- [SAVE]   
  Click this button to add the new attribute group, close the *Add Element* window and return to the *Edit groups* view.

  > [Info] You have to click the [SAVE] button in the *Edit groups* view to save the added group.


### Edit group data
*PIM > Settings > Tab ATTRIBUTE GROUPS > Button Edit > Hover over group > Button Edit*

![Group data](/Assets/Screenshots/PIM/Settings/AttributeGroups/GroupData.png "[Group data]")

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* field is displayed. The system languages *English (United States)* and *Deutsch (Deutschland)* are available in the drop-down list.
  [comment]: <> (Is that right? -> language question)

- *Name (Language)*   
  Click the field to edit the attribute group name in the selected language.

- *Key*   
  Click the field to edit the attribute group key. The key is required for API access and must be system wide unique.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to remove the selected attribute group.

  > [Info] You have to click the [SAVE] button in the *Edit groups* view to finally delete the attribute group.

  > [Warning] Be aware that as soon as you delete an attribute group, you also delete all assigned sub-groups.

- [CANCEL]   
  Click this button to cancel adding an attribute group, close the window and return to the *Edit groups* view.

- [SAVE]   
  Click this button to add the new attribute group, close the window and return to the *Edit groups* view.

  > [Info] You have to click the [SAVE] button in the *Edit groups* view to save the changes.
