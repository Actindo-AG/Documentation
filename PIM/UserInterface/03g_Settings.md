# Variant Sets

*PIM > Settings > Tab VARIANT SETS*

![Variant sets](/Assets/Screenshots/PIM/Settings/VariantSets/VariantSets.png "[Variant sets]")

**Variant Sets**

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an variant set.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of variant sets.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all variant sets in the list are selected.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected variant set. This button is only displayed, when a single checkbox of a variant set is selected. Alternatively, you can click directly a row in the list to edit a variant set. The *Edit variant set* view is displayed.
  For detailed information, see [Edit a variant set](to_be_completed).

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)   
  Click this button to delete the selected variant sets. This button is only displayed, when the checkbox of at least one variant set is selected.       
  For detailed information, see [Delete a variant set](to_be_completed).

The list displays all variant sets.  All fields are read-only. Depending on the settings, the displayed columns may vary.

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

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a variant set. The *Create variant Set* window is displayed.   


## Create variant set
*PIM > Settings > Tab VARIANT SETS > Button Add*

![Create variant set](/Assets/Screenshots/PIM/Settings/VariantSets/CreateVariantSet.png "[Create variant set]")

- *Attribute Set*   
  Click the drop-down list to select the assigned attribute set. All attribute sets are displayed in the drop-down list.

- *Name*   
  Enter the new variant set name.

- [CANCEL]   
  Click this button to cancel creating a variant set, close the *Create variant Set* window and return to the variant sets list.

- [ADD VARIANT SET]   
  Click this button to add the variant set. The *Edit variant set* view is displayed.



## Edit variant set
*PIM > Settings > Tab VARIANT SETS > Button Add > Button Add variant set*   
*PIM > Settings > Tab VARIANT SETS > Select variant set > Button Edit*

![Edit variant set](/Assets/Screenshots/PIM/Settings/VariantSets/EditVariantSet.png "[Edit variant set]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to cancel editing the variant set, close the *Edit variant set* view and return to the variant sets list.

- [CANCEL]   
  Click this button to cancel editing the variant set, close the *Edit variant set* view and return to the variant sets list.

- [SAVE]   
  Click this button to save the variant set, close the *Edit variant set* view and return to the variant sets list.

**BASIC DATA**

- *Name*   
  Click the field to edit the variant set name.


**FORMULAS**

- *Formula for sku*   
  Click the field to edit the formula for the SKU of the variant articles. By default, the formula **{master}-{L}** is predefined. The following placeholders are available:
  - {master}: SKU number of the master entity
  - {L}: consecutive number   
  - In addition to these default placeholders, you can include value of the defining attributes of the variant set into the SKU formula. The corresponding placeholders are displayed when you have added a defining attribute.

- *Attribute Set*   
  Click the drop-down list to change the assigned attribute set. All attribute sets are displayed in the drop-down list. The drop-down list is locked and cannot be changed once you have saved the variant set.

**VARIANTS**

**Attributes (defining)**

- [ADD]   
  Click this button to add a defining attribute to the variant set. The *Defining Attributes* window is displayed.

The list displays all defining attributes to the variant set. All fields are read-only.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected attribute from the box. This button is only displayed, when you hover over an attribute in the box.

**Attributes (differing)**

- [ADD]   
  Click this button to add a differing attribute to the variant set. The *Attributes* window is displayed.

The list displays all differing attributes to the variant set. All fields are read-only.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the selected attribute from the box. This button is only displayed, when you hover over an attribute in the box.


### Defining attributes
*PIM > Settings > Tab VARIANT SETS > Button Add > Button Add variant set > Button Add (defining attributes)*   
*PIM > Settings > Tab VARIANT SETS > Select variant set > Button Edit > Button Add (defining attributes)*

![Defining attributes](/Assets/Screenshots/PIM/Settings/VariantSets/DefiningAttributes.png "[Defining attributes]")

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. Alternatively, you can click directly a row in the list to select the attribute. If you click the checkbox in the header, all attributes in the list are selected.

- [Add x defining attributes to set]   
  Click this button to add the selected attribute(s) to the variant set. This button is only displayed, when the checkbox of an attribute is selected. The *x* in the button indicates the number of selected attributes. The *Defining Attributes* window is closed. The defining attributes are displayed in the box *Attributes (defining)*.

The list displays all available defining attributes. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *ID*   
  Attribute identification number. The ID number is automatically assigned by the system.


### Attributes
*PIM > Settings > Tab VARIANT SETS > Button Add > Button Add variant set > Button Add (differing attributes box)*   
*PIM > Settings > Tab VARIANT SETS > Select variant set > Button Edit > Button Add (differing attributes box)*

![Differing attributes](/Assets/Screenshots/PIM/Settings/VariantSets/Attributes.png "[Differing attributes]")

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an attribute.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of attributes.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. Alternatively, you can click directly a row in the list to select the attribute. If you click the checkbox in the header, all attributes in the list are selected.

- [Add x differing attributes to set]   
  Click this button to add the selected attribute(s) to the variant set. This button is only displayed, when the checkbox of an attribute is selected. The *x* in the button indicates the number of selected attributes. The *Attributes* window is closed. The differing attributes are displayed in the box *Attributes (differing)*.

The list displays all available defining attributes. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*   
  Attribute name.

- *Key*   
  Attribute key.

- *Data Type*   
  Attribute data type. For detailed information about all data types, see [Data types list](to_be_completed).

- *ID*   
  Attribute identification number. The ID number is automatically assigned by the system.
