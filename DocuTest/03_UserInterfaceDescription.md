# All parts that can be deleted

**LIST**  

The *Dispatch notes* menu entry offers an overview of all dispatch notes processed by the system. It also allows the possibility to check the dispatch note status and the corresponding shipment status, among others.


*Fulfillment > Dispatch notes > Tab LIST*

![Dispatch notes](../Assets/Screenshots/DocuTest/DispatchNotes2.png "[Dispatch notes]")

**Dispatch notes**
>ADD

The *Dispatch notes* LIST tab contains a list view. For detailed information on creating and maintaining a view, see LINK in the *Actindo Core1 Platform* documentation.
>END OF ADD

The following further functions are available in the list header of the dispatch notes:       

- *Connections*   
    Click the drop-down list to select a connection. The following options are available:
    - **All connections**  
        Select this option to display the dispatch notes for all configured connections. 
    - **Connection name**  
        Select this option to display the dispatch notes for the selected connection. When a specific connection has been selected, the **All connections** option is no longer displayed. Click the selected connection again to deselect it.    

>DELETE   

- ![Search](../Assets/Icons/Search.png "[Search]") (Search)   -> noch aufnehmen in Core1
    Click this button to display the search bar and search for dispatch notes.

- ![Refresh](../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dispatch notes.   

- ![Columns](../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

>END OF DELETE   

>ADD   
 
The following functions are available in the editing toolbar:   
>END OF ADD
- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dispatch notes in the list are selected.

- [VIEW]  
    Click this button to view a dispatch note. This button is only displayed if a single checkbox in the list of dispatch notes is selected. Alternatively, you can click directly a row in the list to view the corresponding dispatch note. 
    The *Dispatch note "Dispatch note ID"* view is displayed, see [Dispatch note](#dispatch-note). The *Attributes* tab is preselected.

- [EXPORT]  
    Click this button to export a dispatch note to the fulfiller. This button is displayed if the checkbox of at least one dispatch note is selected.

    > [Info] The dispatch note is exported automatically by the system. If the export fails, the dispatch note can be manually re-exported. For detailed information, see [Export a dispatch note](../Operation/01_ManageDispatchNotes.md#export-a-dispatch-note).

- [FORCE COMPLETION]  
    Click this button to complete a dispatch note. This button is displayed if the checkbox of at least one dispatch note is selected.   
    For detailed information, see [Complete a dispatch note](../Operation/01_ManageDispatchNotes.md#complete-a-dispatch-note). 

**Status information fields**   
The list displays all dispatch notes. Depending on the settings, the displayed columns may vary. All fields are read-only. The following status information fields are available:

- *Status*  
    Dispatch note status. The following statuses are available:  
    - **New dispatch note**  
        The dispatch note has been newly created.
    - **Transferred to partner**  
        The dispatch note has been transferred to the fulfiller.
    - **Partner confirmed receival**  
        The fulfiller has confirmed receival of the dispatch note.
    - **Dispatch note completed**  
        The dispatch note has been completed.
    -  **Error**  
        The dispatch note has given an error while exporting.
    - **Void**  
        The dispatch note is void, for instance, because of an order cancellation.

- *Shipment status*  
    Status of shipment associated with the dispatch note. The following options are available:
    - ![Cross](../Assets/Icons/Cross02.png "[Cross]") (Cross)   
        No shipment has been performed yet.  
    - ![Circular arrows](../Assets/Icons/CircularArrows.png "[Circular arrows]") (Circular arrows)   
        The shipment is in progress.   
    - ![Double check](../Assets/Icons/DoubleCheck.png "[Double check]") (Double check)    
        The shipment has been delivered.
    - ![Error](../Assets/Icons/Warning02.png "[Error]") (Error)    
        The fulfiller has reported a shipment error.
    - Empty  
        No information on the shipment status has been received from fulfiller.   


- *Status ID*  
  Dispatch note status identifier. The following options are available:
    - **new**  
        The dispatch note has been newly created.
    - **transferred**  
        The dispatch note has been transferred to the fulfiller.
    - **confirmed**  
        The fulfiller has confirmed receival of the dispatch note.
    - **completed**  
        The dispatch note has been completed.
    - **error**  
        The dispatch note has given an error while exporting.
    - **void**  
        The dispatch note is void, for instance, because of an order cancellation.

- *Shipping type*  
    Type of shipment. The following options are available:  
    - **STND**  
        Standard shipping type.
    - **EXPR**  
        Express shipping type.

    > [Info] The shipping type can be set up in the *PACKAGING TYPES* tab in the *Settings* menu entry, see [Packaging types](./03b_PackagingTypes.md).



## Dispatch note &ndash; Attributes

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Attributes*

![Attributes](../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteAttributes.png "[Attributes]")

> DELETE      

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the dispatch note contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.    

> END OF DELETE  


>ADD   

For detailed information, see LINK in the *DataHub* documentation.    
>END OF ADD



## Dispatch note &ndash; Dependencies

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Dependencies*

![Dependencies](../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteDependencies.png "[Dependencies]")

**Dependencies**   
< DELETE    
The *Dependencies* tab contains all dependencies of the selected dispatch note. Depending on the settings, the displayed columns may vary. All fields are read-only.    
If no dependent entities exist, the *No other entities depend on this entity* notice is displayed.> 
>END OF DELETE

>ADD   

For detailed information on the *Dependencies* tab, see LINK in the *DataHub* documentation.  

>END OF ADD

>DELETE   

The following functions are available:   
- ![Refresh](../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dispatch note dependencies.

- ![Columns](../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependent entities in the list are selected.


- [RERUN MAPPING]   
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.    

>END OF DELETE



## Dispatch note &ndash; Shipments

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments*

![Shipments](../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteShipments.png "[Shipments]")


>DELETE
- ![Refresh](../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of shipments.

- ![Columns](../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.   

>END OF DELETE>

The list displays all shipments. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *ID*  
    Shipment identification number. The ID number is automatically assigned by the system.

- *Carrier*  
    Carrier identifier.

- *Connection*  
    Connection to fulfiller.

- *External ID*  
    Shipment identification number in the fulfiller's system. 

- *Status*  
    Shipment status. The following options are available:
    - **New shipment**
    - **Shipped**
    - **Delivered**
    - **Void**
    - **Error**
    - **Packed**

- *Status info*  
    Additional status information provided by the fulfiller. 

- *Created*  
    Date and time of the creation.

- *Modified*    
    Date and time of the last modification.

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the shipment. The column displays the attribute name, the row displays the corresponding attribute value of the shipment.


### Shipment attributes

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Select a shipment > Sub-tab ATTRIBUTES*

![Shipments](../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesAttributes.png "[Shipments]")

>ADD   

The *Shipment attributes* tab provides an overview on...   

> END OF ADD

<BR>

>DELETE   

**Shipment "Shipment ID"**

- [BACK]  
    Click this button to close the **Shipment "Shipment ID"** view and return to the list of shipments. All changes are rejected.

>END OF DELETE>

### Shipment attributes &ndash; Attributes

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Select a shipment > Sub-tab ATTRIBUTES > Tab Attributes*

![Shipment attributes](../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesAttributes.png "[Shipment attributes]")

  

>ADD   

For detailed information on the *Attributes* tab, see LINK in the *DataHub* documentation.  

>END OF ADD   

<BR>

>DELETE

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the shipment contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. Depending on the selected attribute group, the displayed fields may vary. All fields are read-only.

- ![Collapse/Expand](../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded.

>END OF DELETE

### Shipment attributes &ndash; Dependencies

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Select a shipment > Sub-tab ATTRIBUTES > Tab Dependencies*

![Shipment dependencies](../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesDependencies.png "[Shipment dependencies]")

>ADD   

For detailed information on the *Dependencies* tab, see LINK in the *DataHub* documentation.  

>END OF ADD   


> DELETE

- ![Refresh](../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of shipment dependencies.

- ![Columns](../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependent entities in the list are selected. 



The list displays all dependencies of the selected shipment. Depending on the settings, the displayed columns may vary. All fields are read-only.   
If no dependent entities exist, the *No other entities depend on this entity* notice is displayed. 

- *Dependent entity ID*   
    Identification number of the dependent entity. The ID number is automatically assigned by the system. 

- *Dependent entity type*   
    Type of the dependent entity. 

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance a reference number or an SKU.

- [RERUN MAPPING]   
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.	

>END OF DELETE>


### Shipment packages

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Select a shipment > Sub-tab PACKAGES*

![Shipments](../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsPackages.png "[Shipments]")


>DELETE

- ![Search](../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for packages.

- ![Refresh](../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of packages.

- ![Columns](../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

>END OF DELETE>


The list displays all packages contained in the selected shipment. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Packaging type*  
    Packaging type name. Packaging types can be defined in the *PACKAGING TYPES* tab of the *Settings* menu entry, see [Manage the packaging types](../Integration/02_ManagePackagingTypes.md).

- *Created*  
    Date and time of the creation.

- *Modified*  
    Date and time of the last modification.

- *ID*  
    Packaging type identification number. This number is automatically assigned by the system.

-  *Tracking number*  
    Package tracking number.

- *Tracking link*  
    Package tracking link.

- *Package ID*  
    Package identification number. This identifier is provided by the fulfiller.

- *Proof of delivery*  
    Proof of delivery in the form of link leading to the relevant data, such as a photo of the delivery location or a signed delivery receipt. 

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the shipment package. The column displays the attribute name, the row displays the corresponding attribute value of the shipment package.
    

#### Items

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Select a shipment > Sub-tab PACKAGES > Select a package*

![Items](../Assets/Screenshots/Fulfillment/DispatchNotes/Items01.png "[Items]")


>DELETE

- ![Refresh](../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of items.

- ![Columns](../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

>END OF DELETE>

The list displays all items contained in the selected package. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Item number*  
    Item number in the package.

- *SKU*  
    Stock Keeping Unit. Identification number of the item.

- *Amount*  
    Amount of item units contained in the package.

- *Serial number*  
    Item serial number.

- *ID*  
    Item identification number. The ID number is automatically assigned by the system.

- *Unit net value*  
    Item unit net value.

- *Unit gross value*  
    Item unit gross value.

- *Total net value*  
    Item total net value.

- *Currency*  
    Item currency.

- *Dangerous goods indicator*  
    Indication whether the item has been classified as a dangerous product.

- *"Attribute name"*    
    You can add a column for each attribute that is assigned to the item. The column displays the attribute name, the row displays the corresponding attribute value of the item.



## Dispatch note &ndash; Logs

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Logs*

![Dispatch note logs](../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteLogs.png "[Dispatch note logs]")

This tab displays an extract from the list of intents contained in the *CONNECTIONS* tab of the *Logging* menu entry. The intents displayed in this tab refer to the selected dispatch note. For a detailed description of this window and the corresponding functions, see [Connections (Logging)](./02a_Connections.md).


> DELETE

## Create view

*Fulfillment > Dispatch notes > Tab LIST > Button Points > Menu entry create*

![Create view](../Assets/Screenshots/Fulfillment/DispatchNotes/CreateView.png "[Create view]")

- *Name*   
    Enter a name for the view.

- [CANCEL]   
    Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]   
    Click this button to save the new view and display it in the *VIEW* drop-down list. The *Create view* window is closed.

This window can also be accessed via the following tabs in the user interface:

- [CONNECTIONS (Logging)](02a_Connections.md#create-view)
- [CONNECTIONS (Settings)](03a_Connections.md#create-view)
- [PACKAGING TYPES](03b_PackagingTypes.md#create-view)



## Rename view

*Fulfillment > Dispatch notes > Tab LIST > Button Points > Menu entry rename*

![Rename view](../Assets/Screenshots/Fulfillment/DispatchNotes/RenameView.png "[Rename view]")

- *Name*   
    Click this field to edit the view name.

- [CANCEL]   
    Click this button to cancel renaming the view. The  *Rename view* window is closed.

- [SAVE]   
    Click this button to save the changes and display it in the *VIEW* drop-down list. The *Rename view* window is closed.

This window can also be accessed via the following tabs in the user interface:

- [CONNECTIONS (Logging)](02a_Connections.md#rename-view)
- [CONNECTIONS (Settings)](03a_Connections.md#rename-view)
- [PACKAGING TYPES](03b_PackagingTypes.md#rename-view)

>END OF DELETE