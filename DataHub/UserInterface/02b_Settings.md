# Attribute Sets

*DataHub > Settings > Tab ATTRIBUTE SETS*

![Attribute sets](/Assets/Screenshots/DataHub/Settings/AttributeSets/AttributeSets.png "[Attribute sets]")

- [IMPORT]   
  Click this button to import an attribute set and start the import wizard.   
  For detailed information, see [Import an attribute set](/DataHub/Integration/02_ManageAttributeSets.md#import-an-attribute-set).

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
  Click this button to export the selected attribute set. The export wizard window is displayed. This button is only displayed, when the checkbox of at least one attribute set is selected. For detailed information, see [Export an attribute set](/DataHub/Integration/02_ManageAttributeSets.md#export-an-attribute-set).

- [EDIT]
  Click this button to edit the selected attribute set. This button is only displayed, when a single checkbox of an attribute set is selected. Alternatively, you can click directly a row in the list to edit a attribute set.
  For detailed information, see [Edit an attribute set](/DataHub/Integration/02_ManageAttributeSets.md#edit-an-attribute-set).

- [DELETE]
  Click this button to delete the selected attribute set. This button is only displayed, when the checkbox of at least one attribute set is selected.       

  [comment]: <> (Mostly not possible to delete an attribute set -> no integration procedure to delete an attribute set -> why is the button still existing? Not working... )

The list displays all attribute sets. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Product type name.

- *Key*   
  Product type key.

- *Description*   
  Description to the attribute set.

- *Status*   
  Product type status. The following statuses are available:
  - ![Status](/Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](/Assets/Icons/Status04.png "[Status]") **Inactive**   


- *Read only*   
  Indication whether the attribute set is read-only or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute set is read-only.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute set can be edited.


- *Plugin*   
  Module or plugin from which the attribute set is created.

- *ID*   
  Product type identification number. The ID number is automatically assigned by the system.

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
  Click this button to create an attribute set. The *Create Set* view is displayed.   


## Create attribute set
*DataHub > Settings > Tab ATTRIBUTE SETS > Button Add*

![Create attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/CreateAttributeSet.png "[Create attribute set]")

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

- *Entity Type*   
  Click the drop-down list to select the appropriate entity type. All available entity types are displayed in the list. For detailed information, see [Entity Types List](to_be_completed).  

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
*DataHub > Settings > Tab ATTRIBUTE SETS > Select attribute set*

![Edit attribute set](/Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttributeSet.png "[Edit attribute set]")

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
  Module or plugin from which the attribute is created.

  [comment]: <> (Is that correct?)

- *required*  
  Indication whether the attribute value is required or not. The following options are only displayed, when the ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings) button is inactive:
  When the ![Settings](/Assets/Icons/Settings02.png "[Settings]") (Settings) button is blue, the *required* toggle is displayed. Activate the toggle to set the attribute value as a mandatory field. Deactivate the toggle to set the attribute value as an optional field.   
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


- *Multi-channel*   
  Indication whether the attribute is multi-channel or not:
  - ![Check](/Assets/Icons/Check.png "[Check]") (Checkmark): The attribute is multi-channel.  
  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross): The attribute is single channel.



### Edit attribute for set

[comment]: <> (Not working anymore? Bild fehlt)

*DataHub > Settings > Tab ATTRIBUTE SETS > Select attribute set > Select attribute*

![Edit Attribute for Set](/Assets/Screenshots/DataHub/Settings/AttributeSets/EditAttribute.png "[Edit Attribute for  Set]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Attribute for Set* view and return to *Edit Attribute Set* view. All changes are rejected.

- [CANCEL]   
  Click this button to cancel editing the configuration, close the *Edit Attribute for Set* view and return to the *Edit Attribute Set* view.

- [SAVE]   
  Click this button to save the changes, close the *Edit Attribute for Set* view and return to the *Edit Attribute Set* view.

**CONFIGURATION**

The *CONFIGURATION* section displays the additional configuration for the data type of the selected attribute. The configuration fields differ depending on the data type of the attribute.    
For detailed information about the different configurations of data types, see [Data type list](/PIM/UserInterface/04_DataTypeList.md).


### Add mapping

*DataHub > Settings > Tab ATTRIBUTE SETS > Select attribute set > Select attribute checkbox > Button ADD MAPPING*

![Add mapping](/Assets/Screenshots/DataHub/Settings/AttributeSets/AddMapping.png "[Add mapping]")

**Add Mapping**

This view equals to the attribute mapping in the *DataHub* module: *DataHub > Settings > Tab ETL > Select attribute set mapping > Select mapping line*   

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Mapping* view and return to *Edit Attribute Set* view. All changes are rejected.

- Destination attribute   
  Selected attribute on the right side of the view. The attribute cannot be changed.

- *Language*   
  Language of the destination attribute. The drop-down list is read-only. The drop-down list is only displayed when the destination attribute is multilingual.

- *Channel*   
  Channel of the destination attribute. The drop-down list is read-only. The drop-down list is only displayed when the destination attribute is multi-channel.

- *Extension*   
  Click the drop-down list and select the desired ETL extension for the mapping. The extensions in the list differ depending on the data type of the destination attribute.

- *Override Changetrackingmode*   
  Change tracking mode (ETL mode) for the mapping. The drop-down list is read-only. The option **use default** is preset.

The fields on the left side differ depending on the selected ETL extension. For detailed information about the ETL extensions and how to create an attribute mapping, see [ETL extensions](03_ETLExtensions.md) and [Edit an ETL attribute mapping](/DataHub/Operation/01_ManageETLMappings.md#edit-an-etl-attribute-mapping).


**Configuration**

The *CONFIGURATION* section displays the additional configuration settings. The configuration fields differ depending on the data type of the source and/or destination attribute.    
For detailed information about the different configurations of data types, see [Data type list](/PIM/UserInterface/04_DataTypeList.md).
