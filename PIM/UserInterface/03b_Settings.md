Attribute set# Attribute Sets

*PIM > Settings > Tab ATTRIBUTE SETS*

![Attribute sets](/Assets/Screenshots/PIM/Settings/AttributeSets/AttributeSets.png "[Attribute sets]")

- [IMPORT]   
  Click this button to import a attribute set and start the import wizard.   
  For detailed information, see [Import a attribute set](to_be_completed).

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a attribute sets.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the table of attribute sets.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attribute sets in the table are selected.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected attribute set. This button is only displayed, when a single checkbox of a attribute set is selected. Alternatively, you can click directly a row in the table to edit a attribute set.
  For detailed information, see [Edit a attribute set](to_be_completed).

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected attribute set. This button is only displayed, when the checkbox of a attribute set is selected.       
  For detailed information, see [Delete a attribute set](to_be_completed).

- [EXPORT]   
  Click this button to export the selected attribute set. The [export wizard](#Export-wizard) is displayed.

The table displays all attribute sets.  All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute set name.

- *Key*   
  Attribute set key.

- *Description*   
  Description to the attribute set.

- *Status*   
  Attribute set status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Read only*   
  Indication whether the attribute set is read-only or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute set is read-only.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute set can be edited.


- *Plugin*   
  ???

- *ID*   
  Attribute set identification number. The ID number is automatically assigned by the system.

- *Modified on*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the attribute set.

- *Created on*   
  Date and time of the creation.

- *Created by*   
  Name and username of the user who created the attribute set.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a attribute set. The *Create Set* view is displayed.   


## Create attribute set
*PIM > Settings > Tab ATTRIBUTE SETS > Button Add*

![Create set](/Assets/Screenshots/PIM/Settings/AttributeSets/CreateSet.png "[Create set]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Status*   
  Activate this toggle to set the attribute set status to active. Deactivate the toggle to set the status to inactive. By default, this toggle is active.

**BASIC DATA**

- *Name*   
  Attribute set name.

- *Description*   
  Description to the attribute set.

- *Key*   
  Attribute set key.


**Inheritance**

- *Inherit/Copy Values from*   
  Click the drop-down list to select whether or not the values for the new attribute set should be inherited or copied from an existing attribute set. The following options are available:    
  - **no inheritance**: The values are neither inherited nor copied from an existing attribute set. The toggle *Inherit Configuration* and the drop-down list *Inherit/Copy Values* are locked.
  - **Attribute set name**: The values inherited or copied from the selected attribute set. All existing attribute sets are displayed in the drop-down list.  


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration*   
  Activate this toggle to inherit not only the values of the selected attribute set, but also their configuration. Deactivate the toggle to inherit the values without configuration. By default, this toggle is active. This toggle is locked if the option **no inheritance** is selected in the drop-down list *Inherit/Copy Values from*.


- *Inherit/Copy Values*   
  Click the drop-down list to select the inheritance type. The following types are available:    
  - **Einmal kopieren**: The attribute values are applied once from the selected attribute set, but afterwards they are independent of changes in the selected set.
  - **Vererben**: The attribute values are applied from the selected attribute set and updated each time if the selected set changes.


- [CANCEL]   
  Click this button to cancel creating a attribute set, close the *Create Set* view and return to the attribute sets list.

- [SAVE]   
  Click this button to save the attribute set, close the *Create Set* view and return to the attribute sets list.


**Attribute List**

In the *Create Set* view, no attributes are displayed in the list on the right side of the view. You have to save the attribute set to edit the attribute list.   

[comment]: <> (Is it right that no attributes are displayed on the right side in the *Create Set* view and that the Add button didn't work?)


## Edit attribute set
*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set*

![Edit set](/Assets/Screenshots/PIM/Settings/AttributeSets/EditSet.png "[Edit set]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Status*   
  Activate this toggle to set the attribute set status to active. Deactivate the toggle to set the status to inactive. By default, this toggle is active.

**BASIC DATA**

- *Name*   
  Attribute set name.

- *Description*   
  Description to the attribute set.

- *Key*   
  Attribute set key. In the *Edit Set* view, this field is locked.


**Inheritance**

- *Inherit/Copy Values from*   
  Click the drop-down list to select whether or not the values for the new attribute set should be inherited or copied from an existing attribute set. The following options are available:    
  - **no inheritance**: The values are neither inherited nor copied from an existing attribute set. The toggle *Inherit Configuration* and the drop-down list *Inherit/Copy Values* are locked.
  - **Attribute set name**: The values inherited or copied from the selected attribute set. All existing attribute sets are displayed in the drop-down list.  


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration*   
  Activate this toggle to inherit not only the values of the selected attribute set, but also their configuration. Deactivate the toggle to inherit the values without configuration. By default, this toggle is active. This toggle is locked if the option **no inheritance** is selected in the drop-down list *Inherit/Copy Values from*.


- *Inherit/Copy Values*   
  Click the drop-down list to select the inheritance type. The following types are available:    
  - **Einmal kopieren**: The attribute values are applied once from the selected attribute set, but afterwards they are independent of changes in the selected set.
  - **Vererben**: The attribute values are applied from the selected attribute set and updated each time if the selected set changes.


- [CANCEL]   
  Click this button to cancel creating a attribute set, close the *Create Set* view and return to the attribute sets list.

- [SAVE]   
  Click this button to save the attribute set, close the *Create Set* view and return to the attribute sets list.

**Attribute List**

- ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings)   
  Click this button to unlock the column *required* in the below table of attributes. The color of the button switches to blue if the column is unlocked. Click the button again to lock the column *required*. The button color switches back to gray.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the table are selected.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected attributes configuration. This button is only displayed, when a single checkbox of an attribute is selected and the configuration can be edited. The *Edit attribute for set* view is displayed. Alternatively, you can click directly a row in the table to edit an attribute configuration.

  [comment]: <> (what attributes configuration can be edited?)

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to remove the selected attribute from the attribute set. This button is only displayed, when the checkbox of an attribute is selected.       

  > [Info] If you remove an attribute from the attribute set, the attribute itself is not deleted, but it is unassigned to the selected attribute set.   

The table displays all attributes assigned to the selected attribute set. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *inherited from*   
  Inheritance attribute set. The name of the attribute set from which the attribute value is inherited is displayed. If the attribute value is not inherited, the row is empty.

- *Plugin*   
  ???

- *required*  
  - Indication whether the attribute value is required or not. The following options are only displayed, when the button ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) is inactive:
    - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute value is required and considered for completeness.
    - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute value is optional.   
  - **![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *required***   
    Activate this toggle to set the attribute value as a mandatory field. Deactivate the toggle to set the attribute value as an optional field. The toggle is only displayed, when the button ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) is active. The toggle is locked when the attribute value is inherited from another attribute set.


- *Read only*   
  Indication whether the attribute value is read-only or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute value is read-only.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute value can be edited.


- *Configuration*   
  Attribute configuration.

- *ID*   
  Attribute identification number. The ID number is automatically assigned by the system.

- *Description*   
  Description to the attribute.

- *Multi-language*   
  Indication whether the attribute is multilingual or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-language.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single language.


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.


### Edit attribute for set

[comment]: <> (Not working anymore?)

*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set > Select attribute*

![Edit Attribute for Set](/Assets/Screenshots/PIM/Settings/AttributeSets/EditAttribute.png "[Edit Attribute for  Set]")

- [CANCEL]   
  Click this button to cancel editing the configuration, close the *Edit Attribute for Set* view and return to the *Edit Set* view.

- [SAVE]   
  Click this button to save the changes, close the *Edit Attribute for Set* view and return to the *Edit Set* view.

**CONFIGURATION**

The *CONFIGURATION* section displays the additional configuration for the data type of the selected attribute. The configuration fields differ depending on the data type of the attribute.    
For detailed information about the different configurations, see [Configuration list](to_be_completed).


## Import wizard
*PIM > Settings > Tab ATTRIBUTE SETS > Button IMPORT*

This wizard helps you to import one or multiple attribute set(s).

### Step 1

![Import wizard step 1](/Assets/Screenshots/PIM/Settings/AttributeSets/Import01.png "[Import wizard step 1]")

This wizard window

- [SELECT FILE]   
  Click this button to select a file for import. The explorer is displayed for file selection. Only .json-files are allowed. The selected file is displayed below the button when uploaded. Alternatively, you can select a file using drag & drop.
  [comment]: <> (Is that right?)

- ![Upload](/Assets/Icons/Upload.png "[Upload]") *Drop file here...*   
  Drag the file from your local folder and drop it in this dashed box to upload it. The background color of the box turns to blue when you can drop the file. Only .json-files are allowed. The selected file is displayed below the button when uploaded. Alternatively, you can select a file using the button [SELECT FILE].

- File box   
  When a file is successfully uploaded, the file box displays the uploaded file name with a checkmark ![Checkmark](/Assets/Icons/Check.png "[Checkmark]") to the left of the file name. You can upload one file only.
  Remove a file by clicking the button ![Remove](/Assets/Icons/Cross04.png "[Remove]") (Remove) to the right of the file name.

- ![Toggle](/Assets/Icons/Toggle.png "[Status]") *Move existing attributes into attribute groups specified in the file*   
  Activate this toggle to assign existing attributes to attribute groups specified in the file. Deactivate the toggle to keep the attribute group structure of the existing attributes. By default, this toggle is inactive.

- [CANCEL]   
  Click this button to cancel the import, close the import wizard window and return to the attribute sets list.

- [CONTINUE]   
  Click this button to proceed to the next step. This button is locked until a file is uploaded. The *Step 2* wizard window is displayed.


### Step 2

![Import wizard step 2](/Assets/Screenshots/PIM/Settings/AttributeSets/Import02.png "[Import wizard step 2]")

This wizard window displays a summary of the import. When the import was successfull, *Import completed* is displayed.

- [CANCEL]   
  Click this button to cancel the import, close the import wizard window and return to the attribute sets list.

- [CONTINUE]   
  Click this button to proceed to the next step. The *Step 3* wizard window is displayed.



## Export wizard
*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set > Button EXPORT*

This wizard helps you to export one or multiple attribute set(s).

### Step 1

![Export wizard step 1](/Assets/Screenshots/PIM/Settings/AttributeSets/Export01.png "[Export wizard step 1]")

This wizard window displays all attributes of the selected attribute set(s) for export.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to exclude the selected attribute from the export. If you click the checkbox in the header, all attributes in the table are selected.

The table displays all attributes assigned to the selected attribute set. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *Description*   
  Description to the attribute.

- *Multi-language*   
  Indication whether the attribute is multilingual or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-language.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single language.


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.

- *Plugin*   
  ???

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


- [CANCEL]   
  Click this button to cancel the export, close the export wizard window and return to the attribute sets list.

- [CONTINUE]   
  Click this button to proceed to the next step. If the selected attribute set for export includes variant sets, the *Step 2* wizard window is displayed. Otherwise, the *Step 2* wizard window is skipped and the *Step 3* wizard window is directly displayed.


### Step 2

![Export wizard step 2](/Assets/Screenshots/PIM/Settings/AttributeSets/Export02.png "[Export wizard step 2]")

This wizard window displays all variant set of the selected attribute set(s) for export. It is only displayed, when the selected attribute set for export includes variant sets.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to exclude the selected variant sets from the export. If you click the checkbox in the header, all variant sets in the table are selected.

The table displays all variant sets included to the selected attribute set for export. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Variant set name.

- *Attribute Set*   
  Attribute set name assigned to the variant set.

- *Attributes (defining)*   
  Defining attributes of the variant set.

- *Attributes (differing)*   
  Differing attributes of the variant set.

- *ID*   
  Attribute set identification number. The ID number is automatically assigned by the system.

- *Modified on*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the variant set.

- *Created on*   
  Date and time of the creation.

- *Created by*   
  Name and username of the user who created the variant set.


- [CANCEL]   
  Click this button to cancel the export, close the import wizard window and return to the attribute sets list.

- [FINALIZE]   
  Click this button to complete the import. The import wizard window is closed and the attribute sets list is displayed.


### Step 3

![Export wizard step 3](/Assets/Screenshots/PIM/Settings/AttributeSets/Export03.png "[Export wizard step 3]")

This wizard window displays several tables summarizing the settings for final export. All fields are read-only.

**The following attributes will be exported**

The table displays all attributes that will be exported. All fields are read-only.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *Description*   
  Description to the attribute.

- *Multi-language*   
  Indication whether the attribute is multilingual or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-language.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single language.


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.

- *Plugin*   
  ???


**The following attributes cannot be exported**

The table displays all attributes that cannot be exported. All fields are read-only. The table is only displayed when at least one attribute cannot be exported.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *Description*   
  Description to the attribute.

- *Multi-language*   
  Indication whether the attribute is multilingual or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-language.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single language.


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.

- *Plugin*   
  ???


**The following attributes are excluded from the export**

The table displays all attributes that you selected to be excluded from the export. All fields are read-only. The table is only displayed when at least one attribute is excluded.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *Description*   
  Description to the attribute.

- *Multi-language*   
  Indication whether the attribute is multilingual or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-language.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single language.


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.

- *Plugin*   
  ???


**The following variant sets will be exported**

The table displays all variant sets that will be exported. All fields are read-only. The table is only displayed when at least one variant set will be excluded.

- *Name*   
  Variant set name.

- *Attribute Set*   
  Attribute set name assigned to the variant set.

- *Attributes (defining)*   
  Defining attributes of the variant set.

- *Attributes (differing)*   
  Differing attributes of the variant set.


**The following variant sets cannot be exported**

The table displays all variant sets that cannot be exported. All fields are read-only. The table is only displayed when at least one variant set cannot be exported.

- *Name*   
  Variant set name.

- *Attribute Set*   
  Attribute set name assigned to the variant set.

- *Attributes (defining)*   
  Defining attributes of the variant set.

- *Attributes (differing)*   
  Differing attributes of the variant set.

[comment]: <> (Does this table exist?)


**The following variant sets are excluded from the export**

The table displays all variant sets that you selected to be excluded from the export. All fields are read-only. The table is only displayed when at least one variant set is excluded.

- *Name*   
  Variant set name.

- *Attribute Set*   
  Attribute set name assigned to the variant set.

- *Attributes (defining)*   
  Defining attributes of the variant set.

- *Attributes (differing)*   
  Differing attributes of the variant set.

- [CANCEL]   
  Click this button to cancel the export, close the export wizard window and return to the attribute sets list.

- [EXPORT]   
  Click this button to start the export. By default, the export file is saved in the local download folder. The export wizard window is closed and the attribute sets list is displayed again.
