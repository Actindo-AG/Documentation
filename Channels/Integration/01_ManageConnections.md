[!!User Interface Connections](../UserInterface/to_be_completed)

# Manage the connections

Establish connections via drivers to connect your marketplaces with the *Actindo Core1 Platform*. A marketplace can be either an online shop or a point of sale. You can establish an unlimited number of connection per driver.

In the following, the general settings to create, edit, synchronize or disable connections are described. For certain connection drivers, you have to setup special configurations. Therefore, the connections below are described in separate documents:
- Shopware 6 connection
- Shopify connection
- Sales Force Commerce Cloud connection
- Amazon connection
- Magento 2 connection
- Tradebyte connection
- Scayle connection
- eBay connection

[comment]: <> (Links zu Connections einfügen)

## Create a connection

Create a connection to a certain marketplace. As soon as a connection has been established, an initial synchronization will be triggered, which will transfer the entire data model of the connected marketplace mirrored to Actindo. This means that all attributes and attribute sets from the marketplace are also transferred to Actindo and can be accessed in the *DataHub* module. Depending on the marketplace to be connected, special configurations may be necessary.

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

  > [Info] Drivers must be purchased from the main account and then be installed separately in each sandbox or account where you want to use it. For detailed information, see [Manage the drivers](to_be_completed).

  Depending on the driver, a *Credentials* section is displayed below the drop-down list.

  ![Credentials](../../Assets/Screenshots/Channels/Settings/Connections/Credentials.png "[Credentials]")

  > [Info] Depending on the driver of the connection, the fields in the *Credentials* section differ.

4. If necessary, enter the required data in the fields in the *Credentials* section.

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

3. If necessary, click the *Settings* tab and edit the desired settings of the connection in the corresponding fields.

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

#### Prerequisites

- At least one connection has been established, see [Create a connection](#create-a-connection).
- The connection is active.

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Channels/Settings/Connections/Connections.png "[Connections]")

1. Select the checkbox of the connection you want to disable in the list of connections.   
  The editing toolbar is displayed above the list of connections.

2. Click the [DISABLE] button in the toolbar.   
  The connection has been deactivated.

3. Click the (Refresh) button to update the list of connections.   
  The status of the disabled connection in the *Status* column has switched to **Inactive**.
