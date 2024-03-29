[!!Manage confirmations](../Operation/05_ManageConfirmations.md)


# LIST (Confirmations)

*Payments > Confirmation > Tab LIST*

![LIST (Confirmations)](../../Assets/Screenshots/Payments/Confirmations/LISTConfirmations.png "[LIST (Confirmations)]")

**Confirmations**

- *VIEW*  
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *VIEW* drop-down list to display the context menu. The following menu entries are available:

        - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
            Click this entry to create a view. The *Create view* window is displayed, see [Create view](./06a_ListConfirmations.md#create-view).

        - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
            Click this entry to rename the selected view. The *Rename view* window is displayed, see [Rename view](./06a_ListConfirmations.md#rename-view). This menu entry is only displayed if a view has been selected.

        - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset  
            Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

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
    
- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
   Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.  

- [x]     
   Select the checkbox to the left of one list entry to display the editing toolbar for this single entry.   
   If you click the checkbox in the header, all entries in the list are selected. The editing toolbar shows then all actions you can perform on several entries.

- [EXECUTE]   
  Click this button to release the refund. You can execute several transactions at once. For detailed information, see [Execute confirmation transaction](../Operation/05_ManageConfirmations.md#execute-confirmation-transaction).

- [REJECT]   
  Click this button to reject the refund. You can reject several transactions at once. For detailed information, see [Reject confirmation transaction](../Operation/05_ManageConfirmations.md#reject-confirmation-transaction).

- [VOID]   
  Click this button to invalidate the transaction for the Actindo database. For detailed information, see [Void confirmation transaction](../Operation/05_ManageConfirmations.md#void-confirmation-transaction).  

The list displays all confirmation transactions. Depending on the payment service provider, the displayed columns vary. All fields are read-only. The following standard columns are available.   

- *External ID*   
   ID given by the payment service provider.

- *Original reference*   
   Reference to the authorization transaction. You can use this reference to follow up one payment over the entire process.

- *Type*   
   Kind of the displayed transaction, in this case a confirmation transaction.   

- *Connection*    
     Name of the Connection. Note that this is the customer-specific name that has been given the connection. For detailed information, see [Manage connections to payment service providers (PSP)](../Integration/01_ManageConnection.md).    

- *Created by*   
    Username of the person or API who has created the transaction. Can be a real user or an API user.   

- *Modified by*
    Username of the person or API who has changed the transaction. Can be a real user or an API user.

- *ID*   
   Unique transaction identification. The ID is automatically assigned by the system. 

- *Status ID*   
   Identifier of the status. The following status ID is available, each prefixed by the ID in the list below:
     - **2 - Confirmation required**   
        A refund is reserved but not yet released by an Actindo user.      

- *Status*
   Description of the transaction status.   

- *Connection ID*   
   ID of the connection.   

- *Created At*   
   Date and time when the payment service provider has created the transaction. 

- *Modified At*   
   Date and time when the payment service provider has modified the transaction.   

- *Currency*   
   Currency in which the payment will be posted.    

- *Amount*   
   Invoice amount of the payment in the currency in which the payment will be posted.    

- *Reference*  
   Mostly, depending on the payment service provider, the order number. 

- *Name*   
   First name of the person who has made the payment.   

- *Surname*   
   Last name of the person who has made the payment.   

- *Company*   
   Name of the company on whose behalf the payment was made.    

- *Address*   
   Street and house number of the address.  

- *Postal Code*   
   Zip code of the address.   

- *City*   
   City of the address.    

- *State*   
   If applicable, state of the address.

- *Country*   
   If applicable, country of the address.    

- *Payment Method*   
    The way of payment that the customer has chosen, for example, credit card, PayPal&trade;, direct debit.

- *Status Information*   
   If applicable, specific information on the status of the transaction.  

- *Internal Reference*    
    Actindo-specific reference back to the billing document.

- *Due Date*     
    If applicable, date on which the payment is to be collected.

## Confirmation

*Payments > Confirmation > Tab LIST > Select a confirmation transaction*

![Attributes](../../Assets/Screenshots/Payments/Confirmations/AttributesConfirmation.png "[Attributes]")

**Confirmation "Refund ID"**

![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
Click this button to close the *Refund ID* view and return to the list of confirmation transactions. 

## Confirmation &ndash; Attributes

*Payments > Confirmation > Tab LIST > Select a confirmation transaction > Tab Attributes*

![Attributes](../../Assets/Screenshots/Payments/Confirmations/AttributesConfirmation.png "[Attributes]")


In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. 

- ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Attribute group that contains attribute sub-groups. Click the attribute group or the arrow left to the attribute group to expand the group and display the attribute sub-groups. The following sub-groups are available:
    - *[Payment service provider] Outgoing Payment Base Data*   
      This folder contains attributes that are specific for the payment service provider.
    - *Outgoing Payment Base Data*   
      This folder contains general fields that Actindo needs to query payments data. These data support standard functions of Actindo. See the description of the fields above.
    - *Unassigned Group*   
      This folder contains attributes that are not assigned the other groups.

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Attribute group. Click the attribute group to display all attributes that are assigned to the selected attribute group on the right side of the *Attributes* tab.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column. Depending on the selected attribute group, the displayed fields may vary. The attributes are imported by the payment service provider driver. All fields are read-only.   

 ![Collapse/Expand](../../Assets/Icons/CollapseExpand01.png "[Collapse/Expand]") (Collapse/Expand)    
    Click this button to collapse or expand the left margin column with the attribute groups. When the left margin is expanded and you click this button, the column is collapsed. When the column is collapsed and you click this button, the column is expanded. This is available for the *Unassigned Group* folder only.


## Confirmation &ndash; Dependencies

*Payments > Confirmation > Tab LIST > Select a confirmation transaction > Tab Dependencies*

![Dependencies](../../Assets/Screenshots/Payments/Confirmations/DependenciesConfirmation.png "[Dependencies]")

Since a confirmation transaction has no dependencies to other entities in Actindo by default, this sub-tab is not relevant.



## Create view
*Payments > Confirmation > Tab LIST > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Payments/LIST/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./01a_ListAuthorizations.md#create-view).



## Rename view

*Payments > Confirmation > Tab LIST > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Payments/LIST/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./01a_ListAuthorizations.md#rename-view).
