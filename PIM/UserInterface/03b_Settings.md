# Attribute Sets

*PIM > Settings > Tab ATTRIBUTE SETS*

![Attribute sets](/Assets/Screenshots/PIM/Settings/AttributeSets/AttributeSets.png "[Attribute sets]")

- [IMPORT]   
  Click this button to import an attribute set and start the import wizard.   
  For detailed information, see [Import an attribute set](/PIM/Integration/02_ManageAttributeSets.md#import-an-attribute-set).

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a attribute sets.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attribute sets.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attribute sets in the list are selected.

- [EXPORT]   
  Click this button to export the selected attribute set. The export wizard window is displayed. This button is only displayed, when the checkbox of at least one attribute set is selected. For detailed information, see [Export an attribute set](/PIM/Integration/02_ManageAttributeSets.md#export-an-attribute-set).

- [EDIT]
  Click this button to edit the selected attribute set. This button is only displayed, when a single checkbox of an attribute set is selected. Alternatively, you can click directly a row in the list to edit a attribute set.
  For detailed information, see [Edit an attribute set](/PIM/Integration/02_ManageAttributeSets.md#edit-an-attribute-set).

- [DELETE]
  Click this button to delete the selected attribute set. This button is only displayed, when the checkbox of at least one attribute set is selected.       

  [comment]: <> (Mostly not possible to delete an attribute set -> no integration procedure to delete an attribute set -> why is the button still existing? Not working... )


The list displays all attribute sets. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute set name.

- *Key*   
  Attribute set key. The key is required for API access and must be system wide unique.

- *Description*   
  Description to the attribute set.

- *Status*   
  Attribute set status. The following statuses are displayed:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Read-only*   
  Indication whether the attribute set is read-only or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute set is read-only.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute set can be edited.


- *Plugin*   
  Module or plugin from which the attribute set is created. In the *PIM* module, only PIM attribute sets are displayed.
  [comment]: <> (Is that correct?)

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

- *Name (Language)*   
  Attribute name in the selected language. One *Name (Language)* column is displayed for the system languages *English (United States)* and *Deutsch (Deutschland)*.

- *Description (Language)*   
  Attribute description in the displayed language. For each active language exists one *Description* column.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a attribute set. The *Create Set* view is displayed.   


## Create attribute set
*PIM > Settings > Tab ATTRIBUTE SETS > Button Add*

![Create attribute set](/Assets/Screenshots/PIM/Settings/AttributeSets/CreateAttributeSet.png "[Create attribute set]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create Attribute Set* view and return to the attribute set list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* and *Description (Language)* fields are displayed. The system languages *English (United States)* and *Deutsch (Deutschland)* are available in the drop-down list.
  [comment]: <> (Is that right? -> language question)

- [SAVE]   
  Click this button to save the attribute set, close the *Create Attribute Set* view and return to the attribute set list.

- *Name (Language)*   
  Attribute set name in the selected language.

- *Description (Language)*   
  Description to the attribute set in the selected language.

- *Key*   
  Attribute set key. The key is required for API access and must be system wide unique.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Activate this toggle to set the attribute set status to active. Deactivate the toggle to set the status to inactive. By default, this toggle is active.


- *Inherit/Copy Values from*   
  Click the drop-down list to select whether or not the values for the new attribute set should be inherited or copied from an existing attribute set. The following options are available:    
  - **No inheritance**: The values are neither inherited nor copied from an existing attribute set. The *Inherit Configuration* toggle and the *Inherit/Copy Values* drop-down list are locked.
  - **Attribute set name**: The values inherited or copied from the selected attribute set. All existing attribute sets are displayed in the drop-down list.  


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration*   
  Activate this toggle to inherit not only the values of the selected attribute set, but also their configuration. Deactivate the toggle to inherit the values without configuration. By default, this toggle is active. This toggle is locked if the **no inheritance** option is selected in the *Inherit/Copy Values from* drop-down list.


- *Inherit/Copy Values*   
  Click the drop-down list to select the inheritance type. The following types are available:    
  - **Copy once**: The attribute values are applied once from the selected attribute set, but afterwards they are independent of changes in the selected set.
  - **Inherit**: The attribute values are applied from the selected attribute set and updated each time if the selected set changes.


**Assigned Attributes**

- ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings)   
  Click this button to unlock the *required* column in the attributes list. The color of the button switches to blue if the column is unlocked. Click the button again to lock the *required* column. The button color switches back to gray.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the list are selected.

In the *Create Attribute Set* view, no attributes are displayed in list. You have to save the attribute set to edit the assigned attributes.   


## Edit attribute set
*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set*

![Edit attribute set](/Assets/Screenshots/PIM/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Attribute Set* view and return to the attribute set list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* and *Description (Language)* fields are displayed. The system languages *English (United States)* and *Deutsch (Deutschland)* are available in the drop-down list.
  [comment]: <> (Is that right? -> language question)

- [SAVE]   
  Click this button to save the attribute set, close the *Edit Attribute Set* view and return to the attribute set list.

- *Name (Language)*   
  Attribute set name in the selected language.

- *Description (Language)*   
  Description to the attribute set in the selected language.

- *Key*   
  Attribute set key. The key is required for API access and must be system wide unique. In the *Edit Attribtue Set* view, this field is locked.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Activate this toggle to set the attribute set status to active. Deactivate the toggle to set the status to inactive. By default, this toggle is active.


- *Inherit/Copy Values from*   
  Click the drop-down list to select whether or not the values for the new attribute set should be inherited or copied from an existing attribute set. The following options are available:    
  - **No inheritance**: The values are neither inherited nor copied from an existing attribute set. The *Inherit Configuration* toggle and the *Inherit/Copy Values* drop-down list are locked.
  - **Attribute set name**: The values inherited or copied from the selected attribute set. All existing attribute sets are displayed in the drop-down list.  


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Inherit Configuration*   
  Activate this toggle to inherit not only the values of the selected attribute set, but also their configuration. Deactivate the toggle to inherit the values without configuration. By default, this toggle is active. This toggle is locked if the **no inheritance** option is selected in the *Inherit/Copy Values from* drop-down list.


- *Inherit/Copy Values*   
  Click the drop-down list to select the inheritance type. The following types are available:    
  - **Copy once**: The attribute values are applied once from the selected attribute set, but afterwards they are independent of changes in the selected set.
  - **Inherit**: The attribute values are applied from the selected attribute set and updated each time if the selected set changes.

> [Info] For the *PIM Basic Set* which is predefined by the system, the inheritance settings are read-only.


**Assigned Attributes**

- ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings)   
  Click this button to unlock the *required* column in the attributes list. The color of the button switches to blue if the column is unlocked. Click the button again to lock the *required* column. The button color switches back to gray.

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all attributes in the list are selected.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the configuration of the selected attribute. This button is only displayed, when a single checkbox of an attribute with an editable configuration is selected. The *Edit attribute for set* view is displayed. Alternatively, you can click directly a row in the list to edit an attribute configuration.

[comment]: <> (Not working)

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to remove the selected attribute from the attribute set. This button is only displayed, when at least one checkbox of an attribute is selected.       

  > [Info] If you remove an attribute from the attribute set, the attribute itself is not deleted, but it is unassigned to the selected attribute set.   

- [ADD MAPPING]   
  Click this button to add a mapping to the selected attribute. The *Add mapping* view is displayed. You can only add a mapping for attribute sets that are not inherited from another attribute set. This button is only displayed, when a single checkbox of an attribute is selected.


The list displays all attributes assigned to the selected attribute set. When the ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) button is gray, all fields are read-only.  When the ![Settings](/Assets/Icons/Settings02.png "[Settings]") (Settings) button is blue, the field *required* is editable. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Calculated Field*   
  Indication whether the attribute is an calculated field or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is ???.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is ???.

- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data type list](04_DataTypeList.md).

- *inherited from*   
  Inheritance attribute set. The name of the attribute set from which the attribute value is inherited is displayed. If the attribute value is not inherited, the row is empty.

- *Plugin*   
  Module or plugin from which the attribute is created. In the *PIM* module, only PIM attributes are displayed.
  [comment]: <> (Is that correct?)


- *Required*   
  Indication whether the attribute is an required field in the attribute set or not.
  When the ![Settings](/Assets/Icons/Settings02.png "[Settings]") (Settings) button is blue, the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *required* toggle is displayed. Activate the toggle to set the attribute value as a mandatory field. Deactivate the toggle to set the attribute value as an optional field.   
  When the ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) button is gray, the following options are displayed:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is required.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is optional.   


- *Read-only*   
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


- *Multi-scope*   
  Indication whether the attribute is multi-scope or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-scope.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single scope.


### Edit attribute for set

[comment]: <> (Not working anymore?)

*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set > Select attribute with configuration*

![Edit Attribute for Set](/Assets/Screenshots/PIM/Settings/AttributeSets/EditAttribute.png "[Edit Attribute for Set]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Attribute for Set* view and return to *Edit Attribute Set* view. All changes are rejected.

- [CANCEL]   
  Click this button to cancel editing the configuration, close the *Edit Attribute for Set* view and return to the *Edit Attribute Set* view.

- [SAVE]   
  Click this button to save the changes, close the *Edit Attribute for Set* view and return to the *Edit Attribute Set* view.

**CONFIGURATION**

The *CONFIGURATION* section displays the additional configuration for the data type of the selected attribute. The configuration fields differ depending on the data type of the attribute.    
For detailed information about the different configurations, see [Configuration list](to_be_completed).


### Add mapping

*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set > Select attribute checkbox > Button ADD MAPPING*

![Add mapping](/Assets/Screenshots/PIM/Settings/AttributeSets/AddMapping.png "[Add mapping]")

**Add Mapping**

This view equals to the attribute mapping in the *DataHub* module: *DataHub > Settings > Tab ETL > Select attribute set mapping > Select mapping line*   

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Mapping* view and return to *Edit Attribute Set* view. All changes are rejected.

- Destination attribute   
  Selected attribute on the right side of the view. The attribute cannot be changed.

- *Language*   
  Language of the destination attribute. The drop-down list is read-only. The drop-down list is only displayed when the destination attribute is multilingual.

- *Scope*   
  Scope of the destination attribute. The drop-down list is read-only. The drop-down list is only displayed when the destination attribute is multi-scope.

- *Extension*   
  Click the drop-down list and select the desired ETL extension for the mapping. The extensions in the list differ depending on the data type of the destination attribute.

- *Override Changetrackingmode*   
  Change tracking mode (ETL mode) for the mapping. The drop-down list is read-only. The option **use default** is preset.

The fields on the left side differ depending on the selected ETL extension. For detailed information about the ETL extensions and how to create an attribute mapping, see [ETL extensions](to_be_completed) and [Create a mapping](to_be_completed).


**Configuration**

The *CONFIGURATION* section displays the additional configuration settings. The configuration fields differ depending on the data type of the source and/or destination attribute.    
For detailed information about the different configurations of data types, see [Data type list](04_DataTypeList.md).

----------

[comment]: <> (Import/Export will be changed)

## Import wizard
*PIM > Settings > Tab ATTRIBUTE SETS > Button IMPORT*

This wizard helps you to import one or multiple attribute set(s).

### Import wizard - Step 1

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


### Import wizard - Step 2

![Import wizard step 2](/Assets/Screenshots/PIM/Settings/AttributeSets/Import02.png "[Import wizard step 2]")

This wizard window displays a summary of the import. When the import was successfull, *Import completed* is displayed.

- [CANCEL]   
  Click this button to cancel the import, close the import wizard window and return to the attribute sets list.

- [CONTINUE]   
  Click this button to proceed to the next step. The *Step 3* wizard window is displayed.



## Export wizard
*PIM > Settings > Tab ATTRIBUTE SETS > Select attribute set > Button EXPORT*

This wizard helps you to export one or multiple attribute set(s).

### Export wizard - Step 1

![Export wizard step 1](/Assets/Screenshots/PIM/Settings/AttributeSets/Export01.png "[Export wizard step 1]")

This wizard window displays all attributes of the selected attribute set(s) for export.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to exclude the selected attribute from the export. If you click the checkbox in the header, all attributes in the list are selected.

The list displays all attributes assigned to the selected attribute set. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data type list](04_DataTypeList.md).

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
  Module or plugin from which the attribute is created. In the *PIM* module, only PIM attributes are displayed.
  [comment]: <> (Is that correct?)

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


### Export wizard - Step 2

![Export wizard step 2](/Assets/Screenshots/PIM/Settings/AttributeSets/Export02.png "[Export wizard step 2]")

This wizard window displays all variant set of the selected attribute set(s) for export. It is only displayed, when the selected attribute set for export includes variant sets.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to exclude the selected variant sets from the export. If you click the checkbox in the header, all variant sets in the list are selected.

The list displays all variant sets included to the selected attribute set for export. All fields are read-only. Depending on the settings, the displayed columns may vary.

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


### Export wizard - Step 3

![Export wizard step 3](/Assets/Screenshots/PIM/Settings/AttributeSets/Export03.png "[Export wizard step 3]")

This wizard window displays several lists summarizing the settings for final export. All fields are read-only.

**The following attributes will be exported**

The list displays all attributes that will be exported. All fields are read-only.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data type list](04_DataTypeList.md).

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
  Module or plugin from which the attribute is created. In the *PIM* module, only PIM attributes are displayed.
  [comment]: <> (Is that correct?)


**The following attributes cannot be exported**

The list displays all attributes that cannot be exported. All fields are read-only. The list is only displayed when at least one attribute cannot be exported.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data type list](04_DataTypeList.md).

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
  Module or plugin from which the attribute is created. In the *PIM* module, only PIM attributes are displayed.
  [comment]: <> (Is that correct?)


**The following attributes are excluded from the export**

The list displays all attributes that you selected to be excluded from the export. All fields are read-only. The list is only displayed when at least one attribute is excluded.

- *Name*   
  Attribute name.

- *Status*   
  Attribute status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Key*   
  Attribute key. The key is required for API access and must be system wide unique.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data type list](04_DataTypeList.md).

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
  Module or plugin from which the attribute is created. In the *PIM* module, only PIM attributes are displayed.
  [comment]: <> (Is that correct?)


**The following variant sets will be exported**

The list displays all variant sets that will be exported. All fields are read-only. The list is only displayed when at least one variant set will be excluded.

- *Name*   
  Variant set name.

- *Attribute Set*   
  Attribute set name assigned to the variant set.

- *Attributes (defining)*   
  Defining attributes of the variant set.

- *Attributes (differing)*   
  Differing attributes of the variant set.


**The following variant sets cannot be exported**

The list displays all variant sets that cannot be exported. All fields are read-only. The list is only displayed when at least one variant set cannot be exported.

- *Name*   
  Variant set name.

- *Attribute Set*   
  Attribute set name assigned to the variant set.

- *Attributes (defining)*   
  Defining attributes of the variant set.

- *Attributes (differing)*   
  Differing attributes of the variant set.

[comment]: <> (Does this list exist?)


**The following variant sets are excluded from the export**

The list displays all variant sets that you selected to be excluded from the export. All fields are read-only. The list is only displayed when at least one variant set is excluded.

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
