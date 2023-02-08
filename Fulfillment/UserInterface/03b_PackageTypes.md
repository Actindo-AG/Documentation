# Package types

*Fulfillment > Settings > Tab PACKAGE TYPES*

![List of package types](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/ListPackageTypes.png "[List of package types]")

[comment]: <> (HG: Screenshot aus NoE Test Account. OK oder lieber aus Sandbox?)

**List of package types**

- *VIEW*  
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

        - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
            Click this entry to create a view. The *Create view* window is displayed, see [Create view](#create-view).

        - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
            Click this entry to rename the selected view. The *Rename view* window is displayed, see [Rename view](#rename-view). This menu entry is only displayed if a view has been selected.

        - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset  
            Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

        - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish  
            Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

        - ![Unpublish](../../Assets/Icons/Unpublish.png "[Unpublish]") unpublish  
            Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

        - ![Save](../../Assets/Icons/Save.png "[Save]") save  
            Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

            > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

        - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete  
            Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed if a view has been selected.


- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for package types.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of package types.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar.

- [EDIT]  
    Click this button to edit the selected package type. This button is only displayed if a single checkbox in the list of package types is selected. Alternatively, you can click directly a row in the list to edit a package type. The *Edit package type* view is displayed.

- [DELETE]  
    Click this button to delete one or several selected package types.

The list displays all package types. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *ID*  
    Package type identification number. The ID number is automatically assigned by the system.

- *Name*  
    Package type name.

- *Active*  
    Package type status. The following statuses are displayed:
  - ![Status](../../Assets/Icons/Check.png "[Status]") (Checkmark): The package type is active.
  - ![Status](../../Assets/Icons/Cross02.png "[Status]") (Cross): The package type is inactive.

- *Connection*  
    Connection name.

- *Connection ID*  
    Connection identification number. The ID number is automatically assigned by the system.

- *Max height*  
    Maximal height configured for the package type.

- *Max width*  
    Maximal width configured for the package type.

- *Max weight*  
    Maximal weight configured for the package type.

- *Max value*  
    Maximal value configured for the package type.

- *Carrier*   
    Carrier configured for the package type.  

- *Express*  
    Indication of the configured shipping type. The following options are displayed:  
    - **Yes**: Express shipping type
    - **No**: Standard shipping type

- *Package type identifier*  
    Package type configured for the shipment.  

- *Ship-to country*  
    Country where the package type is shipped to.

- *Priority*  
    Indication of the priority configured for the package type. The priority value is used by the system to determine the package type to be used for a shipment when two or more package types have the same criteria. The lower the number, the higher the priority.

- *Additional services (shipping method)*  
    Additions services offered as defined by the user. Numbers, letters or a combination of characters can be used. 

- *Attribute*    
    You can add an additional column for each attribute that is assigned to the package type. The column displays the attribute name, the row displays the corresponding attribute value of the package type.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)  
  Click this button to add a connection. The *Create connection* view is displayed, see [Create package type](#create-package-type).
  

## Create package type  

*Fulfillment > Settings > Tab PACKAGE TYPES > Button Add*

![Create view](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/CreatePackageType.png "[Create view]")

[comment]: <> (Screenshot evtl. ändern, Actindo Basic kommt nicht bei NoE vor)

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Create package type* view and return to the list of package types. All changes are rejected.

- *Channel*  
    Click the drop-down list to select the channel. All available channels are displayed in the drop-down list. By default, the Actindo Basic channel is preselected.

[comment]: <> (Was ist Actindo Basic? Channel? Attribute Set? Group? Fulfillment Packaging Type Base Attributes? Standard?)

- *Language*      
    Click the drop-down list and select the language in which the fields are displayed. All available languages are displayed. By default, the language set up in the system is preselected.

- [SAVE]   
    Click this button to save the package type, close the *Create package type* view and return to the list of package types.

- *Name*  
    Enter a package type name.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
    Enable this toggle to set the package type status to active. Disable the toggle to set the status to inactive. By default, this toggle is disabled.

- *Connection*  
    Click the drop-down list and select the desired connection. All available connections are displayed.

- *Max height*  
    Maximal height allowed for the package type.
  - *Quantity*  
    Enter the desired value.
  - *Unit*  
    Click the drop-down list and select the applicable unit.

- *Max width*   
  Maximal width allowed for the package type.
  - *Quantity*  
    Enter the desired value.
  - *Unit*  
    Click the drop-down list and select the applicable unit.

- *Max weight*  
  Maximal weight allowed for the package type.
  - *Quantity*  
    Enter the desired value.
  - *Unit*  
    Click the drop-down list and select the applicable unit.

- *Max value*  
  If desired, the maximal monetary value allowed for the package type can be configured.
  - [ADD PRICE]  
    Click this button to enter the base price and scale prices. The *Edit price* window is displayed, see [Edit price](#edit-price).
  - *Base price*  
    Base price defined for the product. This field is read-only and can only be edited in the *Edit price* window.
  - *Current price range*  
    Price range defined for the product. This field is read-only and can only be edited in the *Edit price* window.
  - *# Scale prices*  
    Number of scale prices defined for the product. This field is read-only and can only be edited in the *Edit price* window.
  - ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit)  
  Click this button to edit a configured price. This button is displayed when hovering the mouse over a configured price. The *Edit price* window is displayed, see [Edit price](#edit-price).
  - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)  
  Click this button to deleted the configured price. This button is displayed when hovering the mouse over a configured price.

[comment]: <> (Stimmt das so? Button SAVE funktioniert nicht.)

- *Carrier*  
    Enter the preferred carrier for the package type. Numbers, letters or a combination of characters can be used.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Express*  
    Enable this toggle to set the shipping type for the package type to express. Disable the toggle to set the shipping type for the package type to standard. By default, this toggle is disabled.  

- *Package type identifier*  
    Enter the package type identifier. Numbers, letters or a combination of characters can be used.

- *Ship-to country*  
    Click the drop-down list and select the country where the package type is shipped to.

- *Priority*  
    Enter a number to set the priority for the package type.

- *Additional services (shipping method)*  
    Enter the additional services offered. Numbers, letters or a combination of characters can be used.


## Edit package type

*Fulfillment > Settings > Tab PACKAGE TYPES > Select package type*

![Edit package type](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/EditPackageType.png "[Edit package type]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Edit package type* view and return to the list of package types. All changes are rejected.

- *Channel*  
    Click the drop-down list to select the channel. All available  are displayed in the drop-down list. By default, the *Actindo Basic* channel is preselected.

- *Language*      
    Click the drop-down list and select a different language in which the fields are displayed. All available languages are displayed. By default, the language set up in the system is preselected.  

- [SAVE]   
    Click this button to save any changes made to the package type, close the *Edit package type* view and return to the list of package types.

- *Name*  
    Click this field to edit the package type name.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
    Enable this toggle to set the package type status to active. Disable the toggle to set the status to inactive.

- *Connection*  
    Click the drop-down list and select the applicable connection. All available connections are displayed.

- *Max height*  
    Click these fields to edit the maximal height allowed for the package type.
  - *Quantity*  
    Click this field to edit the desired value.
  - *Unit*  
    Click the drop-down list and select the applicable unit.

- *Max width*   
    Click these fields to edit the maximal width allowed for the package type.
  - *Quantity*  
    Click this field to edit the desired value.
  - *Unit*  
    Click the drop-down list and select the applicable unit.

- *Max weight*  
    Click these fields to edit the maximal weight allowed for the package type.
  - *Quantity*  
    Click this field to edit the desired value.
  - *Unit*  
    Click the drop-down list and select the applicable unit.

- *Max value*  
    If desired, the maximal monetary value allowed for the package type can be edited.
  - [ADD PRICE]  
    Click this button to edit the base price and scale prices. The *Edit price* window is displayed, see [Edit price](#edit-price_1).
  - *Base price*  
    Base price defined for the product. This field is read-only and can only be edited in the *Edit price* window.
  - *Current price range*  
    Price range defined for the product. This field changes automatically when the scale prices are edited in the *Edit price* window.
  - *No. scale prices*  
    Number of scale prices defined for the product. This field is read-only and can only be edited in the *Edit price* window.  
  - ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit)  
  Click this button to edit a configured price. This button is displayed when hovering the mouse over a configured price.
  - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)  
  Click this button to deleted the configured price. This button is displayed when hovering the mouse over a configured price.

- *Carrier*  
    Click this field to edit the preferred carrier. Numbers, letters or a combination of characters can be used.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Express*  
    Enable this toggle to set the shipping type for the package type to express. Disable the toggle to set the shipping type for the package type to standard.   

- *Package type identifier*  
    Click this field to edit the package type identifier. Numbers, letters or a combination of characters can be used.

- *Ship-to country*  
    Click the drop-down list and select the country where the package type is shipped to.

- *Priority*  
    Click this field to edit the priority for the package type.

- *Additional services (shipping method)*  
    Click this field to edit the additional services offered. Numbers, letters or a combination of characters can be used.

### Edit price

*Fulfillment > Settings > Tab PACKAGE TYPES > Button Add > Button ADD PRICE*  

*Fulfillment > Settings > Tab PACKAGE TYPES > Select package type > Button Edit*

![Edit price](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/EditPrice.png "[Edit price]")

**BASE PRICE CALCULATION**

- *Base price*    
    Enter a base price for the product.

**Scale prices**

- *Price*  
    Scale price defined for the product. This field is read-only and can only be edited in the *Edit scale price* window. If no scale price has been added yet, the *No data* notice is displayed.
- *From*  
    Quantity value applicable to scale price. This field is read-only and can only be edited in the *Edit scale price* window. If no scale price has been added yet, the *No data* notice is displayed.

- [ADD SCALE PRICE]   
    The *Edit scale price* window is displayed, see [Edit scale price](#edit-scale-price).

- [CANCEL]  
    Click this button to cancel editing a price. The *Edit price* window is closed.

- [SAVE]  
    Click this button to save the price, close the *Edit price* window and return to the *Create package type* view.

#### Edit scale price

*Fulfillment > Settings > Tab PACKAGE TYPES > Button Add > Button ADD PRICE > Button ADD SCALE PRICE*  

*Fulfillment > Settings > Tab PACKAGE TYPES > Select package type > Button Edit > Button ADD SCALE PRICE*

![Edit scale price](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/EditScalePrice.png "[Edit scale price]")

- *Price*  
    Enter a price value.
- *From*  
    Enter a quantity value applicable to the scale price.


- [CANCEL]  
    Click this button to cancel editing a scale price. The *Edit scale price* window is closed.

- [SAVE]  
    Click this button to save the scale price, close the *Edit scale price* window and return to the *Edit price* window.


## Create view

*Fulfillment > Settings > Tab PACKAGE TYPES > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Fulfillment/DispatchNotes/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./01a_List.md#create-view).


## Rename view

*Fulfillment > Settings > Tab PACKAGE TYPES > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Fulfillment/DispatchNotes/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./01a_List.md#rename-view).

