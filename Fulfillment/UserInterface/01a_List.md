# List

![Dispatch notes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Dispatch notes]")

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

[comment]: <> (Reset auch hier verfügbar?)

- Status drop-down list  
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
  Select this option to displays all dispatch notes that have been completed.
  - **Error**  
  Select this option to display all dispatch notes that have given an error.
  - **Void**  
  Select this option to display all void dispatch notes.


- Connections drop-down list  
  Click the drop-down list and select a connection. The following options are available:
  - *All connections*  
  Select this option to display all configured connections.
  - **Connection name**
  Select this option to display the dispatch notes corresponding to the selected fulfiller.


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
  Click this button to edit the selected dispatch note. This button is only displayed if a single checkbox in the list is selected. Alternatively, you can click directly a row in the list to view a dispatch note. The *Dispatch note "Number"* view is displayed.

- [EXPORT]
  Click this button to export manually the dispatch note to the fulfiller. This button is displayed if the checkbox of at least one dispatch note is selected.

  > [Info] The dispatch note is exported automatically by the system. If the export fails for some reason, the dispatch note can be manually reexported. Nevertheless, this is not a standard procedure but a troubleshooting measure. For detailed information, see [Export dispatch note to fulfiller](../Troubleshooting/01_ExportDispatchNoteFulfiller.md).

  - [FORCE COMPLETION]  
  Click this button to complete the dispatch note.  This button is displayed if the checkbox of at least one dispatch note is selected.

  [comment]: <> (Test, mehr Info dazu)

The list displays all dispatch notes. Depending on the settings, the displayed columns may vary. All fields are read-only.


- *Connection*  
  Connection to fulfiller.

- *Document number*  
  Dispatch note number.

- *Status*  
  Dispatch note status. The following statuses are available:
  - *All statuses*

  - *New dispatch note*

  - *Transferred to partner*

  - *Partner confirmed receival*

  - *Dispatch note completed*

  - *Error*

  - *Void*


- *Shipment status*  
  Status of shipment linked to the dispatch note. The following options are available:
  - ![Filter](../../Assets/Icons/Cross02.png "[Cross]")  
  No shipment yet (new dispatch note or transferred to partner)

  - ![Filter](../../Assets/Icons/CircularArrows.png "[Circular arrows]")
  Waiting for shipment

  - ![Filter](../../Assets/Icons/DoubleCheck.png "[Double check]")
  	Delivered

  - ![Filter](../../Assets/Icons/Warning02.png "[Error]")
    Error

  - Empty  
    If the shipment status is void, the *Shipment status* is empty.

- *Description*
- *Modified*
- *Carrier*
- *Shipping method*
- *Package type*
- *Shipping type*
- *Receiver name*
- *Receiver zip*
- *ID*
- *Status ID*
- *Created*
- *Carrier*

[comment]: <> (Abweichungen zwischen meinem Sandbox und NoE Textaccount - Standard vs. kundenspezifisch? RS S. Walke)

## Dispatch note "Number"

Attributes
Fulfillment dispatch note base attributes
Receiver name
Receiver zip
Package type

Dependencies
Dependent entity ID
Change tracking
Dependent entity friendly identifier

Shipments
ID
Carrier
Connection
External ID
Status
Status info
Modified
Created
Receiver name
Receiver zip
Tracking numbers
Tracking URLs
Proof of delivery
Parcels
Error date
Error message

CLOSE
