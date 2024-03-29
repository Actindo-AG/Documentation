[!!Manage the connections](../../Fulfillment/Integration/01_ManageConnections.md)
[!!User interface Connections](../UserInterface/01_Connections.md)

# Manage the Fiege connection

To establish a connection to Fiege fulfillment system, there are several particularities to consider. Therefore, the creation and the configuration of the Fiege connection are described in detail below.

## Create a Fiege connection

Create the connection to Fiege fulfillment system using the Fiege driver. Further settings can only be configured after the connection has been established.

All necessary credentials and information to establish the connection are provided by Fiege.

#### Prerequisites

The *Fiege Integration* driver has been installed.

> [Info] The current driver version is custom-designed by Fiege and can only be installed in the Core1 with the collaboration of the Actindo IT department.

[comment]: <> (Stand: 23.02.2023)

#### Procedure

*Fulfillment > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Fulfillment/Settings/Connections/Connections.png "[Connections]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create connection* view is displayed.

    ![Create connection](../../Assets/Screenshots/Fulfillment/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the *Fiege Driver* option.  
    The *Credentials* section is displayed below the drop-down list.

    ![Create connection credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/CreateConnectionCredentials.png "[Create connection credentials]")

4. Enter the bearer token in the *Bearer token (fiegeExport)* field.  

5. Click the [SAVE] button.  
    The connection will be established. The *Checking credentials...* notice is displayed. After a few seconds, the *Loading data...* notice is displayed.

    ![Checking credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/CheckingCredentials.png "[Checking credentials]")

    The *Create connection* view is automatically closed when the connection has been established. The *Edit connection* view of the newly created connection is displayed. The *Settings* tab is selected.

    ![Settings warehouse ID fallback](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionSettings_WarehouseIDFallback.png "[Settings warehouse ID fallback]")

    > [Info] By default, all connections that have been established are inactive and must be enabled after the connection configuration, see [Enable a connection](./01_ManageConnections.md#enable-a-connection).

6. If necessary, continue to configure the Fiege connection, see [Configure the Fiege connection](#configure-the-fiege-connection).


## Configure the Fiege connection

After the Fiege connection has been established, further settings can be configured.

#### Prerequisites

- A Fiege connection has been established, see [Create a Fiege connection](#create-a-fiege-connection).
- The warehouses to be managed by Fiege have been configured in the *Warehousing* module. 

#### Procedure

*Fulfillment > Settings > Tab CONNECTIONS*

![Fiege connection](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/Connections.png "[Fiege connection]")

1. Click the Fiege connection to be configured in the list of connections.  
The *Edit connection* view is displayed. By default, the *Credentials* tab is selected.

    ![Edit connection credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionCredentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.   
    The *Settings* tab is displayed. By default, the *Warehouse ID fallback* menu entry is selected.

    ![Settings warehouse ID fallback](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionSettings_WarehouseIDFallback.png "[Settings warehouse ID fallback]")

3. Enter the ID of the warehouse to be used as a fallback warehouse for stock movements if no other reference is found. 

    > [Info] The warehouse IDs configured in Actindo can be found in the *Warehousing* module: *Warehousing > Settings > Warehouse master data > Select a warehouse > Basic data*

4. Click the *Bearer token* menu entry in the left side bar.  
    The bearer token settings are displayed on the right side.  

    ![Settings bearer token](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionSettings_BearerToken.png "[Settings bearer token]")

5. The bearer token is no longer relevant at this point, as it has already been entered in the *Credentials* section. Therefore, this field can be left blank.  

[comment]: <> (Feedback von Development: Bearer token wird aus den Settings in Zukunft abgebaut und nur noch in den Credentials angezeigt werden. Da noch in UI angezeigt, ist es hier noch beschrieben. Text anpassen bzw. löschen, wenn abgebaut.)

6. Click the *A Warehouse* menu entry in the left side bar.  
    The warehouse settings for warehouse A are displayed on the right side.  

    ![Settings A warehouse](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionSettings_AWarehouse.png "[Settings A warehouse]")

7. Enter the ID of the warehouse to be used as warehouse A in the *Warehouse ID A* field.  

8. Click the *B Warehouse* menu entry in the left side bar.  
    The warehouse settings of the warehouse B are displayed on the right side.  

    ![Settings B warehouse](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionSettings_BWarehouse.png "[Settings B warehouse]")

9. Enter the ID of the warehouse to be used as warehouse B in the *Warehouse ID B* field.

10. Click the *C Warehouse* menu entry in the left side bar.  
    The warehouse settings of the warehouse C are displayed on the right side.  

    ![Settings C warehouse](../../Assets/Screenshots/Fulfillment/Settings/Connections/FiegeIntegration/EditConnectionSettings_CWarehouse.png "[Settings C warehouse]")

11.  Enter the ID of the warehouse to be used as warehouse C in the *Warehouse ID C* field.

12. Click the [SAVE] button.  
    All changes have been saved. The *Saving successful* pop-up window is displayed.  

    ![Saving successful](../../Assets/Screenshots/Fulfillment/Settings/Connections/SavingSuccessful.png "[Saving successful]")
  
     > [Info] By default, all connections that have been established are inactive and must be enabled after the connection configuration, see [Enable a connection](./01_ManageConnections.md#enable-a-connection).
