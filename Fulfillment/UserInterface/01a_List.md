# List

*Fulfillment > Dispatch notes > Tab LIST*

![Dispatch notes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Dispatch notes]")

[comment]: <> (Neues screenshot benötigt: MSN angezeigt!)

**Dispatch notes**

- *VIEW*  
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create view](#create-view).

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
      Click this button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

        - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
            Click this entry to create a view. The *Create view* window is displayed.

        - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
          Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed if a view has been selected.

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

- Status  
    Click the drop-down list and select a dispatch note status. The following options are available:
    - **All statuses**  
        Select this option to display all dispatch notes, regardless of their status.
    - **New dispatch note**  
        Select this option to display all new dispatch notes.
    - **Transferred to partner**  
        Select this option to display all dispatch notes that have been transferred to the fulfiller.
    - **Partner confirmed receival**  
        Select this option to display all dispatch notes whose receival has been confirmed by the fulfiller.
    - **Dispatch note completed**  
        Select this option to display all dispatch notes that have been completed.
    - **Error**  
        Select this option to display all dispatch notes that have given an error.
    - **Void**  
        Select this option to display all void dispatch notes.

- Connections  
    Click the drop-down list and select a connection. The following options are available:
    - **All connections**  
        Select this option to display the dispatch notes for all configured connections. 
    - **Connection name**  
        Select this option to display the dispatch notes for the selected connection. When a specific connection has been selected, the **All connection** option is no longer displayed. Click the selected connection again to deselect it.  

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for dispatch notes.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dispatch notes.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dispatch notes in the list are selected.

- [VIEW]  
    Click this button to edit the selected dispatch note. This button is only displayed if a single checkbox in the list of dispatch notes is selected. Alternatively, you can click directly a row in the list to view the corresponding dispatch note. 
    The *Dispatch note "Dispatch note ID"* view is displayed, see [Dispatch note "Dispatch note ID"](#dispatch-note-dispatch-note-id). The *Attributes* tab is preselected.

- [EXPORT]  
    Click this button to export manually the dispatch note to the fulfiller. This button is displayed if the checkbox of at least one dispatch note is selected.

    > [Info] The dispatch note is exported automatically by the system. If the export fails, the dispatch note can be manually reexported. Nevertheless, this is not to be meant a usual procedure but an exceptional measure. For detailed information, see [Export a dispatch note](../Integration/01_ManageDispatchNote.md#export-a-dispatch-note).

- [FORCE COMPLETION]  
    Click this button to complete the dispatch note. This button is displayed if the checkbox of at least one dispatch note is selected.

The list displays all dispatch notes. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Connection*  
    Connection to fulfiller.

- *Document number*  
    Dispatch note number. This number equals the delivery note number in the *Order management* module.

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
        The dispatch note has given an error.
    - **Void**  
        The dispatch note is void.

- *Shipment status*  
    Status of shipment associated with the dispatch note. The following options are available:
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross)   
        No shipment yet. The associated dispatch note is new or has just been transferred to the fulfiller.
    - ![Circular arrows](../../Assets/Icons/CircularArrows.png "[Circular arrows]") (Circular arrows)   
        Waiting for shipment/Shipped/New Shipment. The fulfiller has confirmed receival of the dispatch note and the shipment will be arranged shortly.   
    - ![Double check](../../Assets/Icons/DoubleCheck.png "[Double check]") (Double check)    
        Delivered. The shipment has been delivered.
    - ![Error](../../Assets/Icons/Warning02.png "[Error]") (Error)    
        Error. The shipment has produced an error.
    - Empty  
        If the shipment status is void, the *Shipment status* is empty.

[comment]: <> (SW: Shipment status icons Standard oder kundenspezifisch/NoE? S. Zusammenhang Dispatch note - Shipment status. Error in Dispatch note und alle möglichen Shipment Status. Wieso ist das möglich?)

- *Description*  
    Dispatch note description as defined by the user. Numbers, letters or a combination of characters may be used. The information provided in this field can be entered in the search bar to search for a specific dispatch note.

- *Created*  
    Date and time of the creation.

- *Modified*  
    Date and time of the last modification.

- *ID*  
    Dispatch note identification number. The ID number is automatically assigned by the system.

- *Status ID*  
  Dispatch note status identifier. The following options are available:
    - **new**
    - **transferred**
    - **confirmed**
    - **completed**
    - **error**
    - **void**

- Attribute    
    You can add a column for each attribute that is assigned to the dispatch note. The column displays the attribute name, the row displays the corresponding attribute value of the dispatch note.


## Create view

*Fulfillment > Dispatch notes > Tab LIST > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Fulfillment/DispatchNotes/CreateView.png "[Create view]")

- *Name*   
    Enter a name for the view.

- [CANCEL]   
    Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]   
    Click this button to save the new view and display it in the *VIEW* drop-down list. The *Create view* window is closed.

This window can also be accessed from the following tabs in the user interface:

- [CONNECTIONS (Logging)](02a_Connections.md#create-view)
- [CONNECTIONS (Settings)](03a_Connections.md#create-view)
- [PACKAGE TYPES](03b_PackageTypes.md#create-view)

## Rename view

*Fulfillment > Dispatch notes > Tab LIST > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Fulfillment/DispatchNotes/RenameView.png "[Rename view]")

- *Name*   
    Click this field to edit the view name.

- [CANCEL]   
    Click this button to cancel renaming the view. The  *Rename view* window is closed.

- [SAVE]   
    Click this button to save the changes and display it in the *VIEW* drop-down list. The *Rename view* window is closed.

This window can also be accessed from the following tabs in the user interface:

- [CONNECTIONS (Logging)](02a_Connections.md#rename-view)
- [CONNECTIONS (Settings)](03a_Connections.md#rename-view)
- [PACKAGE TYPES](03b_PackageTypes.md#rename-view)


## Dispatch note "Dispatch note ID"

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note*

![Dispatch note ID](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteAttributes.png "[Dispatch note ID]")

**Dispatch note "Dispatch note ID"**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Dispatch note "Dispatch note ID"* view and return to the list of dispatch notes.  

- [CLOSE]  
    Click this button to close the *Dispatch note "Dispatch note ID"* view. The list of dispatch notes is displayed.


## Dispatch note "Dispatch note ID" &ndash; Attributes

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Attributes*

![Attributes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteAttributes.png "[Attributes]")

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the dispatch note contains attributes that are unassigned, the *Unassigned Group* group is automatically displayed in the left margin column.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. Depending on the attribute group selected, the fields displayed vary. The dispatch note attributes are imported via the fulfiller driver. All fields are locked and, therefore, read-only.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow *>* left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

[comment]: <> (HG: Diese Info ist nicht im Omni-Channel. Hinzufügen dort oder hier wegglassen?)

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
    Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


## Dispatch note "Dispatch note ID" &ndash; Dependencies

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Attributes*

![Dependencies](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteDependencies.png "[Dependencies]")

This tab has no function in the *Fulfillment* module, since dispatch notes have no dependent entities. The notice *No other entities depend on this entity* is displayed.

[comment]: <> (SW: Gar keine Dependencies möglich? Evtl. Standardbeschreibung des Reiters? S. Omni-Channel)


## Dispatch note "Dispatch note ID" &ndash; Shipments

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments*

![Shipments](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteShipments.png "[Shipments]")

[comment]: <> (SW: Unten beschriebene Felder aus NoE Test-Account. Was ist Standard?)


- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dispatch notes.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- *ID*  
    Shipment identification number. The ID number is automatically assigned by the system.

- *Carrier*  
    Carrier identification number.

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

- *Status info*  
    Additional status information. The following options are available:  
    - **Status changed via dispatch note**

[comment]: <> (SW: Option aus NoE. Gibt es andere Optionen oder ist es vom Kd eingestellt?)

- *Created*  
    Date and time of the creation.

- *Modified*    
    Date and time of the last modification.

- Attribute    
    You can add a column for each attribute that is assigned to the shipment. The column displays the attribute name, the row displays the corresponding attribute value of the shipment.


### Shipment attributes

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Sub-tab ATTRIBUTES*

![Shipments](../../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesAttributes.png "[Shipments]")

**Shipment "Shipment ID"**

- [BACK]  
    Click this button to go back to the previous step. The *Shipments* view is displayed.

### Shipment attributes &ndash; Attributes

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Sub-tab ATTRIBUTES > Tab Attributes*

![Shipment attributes](../../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesAttributes.png "[Shipment attributes]")

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the shipment contains attributes that are unassigned, the *Unassigned Group* group is automatically displayed in the left margin column.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. Depending on the attribute group selected, the fields displayed vary. All fields are locked and, therefore, read-only.

[comment]: <> (Vgl. The dispatch note attributes are imported via the fulfiller driver. -> Vermutlich Shipment info auch vom Fulfiller via Driver geschickt?)

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow *>* left to the attribute group to unfold the group and display the attribute sub-groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

[commnet]: <> (HG: Vereinheitlichen mit oben, Omni-Channel... Drin oder weglassen?)

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
    Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.

### Shipment attributes &ndash; Dependencies

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Sub-tab ATTRIBUTES > Tab Dependencies*

![Shipment dependencies](../../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesDependencies.png "[Shipment dependencies]")

This tab has no function in the *Fulfillment* module, since dispatch notes have no dependent entities. The notice *No other entities depend on this entity* is displayed.

[comment]: <> (SW: Vgl. Dependencies oben)

### Shipment packages

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Sub-tab PACKAGES*

![Shipments](../../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsPackages.png "[Shipments]")

The list displays all packages contained in the selected shipment. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Package type*  
    Package type identifier. Packages types can be defined in the *PACKAGE TYPES* tab of the *Settings* menu entry, see [Manage the package types](../Integration/02_ManagePackageTypes.md).

- *Created*  
    Date and time of the creation.

- *Modified*  
    Date and time of the last modification.

- *ID*  
    Package identification number. This number is automatically assigned by the system.

-  *Tracking number*  
    Package tracking number.

- *Tracking link*  
    Package tracking link.

- *Package ID*  
    Package identification number.

- *Proof of delivery*  
  Proof of delivery, if required.

- Attribute    
    You can add a column for each attribute that is assigned to the shipment package. The column displays the attribute name, the row displays the corresponding attribute value of the shipment package.
    
- *SSCC number*  
   Serial shipping container code number as defined by the fulfiller.

- *Shipping method*  
    Shipping method identification number as defined by the fulfiller.

- *Identifier override*  
    Identifier override value as defined by the fulfiller.

- *Shipping method override*  
    Shipping method override value as defined by the fulfiller.

- *Packaging type override*  
    Packaging type override value as defined by the fulfiller.

[comment]: <> (SW: Vermutlich ab SSCC alle Attribute)


#### Items

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Shipments > Sub-tab PACKAGES > Select a package*

![Shipments](../../Assets/Screenshots/Fulfillment/DispatchNotes/Items01.png "[Shipments]")

The list displays all items contained in the selected package. Depending on the settings, the displayed columns may vary. All fields are read-only.

[comment]: <> (Was sind Attribute?)

- *Item number*  
    Item identification number.

- *SKU*  
    Stock Keeping Unit. Identification number of the product.

- *Amount*  
    Amount of units contained in the item.

- *Serial number*  
    Item serial number.

- *ID*  
    Item identification number. The ID number is automatically assigned by the system.

- Attribute    
    You can add a column for each attribute that is assigned to the item. The column displays the attribute name, the row displays the corresponding attribute value of the item.

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

[comment]: <> (SW: Vermutlich ab Unit net value alle Attribute. Beschreiben?)

## Dispatch note "Dispatch note ID" &ndash; Logs

*Fulfillment > Dispatch notes > Tab LIST > Select a dispatch note > Tab Logs*

![Dispatch note logs](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteLogs.png "[Dispatch note logs]")

[comment]: <> (SW: Bug in Logs Tab? Unterschied zu Menüpunkt Logging?)

[comment]: <> (ggf. aus 02a_Connections.md kopieren oder verweisen?)




