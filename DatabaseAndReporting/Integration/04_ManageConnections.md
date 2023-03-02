[!!User interface Connections](../UserInterface/03a_Connections.md)


# Manage the connections

Establish a connection to the InfluxDB software to be able to create InfluxDB time series. The InfluxDB driver is available in two different versions. Depending on the driver version, the credentials differ. All necessary credentials to establish the connection are provided by InfluxDB. For detailed information about InfluxDB, see [InfluxDB](https://docs.influxdata.com/influxdb/v2.6/).

You can create and edit a connection.

[comment]: <> (Löschen nicht möglich? Enable/disable/sync nicht nötig?)


## Create a connection

Create a connection to InfluxDB. 

#### Prerequisites

An InfluxDB driver must be installed in the Core1.

[comment]: <> (Wie kommt man zu den Treibern?)

#### Procedure

*Database and reporting > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/Connections.png "[Connections]")


1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create connection* view is displayed.

    ![Create connection](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the desired driver. The following options are available:

    - InfluxDB driver V1  
    - InfluxDB driver V2  

    Depending on the selected driver, the fields in the *Credentials* section differ.

    
    ![InfluxDB Driver V1](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnectionInfluxDBDriverV1.png "[InfluxDB Driver V1]")

    
    ![InfluxDB Driver V2](../../Assets/Screenshots/DatabaseAndReporting/Settings/Connections/CreateConnectionInfluxDBDriverV1.png "[InfluxDB Driver V1]")

    > [Info] Drivers must be ... and then be installed separately in each sandbox or account where you want to use it.    

