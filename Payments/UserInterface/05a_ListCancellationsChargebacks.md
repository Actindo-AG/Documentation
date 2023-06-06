[!!Monitor cancellations and chargebacks](../Operation/04_ManageCancellationsChargebacks.md)


# LIST (Cancellations and chargebacks)

*Payments > Authorizations > Tab LIST*

![LIST (Cancellations and chargebacks](../../Assets/Screenshots/Payments/Authorizations/LISTAuthorizations.png "[LIST (Cancellations and chargebacks)]")

**Refunds**

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
        Select this option to display authorization transactions for all configured connections. 
    - **Connection name**  
        Select this option to display authorization transactions for the selected connection. When a specific connection has been selected, the **All connections** option is no longer displayed. Click the selected connection again to deselect it.  


The list displays all cancellation and chargeback transactions. Depending on the payment service provider, the displayed columns vary. All fields are read-only. The following standard columns are available.
<!----Hallo Stefan, hier sollten alle Standard-Felder mit Erklärungen stehen, ist die Liste vollständig?--->
- *Charges intended use*   
   Purpose of the fee.
- *Original currency*   
   Currency in which the product(s) were paid 
- *Original currency amount*   
   Invoice amount in the original currency



## Cancellations and chargebacks

*Payments > Refunds > Tab LIST > Select a cancellation and chargeback transaction*

![Cancel ID](../../Assets/Screenshots/Payments/CancellationsChargebacks/AttributesCancellationsChargebacks.png "[Cancel ID]")

**Cancellations and chargebacks transaction "Cancel ID"**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Cancel ID* view and return to the list of cancellation and chargeback transactions. 



## Cancellations and chargebacks &ndash; Attributes
![Attributes ](../../Assets/Screenshots/Payments/CancellationsChargebacks/AttributesCancellationsChargebacks.png "[LIST &ndash; Attributes)]")

In the left margin column, all available attribute groups are displayed. Click a group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the cancellation and chargeback transaction contains attributes that are not assigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

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



## Cancellations and chargebacks &ndash; Dependencies  

![Dependencies](../../Assets/Screenshots/Payments/CancellationsChargebacks/AttributesCancellationsChargebacks.png "[Dependencies]")

Since a refund transaction has no dependencies to other entities in Actindo by default, this sub-tab is not relevant.



## Cancellations and chargebacks &ndash; Logs

![Logs](../../Assets/Screenshots/Payments/CancellationsChargebacks/LogCancellationsChargebacks.png "[Logs)]")

This tab displays messages and intents that have been created during transferring the selected cancellation and chargeback transaction from the payment service provider.    
In contrast to the messages that are provided with the *Logging* menu entry, you see here the logging for the specific refund transaction only. See [LIST (Logging)](./07a_ListLogging.md) for detailed information on fields and functions.   