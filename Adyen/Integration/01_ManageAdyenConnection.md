# Manage Connections


In the following, the procedures to create, edit, enable, or disable *Adyen* connections are described.  
Note the following:   
- If you have more than one merchant account in *Adyen* that you want to manage with *Actindo*, you must create a connection for each.   
- *Adyen* offers the possibility to work with two separate environments, a staging environment for testing purposes and a live environment for production. You must configure the connection for each environment separately.

## Create Adyen connection
Create a connection to the *Adyen* payment service provider.

#### Prerequisites

- You have an Adyen customer account to log in to *Adyen*.
- You have your *Adyen* credentials at hand.
- In the *Actindo Core1 Platform*, you have permission to create connections in the *Payments* module.

#### Procedure
 *Payments > Settings > Tab CONNECTIONS*
 
 ![Connections](../../Assets/Screenshots/Payments/Settings/Settings.png "[Connections]")

1.  Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create Connection* view is displayed.  

    ![Create connection](../../Assets/Screenshots/Payments/Settings/PaymentServiceProviders/Adyen/Integration/CreateConnection.png "[Create connection]")

2.  Enter a name for the connection in the *Name* field.

3.  Click the *Driver* drop-down list and select **Adyen**. 
   The *Credentials* section is displayed.

    ![Credentials](../../Assets/Screenshots/Payments/Settings/CreateConnectionCredentials.png "[Credentials]")

4. Enter the API credentials. For the test environment there are some standard access points. The API credentials for the productive environment you get from *Adyen*.

    -  Enter the checkout API endpoint field in the *Checkout API endpoint* field. For the staging environment it is the **https://checkout-test.adyen.com/checkout/**.
    - Enter the checkout API key field in the *Checkout API key* field.   
    -  Enter the payment API endpoint field in the *Payment API endpoint* field. For the staging environment it is **https://pal-test.adyen.com/pal/servlet/Payment/**

5. Enter the API credentials of the API users that you have created in *Adyen*:     
    
    -  Enter the technical user for the API to transfer the payment transactions in the *Payment user* field.   
    -  Enter the password for the API to transfer the payment transactions in the *Payment password* field.  
    -  Enter the technical user for the reporting API in the *Report user* field.   
    -  Enter the password for the reporting API in the *Report password* field.  
5. Enter the credentials for notifications that Adyen shall send to the *Payments* module via the *http://basic_out_credentials* API.   

    -  Define the technical user for the notification API in the *Notification user* field. You can freely assign the username. Make sure that you store this username in the *Adyen* configuration. For detailed information, see    
    -  Define the password for the notification API in the *Notification password* field. You can freely assign the password. Make sure that you store this password in the *Adyen* configuration. For detailed information, see 

6. Enter the merchant account relevant for this connection in the *Merchant account* field. This is the merchant account that you have created in the *Adyen* configuration.
    
5. Enable the ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *MIT fraud check* toggle if you do not trust the *Adyen* fraud check and want to do your own. This might be relevant if there is a longer period between the *Adyen* fraud check and the authorization receipt. 

6. Click the [SAVE] button.   
   The specified credentials are verified with *Adyen*. 



## Edit Adyen connection




## Configure Adyen connection