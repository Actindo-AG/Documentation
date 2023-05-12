# Establish connections to payment service providers (PSP)


If you want to establish a new connection to a payment service provider (PSP), you can buy the needed connection in the app store. This is valid if you have not yet bought it with your Actindo maintenance contract.<!---Stimmt das?-->   
The data structure of the connection then provides exactly the data that the PSP needs to exchange data with the *Actindo Payments* module.

In the following, the general settings to create, edit, 
or disable connections are described. Except for the Actindo POS driver, you can buy the connections to payment service providers in the app store.<!---???stimmt das?-->


## Create a PSP connection

Create a connection to a certain payment provider. As soon as a connection has been established,..activated?? <!---an initial synchronization will be triggered, which will transfer the entire data model of the connected payment provider to Actindo-->. 



#### Prerequisites
At least one connection has been installed
#### Procedure
*Payments > Settings > Tab CONNECTIONS*
<!--- ![Connection](../../Assets/Screenshots/Payments/Settings/Connections/Connections.png "[Connection]")--->
1.  Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The view for creating a connection is displayed.   
    ![Create connection](../../Assets/Screenshots/Payments/Settings/Connections/CreateConnection.png "[Create connection]")
2.  Enter a name for the connection in the *Name* field.
3.  Click the *Driver* drop-down list and select the desired driver. 
   All already installed drivers are displayed in the list.   
   
     > [Info] If you want to install additional drivers, select the **more...** option and buy a driver in the app store.You have to purchase drivers from the main account. You need to install them separately in each sandbox or account where you want to use it.

     The *Credentials* section is displayed below the drop-down list.

    ![Credentials](../../Assets/Screenshots/Payments/Settings/Connections/Credentials.png "[Credentials]")
     > [Info] Depending on the selected driver, the fields in the *Credentials* section differ.

4. Enter the required data in the fields in the *Credentials* section.
5. If the PSP connection required additional settings, open the *Settings* tab and add further settings.

5. Click the [SAVE] button.   
    The connection will be established. The *Checking credentials...* notice is displayed. After a few seconds, the *Loading data...* notice is displayed.

    ![Checking credentials](../../Assets/Screenshots/Payments/Settings/Connections/CheckingCredentials.png "[Checking credentials]")

    The view for creating connections is automatically closed when the connection has been established. The *Edit connection* view of the newly created connection is displayed. The *Settings* tab is selected.

    ![Edit connection settings](../../Assets/Screenshots/Payments/Settings/Connections/EditConnectionSettings.png "[Edit connection settings]")   


## Edit a PSP connection

Edit a connection to adjust any changed credentials, the connection name or further settings. The driver selection is read-only and you cannot edit it.

#### Prerequisites

At least one connection has been created, see [Create a connection](#create-a-connection).

#### Procedure

*Payments > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Payments/Settings/Connections/Connections.png "[Connections]")

1. Click the connection you want to edit in the list of connections.   
    The *Edit connection* view is displayed.

    > [Info] Depending on the driver of the connection, the *Credentials* and the *Settings* tab are displayed in the *Edit connection* view.

    ![Edit connection](../../Assets/Screenshots/Payments/Settings/Connections/EditConnectionCredentials.png "[Edit connection]")

2. Edit the desired data of the connection in the corresponding fields in the *Credentials* tab.

3. If necessary, click the *Settings* tab and edit the desired settings of the connection in the corresponding fields.

4. Click the [SAVE] button.   
    The *Checking credentials...* notice is displayed.

    ![Credentials](../../Assets/Screenshots/Fulfillment/Settings/Connections/CheckingCredentials.png "[Credentials]")

    The *Edit connection* view is automatically closed when the changes have been saved. The *Connections* view is displayed again.



## Disable a PSP connection
Once a connection has been established, you cannot delete it because of potential dependencies in the existing database. Nevertheless, you can disable the connection if you do not use ist any longer. You can disable several active connections at a time.

#### Prerequisites

- At least one connection has been established, see [Create a connection](#create-a-connection).


#### Procedure

*Payments > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Payments/Settings/Connections/Connections.png "[Connections]")

1. Select the checkbox of the connection you want to disable in the list of connections.   
    The editing toolbar is displayed above the list of connections.

2. Click the [DISABLE] button in the editing toolbar.   
    The connection has been deactivated.

3. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list of connections.   
    The status of the disabled connection in the *Status* column has switched to **Inactive**.