# Manage the Magento 2 connection

To establish a connection to a Magento 2 shop, there are several particularities to consider. Therefore, the configuration of the Magento 2 connection is described in detail below.

- A Magento 2 account has been created.
- The *Magento 2* plugin has been installed.

## Configure the Magento 2 connection   

After the connection to a Magento 2 shop has been established, further settings can be configured for the connection.

#### Prerequisites

- A Magento 2 connection has been established.

> [Info] For the *Omni-Channel* module version 4.1.0 or higher, the *Magento 2* plugin is required in at least version 1.0.0.

[comment]: <> (Stimmt das so? In Platform Manager Magento 2 1.1.1 Version und Magento 2 B.B. 1.0.0 verfügbar.)

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

    > [Info] An order state is a position of an order in the current processing flow. Order states are used internally and are not customizable. Each order state can have one or more order statuses assigned to it. Order statuses are customizable by the store administrator in the Magento system. 

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
    
    + If desired, enter the status for which the orders are to be imported in the *Status to filter for (leave empty if not required)* field. By default, the following statuses are available:
        - *Suspect Fraud*
        - *Processing*
        - *Pending Payment*
        - *Payment Review*
        - *Pending*
        - *On Hold*
        - *Complete*
        - *Closed*
        - *Canceled*
        - *PayPal Canceled Reversal*
        - *Pending PayPal*
        - *PayPal Reversed*
        - *Refunded*

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

13. Enable the applicable toggles as necessary to hide or display the corresponding images in the Magento 2 gallery. 

14. Click the *Image name* menu entry in the left side bar.  
    The *Imagen name* settings are displayed are displayed on the right side.

15. Disable the *Apply from default* toggle.  
    The *Use ECM image name* toggle und the *Regular expressions* field are unlocked.

16. If necessary, disable the *Use ECM image name*.

17. If desired, create regular expressions to define words or descriptions to be removed from the image name.  
The site https://regex101.com/ can be useful to test regular expressions. 

    > [Info] This function allows to create customized image names to make them SEO-friendly and improve search rankings.

18. Click the [Save] button.  
    All changes have been saved. The *Saving successful* pop-up window is displayed.

    ![Saving successful](../../Assets/Screenshots/Channels/Settings/Connections/SavingSuccessful.png "[Saving successful]")



[comment]: <> (Muss man die Verbindung auch synchronisieren oder wird automatisch synchronisiert nach dem Speichern?)

[comment]: <> (Steps 5, 6 und 7 -alle unter Order States menu entry- könnten in einem großen Schritt zusammengelegt werden, mit weitere Unterschritte geteilt werden, wobei er wäre extrem lang und nicht so überschauber. Meinung dazu?)



