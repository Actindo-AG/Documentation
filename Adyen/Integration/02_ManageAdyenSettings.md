# Manage Adyen settings

In addition to the settings in the *Payments* module, there are some settings necessary in the Adyen backend to ensure a smooth data transfer.

The following procedures contain information on the settings to be configured in the Adyen backend. It shows the standard procedure that was current at the time this documentation was created. For the latest detailed descriptions, refer to the Adyen documentation. 

## Create Adyen webhook

Create a webhook to receive payment notifications from Adyen to the *Payments* module such as authorizations and cancellations. For detailed information, see [https://docs.adyen.com/development-resources/webhooks/](https://docs.adyen.com/development-resources/webhooks/) in the Adyen documentation. It includes a video that may also be helpful.



#### Prerequisites

- You have a valid user account in Adyen.
- You are assigned to the **Merchant technical integrator** role in Adyen.


#### Procedure

*Adyen Backend > Developers > Webhooks*

![Webhook configuration in Adyen](../../Assets/Screenshots/Adyen/Integration/AdyenWebhooks.png)

1. Add a new standard webhook.
    A new standard webhook is added.

   ![Create webhook in Adyen](../../Assets/Screenshots/Adyen/Integration/AdyenCreateWebhook.png)

2. Enter the following settings in the *General* section.
    - *Description*  
        Enter a description for the webhook.
    - *Server configuration section*   
         - *URL*   
           Enter the server URL of the Actindo productive system or sandbox you want to connect.    
           For example: https://kundenaccount.dev.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notificationAsync. This example displays the server URL for asynchronous processing. For detailed information on synchronous processing, see [Define synchronous or asynchronous processing](#define-synchronous-or-asynchronous-processing). 
      
         - *Method*   
            You can use the standard setting **JSON** if you have no other requirements.

        - *Encryption protocol*     
           You can use the standard setting **TLSv1.3** if you have no other requirements

        - *Service version*
            You can use the standard setting **1** if you have no other requirements.
            
          ![Define server configuration](../../Assets/Screenshots/Adyen/Integration/AdyenCreateWebhookServerConfig.png).

3. Click the [Apply] button and proceed with the following fields in the *General* section.

    - *Merchant account*   
        Enter the merchant account(s) you want to connect.
    - *Events*   
        Select all events you want to transfer to the *Payments* module. All listed events can be handled by Actindo. You can exclude an event if you want to process specific events by another third-party application, for example. Alternatively, you can define the events to be ignored in the *Payments* module settings, see [Configure Adyen connection](./01_ManageAdyenConnection.md#configure-adyen-connection).

3. Enter the following settings in the *Security* section.

     - *Basic authentication*   
         In the *Payments* module connection credentials, you have defined the credentials for the notification user. You must declare these credentials also in the Adyen backend settings, so that you can get notifications from Adyen.   
         Enter the server's username and password that you have defined as *Notification user* and *Notification password* in the *Payments* settings.

         ![Notification user and password](../../Assets/Screenshots/Adyen/Integration/AdyenNotificatioUser.png)

     - *HMAC key*   
         You can ignore this setting. It is currently not supported by the *Payments* module.   

4. Enter the following settings in the *Additional settings* section.
     - *3D secure*   
        Select all entries.

5. Save your settings.

6. Enable the standard webhook and test your configuration.


## Define synchronous or asynchronous processing

Define whether you want to transfer the payment data using synchronous or an asynchronous processing. For detailed information, see [Configure Adyen connection](./01_ManageAdyenConnection.md).

#### Prerequisites
- An Adyen connection has been created, see [Create Adyen connection](./01_ManageAdyenConnection.md#create-adyen-connection).
- You have a valid user account in Adyen.

#### Procedure

*Adyen Backend > Developers > Webhooks*

![Webhook configuration in Adyen](../../Assets/Screenshots/Adyen/Integration/AdyenWebhooks.png)

1. Open your standard webhook for editing in the Adyen backend.

2. Edit the *Server configuration* setting in the *General* section.

    ![Define server configuration](../../Assets/Screenshots/Adyen/Integration/AdyenCreateWebhookServerConfig.png).

3. Configure the server URL as follows:
     - If you want to process the messages asynchronously, add an **Asynch** to the address. For example: https://kundenaccount.dev.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notificationAsync

    - If you want to process the messages synchronously, add a **2** to the address. For example: https://kundenaccount.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notification2.

4. Click the [Apply] button.
    The synchronous or asynchronous processing has been defined.



## Create API credentials

Create the API credentials to send messages from the *Payments* module to the Adyen backend. For detailed information, see [https://docs.adyen.com/development-resources/api-credentials/](https://docs.adyen.com/development-resources/api-credentials/) in the Adyen documentation. 

You must define both the credentials for the Checkout API and the Report API. 
When you switch to your live environment, you must generate a new API key in your live Customer Area.


#### Prerequisites

You have got information on the API endpoints.

#### Procedure

*Adyen Backend > Developers > API credentials*


API credent