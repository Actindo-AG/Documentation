[!!Manage an attribute group](../Integration/03_ManageAttributeGroups.md)

# Attribute groups

*DataHub > Data model> Tab ATTRIBUTE GROUPS*

![Group attributes](../../Assets/Screenshots/DataHub/Settings/AttributeGroups/GroupAttributes.png "[Group attributes]")

<details><summary>Click for further information on the screens described in this chapter</summary>

For detailed information on the described user interfaces, refer to our *Actindo Core1 Platform* documentation for 
general features and functions, standard buttons, UI elements, and how to use the Actindo documentation. 
Among others, see the following:

- [Use general user interface functions](../../Core1Platform/UsingCore1/04GeneralUIFunctions.md)
- [Standard buttons and functions](../../Core1Platform/UserInterface/04_Buttons.md)
- [Work with lists](../../Core1Platform/UsingCore1/05_WorkWithLists.md)
- [LIST views](../../Core1Platform/UserInterface/03_ViewsLIST.md)

</details>
<BR>


**Attribute groups**   
This view displays both the attribute groups on the left side and the attributes assigned to a selected group on the right side. 

- ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit)   
    Click this button to edit the attribute groups. The *Edit attribute groups* view is displayed.   
    For detailed information, see [Edit an attribute group](../Integration/03_ManageAttributeGroups.md#edit-an-attribute-group).

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow *>* left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group in the *Assigned attributes* list.

**Assigned attributes**

The list displays all attributes assigned to the selected attribute group. Depending on the settings, the displayed columns may vary. All fields are read-only. If no attribute is assigned to the selected attribute group, the notice *No attribute assigned. Use + button to assign one* is displayed.

- ![Sort](../../Assets/Icons/Sort02.png "[Sort]") (Sort)   
    Click this button to display the *Assigned Attributes (Sorting Mode)* view on the right side of the workspace. This button is only displayed if an attribute group is selected.

The following functions are available for the editing toolbar:

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the list are selected.

- ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete)   
    Click this button to remove the selected attribute from the attribute group. The button is only displayed if the checkbox of an attribute is selected.       

    > [Info] If you remove an attribute from the attribute group, the attribute itself is not deleted, but it is unassigned to the selected attribute group.  

The following functions and fields are available in this section:

- *Name*   
    Attribute name.

- *Key*   
    Attribute key.

- *Description*   
    Description to the attribute.

- *Plugin*   
    Module or plugin that owns the attribute.

- *Read-only*   
    Indication whether the attribute is read-only or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is read-only.  
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute can be edited.

- *ID*   
    Attribute identification number. The ID number is automatically assigned by the system.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to add an attribute to the selected attribute group. The *Add attributes to attribute group* view is displayed.   


## Add attributes to group

*DataHub > Data model > Tab ATTRIBUTE GROUPS > Button Add*

![Add attributes](../../Assets/Screenshots/DataHub/Settings/AttributeGroups/AddAttributes.png "[Add attributes]")

**Add attributes to group "Attribute group name"**

The list displays all attributes that are not assigned to the selected attribute group. Depending on the settings, the displayed columns may vary. All fields are read-only.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Only unassigned attributes*   
    Enable this toggle to display only the attributes that are not yet assigned to any attribute group. Disable the toggle to display all attributes. By default, this toggle is disabled.

    > [Info] An attribute can be assigned to one attribute group or sub-group only. When you add an attribute to an attribute group that is already added to another group, it is automatically removed from the former attribute group.

The following functions are available for the editing toolbar:

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the list are selected. Alternatively, you can click directly a row in the list to select the attribute.

- [ADD]   
    Click this button to add the selected attribute to the attribute group. The *Add attributes to attribute group* view is closed.

The following functions and fields are available in this view:

- *Name*   
    Attribute name.

- *Key*   
    Attribute key.

- *Current attribute group*   
    Attribute group to which the attribute is currently assigned.

- *Description*   
    Description to the attribute.

- *Status*   
    Attribute status. The following statuses are available:
    - ![Status](../../Assets/Icons/Status01.png "[Status]") **Active**
    - ![Status](../../Assets/Icons/Status04.png "[Status]") **Inactive**   

- *Read-only*   
    Indication whether the attribute is read-only or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is read-only.  
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute can be edited.

- *ID*   
    Attribute identification number. The ID number is automatically assigned by the system.



## Edit attribute groups

*DataHub > Data model > Tab ATTRIBUTE GROUPS > Button Edit*

![Edit attribute groups](../../Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroups.png "[Edit attribute groups]")

**Edit attribute groups**


- ![Sort](../../Assets/Icons/Sort01.png "[Sort]") (Sort)   
    Click and hold this button to move the selected attribute group to another position in the list using drag and drop.

- ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit)   
    Click this button to edit the selected attribute group. The attribute group data window is displayed. This button is only displayed if you hover over an attribute group or sub-group.

- *"Attribute group name"*   
    Top attribute group. Click the attribute group to display the attribute sub-group column and all assigned attribute sub-groups. Hover over the attribute group to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- *"Attribute sub-group name"*   
    Attribute sub-group to the selected attribute group. Hover over the attribute sub-group to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to add an attribute group or sub-group. A plus sign is displayed in each displayed column. Click the plus sign in the desired column to add a new attribute group or sub-group to the selected attribute group. The *Add element* window is displayed.   

    > [Info] Attribute groups are organized in a tree structure with a maximum depth of two levels. That means that a maximum of one sub-group level can be added to an attribute group.


### Add element

*DataHub > Data model > Tab ATTRIBUTE GROUPS > Button Edit > Button Add*

![Add element](../../Assets/Screenshots/DataHub/Settings/AttributeGroups/AddElement.png "[Add element]")

> [Info] The *Add element* window for attribute groups and sub-groups is identical.

- *"Language name"*   
    Click the drop-down list and select the system language in which the *Name (Language)* and *Description (Language)* fields are displayed. By default, the following options are available:
    - **English (United States)**
    - **Deutsch (Deutschland)**

- *Name (Language)*   
    Enter an attribute group name in the selected language.

- *Key*   
    Enter an attribute group key. The number of characters is limited to 190.

- [CANCEL]   
    Click this button to cancel adding an attribute group. The *Add element* window is closed.

- [SAVE]   
    Click this button to add the new attribute group. The *Add element* window is closed.

    > [Info] You have to click the [SAVE] button in the *Edit attribute groups* view to save the added attribute group. Otherwise, all changes are rejected.


### Edit attribute group data

*DataHub > Data model > Tab ATTRIBUTE GROUPS > Button Edit > Hover over attribute group > Button Edit*

![Edit attribute group data](../../Assets/Screenshots/DataHub/Settings/AttributeGroups/EditAttributeGroupData.png "[Edit attribute group data]")

> [Info] The *Edit attribute group data* window for attribute groups and sub-groups is identical.

- *"Language name"*   
    Click the drop-down list and select the system language in which the *Name (Language)* and *Description (Language)* fields are displayed. By default, the following options are available:
    - **English (United States)**
    - **Deutsch (Deutschland)**

- *Name (Language)*   
    Click the field to edit the attribute group name in the selected language.

- *Key*   
    Click the field to edit the attribute group key. The number of characters is limited to 190.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)   
    Click this button to remove the selected attribute group.

    > [Info] You must click the [SAVE] button in the *Edit attribute groups* view to permanently delete the attribute group.

    > [Caution] Be aware that as soon as you delete an attribute group, you also delete all assigned attribute sub-groups.

- [CANCEL]   
    Click this button to cancel editing the attribute group. The *Edit attribute group data* window is closed.

- [SAVE]   
    Click this button to save any changes to the attribute group. The *Edit attribute group data* window is closed.

    > [Info] You have to click the [SAVE] button in the *Edit attribute groups* view to save the changes. Otherwise, all changes are rejected.
