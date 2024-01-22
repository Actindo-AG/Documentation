# Manage Adyen settings

In addition to the settings in the *Payments* module, there are some settings necessary in the Adyen backend to ensure a smooth data transfer.



## Declare notification user and password

In the Payments module connection credentials, you have defined the credentials for the notification user. You must declare these credentials also in the Adyen backend settings, so that you can get notifications from Adyen.


#### Prerequisites

You have defined the credentials for the notification user, see [Configure Adyen connection](./01_ManageAdyenConnection.md).

#### Procedure


https://kundenaccount.dev.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notificationAsync


## Specify webhooks credentials

#### Prerequisites


#### Procedure



## Define synchronous or asynchronous processing

Define whether you want to transfer the payment data using synchronous or an asynchronous processing. For detailed information, see [Configure Adyen connection](./01_ManageAdyenConnection.md).

#### Prerequisites
- An Adyen connection has been created, see [Create Adyen connection](./01_ManageAdyenConnection.md#create-adyen-connection).
- You have a valid user account in Adyen.

#### Procedure

2. If you want to process the messages asynchronously, add an **Asynch** to the address. For example: https://kundenaccount.dev.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notificationAsync

3. If you want to process the messages synchronously, add a **2** to the address. For example: https://kundenaccount.actindo.com/Actindo.Extensions.Actindo.Adyen.Notification.notification2.


## Define event codes to be ignored

