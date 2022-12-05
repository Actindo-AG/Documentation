# Manage the Amazon connection

To establish a connection to an Amazon shop, there are several particularities to consider. Therefore, the creation and the configuration of the Amazon connection are described in detail below.


## Create a Amazon connection

Create the connection to an Amazon shop using the Amazon driver. Further settings can only be configured after the connection has been established.

#### Prerequisites

- An Amazon seller account has been created.
- The *Omni-Channel Amazon Integration* plugin has been installed. 
- The OAuth authorization URI has been constructed, see [Construct an OAuth authorization URI](https://developer-docs.amazon.com/sp-api/docs/authorizing-selling-partner-api-applications).

> [Info] For the *Omni-Channel* module version 4.1.0 or higher, the *Omni-Channel Amazon Integration* plugin is required in at least version 1.5.0. 

[comment]: <> (Omni-Channel Amazon Integration - aktuell nur mit Omni-Channel Version 2.6.13? In der Zukunft auch mit 4. Version möglich? Check versions!) 

[comment]: <> (The OAuth authorization URI redirects a browser to an Amazon consent page, where you or a selling partner can give your application consent to make calls to the Selling Partner API.)

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Connection](../../Assets/Screenshots/Channels/Settings/Connections/Connection.png "[Connection]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
  The *Create connection* view is displayed.

    ![Create connection](../../Assets/Screenshots/Channels/Settings/Connections/CreateConnection.png "[Create connection]")

2. Enter a name for the connection in the *Name* field.

3. Click the *Driver* drop-down list and select *Omni-Channel Amazon Integration* driver.  
  The *Credentials* section is displayed below the drop-down list.  

    ![Credentials](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Credentials.png "[Credentials]")


4. To find your Seller ID, log in to your seller account in the Amazon Seller Central.

    ![Amazon Seller Profile](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/AmazonSellerProfile.png "[Amazon Seller Profile]")

5. Click *Settings* on the upper right corner and select the *Account Info* menu entry.  
    The *Seller Account Information* window is displayed.

    ![Seller account information](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/SellerAccountInfo.png "[Seller account information]")

6. Click *Your Merchan Token* in the *Business Information* section.  
    The *Merchant Token* window is displayed.

    ![Merchant token](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/MerchantToken.png "[Merchant token]")

7. Copy the *Merchant Token* to your clipboard, then switch back to the *Core1 Actindo Platform* and paste it in the *Seller ID* field in the *Credentials* section.

8. Click [AUTHORIZE].  
    You are automatically redirected to the *Authorize Actindo* window in the Amazon Seller Central.

    ![Actindo Authorization](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/ActindoAuthorization.png "[Actindo Authorization]")

9. Select the checkbox with the notice *I request Amazon to grant Actindo access to my seller account and the corresponding data. I am responsible for all measures that may be taken by this application* and click [Confirm].  

    A new window with the notice *We authorize Actindo to access your seller details* is displayed. You are redirected back to the *Actindo Core1 Platform*. The *Access Token* field has been automatically filled in.

    ![Access token](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/AccessToken.png "[Access token]")

[comment]: <> (Selber übersetzt. Nicht sicher, was eigentlich steht. Fraglich, ob man alle Screenshots bekommen kann. Prüfen und ggf. rauslassen)

10. Click the *Amazon Marketplace* drop-down list and select the applicable marketplace.
    > [Info] Once it has been saved, the selected marketplace cannot be edited anymore.

11. Click [SAVE].  
    A new window with the notice *Checking credentials* is displayed. The credentials are checked, the connection established and the synchrozation is triggered. The *Synchronization triggered* is displayed. 

    ![Synchronization triggered](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/SynchronizationTriggered.png "[Synchronization triggered]")

    The *CONNECTIONS* tab in the *Settings* menu entry of the *Omni-Channel* module is displayed when the connection has been established. The *Amazon* connection is displayed in the list of connections.

    ![Amazon connection](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Connection.png "[Amazon connection]")

[comment]: <> (Letzter Satz von Shopify genommen. Evtl. mit Result oben -11- integrieren. Alle Dateien vereinheitlichen, wenn möglich.)

12. If necessary, continue to [Configure the Amazon connection](#configure-the-amazon-connection).


## Configure the Amazon connection   

After the connection to an Amazon shop has been established, further settings can be configured for the connection.

#### Prerequisites

An Amazon connection has been established.

#### Procedure

*Omni-Channel > Settings > Tab CONNECTIONS*

![Amazon connection](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Connection.png "[Amazon connection]")

1. Click the Amazon connection in the list of connections.   
  The *Edit connection* view is displayed. By default, the *Credentials* tab is displayed.

    ![Edit connection credentials](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Credentials.png "[Edit connection credentials]")

2. Click the *Settings* tab.   
  The *Settings* tab is displayed. By default, the *Offers* setting is displayed. In the right side bar, the *Apply from default* toggle is preselected and the *Update stock for 'Fulfillment by Amazon (FBA)' offers* is locked.  

    > [Info] It is recommended to leave this settings unchanged, since Amazon manages stock for FBA offers.

    ![Offers](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Settings_Offers.png "[Offers]")

3. Click the *Order import* menu entry in the left side bar.    
  The *Order import* setting is displayed in the right side bar.    

    ![Order import](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Settings_OrderImport.png "[Order import]")

4. Configure the following settings to filter the orders to be imported:

  - In the *'Merchant Fulfilled Network' (MFN) orders* section: 
    - Enable or disable the *Import 'Merchant Fulfilled Network' (MFN) orders* and *Import 'Prime by Merchant' orders* toggles to determine the MFN orders to be imported.  

    - If desired, enter a date in the *Import MFN orders from* field to import orders from the entered date onwards. The valid date format is DD.MM.YYYY. 

  - In the *'Fulfillment by Amazon' (AFN) orders* section:  
    - Enable or disable the *Import 'Fulfillment by Amazon' (AFN) orders* toggle to import the AFN, also called FBA, orders. 
  
    - Enable or disable the *Mark 'Fulfillment by Amazon' orders as shipped during import and disable warehousing* to determine the further processing of AFN orders.  
  
    - Enable or disabled as necessary the *Is the VAT calculation services (VCS) enabled?* toggle. This feature is needed to determine whether the prices in the FBA reports are gross (VCS disabled) or net (VCS enabled).  

    > [Info] When importing AFN orders, it is highly recommended to enable the VCS to makes sure that the gross/net prices are imported correctly from Amazon reports.

    - If desired, enter a date in the *Import AFN/FBA orders from* field to import orders from the entered date onwards. The valid date format is DD.MM.YYYY. 

  - In the *Addresses* section:
    - Click the *Packstation address split* drop-down list and select the appropriate option. The following options are available:  
      - **Customer number in address line**
      - **Customer number in company** 

5. Click the *Order export/invoice upload* menu entry in the left side bar.    
  The *Order export/invoice upload* setting is displayed in the right side bar.    

    ![Order export/invoice upload](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Settings_OrderExport.png "[Order export/invoice upload]")

6. If necessary, disable the *Apply from default* toggle to unlock the checkboxes.

7. Once unlocked, select the checkboxes corresponding to the relevant marketplaces.

8. Click the *Shipping provider mapping* menu entry in the left side bar.    
  The *Shipping provider mapping* setting is displayed in the right side bar. All shipping methods offered by Amazon are displayed in the AmazonShipOption section. All available shipping methods must be assigned to a shipping provider in the *Assigned shipping provider* section.  

    ![Shipping provider mapping](../../Assets/Screenshots/Channels/Settings/Connections/Amazon/Settings_ShippingProviderMapping.png "[Shipping provider mapping]")

9.  If necessary, click the corresponding drop-down list in the *Assigned shipping provider* section and select the applicable shipping provider. If no shipping provider is selected, the default shipping provider applies.

  > [Info] The shipping provider can be set up in the *Order management* module.

[comment]: <> (Wo, wie? Link oder Pfad dahin?)

10. Click [SAVE].  
    All changes have been saved. The *Saving successful* pop-up window is displayed.

    ![Saving successful](../../Assets/Screenshots/Channels/Settings/Connections/SavingSuccessful.png "[Saving successful]")

[comment]: <> (Check, ob das auch bei Amazon stimmt)

11. After saving, it is necessary to synchronize the connection to update the corresponding ETL mapping. 
  The *Synchronization triggered* pop-up window is displayed with the notice 'The synchronization has been triggered and will be performed shortly in the background'.

[comment]: <> (Wie macht man Sync? Nicht deutlich in Wissenstranfer. Connection checkbox auswählen und SYNCHRONIZE button in editing tool? Verweis darauf?)
