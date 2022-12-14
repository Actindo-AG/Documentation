[!!Configure the orders and returns](../Integration/04_ConfigureOrdersReturns.md)
[!!Manage the orders and returns](../Operation/04_ManageOrdersReturns.md)


# Orders

*Omni-Channel > Orders and returns > Tab ORDERS*

![Orders](../../Assets/Screenshots/Channels/OrdersReturns/Orders/Orders.png "[Orders]")

**Orders**

- *Combined status*  
    Combined of all orders. The following statuses are available:
    - ![red](../../Assets/Icons/Status02.png "[red]") (red)  
        There are errors in the orders. Click the *>> more* button to switch to the *ERRORS* tab.   
    - ![yellow](../../Assets/Icons/Status05.png "[yellow]") (yellow)  
        There are pending orders.
    - ![green](../../Assets/Icons/Status03.png "[green]") (green)  
        There are no errors in the orders.

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an order.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of orders.

- *VIEW*  
 Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu and create or edit a view.    
  For detailed information, see [Create a view](#create-a-view).

  - View context menu   
    Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![Create](../../Assets/Icons/Plus06.png "[Create]") create   
      Click this entry to create a view. The *Create view* window is displayed.

    - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename    
      Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed if a view has been selected.

    - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset    
      Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

    - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish    
      Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

    - ![Private view](../../Assets/Icons/Unpublish.png "[Unpublish]") private view    
      Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

    [comment]: <> (Private view oder unpublish? Cf. default sentences)

    - ![Save](../../Assets/Icons/Save.png "[Save]") save    
      Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

      > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete    
      Click this entry to delete the selected view. A confirmation window is displayed to confirm the deletion. This menu entry is only displayed if a view has been selected.

- *All Connections*    
  Click the drop-down list to select a connection. All supported connections are displayed in the list. When selecting a connection, the [Import orders for all connections] button changes to the [Import orders] button.

- [Import orders for all connections]  
  Click this button to import orders for all connections.

- [Import orders]  
  Click this button to import only orders for the selected connection. This button is only displayed, if a connection has been selected in the *All connections* drop-down list.

- [Download orders automatically]  
  Click the drop-down list and select the desired time interval at which the orders should be automatically downloaded. This button is only displayed, if a connection has been selected in the *All connections* drop-down list. The following options are available:
    - **never**
    - **every 2 minutes**
    - **every 5 minutes**
    - **every 10 minutes**
    - **every 15 minutes**
    - **every 20 minutes**
    - **every 30 minutes**
    - **every 60 minutes**

- [SAVE]  
  Click this button to save the settings.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all orders in the list are selected.

- [VIEW]  
  Click this button to view a selected order. This button is only displayed if a single checkbox in the list of connections is selected.

- [EXPORT TO OMS]  
  Click this button to view one or several selected orders. This button is only displayed if the checkbox of at least one order is selected.

- [RETRY IMPORT]  
  Click this button to view one or several selected orders. This button is only displayed if the checkbox of at least two orders is selected.


The list displays all orders available. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Connection*	
   Connection name. 

- *Status of import from Omni-Channel*   
   Status of the order import from Omni-Channel to ... 
    - **Order complete**  	
    - **Canceled**  	

[comment]: <> (Status of import from marketplace into Omni-Channel? Further info needed)

- *Status of export to Omni-Channel*  
    - **Exported**	
    - **No changes to sync**	

- *Status of export to OMS*  
   Status of the order export to the *Order management* module for further processing. The following options are available: 
    - **Exported**	
    - **Not exported**	
    - **Not exported: Pending > 30 minutes to OMS**
    - **Being exported**

- *Created on*  
   Date and time of the creation. 

- *Edited*  
   Date and time of the last modification. 

- *Remote ID*  

- *ID in OMS*  
   Identification number in the *Order management* module. This number equals the order confirmation.   

[comment]: <> (AB oder LI? S. Fakturierung)

- *\# Line items*  
  Number of line items contained in the order.

- *Line items*  
   SKU of line item contained in the order. 

- *ID*  
   Order identification number. The ID number is automatically assigned by the system.

- *Order number*  
   Order number as defined in the marketplace. 

- *Order ID*  
   Order identification number. The ID number is automatically assigned by the system.

[comment]: <> (Unterschied zwischen ID, Order number und Order ID?)

- *Total (net)*  
   Order total net value. 

- *Total (gross)*  
   Order total gross value. 

- *Currency*  
   Currency in which the order has been invoiced. 

- *Discount percent*  
   Discount percent applied to the order. 

- *Price bracket*  
   Price range of the product(s) ordered. 

- *Order time*  
   Date and time when the order has been placed. 

- *Payment method*  
   Payment method used to place the order. 

- *Payment method marketplace*  
   Payment method  used to place the order in the marketplace.

[comment]: <> (Unterschied zwischen Payment method and Payment method marketplace?)

- *Purchaser name*  
   Buyer name. 

- *Order status*

- *Payment reference*

- *Basket ID*

- *Language*	

- *Customer comment*	

- *Bill number*	

- *Note*	

- *Discount description*	

- *Amount to pay (after voucher)*	

- *Customer receipt*

- *Merchant receipt*	


[comment]: <> (Felder/Spalten aus UI File genommen. Die meisten sind aber Attributes, s. Order > Attributes Tab. Relevant/Standard oder weglassen?)

## Order from connection "Connection name"

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order*

![Order connection](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionAttributes.png "[Order connection]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Order from connection "Connection name"* view and return to the list of orders.

- [CLOSE]  
  Click this button to close the *Order from connection "Connection name"* view. The list of orders is displayed.

- *ID in Shop:*  

- *Bill ID:*  

- *Import status:*    

- *Export status:*  

- [EXPORT TO OMS]


## Order from connection "Connection name" &ndash; Attributes

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Attributes*

![Order connection attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionAttributes.png "[Order connection attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the order contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. Depending on the attribute group selected, the fields displayed vary. The dispatch note attributes are imported via the connection driver. All fields are locked and, therefore, read-only.

The attributes assigned to each group can be managed and customized in the *DataHub* module. For detailed information, see [Attribute groups](../../../DataHub/UserInterface/02c_AttributeGroups.md).


- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
  Attribute group that contains attribute sub-groups. Click the attribute group or the arrow *>* left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
  Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.


- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
  Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


## Order from connection "Connection name" &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Dependencies*

![Order connection dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionDependencies.png "[Order connection dependencies]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependencies in the list are selected.

- [RERUN MAPPING]  

The list displays all dependencies available. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Dependent entity ID*  

- *Dependent entity type*  

- *Change tracking*  

- *Dependent entity friendly identifier*  


## Order from connection "Connection name" &ndash; Line items

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Line items*

![Order connection line items](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrderConnectionLineItems.png "[Order connection line items]")

**Line items**

- *VIEW*  
 Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu and create or edit a view.    
  For detailed information, see [Create a view](#create-a-view).

  - View context menu   
    Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![Create](../../Assets/Icons/Plus06.png "[Create]") create   
      Click this entry to create a view. The *Create view* window is displayed.

    - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename    
      Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed if a view has been selected.

    - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset    
      Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

    - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish    
      Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

    - ![Private view](../../Assets/Icons/Unpublish.png "[Unpublish]") private view    
      Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

    [comment]: <> (Private view oder unpublish? Cf. default sentences)

    - ![Save](../../Assets/Icons/Save.png "[Save]") save    
      Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

      > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete    
      Click this entry to delete the selected view. A confirmation window is displayed to confirm the deletion. This menu entry is only displayed if a view has been selected.


- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an order.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of orders.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all orders in the list are selected.

- [VIEW]  
  Click this button to view a selected line item. This button is only displayed if a single checkbox in the list of line items is selected.

The list displays all line items available. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *SKU*  

- *Type*  

- *ID*  

- ...

### Line item 

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Line items > Select line item*

![Line item](../../Assets/Screenshots/Channels/OrdersReturns/Orders/LineItemAttributes.png "[Line item]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Line item* view and return to the list of line items.

- [CANCEL]  
  Click this button to close the *Line item* view. The list of line items is displayed.

### Line item &ndash; Attributes

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Line items > Select line item > Tab Attributes*

![Line item attributes](../../Assets/Screenshots/Channels/OrdersReturns/Orders/LineItemAttributes.png "[Line item attributes]")


### Line item &ndash; Dependencies

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Line items > Select line item > Tab Dependencies*

![Line item dependencies](../../Assets/Screenshots/Channels/OrdersReturns/Orders/LineItemDependencies.png "[Line item dependencies]")


## Order from connection "Connection name" &ndash; Errors

*Omni-Channel > Orders and returns > Tab ORDERS > Select an order > Tab Errors*

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

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all orders in the list are selected.

- [VIEW]  
  Click this button to view a selected error. This button is only displayed if a single checkbox in the list of line errors is selected.

[comment]: <> (Check, ob das stimmt, wenn errors vorhanden)

The list displays all line errors available. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Log*  

- *Message*  

- *Message*  

- *Created* 

- *Creator*  

- *Last modified*  

- *Editor*  


## Create view

*Omni-Channel > Orders and returns > Tab ORDERS > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Channels/CreateView.png "[Create view]")


For a detailed description of this window and the corresponding functions, see [Create view](./02a_Offers.md#create-view).


## Rename view

*Omni-Channel > Orders and returns > Tab ORDERS > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Channels/RenameView.png "[Rename view]")


For a detailed description of this window and the corresponding functions, see [Rename view](./02a_Offers.md#rename-view).
