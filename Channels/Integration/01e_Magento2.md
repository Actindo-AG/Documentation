[!!Manage the connections](./01_ManageConnections.md)

# Manage the Magento 2 connection

To establish a connection to a Magento 2 shop, there are several particularities to consider. Therefore, the creation and the configuration of the Magento 2 connection are described in detail below.


## Create a Magento 2 connection

Create the connection to a Magento 2 shop using the Magento 2 driver. Further settings can only be configured after the connection has been established.

All necessary credentials to establish the connection, that is username and password, are provided in the Magento 2 admin backend.

[comment]: <> (Stimmt das so? Prerequisites unten dementsprechend anpassen > ggf. eher in Procedure als Info oder direkt in Schritt einbinden (genauere Info von Oli, wo das zu finden ist)

#### Prerequisites

- A Magento 2 account has been created.
- The user has administrator rights in Magento 2.
- The *Magento 2* plugin has been installed.

> [Info] For the *Omni-Channel* module version 4.1.0 or higher, the *Magento 2* plugin is required in at least version 1.0.0.

[comment]: <> (Stimmt das so? In Platform Manager bis Magento 2 1.1.1 Version und Magento 2 B.B. 1.0.0 verfügbar. Pre-releases 1.1.2 und 1.2.0)

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connection](../../Assets/Screenshots/Channels/Settings/Connections/Connection.png "[Connection]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
  The *Create connection* view is displayed.

  ![Create connection](../../Assets/Screenshots/Channels/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the *Magento 2* driver.  
  The *Credentials* section is displayed below the drop-down list.

4. Enter the shop URL in the *URL* field.

5. Enter the username in the *Username* field.

6. Enter the password in the *Password* field.

7. Click the [SAVE] button.  
  The *Checking credentials* notice is displayed. The connection will be established and the synchronization is triggered. The *Sync triggered* pop-up window is displayed.  

  ![Sync triggered](../../Assets/Screenshots/Channels/Settings/Connections/SyncTriggered.png "[Sync triggered]")

  The *CONNECTIONS* tab in the *Settings* menu entry of the *Omni-Channel* module is displayed when the connection has been established. The *Magento 2* connection is displayed in the list of connections.

  ![Magento 2 connection](../../Assets/Screenshots/Channels/Settings/Connections/Magento/Connection.png "[Magento 2 connection]")	

8. If necessary, continue to [Configure the Magento 2 connection](#configure-the-Magento-2-connection).



## Configure the Magento 2 connection   

After the connection to a Magento 2 shop has been established, further settings can be configured for the connection.

#### Prerequisites

A Magento 2 connection has been established.

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Magento 2 connection](../../Assets/Screenshots/Channels/Settings/Connections/Magento2/Connection.png "[Magento 2 connection]")

1. Click the Magento 2 connection in the list of connections.   
  The *Edit connection* view is displayed. By default, the *Credentials* tab is selected.

  ![Edit connection credentials](../../Assets/Screenshots/Channels/Settings/Connections/Magento2/EditConnectionCredentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.   
  The *Settings* tab is displayed. By default, the *Store view languages* setting is selected.

  ![Edit connection settings](../../Assets/Screenshots/Channels/Settings/Connections/Magento2/EditConnectionSettings.png "[Edit connection settings]")

3. Click the *Store view* drop-down list and select the language in which the products will be uploaded to the store. All available languages are displayed in the list.    
   
4. Click the *Order states* menu entry in the left side bar.  
  The order states settings are displayed on the right side.  

5. Configure the following settings to filter the orders to be imported in the *Filter orders to import* section:   
    
    + Enable the toggles of all states for which the orders are to be imported. The following states are available:
        - *new*
        - *pending*
        - *pending_payment*
        - *payment_review*
        - *processing*
        - *holded*
        - *completed*
        - *closed*
        - *canceled*  
   
    + If desired, enter an order number in the *Import only orders with a higher number than this* field. Only orders with a higher order number than the specified number will be imported.  
    
    + If desired, enter the status for which the orders are to be imported in the *Status to filter for (leave empty if not required)* field. All statuses configured in Magento 2 are available.

6. Configure the following settings to define the order states and/or statuses to be set after a certain event has occurred in the *Update order state and status on certain events* section:  

    + Click the *Order state to be set in shop after successful import* drop-down list and select the state to be set when an order has been successfully imported. The following options are available:  
        - **new**
        - **pending**
        - **pending_payment**
        - **payment_review**
        - **processing**
        - **holded**
        - **completed**
        - **closed**
        - **canceled**  

    + Enter the order status to be set when an order has been successfully imported in the *Order status to be set in shop after successful import* field.
    
    + Enter the order status to be set when an order has been partially shipped in the *Order status to be set in shop after partially shipped* field.

    + Click the *Order state to be set in shop after fully shipped* drop-down list and select the state to be set when an order has been fully shipped. The following options are available:  
        - **new**
        - **pending**
        - **pending_payment**
        - **payment_review**
        - **processing**
        - **holded**
        - **completed**
        - **closed**
        - **canceled**  

    + Enter the order status to be set when an order has been fully shipped in the *Order status to be set in shop after fully shipped* field.

    + Enter the order status to be set when an order has been partially paid in the *Order status to be set in shop after partially paid* field.

    + Enter the order status to be set when an order has been fully paid in the *Order status to be set in shop after fully paid* field.

    + Enter the order status to be set when a tracking number has been set for the order in the *Order status to be set in shop after tracking number set* field.

7.  If necessary, configure the following settings in the *Magento invoice handling* section:

    + Enable the *Create an invoice in Magento for orders that are fully paid* toggle to create invoices in Magento 2 for fully paid orders and ensure the correct processing of vouchers.  
        
    + Enable the *Notify customer about the invoice* toggle to notify customers when an invoiced is generated. This toggle is only unlocked if the *Create an invoice in Magento for orders that are fully paid* toggle is enabled.
    
8. Click the *Tax classes* menu entry in the left side bar.  
  All tax classes available in the *Actindo Core1 Platform* are displayed on the right side.

9. Click the *Select Magento 2 tax class for Core1 tax class* drop-down list and select the applicable Magento tax class. All tax classes available in Magento 2 are displayed in the list. Repeat this step for all displayed tax classes.

10. Click the *Global default language for Magento 2* menu entry in the left side bar.  
  The *Select global default language for Magento backend* section is displayed on the right side.

11. Click the *Select Core1 language to be set as default* drop-down list and select the appropriate language. All languages available in the *Actindo Core1 Platform* are displayed.

[comment]: <> (Unklar - RS mit Oli)

12. Click the *Image handling* menu entry in the left side bar.  
  All available image attributes available in the Magento 2 gallery are displayed on the right side.

13. Enable all toggles of the image attributes whose images you want to be hidden in the Magento 2 gallery. 

14. Click the *Image name* menu entry in the left side bar.  
  The *Image name* settings are displayed are displayed on the right side.

15. Disable the *Apply from default* toggle to configure how the image names should be customized before uploading to the Magento 2 shop.    
  The *Use ECM image name* toggle and the *Regular expressions* field are unlocked.

    > [Info]  The following settings are used to improve the SEO of your images.

16. If desired, disable the *Use ECM image name* toggle. By default, the toggle is enabled.

17. If desired, define regular expressions that will be removed from the image name.  
For detailed information about regular expressions, see https://regex101.com/. 

18. Click the [SAVE] button.  
  All changes have been saved. The *Saving successful* pop-up window is displayed.

  ![Saving successful](../../Assets/Screenshots/Channels/Settings/Connections/SavingSuccessful.png "[Saving successful]")





