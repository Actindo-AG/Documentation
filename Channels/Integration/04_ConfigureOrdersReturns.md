[!!User interface Orders](../UserInterface/05a_Orders.md)
[!!User interface Returns](../UserInterface/05b_Returns.md)

# Configure the orders and returns

When an order is placed in the marketplace, this order must be imported to *Omni-Channel* in order to further process it in the *Order Management* module.   

To import orders and returns to *Omni-Channel*, you can configure an automatic import at a certain time interval.


## Configure the order import

Configure the time interval at which the orders will be automatically imported to the *Omni-Channel* module. You can configure a different interval for each connection.

#### Prerequisites

A connection to a marketplace has been established, see [Create a connection](../../Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Omni-Channel > Orders and Returns > Tab ORDERS*

![Orders](../../Assets/Screenshots/Channels/OrdersReturns/Orders/Orders.png "[Orders]")

1. Click the *All connections* drop-down list and select the connection for which you want to configure the import settings. All available connections are displayed in the list.   
    The *Download orders automatically* drop-down list and the [SAVE] button are displayed to the right of the *All connections* drop-down list.

    ![Orders connection](../../Assets/Screenshots/Channels/OrdersReturns/Orders/OrdersConnection.png "[Orders connection]")

2. Click the *Download orders automatically* drop-down list and select the desired time interval at which the orders will be automatically downloaded. By default, the **never** option is preselected. The following options are available:   
    - **never**
    - **every 2 minutes**
    - **every 5 minutes**
    - **every 10 minutes**
    - **every 15 minutes**
    - **every 20 minutes**
    - **every 30 minutes**
    - **every 60 minutes**

3. Click the [SAVE] button.    
    The configured time interval is saved for the selected connection.

> [Info] Repeat this procedure for each connection to configure a time interval for the automatic download of orders. To manually import the orders, see [Import orders](../Operation/04_ManageOrdersReturns.md#import-orders).



## Configure the return import

Configure the time interval at which the returns will be automatically imported to the *Omni-Channel* module. You can configure a different interval for each connection.

#### Prerequisites

A connection to a marketplace has been established, see [Create a connection](../../Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Omni-Channel > Orders and Returns > Tab RETURNS*

![Returns](../../Assets/Screenshots/Channels/OrdersReturns/Returns/Returns.png "[Returns]")

1. Click the *All connections* drop-down list and select the connection for which you want to configure the import settings. All available connections are displayed in the list.   
    The *Download returns automatically* drop-down list and the [SAVE] button are displayed to the right of the *All connections* drop-down list.

    ![Returns connection](../../Assets/Screenshots/Channels/OrdersReturns/Returns/ReturnsConnection.png "[Returns connection]")

2. Click the *Download returns automatically* drop-down list and select the desired time interval at which the returns will be automatically downloaded.  By default, the **never** option is preselected. The following options are available:   
    - **never**
    - **every 2 minutes**
    - **every 5 minutes**
    - **every 10 minutes**
    - **every 15 minutes**
    - **every 20 minutes**
    - **every 30 minutes**
    - **every 60 minutes**   

3. Click the [SAVE] button.    
    The configured time interval is saved for the selected connection.

> [Info] Repeat this procedure for each connection to configure a time interval for the automatic download of returns. To manually import the returns, see [Import returns](../Operation/04_ManageOrdersReturns.md#import-returns).