[!!Connections (Settings)](../UserInterface/08a_Connections.md)

# Manage connections to payment service providers (PSP)   

If you want to establish a new connection to a payment service provider (PSP), you can buy, depending on the payment service provider, the needed connection in the app store or license it directly at the payment service provider. By default, Actindo supports the following drivers:
- Adyen&trade;
- Amazon pay&trade;
- EBICS&trade;
- Stripe&trade;
- A dummy driver to simulate payments     

The data structure of the connection then provides exactly the data that the PSP needs to exchange data with the Actindo *Payments* module.

In the following, the general settings to create, edit, 
or disable connections are described. 


## Create a PSP connection

Create a connection to a certain payment provider. As soon you have established a connection, an initial synchronization will be triggered, which will transfer the entire data model of the connected payment provider to Actindo. 


#### Prerequisites

At least one connection has been installed.


#### Procedure    

*Payments > Settings > Tab CONNECTIONS*   

![Connections](../../Assets/Screenshots/Payments/Settings/Connections.png "[Connections]")
1.  Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The view for creating a connection is displayed.   
    ![Create connection](../../Assets/Screenshots/Payments/Settings/CreateConnection.png "[Create connection]")
2.  Enter a name for the connection in the *Name* field.
3.  Click the *Driver* drop-down list and select the desired driver. 
   All already installed drivers are displayed in the list.   
   
     > [Info] If you want to install additional drivers, select the **more...** option and buy a driver in the app store. You have to purchase drivers from the main account. You need to install them separately in each sandbox or account where you want to use it.

     The *Credentials* section is displayed below the drop-down list.

    ![Credentials](../../Assets/Screenshots/Payments/Settings/CreateConnectionCredentials.png "[Credentials]")
     > [Info] Depending on the selected driver, the fields in the *Credentials* section differ. 

4. Enter the required data in the fields in the *Credentials* section. Use the information you received from the payment service provider to fill the credentials.   
5. If the PSP connection requires additional settings, open the *Settings* tab and add further settings.

6. Click the [SAVE] button.   
    The connection will be established. The *Checking credentials...* notice is displayed. After a few seconds, the *Loading data...* notice is displayed.

     ![Checking credentials](../../Assets/Screenshots/Payments/Settings/CheckingCredentials.png "[Checking credentials]")

    The view for creating connections is automatically closed when the connection has been established. The *Edit connection* view of the newly created connection is displayed. The *Settings* tab is selected.
      ![Credentials](../../Assets/Screenshots/Payments/Settings/EditConnectionSettings.png "[Credentials]")
    <!-----Stefan: stimmt das? Ich kann es nicht nachmachen--->


## Edit a PSP connection

Edit a connection to adjust any changed credentials, the connection name or further settings. 

#### Prerequisites

At least one connection has been created, see [Create a connection](#create-a-connection).

#### Procedure

*Payments > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Payments/Settings/ChangeConnections.png "[Connections]")

1. Click the checkbox on the left to select the connection you want to edit.  
   The editing toolbar is displayed above the list of connections.      
2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") button
   
    The *Edit connection* view is displayed.

    > [Info] Depending on the driver, the *Credentials* as well as the *Settings* tab are displayed in the *Edit connection* view.

    ![Connection credentials](../../Assets/Screenshots/Payments/Settings/EditConnectionCredentials.png "[Connection credentials]")

2. Edit the desired data of the connection in the corresponding fields in the *Credentials* tab.

3. If necessary, click the *Settings* tab and edit the desired settings of the connection in the corresponding fields.

4. Click the [SAVE] button.   
    The *Checking credentials...* notice is displayed.
    ![Checking credentials](../../Assets/Screenshots/Payments/Settings/CheckingCredentials.png "[Checking credentials]")
    The *Edit connection* view is automatically closed when the changes have been saved. The *CONNECTIONS* view is displayed again.

## Disable a PSP connection
Once a connection has been established, you cannot delete it because of potential dependencies in the existing database. Nevertheless, you can disable the connection if you no longer use it. You can disable several active connections at a time.

#### Prerequisites

- At least one connection has been established, see [Create a connection](#create-a-connection).
- The connection is active.


#### Procedure

*Payments > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Payments/Settings/ChangeConnections.png "[Connections]")

1. Select the checkbox of the connection you want to disable in the list of connections.   
    The editing toolbar is displayed above the list of connections.

2. Click the [DISABLE] button in the editing toolbar.   
    The connection has been deactivated.

3. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list of connections.   
    The status of the disabled connection in the *Status* column has switched to **Inactive**.

## Enable a PSP connection
Once a connection has been established, you can disable it if you no longer need it. If you have done this by mistake, you can enable the connection again. You can enable several active connections at once.

#### Prerequisites

- At least one connection has the status *Inactive*.


#### Procedure

*Payments > Settings > Tab CONNECTIONS*

![Connections](../../Assets/Screenshots/Payments/Settings/ChangeConnections.png "[Connections]")
<!----Stefan, kannst Du mir einen Screenshot machen?Eigentlich brauche ich nur einen grünen Enable button --->

1. Select the checkbox of the connection you want to enable in the list of connections.   
    The editing toolbar is displayed above the list of connections.

2. Click the [ENABLE] button in the editing toolbar.   
    The connection has been activated.

3. Click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list of connections.   
    The *Checking credentials...* notice is displayed. 
    The status of the enabled connection in the *Status* column has switched to **Active**.