[!!Configure the orders and returns](../Integration/04_ConfigureOrdersReturns.md)
[!!Manage the orders and returns](../Operation/04_ManageOrdersReturns.md)

[comment]: <> (Add link to Order management if available)

# Returns

*Omni-Channel > Orders and returns > Tab RETURNS*

![Returns](../../Assets/Screenshots/Channels/OrdersReturns/Returns/Returns.png "[Returns]")

> [Info] Returns are only displayed in this tab, if at least one of the configured connections supports the return import and export to its marketplace. Otherwise, no returns will be displayed. 

**Returns**

- *Combined status*  
    Combined status of all returns. The following statuses are available:
    - ![red](../../Assets/Icons/Status02.png "[red]") (red)  
        At least one return is faulty. Click the [>> more] button right to the status to switch to the *ERRORS* tab, see [User interface Errors (Orders and returns)](./05c_Errors.md).   
    - ![yellow](../../Assets/Icons/Status05.png "[yellow]") (yellow)  
        At least one return is still pending.
    - ![green](../../Assets/Icons/Status03.png "[green]") (green)  
        All returns are completed.

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a return.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of returns.

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
    Click the drop-down list to select a connection. All available connections are displayed in the list. When a connection has been selected, the [Import returns] button, the *Download returns automatically* drop-down list and the [SAVE] button are displayed.

- [Import returns for all connections]  
    Click this button to import the returns for all connections. This button is only displayed if no connection has been selected in the *All connections* drop-down list.

- [Import returns]  
    Click this button to import all returns for the selected connection. This button is only displayed if a connection has been selected in the *All connections* drop-down list.

- [Download returns automatically]  
    Click the drop-down list and select the desired time interval for the automatic download of returns. This drop-down list is only displayed if a connection has been selected in the *All connections* drop-down list. By default, the **never** option is preselected. The following options are available:
    - **never**
    - **every 2 minutes**
    - **every 5 minutes**
    - **every 10 minutes**
    - **every 15 minutes**
    - **every 20 minutes**
    - **every 30 minutes**
    - **every 60 minutes**

- [SAVE]  
    Click this button to save the settings for the automatic download of returns. This button is only displayed if a connection has been selected in the *All connections* drop-down list.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all returns in the list are selected.

- [VIEW]  
    Click this button to display the *Return from connection "Connection name"* view of the selected return. Alternatively, you can click directly a row in the list to display the corresponding return. This button is only displayed if a single checkbox in the list of connections is selected.

- [EXPORT TO OMS]  
    Click this button to export the selected return(s) to the *Order management* module. This button is only displayed if the checkbox of at least one return is selected.

- [RETRY IMPORT]  
    Click this button to retry the import of the selected return(s). This button is only displayed if the checkboxes of at least two returns is selected. The *Import will be retried* pop-up window is displayed.

    ![Import will be retried](../../Assets/Screenshots/Channels/OrdersReturns/Orders/ImportRetried.png "[Import will be retried]")

[comment]: <> (pop-up window spricht von "order" obwohl es return ist. -> Bug reported: BUG-198 Wenn richtig, neuer screenshot.)

[comment]: <> (aktuell noch BUG -> wird nur bei Auswahl von mindestens zwei orders angezeigt -> Bug reported: BUG-144)

The list displays all returns, either for all connections or for the selected connection. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Connection*  
    Connection name. 

- *Status of import from channel*   
    Status of the return import from the marketplace to the *Omni-Channel* module. The following options are available:  
    - **Not imported**  
        The return has not been imported.
    - **Imported**  
        The return has been imported.
    - **Complete**  
        The return import has been successfully completed.   	
    - **Error**  
        The return import has failed. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).
    - **Canceled**  
        The return import has been canceled.  

- *Status of export to channel*  
    Status of the return export from the *Omni-Channel* module to the marketplace. The following options are available:  
    - **Exported**  
        The return has been exported.
    - **No changes to sync**  
        The return has no changes to synchronize.
    - **Error**   
        The return export has failed. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).

- *Status of export to OMS*  
    Status of the return export from the *Omni-Channel* module to the *Order management* module for further processing. The following options are available:  
    - **Exported**  
        The return has been exported.
    - **Not exported**  
        The return has not been exported.  
    - **Not exported: Pending > 30 minutes to OMS**  
        The return export is pending.
    - **Being exported**  
        The return is currently being exported.

- *Created on*  
    Date and time of the creation. 

- *Modified on*  
    Date and time of the last modification. 

- *Remote ID*  
    Identification number of the return in the marketplace.

- *ID in OMS*  
    Identification number of the document in the *Order management* module.    

- *\# Line items*  
    Number of the line items in the return.

- *Line items*  
    SKU of the line item(s) in the return. 

- *ID*  
    Return identification number. The ID number is automatically assigned by the system.

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the return. The column displays the attribute name, the row displays the corresponding attribute value of the return.



## Return from connection "Connection name"

*Omni-Channel > Orders and returns > Tab RETURNS > Select return*

![Return connection](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionAttributes.png "[Return connection]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Return from connection "Connection name"* view and return to the list of returns. All changes are rejected.

- [CLOSE]  
    Click this button to close the *Return from connection "Connection name"* view.

- *ID in shop:*  
    Identification number of the return in the marketplace. 

- *Bill ID:*  
    Identification number of the document in the *Order management* module.   
  
- *Import status:*  
    Return import status from the marketplace to the *Omni-Channel* module. The following statuses are available:  
    - **Not imported**
    - **Complete**  
    - **Canceled**
    - **Error**

- *Export status:*  
    Return export status from the *Omni-Channel* module to the marketplace. The following statuses are available:  
    - **Exported**
    - **Being Exported**
    - **Not exported**  
    
[comment]: <> (Export status Anzeige funktioniert nicht, nicht klar definiert welcher export status -> FETA-15, BUG-147)

- [EXPORT TO OMS]  
    Click this button to export the return to the *Order management* module. This button is only displayed if the status in the *Status of export to OMS* column equals **Not exported: Pending > 30 minutes to OMS**. The export status changes to **Being exported**.

- [RE-TRIGGER IMPORT]    
    Click this button to trigger the return import again. This button is only displayed if the status in the *Status of import from channel* column equals **Not imported**. The *Return import triggered* pop-up window is displayed.

    ![Return import triggered](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnImportTriggered.png "[Return import triggered]")

[comment]: <> (Button umbenennen in RETRY IMPORT -> Konsistenz! -> FETA-16)

The *Return from connection "Connection name"* view is composed of the following tabs:
- [Return from connection "Connection name" &ndash; Attributes](#return-from-connection-connection-name--attributes)
- [Return from connection "Connection name" &ndash; Dependencies](#return-from-connection-connection-name--dependencies)
- [Return from connection "Connection name" &ndash; Line items](#return-from-connection-connection-name--line-items)
- [Return from connection "Connection name" &ndash; Shipments](#return-from-connection-connection-name--shipments)
- [Return from connection "Connection name" &ndash; Cancellations](#return-from-connection-connection-name--cancellations)
- [Return from connection "Connection name" &ndash; Errors](#return-from-connection-connection-name--errors)



## Return from connection "Connection name" &ndash; Attributes

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Attributes*

![Return connection attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionAttributes.png "[Return connection attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the return contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.



## Return from connection "Connection name" &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Dependencies*

![Return connection dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionDependencies.png "[Return connection dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance the SKU number or a bill number.



## Return from connection "Connection name" &ndash; Line items

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Line items*

![Return connection line items](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionLineItems.png "[Return connection line items]")

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
    Click this button to display the *Line item* view of the selected line item. Alternatively, you can click directly a row in the list to view the corresponding line item. This button is only displayed if a single checkbox in the list of line items is selected.

The list displays all line items of the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *SKU*  
    Stock Keeping Unit. Identification number of the return line item.

- *Type*  
    Line item type. The following options are available:
    - **Line item**
    - **Shipping**
    - **Discount**
    - **Payment**
    - **Redeem voucher**
    - **Service**
    - **Return line item**
    - **Ancillary return line item**
    - **Shipment line item**
    - **Cancellation line item**

- *ID*  
    Return line item identification number. The ID number is automatically assigned by the system after creation.

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the return line item. The column displays the attribute name, the row displays the corresponding attribute value of the item.


### Line item 

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Line items > Select line item*

![Line item](../../Assets/Screenshots/Channels/OrdersReturns/Returns/LineItemAttributes.png "[Line item]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Line item* view and return to the list of line items. All changes are rejected.

- [CANCEL]  
    Click this button to close the *Line item* view.

The *Line item* view is composed of the following tabs:
- [Line item &ndash; Attributes](#line-item--attributes)
- [Line item &ndash; Dependencies](#line-item--dependencies)


### Line item &ndash; Attributes

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Line items > Select line item > Tab Attributes*

![Line item attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/LineItemAttributes.png "[Line item attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.


### Line item &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Line items > Select line item > Tab Dependencies*

![Line item dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Returns/LineItemDependencies.png "[Line item dependencies]")

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
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance the SKU number or a bill number.



## Return from connection "Connection name" &ndash; Shipments

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments*

![Return connection shipments](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionShipments.png "[Return connection shipments]")

**Shipments**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a shipment.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of shipments.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all shipments in the list are selected.

- [VIEW]  
    Click this button to display the *Shipment for return* view of the selected shipment. Alternatively, you can click directly a row in the list to view the corresponding shipment. This button is only displayed if a single checkbox in the list of shipments is selected.

The list displays all shipments for the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Status of import from channel*  
    Status of the return import from the marketplace to the *Omni-Channel* module. The following options are available:  
    - **Not imported**  
        The return has not been imported.
    - **Imported**  
        The return has been imported.
    - **Complete**  
        The return import has been successfully completed.   	
    - **Error**  
        The return import has failed. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).
    - **Canceled**  
        The return import has been canceled.  

- *Status of export to channel*  
    Status of the return export from the *Omni-Channel* module to the marketplace. The following options are available:  
    - **Exported**  
        The return has been exported.
    - **No changes to sync**  
        The return has no changes to synchronize.
    - **Error**   
        The return export has failed. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).

- *ID*  
    Shipment identification number. The ID number is automatically assigned by the system.

- *"Attribute name"*  
    You can add a column for each attribute that is assigned to the shipment. The column displays the attribute name, the row displays the corresponding attribute value of the shipment.


### Shipment for return "Return ID"

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment*

![Shipment attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentAttributes.png "[Shipment attributes]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Shipment for return "Return ID"* view and return to the shipment list. All changes are rejected.

- [CLOSE]  
    Click this button to close the *Shipment for return "Return ID"* view.

The *Shipment for return "Return ID"* view is composed of the following tabs:
- [Shipment for return "Return ID" &ndash; Attributes](#shipment-for-return-return-id--attributes)
- [Shipment for return "Return ID" &ndash; Dependencies](#shipment-for-return-return-id--dependencies)
- [Shipment for return "Return ID" &ndash; Shipment line items](#shipment-for-return-return-id--shipment-line-items)


### Shipment for return "Return ID" &ndash; Attributes

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment > Tab Attributes*

![Shipment attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentAttributes.png "[Shipment attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.


### Shipment for return "Return ID" &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment > Tab Dependencies*

![Shipment dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentDependencies.png "[Shipment dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies to the shipment.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies to the shipment in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected shipment. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance the SKU number or a bill number.


### Shipment for return "Return ID" &ndash; Shipment line items

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment > Tab Shipment line items*

![Shipment line items](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentLineItems.png "[Shipment line items]")

**Shipment line items**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a shipment line item.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of shipment line items.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. You can only select one checkbox at a time. 

- [VIEW]  
    Click this button to display the *Shipment line item* view of the selected shipment line item. Alternatively, you can click directly a row in the list to view the corresponding shipment line item. This button is only displayed if a single checkbox in the list of shipment line items is selected.

The list displays all shipment line items of the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *SKU*  
    Stock Keeping Unit. Identification number of the shipment line item.

- *ID*  
    Shipment line item identification number. The ID number is automatically assigned by the system after creation.

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the return. The column displays the attribute name, the row displays the corresponding attribute value of the return.


#### Shipment line item

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment > Tab Shipment line items > Select shipment line item*

![Shipment line item](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentLineItemAttributes.png "[Shipment line item]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Shipment line item* view and return to the shipment line item list. All changes are rejected.

- [CANCEL]  
    Click this button to close the *Shipment line item* view.

The *Shipment line item* view is composed of the following tabs:
- [Shipment line item &ndash; Attributes](#shipment-line-item--attributes)
- [Shipment line item &ndash; Dependencies](#shipment-line-item--dependencies)


#### Shipment line item &ndash; Attributes

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment > Tab Shipment line items > Select shipment line item > Tab Attributes*

![Shipment line item attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentLineItemAttributes.png "[Shipment line item attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.


#### Shipment line item &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Shipments > Select shipment > Tab Shipment line items > Select shipment line item > Tab Dependencies*

![Shipment line item dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ShipmentLineItemDependencies.png "[Shipment line item dependencies]")

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected shipment line item. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance the SKU number or a bill number.



## Return from connection "Connection name" &ndash; Cancellations

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations*

![Return connection cancellations](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionCancellations.png "[Return connection cancellations]")

**Cancellations**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a cancellation.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of cancellations.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all cancellations in the list are selected.

- [VIEW]  
    Click this button to display the *Cancellation line item* view of the selected cancellation. Alternatively, you can click directly a row in the list to view the corresponding cancellation. This button is only displayed if a single checkbox in the list of cancellations is selected.

The list displays all cancellations for the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Status of import from channel*  
    Status of the return import from the marketplace to the *Omni-Channel* module. The following options are available:  
    - **Not imported**  
        The return has not been imported.
    - **Imported**  
        The return has been imported.
    - **Complete**  
        The return import has been successfully completed.   	
    - **Error**  
        The return import has failed. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).
    - **Canceled**  
        The return import has been canceled.  

- *Status of export to channel*  
    - **Exported**  
        The return has been exported.
    - **No changes to sync**  
        The return has no changes to synchronize.
    - **Error**   
        The return export has failed. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).

- *ID*  
    Cancellation identification number. The ID number is automatically assigned by the system.


### Cancellation for return "Return ID"

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation*

![Cancellation attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationAttributes.png "[Cancellation attributes]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Cancellation for return "Return ID"* view and return to the cancellation list. All changes are rejected.

- [CLOSE]  
    Click this button to close the *Cancellation for return "Return ID"* view.

The *Cancellation for return "Return ID"* view is composed of the following tabs:
- [Cancellation for return "Return ID" &ndash; Attributes](#cancellation-for-return-return-id--attributes)
- [Cancellation for return "Return ID" &ndash; Dependencies](#cancellation-for-return-return-id--dependencies)
- [Cancellation for return "Return ID" &ndash; Cancellation line items](#cancellation-for-return-return-id--cancellation-line-items)


### Cancellation for return "Return ID" &ndash; Attributes

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation > Tab Attributes*

![Cancellation attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationAttributes.png "[Cancellation attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.


### Cancellation for return "Return ID" &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation > Tab Dependencies*

![Cancellation dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationDependencies.png "[Cancellation dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies to the cancellation.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies to the cancellation in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected cancellation. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance the SKU number or a bill number.


### Cancellation for return "Return ID" &ndash; Cancellation line items

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation > Tab Cancellation line items*

![Cancellation line items](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationLineItems.png "[Cancellation line items]")

**Cancellation line items**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a cancellation line item.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of cancellation line items.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. You can only select one checkbox at a time. 

- [VIEW]  
    Click this button to display the *Cancellation line item* view of the selected cancellation line item. Alternatively, you can click directly a row in the list to view the corresponding cancellation line item. This button is only displayed if a single checkbox in the list of cancellation line items is selected.

The list displays all cancellation line items of the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *SKU*  
    Stock Keeping Unit. Identification number of the cancellation line item.

- *ID*  
    Cancellation line item identification number. The ID number is automatically assigned by the system after creation.

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the return. The column displays the attribute name, the row displays the corresponding attribute value of the return.


#### Cancellation line item

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation > Tab Cancellation line items > Select line item*

![Cancellation line item](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationLineItemAttributes.png "[Cancellation line item]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Cancellation line item* view and return to the cancellation line item list. All changes are rejected.

- [CANCEL]  
    Click this button to close the *Cancellation line item* view.

The *Cancellation line item* view is composed of the following tabs:
- [Cancellation line item &ndash; Attributes](#cancellation-line-item--attributes)
- [Cancellation line item &ndash; Dependencies](#cancellation-line-item--dependencies)


#### Cancellation line item &ndash; Attributes

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation > Tab Cancellation line items > Select line item > Tab Attributes*

![Cancellation line item attributes](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationLineItemAttributes.png "[Cancellation line item attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the line item contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. All fields are read-only.

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.


#### Cancellation line item &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Cancellations > Select cancellation > Tab Cancellation line items > Select line item > Tab Dependencies*

![Cancellation line item dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Returns/CancellationLineItemDependencies.png "[Cancellation line item dependencies]")

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dependencies to the cancellation.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies to the cancellation in the list are selected.

- [RERUN MAPPING]  
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.

The list displays all dependencies of the selected cancellation. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance the SKU number or a bill number.



## Return from connection "Connection name" &ndash; Errors

*Omni-Channel > Orders and returns > Tab RETURNS > Select return > Tab Errors*

![Return connection errors](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnConnectionErrors.png "[Return connection errors]")

**Error list**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an error.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of errors.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

The list displays all errors of the selected return. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Log ID*  
    Log identification number. The ID number is automatically assigned by the system.   

- *Message*  
    Description of the error. Click the [Show log message] button in the column to display the corresponding log message in the *LOG* tab, see [User interface LOG](./06a_Log.md).

- *Short Message*  
    Short description of the error.

- *Created*  
    Date and time of the creation.

- *Creator*  
    Name and username of the user who triggered the action that caused the error. By default, the field is blank as the job is created by the system.

- *Last modified*  
    Date and time of the last modification.

- *Editor*  
    Name and username of the user who modified the action that caused the error. By default, the field is blank as the job is modified by the system.
    


## Create view

*Omni-Channel > Orders and returns > Tab RETURNS > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Channels/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./02a_Offers.md#create-view).



## Rename view

*Omni-Channel > Orders and returns > Tab RETURNS > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Channels/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./02a_Offers.md#rename-view).
