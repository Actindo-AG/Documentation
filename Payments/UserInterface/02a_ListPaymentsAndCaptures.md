[!!Monitor payments and captures](../Operation/02_ManagePaymentsAndCaptures.md)


# LIST (Payments and captures)

*Payments > Authorizations > Tab LIST*

![LIST (Payments and captures)](../../Assets/Screenshots/Payments/PaymentsCaptures/LISTPaymentsCaptures.png "[LIST (Payments and captures)]")
*Authorizations**

- *VIEW*  
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

        - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
            Click this entry to create a view. The *Create view* window is displayed, see [Create view](#create-view).

        - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
            Click this entry to rename the selected view. The *Rename view* window is displayed, see [Rename view](#rename-view). This menu entry is only displayed if a view has been selected.

        <!---- Eintrag gibt es nicht mehr [Reset](../../Assets/Icons/Reset.png "[Reset]") reset  
            Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.--->

        - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish  
            Click this entry to publish the view. This menu entry is only displayed if you have selected an unpublished view. As long as you have not published a view, your views are visible for you only.

        - ![Unpublish](../../Assets/Icons/Unpublish.png "[Unpublish]") unpublish  
            Click this entry to unpublish the view so that it is visible only to you again. This menu entry is only displayed if you have selected and published a view.

        - ![Save](../../Assets/Icons/Save.png "[Save]") save  
            Click this entry to save the current view settings in the selected view. This menu entry is only displayed if you have selected a view.

            > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

        - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete  
            Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed if you have selected a view.   
 

- *Connections*   
    Click the drop-down list to select a connection. The following options are available:
    - **All connections**  
        Select this option to display payment and capture transactions for all configured connections. 
    - **Connection name**  
        Select this option to display payment and capture transactions for the selected connection. When a specific connection has been selected, the **All connections** option is no longer displayed. Click the selected connection again to deselect it.  



- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for authorization transactions.   


- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of authorization transactions.   

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and to customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.   
    > [Info] It is recommended to add the following columns to your view to get the required information and to better filter and sort the entries: Status ID, Status information (if applicable).    

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.  

- [x]     
    Select the checkbox to the left of one list entry to display the editing toolbar for this single entry.   
    If you click the checkbox in the header, all entries in the list are selected. The editing toolbar shows all actions you can perform on several entries.   

- [REFUND]   
   Click this button to refund the payment manually, so that the order process can be continued. For detailed information, see [Refund payment and capture](../Operation/02_ManagePaymentsAndCaptures.md#refund-payments-and-capture-transaction).   

- [VOID]   
  Click this button to disable the transaction for the Actindo database. For detailed information, see [Void payment and capture transaction](../Operation/02_ManagePaymentsAndCaptures.md#void-payment-and-capture-transaction).


The list displays all capture transactions. Depending on the payment service provider, the displayed columns vary. All fields are read-only. The following standard columns are available.
<!----Liste der Standardfelder aus den Authorizations kopieren--->



## Payments and captures

*Payments > Payments and captures > Tab LIST > Select a payment and capture transaction*

![Authorization ID](../../Assets/Screenshots/Payments/PaymentsCaptures/AttributesPaymentsCaptures.png "[Authorization ID]")

**Payment and Capture transaction "Capture ID"**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Capture ID* view and return to the list of payment and capture transactions. 

## Payments and captures &ndash; Attributes

*Payments > Payments and captures > Tab LIST > Select a payment and capture transaction*   

![Attributes](../../Assets/Screenshots/Payments/Authorizations/AuthorizationAttributes.png "[Attributes]")

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the authorization transaction contains attributes that are not assigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to expand the group and to display the attribute sub-groups. The following sub-groups are available:
    - *[Payment service provider] Incoming Payment Base Data*   
      This folder contains attributes that are specific for the payment service provider.   

    - *Incoming Payment Base Data*   
      This folder contains general attributes that Actindo needs to query payments data. These data support standard functions of Actindo.   

    - *Unassigned Group*   
      This folder contains attributes that are not assigned the other groups.   

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)   
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. Depending on the selected attribute group, the displayed fields may vary. The attributes are imported by the payment service provider driver. All fields are read-only.   

- ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded. This is available for the *Unassigned Group* folder only.



## Payments and captures &ndash; Dependencies

![Dependencies](../../Assets/Screenshots/Payments/PaymentsCaptures/DependenciesPaymentsCaptures.png "[LIST &ndash; Dependencies]")   

Since a payment and capture transaction has no dependencies to other entities in Actindo by default, this sub-tab is not relevant.



## Payments and captures &ndash; Logs

![Logs](../../Assets/Screenshots/Payments/PaymentsCaptures/LogPaymentCaptures.png "[LIST &ndash; Dependencies]")   

This tab displays messages and intents that have been created during transferring the selected payment and capture transaction from the payment service provider.    
In contrast to the messages that are provided with the *Logging* menu entry, you see here the logging for the specific payment and capture transaction only. See [LIST (Logging)](./07a_ListLogging.md) for detailed information on fields and functions.   



## Create view

*Payments > Payments and captures > Tab LIST > Button Points > Menu entry "create"*

![Create view](../../Assets/Screenshots/Payments/LIST/CreateView.png "[Create view]")

- *Name*   
    Enter a name for the view.

- [CANCEL]   
    Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]   
    Click this button to save the new view and display it in the *VIEW* drop-down list. The *Create view* window is closed.



## Rename view

*Payments > Payments and captures > Tab LIST > Button Points > Menu entry "rename"*

![Rename view](../../Assets/Screenshots/Payments/LIST/RenameView.png "[Rename view]")

- *Name*   
    Click this field to edit the view name.

- [CANCEL]   
    Click this button to cancel renaming the view. The *Rename view* window is closed.

- [SAVE]   
    Click this button to save the changes and display the new name in the *VIEW* drop-down list. The *Rename view* window is closed.

