[!!Manage Adyen connection](./02_ManageAdyenConnection.md#).

# Manage settings in Adyen

The following procedures contain information on the settings to be configured in the Adyen&trade; backend. It shows the standard procedures and screens that were current at the time this documentation was created. For the latest detailed descriptions, refer to the Adyen&trade; documentation. 

In addition to the credentials settings in the Adyen&trade; backend, the same data is required in the *Payments* module to ensure a smooth data transfer. Note that once you have saved the credentials in Adyen&trade; or the *Payments* module, you can no longer copy them in order to specify them on the other side of the connection. Therefore, we recommend that you enter the connection data in parallel, which means alternately in the *Payments* module and in the Adyen&trade; backend. Alternatively, you can cache the credentials in a file. For detailed information on the Payments settings, see also [Configure Adyen connection](./02_ManageAdyenConnection.md#configure-adyen-connection).

Note the following: 

- Adyen™ offers the possibility to work with two separate environments, a staging environment for testing purposes and a live environment for production. You must configure the connection for each environment separately.   
- If you have more than one merchant account in Adyen&trade; that you want to manage with Actindo, you must create connections for each.   


**Additional information**   

Adyen&trade; uses TLS certificates that are changed from time to time. Adyen&trade; users will be informed about this. You can ignore this information from Adyen because Actindo only checks if the certificates are valid in general and does not validate specific certificates. See also an update example from Adyen&trade;: [TLS Certificates on Adyen services](https://help.adyen.com/updates/tls-certificates-on-adyen-services "[https://help.adyen.com/updates/tls-certificates-on-adyen-services]"). 



## Create Adyen webhook

Create a webhook to receive payment notifications from Adyen&trade; to the *Payments* module such as authorizations and cancellations. For detailed information, see also [Webhooks](https://docs.adyen.com/development-resources/webhooks/ "[https://docs.adyen.com/development-resources/webhooks/]") in the Adyen&trade; documentation. It includes a video that may be helpful, too.


#### Prerequisites

- You have an Adyen&trade; customer account to log in to Adyen&trade;.
- You are logged in to Adyen&trade;.
- You are assigned to the required user roles in Adyen&trade;. 
- The *Adyen* plugin is installed on the *Actindo Core1 Platform* system.
- At least one Adyen&trade; connection has been created in the *Payments* module, see [Create Adyen connection](./02_ManageAdyenConnection.md#create-adyen-connection).
- You are logged in to your Actindo instance under *Payments > Settings > Select connection > Credentials tab*.

#### Procedure

*Adyen&trade; > Developers > Webhooks*

![Webhook configuration in Adyen](../../Assets/Screenshots/Adyen/Integration/AdyenWebhooks.png)

1. Click the [+ Webhook] button.   
    The *Create new webhook* window is displayed.

 2. Select the [Add] button at the *Standard webhook* entry in the *Recommended webhooks* section.   
    The settings for the standard webhook are displayed.

    ![Create webhook in Adyen](../../Assets/Screenshots/Adyen/Integration/AdyenCreateWebhook.png "[Create webhook in Adyen]")

3. Enter the following settings in the *General* section.
    - *Description*  
        Enter a description for the webhook.
    - *Server configuration section*   
         - *URL*   
           Enter the server URL of the Actindo production system or sandbox you want to connect.    
           For example: `https://customeraccount.dev.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notificationAsync`. This example displays the server URL for asynchronous processing. For detailed information on synchronous processing, see [Define synchronous or asynchronous processing](#define-synchronous-or-asynchronous-processing). 
      
         - *Method*   
            You can use the **JSON** standard setting if you have no other requirements.

        - *Accept webhook*   
            Adyen&trade; requires you to acknowledge every webhook event with a successful HTTP response status code, for example 200. You can use the standard setting. For detailed information, see [Accept webhooks](https://docs.adyen.com/issuing/webhooks/#accept-webhooks "https://docs.adyen.com/issuing/webhooks/#accept-webhooks") in the Adyen&trade; documentation.

        - *Encryption protocol*     
           You can use the **TLSv1.3** standard setting if you have no other requirements.

        - *Version*   
            Displays the version number.
            
          ![Define server configuration](../../Assets/Screenshots/Adyen/Integration/AdyenCreateWebhookServerConfig.png "[Define server configuration]").

4. Click the [Apply] button and proceed with the following fields in the *General* section.

    - *Merchant accounts*   
        Enter the merchant account(s) you want to connect.
    - *Events*   
        Select all the events whose messages you want to transfer to the *Payments* module. All listed events can be handled by Actindo.  You can exclude an event if you want to process specific events by another third-party application, for example. Alternatively, you can define the events to be ignored in the *Payments* module settings, see [Configure Adyen connection](./02_ManageAdyenConnection.md#configure-adyen-connection).

        ![Events](../../Assets/Screenshots/Adyen/Integration/AdyenEvents.png "[Events]")

5. Click the [Apply] button and enter the following settings in the *Security* section.

     - *Basic authentication*   
         - Define a username and password for the notification user, so that you can get notifications from Adyen&trade;. You can freely define them.

            ![Basic authentification](../../Assets/Screenshots/Adyen/Integration/BasicAuthentification.png "[Basic authentification]")

         - Change to your Actindo instance and enter the username and password in the *Notification user* and *Notification password* fields in the *Payments* settings. 
         
            ![Notification user and password](../../Assets/Screenshots/Adyen/Integration/AdyenNotificatioUser.png "[Notification user and password]")

         - Change back to Adyen&trade; and click the [Apply] button.
      
     - *HMAC key*   
         You can ignore this setting. It is currently not supported by the *Payments* module.   

6. Enter the following settings in the *Additional settings* section.
     - *3D Secure*   
        Select all entries and click the [Apply] button.

        ![3D Secure](../../Assets/Screenshots/Adyen/Integration/Adyen3DSecure.png)

7. Click the [Save changes] button in the bottom right corner.

8. Enable the standard webhook and test your configuration after you have saved the notification user and password in Actindo.  
<!--- Stefan, geht das hier schon, oder muss alles in Actindo eingetragen sein?-->



## Define synchronous or asynchronous processing

Define whether you want to transfer the payment data using synchronous or asynchronous processing. 
- At synchronous processing, Adyen&trade; creates a connection for each event that occurs. This has the advantage that Adyen&trade; is immediately informed if a message cannot be processed. The disadvantage is that the message transfer might be slow if a lot of events are to be transferred. See also [Blocked queue at synchronous processing](../Troubleshooting/01_SynchronousProcessing.md) in the Troubleshooting chapter.   
- At asynchronous processing, a message is not processed directly so that a lot of traffic can be handled. The message is first accepted and roughly checked for plausibility. It is then written to a message queue. After that, the message queue is processed periodically and can be run with parallel jobs. 


#### Prerequisites

- You have an Adyen&trade; customer account to log in to Adyen&trade;.
- You are logged in to Adyen&trade;.
- You are assigned to the required user roles in Adyen&trade;.


#### Procedure

*Adyen&trade; Backend > Developers > Webhooks*

![Webhook configuration in Adyen](../../Assets/Screenshots/Adyen/Integration/AdyenWebhooks.png "[Webhook configuration in Adyen]")

1. Click on your standard webhook.

2. Expand the *Server configuration* setting in the *General* section.

    ![Define server configuration](../../Assets/Screenshots/Adyen/Integration/AdyenChangeWebhookServerConguration.png "[Define server configuration]").

3. Configure the server URL as follows:   
    - If you want to process the messages asynchronously, add an **Async** to the address. For example: `https://customeraccount.dev.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notificationAsync`.

    - If you want to process the messages synchronously, add a **2** to the address. For example: `https://customeraccount.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notification2`.

4. Click the [Apply] button.   
    The synchronous or asynchronous processing has been defined.

5. Click the [Save changes] button in the bottom right corner.



## Create web service API credentials

Create the web service API credentials to send messages from the *Payments* module to the Adyen&trade; backend. For detailed information, see [API credentials](https://docs.adyen.com/development-resources/api-credentials/ "https://docs.adyen.com/development-resources/api-credentials/") in the Adyen&trade; documentation. 
<!---Hallo Stefan, kannst Du noch mal schauen ob die Richtung stimmt?Also von Payments to Adyen?--->

You must generate a web service API key for both the test environment and the live environment.

#### Prerequisites

- You have a valid user account in Adyen&trade;.
- You are assigned to the required user roles in Adyen&trade;.
- At least one connection has been created in the *Payments* module, see [Create Adyen connection](./02_ManageAdyenConnection.md#create-adyen-connection).
- The *Adyen* plugin is installed on the *Actindo Core1 Platform* system.
- You are logged in to your Actindo instance under *Payments > Settings > Select connection > Credentials tab*. For detailed information, see [Configure Adyen connection](02_ManageAdyenConnection.md#configure-adyen-connection).

#### Procedure

*Adyen&trade; Backend > Developers > API credentials*

![API credentials](../../Assets/Screenshots/Adyen/Integration/AdyenAPICredentialspng.png "[API credentials]")

1. Click the *Create new credential* button.   
   The *Create API credential* window is displayed. The *Web service user* credential type is selected by default. The username has been created automatically by the system.
   
   ![Create API credential](../../Assets/Screenshots/Adyen/Integration/AdyenCreateAPIcredential.png "[Create API credential]")

2. Copy the username.

3. Change to your Actindo instance. Enter the username in the *Payment user* field.
 
     ![Payment user](../../Assets/Screenshots/Adyen/Integration/AdyenWebServiceUser.png "[Payment user]")

4. Return to your Adyen&trade; account and enter a description for the web service user in the *Description* field.

    ![Create API credential](../../Assets/Screenshots/Adyen/Integration/AdyenCreateAPIcredential.png "[Create API credential]")

5. Click the [Create credential] button.   
    The *Configure API credential* view is displayed. The API key tab is displayed by default.

6. Generate the *Web service* API key and enter it in Actindo. To do this, follow these steps:

    1. Click the *API key* tab in the *Server settings > Authentication* section. 

    2. Click the [Generate API key] button, if you want to generate a new key.    
      The API key is automatically generated.

        ![Generate Checkout API key](../../Assets/Screenshots/Adyen/Integration/AdyenAuthentication.png "[Generate Checkout API key]")
    
    3. Click the *Copy API key* button.

    4. Change to your Actindo instance and insert the API key in the *Checkout API key* field. 

        ![Checkout API key](../../Assets/Screenshots/Adyen/Integration/AdyenCheckoutAPIkey.png "[Checkout API key]")

7. Return to your Adyen&trade; account and generate the *Web service* API password and enter it in Actindo. To do this, follow these steps:

    1. Click the *Basic auth* tab and click the [Generate password] button, if you want to generate a new password.   
      The password is automatically created.

        ![Web service password](../../Assets/Screenshots/Adyen/Integration/AdyenWebServicePassword.png "[Web service password]")
    
    2. Click the *Copy password* button. 

    3. Change to your Actindo instance and insert the password in the *Payment password* field.

       ![Payment password](../../Assets/Screenshots/Adyen/Integration/AdyenPaymentPassword.png "[Payment password]")

8. Return to Adyen&trade; and click the [Save changes] button in the bottom right corner.   
    The credentials for the *Web service* API are applied.

9. If necessary, configure your wallet payment methods in the *Wallet payment methods* section. Refer to the Adyen&trade; documentation. 

10. If necessary, assign roles to define the permissions of the API credentials in the *Permissions > Roles* section. For detailed information, see [API permissions](https://docs.adyen.com/development-resources/api-credentials/#api-permissions "[https://docs.adyen.com/development-resources/api-credentials/#api-permissions]") in the Adyen&trade; documentation.



## Create report service API credentials

Create the report service API credentials to receive the daily report from Adyen™. It collects all events of the day in a CSV file and sends it to Actindo. The *Payments* module then automatically checks if all these events have been successfully transferred (reconciliation).   
For detailed information, see [API credentials](https://docs.adyen.com/development-resources/api-credentials/ "[https://docs.adyen.com/development-resources/api-credentials/]") in the Adyen&trade; documentation. 

You must generate a report service API key for both the test environment and the live environment.

#### Prerequisites
- You have an Adyen&trade; customer account to log in to Adyen&trade;.
- You are logged in to Adyen&trade;.
- You are assigned to the required user roles in Adyen&trade;.
- The *Adyen* plugin is installed on the *Actindo Core1 Platform* system.
- At least one connection has been created in the *Payments* module, see [Create Adyen connection](./02_ManageAdyenConnection.md#create-adyen-connection).
- You are logged in to your Actindo instance under *Payments > Settings > Select connection > Credentials tab*.

#### Procedure

*Adyen&trade; Backend > Developers > API credentials*

![API credentials](../../Assets/Screenshots/Adyen/Integration/AdyenAPICredentialspng.png "[API credentials]")

1. Click the *Create new credential* button.   
   The *Create API credential* window is displayed. The *Web service user* credential type is displayed by default.
       
    ![Create API credential](../../Assets/Screenshots/Adyen/Integration/AdyenCreateAPIcredential.png "[Create API credential]")
   
2. Select the *Report service user* credential type.   
   The username is automatically created by the system.

    ![Create report service credentials](../../Assets/Screenshots/Adyen/Integration/AdyenReportServiceAPIcredential.png "[Create report service credentials]")   

3. Copy the username.

4. Change to your Actindo instance and paste the report username in the *Report user* field.
  
   ![Report username](../../Assets/Screenshots/Adyen/Integration/AdyenReportUser.png "[Report username]")   

5. Return to your Adyen&trade; account and enter a description for the report service user in the *Description* field.

    ![Create report service credentials](../../Assets/Screenshots/Adyen/Integration/AdyenReportServiceAPIcredential.png "[Create report service credentials]")

6. Click the [Create credential] button.   
    The *Configure API credential* view is displayed. The API key tab is displayed by default.

7. Generate the *Report service* API key and password. To do this, follow these steps:

    1. Click the *API key* tab in the *Server settings > Authentication* section.
    
    2. Click the [Generate API key] button, if you want to generate a new key.    
        The API key is automatically applied.  
        
        ![Configure API credentials](../../Assets/Screenshots/Adyen/Integration/AdyenAuthentication.png "[Configure API credentials]")

        > [Info] You do not need to enter the report API key in your *Payments* connection settings. For the *Payments* module, the report name and password are sufficient.

    3. Click the *Basic auth* tab in the *Server settings > Authentication* section.
   
    4. Click the [Generate password] button, if you want to generate a new password.   
      The password is automatically created.
   
       ![Report service password](../../Assets/Screenshots/Adyen/Integration/AdyenWebServicePassword.png "[Report service password]")

    5. Click the *Copy password* button.

8. Change to your Actindo instance and insert the password in the *Report password* field. 

   ![Report service password](../../Assets/Screenshots/Adyen/Integration/AdyenReportServicePassword.png "[Report service password]")

9. Return to your Adyen&trade; account and click the [Save changes] button in the bottom right corner.   
    The credentials for the *Report service* API are applied.

10. If necessary, assign the required report role to allow the technical user to download reports in the *Permissions > Roles > REPORT* section. For detailed information, see [API permissions](https://docs.adyen.com/development-resources/api-credentials/#api-permissions "[https://docs.adyen.com/development-resources/api-credentials/#api-permissions]") in the Adyen&trade; documentation.




