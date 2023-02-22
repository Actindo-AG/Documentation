[!!User interface Connections](../UserInterface/07a_Connections.md)

# Manage the connections

Establish connections via drivers to connect your marketplaces with the *Actindo Core1 Platform*. A marketplace can be either an online shop or a point of sale. You can establish an unlimited number of connections per driver.

In the following, the general settings to create, edit, synchronize or disable connections are described. For certain connection drivers, you have to set up special configurations. Therefore, the connections below are described in separate documents:
- [Shopware 6 connection](./01a_Shopware6.md)
- [Shopify connection](./01b_Shopify.md)
- [Sales Force Commerce Cloud connection](./01c_Salesforce.md)
- [Amazon connection](./01d_Amazon.md)
- [Magento 2 connection](./01e_Magento2.md)
- [Tradebyte connection](./01f_Tradebyte.md)
- [Scayle connection](./01g_Scayle.md)
- [eBay connection](./01h_eBay.md)


## Create a connection

Create a connection to a certain marketplace. As soon as a connection has been established, an initial synchronization will be triggered, which will transfer the entire data model of the connected marketplace mirrored to Actindo. This means that all attributes and attribute sets from the marketplace are also transferred to Actindo and can be accessed in the *DataHub* module. Depending on the marketplace to be connected, special configurations are necessary.

[comment]: <> (POS auch in eigener Procedure erklären?)

#### Prerequisites

At least one driver has been installed.

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connection](../../Assets/Screenshots/Channels/Settings/Connections/Connection.png "[Connection]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create connection* view is displayed.

    ![Create connection](../../Assets/Screenshots/Channels/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the desired driver. All available drivers are displayed in the list.   

    > [Info] Drivers must be purchased from the main account and then be installed separately in each sandbox or account where you want to use it.    
    For detailed information, see [Manage the drivers](to_be_completed).

    Depending on the selected driver, a *Credentials* section is displayed below the drop-down list.

    ![Credentials](../../Assets/Screenshots/Channels/Settings/Connections/Credentials.png "[Credentials]")

    > [Info] Depending on the selected driver, the fields in the *Credentials* section differ.

4. If available, enter the required data in the fields in the *Credentials* section.

5. Click the [SAVE] button.    
    The connection will be established. The *Checking credentials...* notice is displayed.

    ![Credentials](../../Assets/Screenshots/Channels/Settings/Connections/CheckingCredentials.png "[Credentials]")

    The *Create connection* view is automatically closed when the connection has been established. The initial sync has been automatically triggered. The *Sync triggered* pop-up window is displayed.

    ![Sync triggered](../../Assets/Screenshots/Channels/Settings/Connections/SyncTriggered.png "[Sync triggered]")


## Edit a connection

Edit a connection to adjust any changed credentials, the connection name or further settings. The driver selection is read-only and cannot be edited.

#### Prerequisites

At least one connection has been established, see [Create a connection](#create-a-connection).

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Channels/Settings/Connections/Connections.png "[Connections]")

1. Click the connection you want to edit in the list of connections.   
    The *Edit connection* view is displayed.

    > [Info] Depending on the driver of the connection, the *Credentials* and the *Settings* tab are displayed in the *Edit connection* view.

    ![Edit connection](../../Assets/Screenshots/Channels/Settings/Connections/EditConnection.png "[Edit connection]")

2. Edit the desired data of the connection in the corresponding fields in the *Credentials* tab.

3. If available, click the *Settings* tab and edit the desired settings of the connection in the corresponding fields.

4. Click the [SAVE] button.   
    The *Checking credentials...* notice is displayed.

    ![Credentials](../../Assets/Screenshots/Channels/Settings/Connections/CheckingCredentials.png "[Credentials]")

    The *Edit connection* view is automatically closed when the changes have been saved. The sync has been automatically triggered. The *Sync triggered* pop-up window is displayed.

    ![Sync triggered](../../Assets/Screenshots/Channels/Settings/Connections/SyncTriggered.png "[Sync triggered]")



## Synchronize a connection

If any changes have been made in the marketplace, it is necessary to synchronize the connection to apply these changes to the *Actindo Core1 Platform*.

#### Prerequisites

At least one connection has been established, see [Create a connection](#create-a-connection).

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Channels/Settings/Connections/Connections.png "[Connections]")

1. Select the checkbox of the connection you want to synchronize in the list of connections.   
    The editing toolbar is displayed above the list of connections.

2. Click the [SYNCHRONIZE] button in the toolbar.   
    The sync has been started. The *Sync triggered* pop-up window is displayed.

    ![Sync triggered](../../Assets/Screenshots/Channels/Settings/Connections/SyncTriggered.png "[Sync triggered]")

    > [Info] It may take several minutes until the sync has been completed. Click the ![Processes](../../Assets/Icons/Process.png "[Processes]") (Processes) button in the header to check for currently running jobs.



## Disable a connection

Once a connection has been established, it cannot be deleted. Nevertheless, the connection can be disabled to prevent any further data from being synchronized via the connection.

[comment]: <> (Stimmt es, dass connections nicht mehr gelöscht werden können? Warum gibt es dann einen Delete button?)

#### Prerequisites

- At least one connection has been established, see [Create a connection](#create-a-connection).
- The connection is active.

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Channels/Settings/Connections/Connections.png "[Connections]")

1. Select the checkbox of the connection you want to disable in the list of connections.   
    The editing toolbar is displayed above the list of connections.

2. Click the [DISABLE] button in the editing toolbar.   
    The connection has been deactivated.

3. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the top right corner to update the list of connections.   
    The status of the disabled connection in the *Status* column has switched to **Inactive**.



## Enable a connection

A connection can only be used if it is active. Otherwise, no data is being synchronized via the connection. By default, all connection that has been established are active. If a connection has been disabled, you can enable this connection again.

#### Prerequisites

At least one connection has been disabled, see [Disable a connection](#disable-a-connection).

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Channels/Settings/Connections/Connections.png "[Connections]")

1. Select the checkbox of the connection you want to enable in the list of connections.   
    The editing toolbar is enabled above the list of connections.

2. Click the [ENABLE] button in the editing toolbar.   
    The connection has been activated.

3. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the top right corner to update the list of connections.   
    The status of the enabled connection in the *Status* column has switched to **Active**.