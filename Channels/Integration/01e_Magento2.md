# Manage the Magento 2 connection

To establish a connection to a Magento 2 shop, there are several particularities to consider. Therefore, the configuration of the Magento 2 connection is described in detail below.

## Configure the Magento 2 connection   

After the connection to a Magento 2 shop has been established, further settings can be configured for the connection.

#### Prerequisites

- A Magento 2 account has been created.
- The *Magento 2* plugin has been installed.
- A Magento 2 connection has been established.

> [Info] For the *Omni-Channel* module version 4.1.0 or higher, the *Magento 2* plugin is required in at least version 1.0.0.

[comment]: <> (Stimmt das so? In Platform Manager Magento 2 1.1.1 Version und Magento 2 B.B. 1.0.0 verfügbar.)

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Magento 2 connection](../../Assets/Screenshots/Channels/Settings/Connections/Magento2/Connection.png "[Magento 2 connection]")

1. Click the Magento 2 connection in the list of connections.   
  The *Edit connection* view is displayed. By default, the *Credentials* tab is displayed.

  ![Edit connection credentials](../../Assets/Screenshots/Channels/Settings/Connections/Magento2/EditConnectionCredentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.   
  The *Settings* tab is displayed. By default, the *Store view languages* setting is displayed. All store views configured in the webshop are displayed in the right side bar.

  ![Edit connection settings](../../Assets/Screenshots/Channels/Settings/Connections/Magento2/EditConnectionSettings.png "[Edit connection settings]")

3. Click the desired *Store view* drop-down list and select the appropriate language. The available languages are displayed in the drop-down list.  

    > [Info] The selected language determines the language of the products to be uploaded in the corresponding store view. If further languages are needed, they must be added in the *DataHub* module first, see [Manage the languages](../../../DataHub/Integration/05_ManageLanguages.md).

[comment]: <> (Stimmt das so?)

4. Click the *Order states* menu entry in the left side bar.  
    The order states and statuses are displayed in the right side bar.  

    > [Info] An order state is a position of an order in the current processing flow. Order states are used interally and are not customizable. Each order state can have one or more order statuses assigned to it. Order statuses are customizable by the store administrator in the Magento system. 

5. Configure the following settings to filter the orders to be imported in the *Filter orders to import* box:   

    - Enable the applicable toggle(s) to determine the order states. The following states are available:
        - *new*
        - *pending*
        - *pending_payment*
        - *payment_review*
        - *processing*
        - *holded*
        - *completed*
        - *closed*
        - *canceled*  

    - If desired, enter the applicable order number in the *Import only orders with a higher number that this* field.  

    - If desired, enter the applicable status in the *Status to filter for (leave empty if not required)*. If it is not required, this field can be left empty. By default, there are 13 statuses available:
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

6. Configure the following settings to define the desired order statuses or states to be set after a certain event has occurred in the *Update order state and status on certain events* box:   

    - Click the *Order state to be set in shop after successful import* drop-down list and select the desired state. The following states are available:  
        - **new**
        - **pending**
        - **pending_payment**
        - **payment_review**
        - **processing**
        - **holded**
        - **completed**
        - **closed**
        - **canceled**  

    - Enter the desired order status to be set when an order has been successfully imported in the *Order status to be set in shop after successful import* field.
    
    - Enter the desired order status to be set when an order has been partially shipped in the *Order status to be set in shop after partially shipped* field.

    - Click the *Order state to be set in shop after fully shipped* drop-down list and select the desired state. The following states are available:  
        - **new**
        - **pending**
        - **pending_payment**
        - **payment_review**
        - **processing**
        - **holded**
        - **completed**
        - **closed**
        - **canceled**  

    - Enter the desired order status to be set when an order has been fully shipped in the *Order status to be set in shop after fully shipped* field.

    - Enter the desired order status to be set when an order has been partially paid in the *Order status to be set in shop after partially paid* field.

    - Enter the desired order status to be set when an order has been fully paid in the *Order status to be set in shop after fully paid* field.

    - Enter the desired order status to be set when a tracking number has been set for the order in the *Order status to be set in shop after tracking number set* field.

7.  If necessary, configure the following settings in the *Magento invoice handling* box:

    - Enable the *Create an invoice in Magento for orders that are fully paid* toggle. 
    
        > [Info] If enabled, invoice creation is triggered in Magento 2 as soon as an order is fully paid. This function is particularly relevant for the correct processing of vouchers.  
    
        The *Notify customer about the invoice* toggle is unlocked.

    - Enable the *Notify customer about the invoice* toggle to notify customers when an invoiced is generated.
    

8. Click the *Tax classes* menu entry in the left side bar.  
    The tax classes available in the *Actindo Core1 Platform* are displayed in the right side bar.

9. Click the *Select Magento 2 tax class for Core1 tax class* drop-down list and select the applicable Magento tax class. All available tax classes are displayed in the list. Repeat this step for all the applicable tax classes.

[comment]: <> (Gibt es Default tax classes bei Magento, z.B. die auf dem Video angezeigt oder abhängig von weiteren Vor-/Einstellungen in Magento? Neue tax classes können bei Magento auch erstellt werden, also: All available tax classes are displayed in the list oder By default, the following options are available?)

10. Click the *Global default language for Magento 2* menu entry in the left side bar.  
    The *Select global default language for Magento backend* section is displayed in the right side bar.

11. Click the *Select Core1 language to be set as default* drop-down list and select the appropriate language. All languages available in the *Actindo Core1 Platform* are displayed.

[comment]: <> (Unklar - RS mit Oli)

12. Click the *Image handling* menu entry in the left side bar.  
    All available image attributes available in the Magento 2 gallery are displayed in the right side bar.

13. Enable the applicable toggles as necessary to hide or display the corresponding images in the Magento 2 gallery. 

14. Click the *Image name* menu entry in the left side bar.  
    The *Imagen name* settings are displayed are displayed in the right side bar.

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



