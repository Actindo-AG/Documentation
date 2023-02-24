[!!Configure the orders and returns](../Integration/04_ConfigureOrdersReturns.md)
[!!Manage the orders and returns](../Operation/04_ManageOrdersReturns.md)

[comment]: <> (Add link to Order management if available)

# Orders

*Omni-Channel > Orders and returns > Tab ORDERS*

![Orders](../../Assets/Screenshots/Channels/OrdersReturns/Orders/Orders.png "[Orders]")

**Orders**

- *Combined status*  
    Combined status of all orders. The following statuses are available:
    - ![red](../../Assets/Icons/Status02.png "[red]") (red)  
        At least one order is faulty. Click the [>> more] button right to the status to switch to the *ERRORS* tab, see [User interface Errors (Orders and returns)](./05c_Errors.md).   
    - ![yellow](../../Assets/Icons/Status05.png "[yellow]") (yellow)  
        At least one orders is still pending.
    - ![green](../../Assets/Icons/Status03.png "[green]") (green)  
        All orders are completed.

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an order.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of orders.

- *VIEW*   
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *VIEW* drop-down list to display the context menu. The following menu entries are available:

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

- *All Connections*    
    Click the drop-down list to select a connection. All available connections are displayed in the list. When a connection has been selected, the [Import orders] button, the *Download orders automatically* drop-down list and the [SAVE] button are displayed.

- [Import orders for all connections]  
    Click this button to import the orders for all connections. This button is only displayed if no connection has been selected in the *All connections* drop-down list.

- [Import orders]  
    Click this button to import all orders for the selected connection. This button is only displayed if a connection has been selected in the *All connections* drop-down list.

- [Download orders automatically]  
    Click the drop-down list and select the desired time interval for the automatic download of orders. This drop-down list is only displayed if a connection has been selected in the *All connections* drop-down list. The following options are available:
    - **never**
    - **every 2 minutes**
    - **every 5 minutes**
    - **every 10 minutes**
    - **every 15 minutes**
    - **every 20 minutes**
    - **every 30 minutes**
    - **every 60 minutes**

- [SAVE]  
    Click this button to save the settings for the automatic download of orders. This button is only displayed if a connection has been selected in the *All connections* drop-down list.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all orders in the list are selected.

- [VIEW]  
    Click this button to display the *Order from connection "Connection name"* view of the selected order. Alternatively, you can click directly a row in the list to display the corresponding order. This button is only displayed if a single checkbox in the list of connections is selected.

- [EXPORT TO OMS]  
    Click this button to export the selected order(s) to the *Order management* module. This button is only displayed if the checkbox of at least one order is selected.

- [RETRY IMPORT]  
    Click this button to retry the import of the selected order(s). This button is only displayed if the checkboxes of at least two orders is selected. The *Import will be retried* pop-up window is displayed.

    ![Import will be retried](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ImportRetried.png "[Import will be retried]")

[comment]: <> (warum kann man nicht ein order nochmals importieren - BUG?)


- [CANCEL ORDER]/[CANCEL ORDERS]  
    Click this button to cancel the import of the selected order(s). This button is only displayed if the checkbox of at least one order with the **Error** status in the *Status of import from channel* column is selected. 

[comment]: <> (wird nach Ausführung irgendein pop-up fenster angezeigt?)

The list displays all orders, either for all connections or for the selected connection. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Connection*  
    Connection name. 

- *Status of import from channel*   
    Status of the order import from the marketplace to the *Omni-Channel* module. The following options are available:  
    - **Not imported**  
        The order import has not been performed.
    - **Complete**  
        The order import has been successfully completed.   	
    - **Canceled**  
        The order import has been canceled.  
    - **Error**  
        The order import has given an error. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).

- *Status of export to channel*  
    Status of the order export from the *Omni-Channel* module to the marketplace. The following options are available:  
    - **Exported**  
        The order has been successfully exported.  
    - **No changes to sync**  
        There are no changes to synchronize.
    - **Error**   
        Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).


- *Status of export to OMS*  
    Status of the order export from the *Omni-Channel* module to the *Order management* module for further processing. The following options are available:  
    - **Exported**  
        The order has been successfully exported.
    - **Not exported**  
        The order has not been exported.  
    - **Not exported: Pending > 30 minutes to OMS**  
        The order export is pending.
    - **Being exported**  
        The order is currently being exported.

[comment]: <> (Weitere status?)

- *Created on*  
    Date and time of the creation. 

- *Modified on*  
    Date and time of the last modification. 

- *Remote ID*  
    Identification number of the order in the marketplace.

- *ID in OMS*  
    Identification number of the document in the *Order management* module.    

- *\# Line items*  
    Number of line items in the order.

- *Line items*  
    SKU of line item(s) in the order. 

- *ID*  
    Order identification number. The ID number is automatically assigned by the system.

- Attribute    
    You can add a column for each attribute that is assigned to the order. The column displays the attribute name, the row displays the corresponding attribute value of the order.



## Order from connection "Connection name"

*Omni-Channel > Orders and returns > Tab ORDERS > Select order*

![Order connection](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionAttributes.png "[Order connection]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Order from connection "Connection name"* view and return to the order list. All changes are rejected.

- [CLOSE]  
    Click this button to close the *Order from connection "Connection name"* view.

- *ID in shop:*  
    Identification number of the order in the marketplace. 

- *Bill ID:*  
    Identification number of the document in the *Order management* module.   
  
- *Import status:*  
    Order import status from the marketplace to the *Omni-Channel* module. The following statuses are available:  
    - **Not imported**
    - **Complete**  
    - **Canceled**
    - **Error**

- *Export status:*  
    Order export status from the *Omni-Channel* module to the marketplace. The following statuses are available:  
    - **Exported**
    - **No changes to sync**  
    
[comment]: <> (Stimmt das? Feld immer/meistens leer hier, auch wenn in Order Liste Status angezeigt. Bezieht sich auf Status of Export to Channel oder Status of Export to OMS? Andere Möglichkeiten?)

- [EXPORT TO OMS]  
    Click this button to export the order to the *Order management* module. This button is only displayed if the status in the *Status of export to OMS* column equals **Not exported: Pending > 30 minutes to OMS**.

- [RE-TRIGGER IMPORT]    
    Click this button to trigger the order import again. This button is only displayed if the status in the *Status of import from channel* column equals **Not imported**. The *Order import triggered* pop-up window is displayed.

    ![Order import triggered](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderImportTriggered.png "[Order import triggered]")

[comment]: <> (Andere Buttons möglich?)


## Order from connection "Connection name" &ndash; Attributes

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Attributes*

![Order connection attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionAttributes.png "[Order connection attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the order contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
    Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


## Order from connection "Connection name" &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Dependencies*

![Order connection dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionDependencies.png "[Order connection dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The following options are available:
    - **Omni-Channel Offer**
    - **UCS Product**
    - **UCS Faktura**

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   

[comment]: <> (what id number is that? How is it created?)



## Order from connection "Connection name" &ndash; Line items

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Line items*

![Order connection line items](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionLineItems.png "[Order connection line items]")

**Line items**

- *VIEW*   
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *VIEW* drop-down list to display the context menu. The following menu entries are available:

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
    Click this button to display the search bar and search for a line item.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of line items.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. You can only select one checkbox at a time. 

- [VIEW]  
    Click this button to display the *Line item* view of the selected line item. Alternatively, you can click directly a row in the list to view the corresponding line item.  This button is only displayed if a single checkbox in the list of line items is selected.


The list displays all line items of the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *SKU*  
    Stock Keeping Unit. Identification number of the product to the order.

- *Type*  
    Line item type. The following options are available:
    - **Line item**
    - **Shipping**

[comment]: <> (Andere Typen?)

- *ID*  
    Order identification number. The ID number is automatically assigned by the system after creation.

- Attribute    
    You can add a column for each attribute that is assigned to the line item. The column displays the attribute name, the row displays the corresponding attribute value of the item.


### Line item 

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Line items > Select line item*

![Line item](../../Assets/Screenshots/Channels/OrdersReturns/Orders/LineItemAttributes.png "[Line item]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Line item* view and return to the list of line items. All changes are rejected.

- [CANCEL]  
    Click this button to close the *Line item* view.

  
### Line item &ndash; Attributes

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Line items > Select line item > Tab Attributes*

![Line item attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/LineItemAttributes.png "[Line item attributes]")

[comment]: <> (Hinzufügen/erklären? The attributes tab reproduces the fields available in the marketplace.)

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
    Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


### Line item &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Line items > Select line item > Tab Dependencies*

![Line item dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Orders/LineItemDependencies.png "[Line item dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected line item. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The following options are available:
    - **Omni-Channel Offer**
    - **UCS Product**
    - **UCS Faktura Order Position**

[comment]: <> (What else? Vermutlich eher Standardsatz wie All available dependent entity types are displayed.)

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   

[comment]: <> (what id number is that? How is it created?)


## Order from connection "Connection name" &ndash; Shipments

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments*

![Order connection shipments](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionShipments.png "[Order connection shipments]")

**Shipments**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an error.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of errors.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all errors in the list are selected.

- [VIEW]  
    Click this button to display the *Shipment for order* view of the selected shipment. Alternatively, you can click directly a row in the list to view the corresponding shipment. This button is only displayed if a single checkbox in the list of shipments is selected.

The list displays all shipments for the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Status of import from channel*  
    Status of the order import from the marketplace to the *Omni-Channel* module. The following options are available:  
    - **Not imported**  
        The order import has not been performed.
    - **Complete**  
        The order import has been successfully completed.   	
    - **Canceled**  
        The order import has been canceled.  
    - **Error**  
        The order import has given an error.

- *Status of export to channel*  
    Status of the order export from the *Omni-Channel* module to the marketplace. The following options are available:  
    - **Exported**  
        The order has been successfully exported.  
    - **No changes to sync**  
        There are no changes to synchronize.

[comment]: <> (Check, ob es stimmt. Status bezieht sich auf Order oder Shipment? Andere Möglichkeiten?)

- *ID*  
    Shipment identification number. The ID number is automatically assigned by the system.

- Attribute  
    You can add a column for each attribute that is assigned to the shipment. The column displays the attribute name, the row displays the corresponding attribute value of the shipment.

### Shipment for order "Order ID"

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment*

![Shipment attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentAttributes.png "[Shipment attributes]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Shipment for order "Order ID"* view and return to the shipment list. All changes are rejected.

- [CLOSE]  
    Click this button to close the *Shipment for order "Order ID"* view.

### Shipment for order "Order ID" &ndash; Attributes

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment > Tab Attributes*

![Shipment attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentAttributes.png "[Shipment attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
    Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.

### Shipment for order "Order ID" &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment > Tab Dependencies*

![Shipment dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentDependencies.png "[Shipment dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The following options are available:
    - **Omni-Channel Offer**
    - **UCS Product**
  
[comment]: <> (What else?)

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   

[comment]: <> (what id number is that? How is it created?)


### Shipment for order "Order ID" &ndash; Shipment line items

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment > Tab Shipment line items*

![Shipment line items](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentLineItems.png "[Shipment line items]")

**Shipment line items**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a line item.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of line items.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. You can only select one checkbox at a time. 

- [VIEW]  
    Click this button to display the *Line item* view of the selected line item. Alternatively, you can click directly a row in the list to view the corresponding line item.  This button is only displayed if a single checkbox in the list of line items is selected.


The list displays all items of the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *SKU*  
    Stock Keeping Unit. Identification number of the product to the order.

- *Type*  
    Item type. The following options are available:
    - **Line item**
    - **Shipping**

[comment]: <> (what else?)

- *ID*  
    Order identification number. The ID number is automatically assigned by the system after creation.

- Attribute    
    You can add a column for each attribute that is assigned to the order. The column displays the attribute name, the row displays the corresponding attribute value of the order.

#### Shipment line item

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment > Tab Shipment line items > Select line item*

![Shipment line item](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentLineItemAttributes.png "[Shipment line item]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Shipment line item* view and return to the shipment line item list. All changes are rejected.

- [CANCEL]  
    Click this button to close the *Shipment line item* view.


#### Shipment line item &ndash; Attributes

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment > Tab Shipment line items > Select line item > Tab Attributes*

![Shipment line item attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentLineItemAttributes.png "[Shipment line item attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
    Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


#### Shipment line item &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Shipments > Select shipment > Tab Shipment line items > Select line item > Tab Dependencies*

![Shipment line item dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ShipmentLineItemDependencies.png "[Shipment line item dependencies]")


- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The following options are available:
    - **Omni-Channel Offer**
    - **UCS Product**

[comment]: <> (what else?)

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   

[comment]: <> (what id number is that? How is it created?)


## Order from connection "Connection name" &ndash; Cancellations

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Cancellations*

![Order connection cancellations](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionCancellations.png "[Order connection cancellations]")

**Cancellations**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an error.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of errors.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all errors in the list are selected.

- [VIEW]  
    Click this button to display the *Shipment for order* view of the selected shipment. Alternatively, you can click directly a row in the list to view the corresponding shipment. This button is only displayed if a single checkbox in the list of shipments is selected.

The list displays all shipments for the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Status of import from channel*  
    Status of the order import from the marketplace to the *Omni-Channel* module. The following options are available:  
    - **Not imported**  
        The order import has not been performed.
    - **Complete**  
        The order import has been successfully completed.   	
    - **Canceled**  
        The order import has been canceled.  
    - **Error**  
        The order import has given an error.

- *Status of export to channel*  
    Status of the order export from the *Omni-Channel* module to the marketplace. The following options are available:  
    - **Exported**  
        The order has been successfully exported.  
    - **No changes to sync**  
        There are no changes to synchronize.

[comment]: <> (Check, ob es stimmt. Status bezieht sich auf Order oder Shipment? Andere optionen?)

- *ID*  
    Shipment identification number. The ID number is automatically assigned by the system.

[comment]: <> (Unterfenster wie bei Shipments?)


## Order from connection "Connection name" &ndash; Errors

*Omni-Channel > Orders and returns > Tab ORDERS > Select order > Tab Errors*

![Order connection errors](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionErrors.png "[Order connection errors]")

**Error list**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an error.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of errors.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

The list displays all errors of the selected order. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Log ID*  
    Log identification number. The ID number is automatically assigned by the system.   

- *Message*  
    Description of the error. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).

- *Short Message*  
    Short description of the error.

- *Created*  
    Date and time of the creation.

- *Creator*  
    Name and username of the user who created the error.

- *Last modified*  
    Date and time of the last modification.

- *Editor*  
    Name and username of the user who modified the error.  

[comment]: <> (bezieht sich  Editor und Creator auf das offer oder den error? Leeres Feld bei systemfehler?)


## Create view

*Omni-Channel > Orders and returns > Tab ORDERS > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Channels/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./02a_Offers.md#create-view).


## Rename view

*Omni-Channel > Orders and returns > Tab ORDERS > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Channels/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./02a_Offers.md#rename-view).
