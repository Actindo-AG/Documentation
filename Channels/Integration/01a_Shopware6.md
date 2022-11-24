# Manage the Shopware 6 connection

To establish a connection to a Shopware 6 shop, there are several particularities to consider. Therefore, the creation and the configuration of the Shopware 6 connection are described in detail below.


## Create a Shopware 6 connection

Create the connection to a Shopware 6 shop using the Shopware 6 driver. Further settings can only be configured after the connection has been established.

Shop URL  
API credentials (erzeugt in Shopware backend)
Access key ID
Secret access key

[comment]: <> (S. Wissenstransfer ab Min. ca. 5:25-> Shopware 6 Seite -> zu beschreiben wie in Shopify?)

Besonderheit: Alle Sprachen konfiguriert in Shopware müssen auch in Core1 (DataHub) angelegt sein, sonst Fehler bzw. Verbindungerstellung abgebrochen/nicht möglich (Shopware 6 bricht die Installation ab). 


## Configure the Shopware 6 connection   

After the connection to a Shopware 6 shop has been established, further settings can be configured for the connection.

#### Prerequisites

- A Shopware 6 account has been created.
- The *Shopware 6 Integration* plugin has been installed.
- A Shopware 6 connection has been established.

> [Info] For the *Omni-Channel* module version 4.1.0 or higher, the *Shopware 6 Integration* plugin is required in at least version 1.0.0.

[comment]: <> (Stimmt das so? In Platform Manager Shopware 6 2 1.1.1 Version und Magento 2 B.B. 1.0.0 verfügbar.)

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Shopware 6 connection](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/Connection.png "[Shopware 6 connection]")

1. Click the Shopware 6 connection in the list of connections.   
  The *Edit connection* view is displayed. By default, the *Credentials* tab is displayed.

  ![Edit connection credentials](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/EditConnectionCredentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.   
  The *Settings* tab is displayed. By default, the *Default language* setting is displayed. Shopware 6 default language is displayed in the right side bar.

    > [Info] In Shopware 6 there is a standard language, which is configured during the installation and cannot be subsequently edited. The standard language cannot be detected via API and must be therefore manually configured in the *Actindo Core1 Platform* after the connection has been established. When uploading products, Shopware 6 requires some fields to be filled for the standard language.

  ![Edit connection settings](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/EditConnectionSettings.png "[Edit connection settings]")

3. Click the *Order* menu entry in the left side bar.  
    The order import settings are displayed in the right side bar.  

4. Configure the following settings to filter the orders to be imported:
    - If desired, enter the applicable order number in the *Import only orders with a higher number that this* field.  

    - Enable the applicable toggle(s) to determine the order status. All statuses available in Shopware 6 are displayed.
        
    - If desired, click the *Order state to set in shop after successful import* drop-down list and select the appropriate status. All statuses available in Shopware 6 are displayed.

    - If desired, click the *Order state to set in shop after the order is fully shipped* drop-down list and select the appropriate status. All statuses available in Shopware 6 are displayed.

5. Click the *Tax classes* menu entry in the left side bar.  
    The available tax classes are displayed in the right side bar.  

6. Ratepay (nicht standard / Extension für Treiber - beschreiben?)

7. Price rules
