# Manage the Fiege connection

To establish a connection to Fiege fulfillment system, there are several particularities to consider. Therefore, the creation and the configuration of the Fiege connection are described in detail below.

## Create a Fiege connection

Create the connection to Fiege fulfillment system using the Fiege driver. Further settings can only be configured after the connection has been established.

All necessary credentials and information to establish the connection are provided by Fiege.

#### Prerequisites

The *Fiege* driver has been installed in the Core1 account.

> [Info] The current driver version is custom-designed by Fiege and can only be installed in the Core1 with the collaboration of the Actindo IT department.

[comment]: <> (Stand: 23.02.2023)

#### Procedure

*Fulfillment > Settings > Tab CONNECTIONS*

![Connection](../../Assets/Screenshots/Fulfillment/Settings/Connections/Connections.png "[Connection]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create connection* view is displayed.

    ![Create connection](../../Assets/Screenshots/Fulfillment/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the *Fiege Driver* option.  
    The *Credentials* section is displayed below the drop-down list.

    ![Connection credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/CreateConnectionCredentials.png "[Connection credentials]")

4. Enter the bearer token as provided by Fiege in *Bearer token (fiegeExport)* field.  

5. Click the [SAVE] button.  
    The connection will be established. The *Checking credentials...* notice is displayed. After a few seconds, the *Loading data...* notice is displayed.

    ![Checking credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/CheckingCredentials.png "[Checking credentials]")

    The *Create connection* view is automatically closed when the connection has been established. The *Edit connection* view of the newly created connection is displayed. The *Settings* tab is preselected.

    > [Info] By default, all connections that have been established are first inactive and therefore must be enabled after the connection configuration.    

[comment]: <> (Check, ob Checking credentials und Loading data Nachrichten bei Fiege auch vorkommen)

[comment]: <> (Ist es möglich, noch ein Screenshot hier hinzufügen? Direkt nach der Erstellung, Settings tab noch nicht ausgefüllt?)

6. Proceed to configure the connection, see [Configure the Fiege connection](#configure-the-fiege-connection).


## Configure the Fiege connection

After the Fiege connection has been established, further settings must be configured.

#### Prerequisites

- A Fiege connection has been established, see [Create a Fiege connection](#create-a-fiege-connection).
- The warehouses to be managed by Fiege have been configured in the *Warehouse* module. 
- The corresponding order workflows have been defined in the *Workflows* module.

[comment]: <> (Unsicher von Workflows - prerequisite für die Settings?)

#### Procedure

*Fulfillment > Settings > Tab CONNECTIONS*

![Fiege connection](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/Connections.png "[Fiege connection]")

1. Click the Fiege connection to be edited in the list of connections.  
The *Edit connection* view is displayed. By default, the *Credentials* tab is selected.

    ![Edit connection credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/EditConnectionCredentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.
    The *Settings* tab is displayed. By default, the *Warehouse ID fallback* menu entry is selected.

    ![Connection](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/EditConnectionSettings_WarehouseIDFallback.png "[Connection]")

3. Enter the number of the warehouse to be used as fallback warehouse for stock movements if no other reference is found. 

    > [Info] The warehouse numbers configured in the Core1 can be found in the *Warehouse* module: *Warehouse > Settings > Warehouse master data > Select a warehouse > Basic data*

4. Click the *Bearer token* menu entry in the left side bar.  
    The bearer token settings are displayed on the right side.  

    ![Settings bearer token](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/EditConnectionSettings_BearerToken.png "[Settings bearer token]")

5. Enter the bearer token for authentication with the Fiege API as provided by Fiege in the *Bearer token* field.

[comment]: <> (Unsicher, ob beide bearer token eingetragen werden müssen -Credentials und Settings, oder nur eins davon, oder ob sie gleich oder unterschiedlich sind. Evtl. check mit Simon)

6. Click the *A Warehouse* menu entry in the left side bar.  
    The A Warehouse settings are displayed on the right side.  

    ![Settings A warehouse](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/EditConnectionSettings_AWarehouse.png "[Settings A warehouse]")

7. Enter the number of the warehouse to be used as A warehouse.  

8. Click the *B Warehouse* menu entry in the left side bar.  
    The B Warehouse settings are displayed on the right side.  

    ![Settings B warehouse](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/EditConnectionSettings_BWarehouse.png "[Settings B warehouse]")

9. Enter the number of the warehouse to be used as B warehouse.

10. Click the *C Warehouse* menu entry in the left side bar.  
    The C Warehouse settings are displayed on the right side.  

    ![Settings C warehouse](../../Assets/Screenshots/Fulfillment/Settings/Connections/Fiege/EditConnectionSettings_CWarehouse.png "[Settings C warehouse]")

11.  Enter the number of the warehouse to be used as C warehouse.

12. Click the [SAVE] button.  
    All changes have been saved. The *Saving successful* pop-up window is displayed.  

    ![Saving successful](../../Assets/Screenshots/Channels/Settings/Connections/SavingSuccessful.png "[Saving successful]")

[comment]: <> (Unsicher, ob das in Fulfillment/Fiege stimmt. Check mit Simon.)
  
13. When necessary, proceed to enable the connection, see [Enable a connection](./01_ManageConnections.md#enable-a-connection).