[!!Create a language](../../DataHub/Integration/05_ManageLanguages.md#create-a-language)

# Manage the Shopware 6 connection

To establish a connection to a Shopware 6 shop, there are several particularities to consider. Therefore, the creation and the configuration of the Shopware 6 connection are described in detail below.


## Create a Shopware 6 connection

Create the connection to a Shopware 6 shop using the Shopware 6 driver. Further settings can only be configured after the connection has been established.

Be aware that, before a Shopware 6 connection can be established in the *Actindo Core1 Platform*, the corresponding integration must be created in Shopware 6. Besides, all languages configured in Shopware 6 must be available in the *DataHub* module. Otherwise, an error is displayed when trying to create the connection in the *Actindo Core1 Platform*. The connection creation is then cancelled.

#### Prerequisites

- A Shopware 6 account has been created.
- The *Shopware 6* plugin has been installed.  
- All languages configured in the Shopware 6 account have also been created in the *DataHub* module, see [Create a language](../../DataHub/Integration/05_ManageLanguages.md#create-a-language). 

> [Info] For the *Omni-Channel* module version 4.1.0 or higher, the *Shopware 6* plugin is required in at least version 4.0.0.

[comment]: <> (Stimmt Version? 4.0.0 ist die neueste. Stimmen prerequisites? Oder besser Zwei subprocedures: 1 create integration in Shopware 6 + create connection in Core1? -> Verweis auf Manage connections?)

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connection](../../Assets/Screenshots/Channels/Settings/Connections/Connection.png "[Connection]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
  The *Create connection* view is displayed.

  ![Create connection](../../Assets/Screenshots/Channels/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select the *Shopware 6* driver.  
  The *Credentials* section is displayed below the drop-down list.

4. Enter the shop URL in the *URL* field.  

5. In a new browser window, go to your Shopware 6 account and log in.  
  The Shopware 6 dashboard is displayed.

6. In the Shopware 6 backend, go to *Settings > System > Integrations* and click the [Create integration] button in the top right corner.  
  The *Create integration* window is displayed.

  ![Create integration](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/CreateIntegration.png "[Create integration]")

7. Enter a name for the integration in the *Name* field and enable the *Administrator* toggle.

8. Copy the access key ID in the *Access key ID* field to your clipboard.

9. Switch to the *Actindo Core1 Platform* and paste the access key ID from your clipboard in the *Access key ID* field in the *Credentials* section.  
  
10. Repeat the steps **8** and **9** for the secret access key in the *Secret access key* field.

11. Switch to your Shopware 6 account and click the [Save integration] button.  
  The integration is saved. The *Success* pop-up window is displayed.

  ![Integration  created](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/IntegrationCreated.png "[Integration created]")

12. Switch to the *Actindo Core1 Platform* and click the [SAVE] button.  
  The connection has been created. The *CONNECTIONS* tab in the *Settings* menu entry of the *Omni-Channel* module is displayed when the connection has been established. The *Shopware 6* connection is displayed in the list of connections.

  ![Shopware 6 connection](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/Connection.png "[Shopware 6]")

13. If necessary, continue to configure the Shopware 6 connection settings, see [Configure the Shopware 6 connection](#configure-the-shopware-6-connection).

[comment]: <> (Was genau passiert nach SAVE in Core1? Einige Minuten Zeit/Sync/Platform initialized? Satz aus Shopify genommen.)



## Configure the Shopware 6 connection   

After the connection to a Shopware 6 shop has been established, further settings can be configured for the connection.

#### Prerequisites

A Shopware 6 connection has been established, see [Create a Shopware 6 connection](#create-a-shopware-6-connection).

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Shopware 6 connection](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/Connection.png "[Shopware 6 connection]")

1. Click the Shopware 6 connection in the list of connections.   
  The *Edit connection* view is displayed. By default, the *Credentials* tab is selected.

  ![Edit connection credentials](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/EditConnectionCredentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.   
  The *Settings* tab is displayed. By default, the *Default language* menu entry is selected.
  
3. In the *Default language* settings, click the *Select Shopware default language* drop-down list and select the appropriate language. The languages available in the *Actindo Core1 Platform* are displayed in the drop-down list.  

    > [Info] In Shopware 6 is a standard language, which is configured during the installation and cannot be subsequently edited. The standard language cannot be detected via API and must be therefore manually configured in the *Actindo Core1 Platform* after the connection has been established. When uploading products, Shopware 6 requires some fields to be filled for the standard language. 

  ![Edit connection settings](../../Assets/Screenshots/Channels/Settings/Connections/Shopware6/EditConnectionSettings.png "[Edit connection settings]")

4. Click the *Orders* menu entry in the left side bar.  
  The import settings for orders are displayed on the right side.  

5. Configure the following settings:
    + If desired, enter an order number in the *Import only orders with a higher number than this* field. Only orders with a higher order number than the specified number will be imported.  

    + Enable the toggles of all statuses for which the orders are to be imported. All statuses available in Shopware 6 are displayed.
        
    + If desired, click the *Order state to set in shop after successful import* drop-down list and select the state that will be set for the order if the import has been successful. All states available in Shopware 6 are displayed.

      > [Info] The order states in Shopware 6 have fixed transitions. This means that, once an order has a certain state, only specific states can be selected for the next state of the order. Make sure that the selected state is also supported by Shopware 6.    

    + If desired, click the *Order state to set in shop after the order is fully shipped* drop-down list and select the state that will be set for the order if the shipment has been completed. All states available in Shopware 6 are displayed.
  
    + If desired, enable for each payment method the toggles of all states for which the orders are to be imported. If you select no payment states for a certain payment method, all orders with this payment method, regardless of their state, will be imported. All states available in Shopware 6 are displayed for each payment method. All payment methods configured in Shopware 6 are displayed.

6. Click the *Tax classes* menu entry in the left side bar.  
  The tax classes available in Shopware 6 are displayed on the right side.  

7. Click the *Select Core1 tax class for Shopware 6 "Shopware tax class name"* drop-down list and select the corresponding tax class in the *Actindo Core1 Platform*. All available tax classes are displayed in the list. Repeat this step for all Shopware 6 tax classes.

8. If available, click the *Ratepay* menu entry in the left side bar.  
  The Ratepay settings are displayed on the right side.

    > [Info] The *Ratepay* menu entry is only displayed if the *Ratepay Integration for Shopware 6* plugin has been installed in your *Actindo Core1 Platform* and the *Ratepay Payment Plugin for Shopware 6* has been installed in your Shopware 6 account.
  
9. If desired, enable the *Enable Ratepay integration for this connection* toggle.  

    > [Info] The *Ratepay Payment Plugin for Shopware 6* provides additional information to the orders, which can be imported for further processing.  
 
[comment]: <> (nicht standard / Extension für Treiber - beschreiben oder wegglassen? -> RS Oli)

10. Click the *Price rules* menu entry in the left side bar.  
  The price rule settings are displayed on the right side.

11. Enable the toggles for all price rules for which you want to create a price attribute in the *Actindo Core1 Platform* to maintain deviating prices. All price rules available in Shopware 6 are displayed. 

    > [Info] You have to save the changes and synchronize the connection to create the corresponding price attribute. Once a price attribute has been created, the corresponding toggle is locked and cannot be disabled anymore.

12. Click the [SAVE] button.  
  All changes have been saved. The *Saving successful* pop-up window is displayed.

  ![Saving successful](../../Assets/Screenshots/Channels/Settings/Connections/SavingSuccessful.png "[Saving successful]")

13. Synchronize the connection to update the ETL mapping, see [Synchronize a connection](../Integration/01_ManageConnections.md#synchronize-a-connection)    
  The *Sync triggered* pop-up window is displayed.

  ![Sync triggered](../../Assets/Screenshots/Channels/Settings/Connections/SyncTriggered.png "[Sync triggered]")