# Attributes

*DataHub > Settings > Tab ATTRIBUTES*

![Attributes](../../Assets/Screenshots/DataHub/Settings/Attributes/Attributes.png "[Attributes]")

**Attribute list**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. You cannot select multiple checkboxes at once.

- [EDIT]   
  Click this button to edit the selected attribute. This button is only displayed, when the checkbox of an attribute is selected. Alternatively, you can click directly a row in the list to edit an attribute.
  For detailed information, see [Edit an attribute](../Integration/01_ManageAttributes.md#edit-an-attribute).

- [DELETE]   
  Click this button to delete the selected attribute. This button is only displayed, when the checkbox of an attribute is selected.       
  For detailed information, see [Delete an attribute](../Integration/01_ManageAttributes.md#delete-an-attribute).

The list displays all attributes. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](../../Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](../../Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Group*   
  Attribute group assigned to the attribute. If the attribute is not assigned to any attribute group, *not assigned* is displayed.

- *Key*   
  Attribute key.

- *Data type*   
  Attribute data type. For detailed information about all data types, see [Data type list](../../PIM/UserInterface/04_DataTypeList.md).

- *Description*   
  Description to the attribute.

- *Multi-language*   
  Indication whether the attribute is multi-language or not:
  - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-language.  
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single language.


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.


- *Plugin*   
  Module or plugin from which the attribute is created.

- *ID*   
  Attribute identification number. The ID number is automatically assigned by the system.

- *Modified on*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the attribute.

- *Created on*   
  Date and time of the creation.

- *Created by*   
  Name and username of the user who created the attribute.

- *Name (Language)*   
  Attribute name in the selected language. A single *Name (Language)* column is displayed for the system languages *English (United States)* and *Deutsch (Deutschland)*.

- *Description (Language)*   
  Attribute description in the displayed language. A single *Description (Language)* column is displayed for the system languages *English (United States)* and *Deutsch (Deutschland)*.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create an attribute. The *Create attribute* view is displayed.   


## Create attribute
*DataHub > Settings > Tab ATTRIBUTES > Button Add*

![Create attribute](../../Assets/Screenshots/DataHub/Settings/Attributes/CreateAttribute.png "[Create attribute]")

**Create attribute**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create attribute* view and return to the attributes list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* and *Description (Language)* fields are displayed. The system languages *English (United States)* and *Deutsch (Deutschland)* are available in the drop-down list.

- [SAVE]   
  Click this button to save the attribute, close the *Create attribute* view and return to the attributes list.

- *Name (Language)*   
  Enter an attribute name in the selected language.

- *Description (Language)*   
  Enter a description to the attribute in the selected language.

- *Data type*   
  Click the drop-down list and select an attribute data type. For detailed information about all data types, see [Data type list](../../PIM/UserInterface/04_DataTypeList.md).

- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Multi-language*   
  Enable this toggle to create a multi-lingual attribute. Disable the toggle to create a single language attribute. By default, this toggle is inactive.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Multi-channel*   
  Enable this toggle to create a multi-channel attribute. Disable the toggle to create a single channel attribute. By default, this toggle is inactive.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Enable this toggle to set the attribute status to active. Disable the toggle to set the status to inactive. By default, this toggle is active.

- *Assigned sets*   
    Click the drop-down list and select an attribute set to which the attribute is assigned after creation. All active attribute sets are displayed. The drop-down list is only displayed when at least one attribute set drop-down list has been added.

  - ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add)    
    Click this button to add an attribute set drop-down list. You can add an infinite number of attribute sets.

  - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)   
    Click this button to delete the corresponding attribute set.

    > [Info] When you assign the attribute to no attribute set in this view, you have to assign the attribute afterwards to an attribute set, see [Add an attribute to the set](../Integration/02_ManageAttributeSets.md#add-an-attribute-to-the-set).


**CONFIGURATION**

The *CONFIGURATION* section displays the additional configuration for the selected data type. The configuration fields differ depending on the selected data type.    
For detailed information about the different configurations of data types, see [Data type list](../../PIM/UserInterface/04_DataTypeList.md).


## Edit attribute

*DataHub > Settings > Tab ATTRIBUTES > Select attribute > Tab Data*

![Edit attribute](../../Assets/Screenshots/DataHub/Settings/Attributes/EditAttribute.png "[Edit attribute]")

**Edit attribute**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit attribute* view and return to the attributes list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* and *Description (Language)* fields are displayed. The system languages *English (United States)* and *Deutsch (Deutschland)* are available in the drop-down list.

- [SAVE]   
  Click this button to save the attribute, close the *Edit attribute* view and return to the attributes list.

### Edit attribute &ndash; Data

*DataHub > Settings > Tab ATTRIBUTES > Select attribute > Tab Data*

![Edit attribute](../../Assets/Screenshots/DataHub/Settings/Attributes/EditAttribute.png "[Edit attribute]")

- *Name (Language)*   
  Click the field to edit the attribute name in the selected language.

- *Description (Language)*   
  Click the field to edit the description to the attribute in the selected language.

- *Data type*   
  Attribute data type. In the *Edit attribute* view, this field is locked. For detailed information about all data types, see [Data type list](../../PIM/UserInterface/04_DataTypeList.md).

- *Key*   
  Attribute key. The key is required for API access and must be system wide unique. In the *Edit attribute* view, this field is locked.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Multi-language*   
  Enable this toggle to create a multi-lingual attribute. Disable the toggle to create a single language attribute. In the *Edit attribute* view, this toggle is read-only.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Multi-channel*   
  Enable this toggle to create a multi-channel attribute. Disable the toggle to create a single channel attribute. In the *Edit attribute* view, this toggle is read-only.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Enable this toggle to set the attribute status to active. Disable the toggle to set the status to inactive. By default, this toggle is active.

**CONFIGURATION**

The *CONFIGURATION* section displays the additional configuration for the selected data type. The configuration fields differ depending on the selected data type.    
For detailed information about the different configurations of data types, see [Data type list](../../PIM/UserInterface/04_DataTypeList.md).



### Edit attribute &ndash; Attribute set assignments

*DataHub > Settings > Tab ATTRIBUTES > Select attribute > Tab Attribute set assignments*

![Attribute set assignments](../../Assets/Screenshots/DataHub/Settings/Attributes/EditAttribute_Assignments.png "[Attribute set assignments]")

**Attribute set assignments**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

The list displays all attributes. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Attribute set*   
  Assigned attribute set.


- *Required*   
  Indication whether the attribute is an required field in the attribute set or not:
  - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is required.  
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is optional.


- *Inherited*   
  Indication whether the attribute is an inherited attribute to the attribute set or not:
  - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is inherited.  
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is not inherited.


- *Calculated field*   
  Indication whether the attribute is a calculated field or not:
  - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is a calculated field.   
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is no calculated field.

  [comment]: <> (What means 'Calculated'? completeness calculation? what field are calculated?)