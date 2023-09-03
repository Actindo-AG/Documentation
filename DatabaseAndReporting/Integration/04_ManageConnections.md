[!!User interface Connections](../UserInterface/03a_Connections.md)

# Manage the connections

Establish a connection to a time series database; in order to write data from your databases to a time series database at regular intervals.

A driver to connect to InfluxDB&trade;[^1] is preinstalled in the *Database and reporting* module and is available in two versions. We currently support version 1 and 2 of InfluxDB&trade;. Depending on the version, the credentials differ. All necessary credentials to establish the connection have to be provided by the administrator managing InfluxDB&trade; instance. For detailed information, see the [InfluxDB&trade; website](https://influxdata.com).

The connections can be created, edited, and deleted.



## Create a connection

Create a connection to InfluxDB&trade; to be able to write data from your databases to a time series database. 


### Add a connection

Add a new connection to InfluxDB&trade; using one of the available InfluxDB&trade; drivers.

#### Prerequisites

InfluxDB&trade; has been purchased.

#### Procedure

*Database and reporting > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/NoConnections.png "[Connections]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create connection* view is displayed.

    ![Create connection](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the desired driver. The following options are available:

    - **Driver V1**  
    - **Driver V2**  

    Depending on the selected driver, the fields in the *Credentials* section differ. All necessary credentials are provided by InfluxDB&trade;.
   
    ![Drivers](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnectionInfluxDBDriverV1und2.png "[Drivers]")

4. For the next steps to create a connection, follow the appropriate procedure:

    - [Create a connection with driver V1](#create-a-connection-with-driver-v1)
    - [Create a connection with driver V2](#create-a-connection-with-driver-v2) 


### Create a connection with driver V1

Enter the credentials as provided by InfluxDB&trade; in the corresponding fields of the *Credentials* section to create a connection using the driver V1.

#### Prerequisites

- A connection has been added, see [Add a connection](#add-a-connection).
- The driver V1 has been selected. 

#### Procedure

*Database and reporting > Settings > Tab CONNECTIONS > Add connection > Select driver V1*

![Driver V1](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnectionInfluxDBDriverV1.png "[Driver V1]")

1. Enter the URL path in the *URL* field.

2. Enter the database identifier in the *Database* field.

3. Enter the username in the *Username* field.

4. Enter the password in the *Password* field. 

5. Click the [SAVE] button.  
    The connection has been saved. The *Create connection* view is closed. The new connection is displayed in the list of connections.

    ![Connection created](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/ConnectionsV1.png "[Connection created]")


### Create a connection with driver V2

Enter the credentials as provided by InfluxDB&trade; in the corresponding fields of the *Credentials* section to create a connection using the driver V2.

#### Prerequisites

- A connection has been added, see [Add a connection](#add-a-connection).
- The driver V2 has been selected. 

#### Procedure

*Database and reporting > Settings > Tab CONNECTIONS > Add connection > Select driver V2*

![Driver V2](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnectionInfluxDBDriverV2.png "[Driver V2]")

1. Enter the URL path in the *URL* field.

2. Enter the organization name in the *Organization* field.

3. Enter the database identifier in the *Bucket* field.

4. Enter the API token in the *API token* field.

5. Click the [SAVE] button.  
    The connection has been saved. The new connection is displayed in the list of connections.

    ![Connection created](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/ConnectionsV2.png "[Connection created]")


## Edit a connection

Edit a connection to adjust any changed credentials or the connection name. The driver selection is read-only and cannot be edited.

#### Prerequisites

At least one connection has been established, see [Create a connection](#create-a-connection).

#### Procedure

*Database and reporting > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/ConnectionsV2.png "[Connections]")

1. Click the connection to be edited in the list of connections. Alternatively, select the checkbox of the connection to be edited and click the ![Edit](../../Assets/Icons/Edit01.png) (Edit) button in the editing toolbar.  
    The *Edit connection* view is displayed.
    
    ![Edit connection](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/EditConnectionV2.png "[Edit connection]")

2.  Edit the desired data of the connection in the corresponding fields in the *Credentials* section. 

    > [Info] The fields in the *Credentials* section differ depending on the driver version.

3. Click the [SAVE] button.  
    The *Checking credentials* notice is displayed.

    ![Checking credentials](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CheckingCredentials.png "[Checking credentials]")

    The *Edit connection* is automatically closed when the changes have been saved. The edited connection is displayed in the list of connections.



## Delete a connection

Delete a connection if it is no longer in use.

#### Prerequisites

At least one connection has been established, see [Create a connection](#create-a-connection).

#### Procedure

*Database and reporting > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/ConnectionsV2.png "[Connections]")

1. Select the checkbox of the connection to be deleted.   
    The editing toolbar is displayed.

2. Click the ![Delete](../../Assets/Icons/Trash03.png) (Delete) button in the editing toolbar.  
    The *Connection xxxx* pop-up window is displayed. The *xxxx* indicates the identifier of the deleted connection as displayed in the *ID* column. The deleted connection is removed from the list of connections.

    ![Deleted connection](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/DeletedConnection.png "[Deleted connection]")

[comment]: <> (Julian: Bitte Screenshot einbauen, ziehen und zukommen lassen.)



[^1]: **Disclaimer:** InfluxDB&trade; is a trademark owned by InfluxData, which is not affiliated with, and does not endorse, this site.  