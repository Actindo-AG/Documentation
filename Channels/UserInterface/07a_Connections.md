[!!Manage the connections](../Integration/01_ManageConnections.md)

# Connections

*Omni-Channel > Settings > Tab CONNECTIONS*

[comment]: <> (Datei Fulfillment/UserInterface/03a_Connections.md als Referenz. Ggf. Änderungen hier auch übernehmen)

![Connections](../../Assets/Screenshots/Channels/Settings/Connections/Connections.png "[Connections]")

**Connections**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of connections.


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


- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all connections in the list are selected.

- [DELETE]  
    Click this button to delete the selected connection. This button is only displayed if a single checkbox in the list of connections is selected.

[comment]: <> (Button funktioniert nicht. Ist es überhaupt vorgesehen, dass connections gelöscht werden können? Wenn nicht -> button raus, wenn doch -> unter welchen voraussetzungen?)

- [SYNCHRONIZE]  
    Click this button to synchronize the selected connection. This button is only displayed if a single checkbox in the list of connections is selected. The *Sync triggered* pop-up window is displayed.

    ![Sync triggered](../../Assets/Screenshots/Channels/Settings/Connections/SyncTriggered.png "[Sync triggered]")

- [DISABLE]  
    Click this button to disable the selected connection(s). This button is only displayed if the checkbox of at least one active connection is selected.

- [ENABLE]  
    Click this button to enable the selected connection(s). This button is only displayed if the checkbox of at least one inactive connection is selected. 

- ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit)  
    Click this button to edit the selected connection. This button is only displayed if a single checkbox in the list of connections is selected. Alternatively, you can click directly a row in the list to edit a connection. The *Edit connection* view is displayed, see [Edit connection](#edit-connection).


The list displays all available connections. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Name*  
    Connection name.

- *Status*  
    Connection status. The following statuses are available:
    - ![Status](../../Assets/Icons/Status01.png "[Status]") **Active**   
        The connection is enabled and data is being synchronized via the connection.
    - ![Status](../../Assets/Icons/Status04.png "[Status]") **Inactive**   
        The connection is disabled and no data is being synchronized via the connection.   

- *Order/Return have errors*  
    Indication whether errors have occurred in orders or  returns:. The following options are available:  
    - **Yes**   
        Errors have occurred.   
    - **No**   
        No errors have occurred.

- *Driver*  
    Driver name.

- *ID*  
    Connection identification number. The ID number is automatically assigned by the system.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)  
    Click this button to add a connection. The *Create connection* view is displayed, see [Create connection](#create-connection).


## Create connection

*Omni-Channel > Settings > Tab CONNECTIONS > Button Add*

![Create connection](../../Assets/Screenshots/Channels/Settings/Connections/CreateConnection.png "[Create connection]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Create connection* view and return to the connection list. All changes are rejected.

- *Name*   
    Enter a connection name.

- ![Apply](../../Assets/Icons/Check.png "[Apply]") (Apply)  
    Click this button to apply the entered connection name. This button is only displayed if the connection name has not yet been confirmed. 

[comment]: <> (Der button ist ziemlich sinnfrei: Auch wenn ich nicht den button klicke, aber anschließend auf SAVE klicke, werden Änderungen im Namen übernommen - wozu ist der also da?)

- ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit)  
    Click this button to edit the connection name. This button is only displayed if the connection name has been confirmed. 

- *Driver*  
    Click the drop-down list and select the desired driver. All installed drivers are displayed. Depending on the connection driver, a *Credentials* section is displayed below the drop-down list.

    > [Info] Drivers are licensed and must be acquired via the app store or the corresponding e-commerce partner platform. The applicable driver credentials to establish the connection are obtained when acquiring the corresponding license.


**Credentials**

The fields displayed in the *Credentials* section vary depending on the selected driver.

- [SAVE]  
    Click this button to save the connection.



## Edit connection

*Omni-Channel > Settings > Tab CONNECTIONS > Select a connection*

![Edit connection](../../Assets/Screenshots/Channels/Settings/Connections/EditConnection.png "[Edit connection]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Edit connection* view and return to the connection list. All changes are rejected.

- *Name*   
    Connection name. Click the button ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the name to edit it.

- ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit)  
    Click this button to edit the connection name.

- ![Apply](../../Assets/Icons/Check.png "[Apply]") (Apply)  
    Click this button to apply the changes to the connection name.  This button is only displayed if you are editing the connection name.

- *Created DD/MM/YYYY*  
    Creation date of the connection. This field is read-only.  


## Edit connection &ndash; Credentials

*Omni-Channel > Settings > Tab CONNECTIONS > Select a connection > Tab Credentials*

![Edit credentials](../../Assets/Screenshots/Channels/Settings/Connections/EditConnection.png "[Edit credentials]")

This tab is only displayed for drivers with further credentials.

- *Driver*  
    Selected driver name. This drop-down list is read-only.

**Credentials** 

The fields displayed in the *Credentials* section vary depending on the selected driver.

- [SAVE]  
    Click this button to save any changes made.


## Edit connection &ndash; Settings

*Omni-Channel > Settings > Tab CONNECTIONS > Select a connection > Tab Settings*

![Edit settings](../../Assets/Screenshots/Channels/Settings/Connections/Settings.png "[Edit settings]")

This tab is only displayed for drivers with further settings.
The fields displayed vary depending on the driver.

- [SAVE]  
    Click this button to save any changes made.

    > [Info] If no settings are available for the selected connection, the *There are no settings available* notice is displayed.


## Create view

*Omni-Channel > Settings > Tab CONNECTIONS > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Channels/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./02a_Offers.md#create-view).


## Rename view

*Omni-Channel > Settings > Tab CONNECTIONS > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Channels/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./02a_Offers.md#rename-view).
