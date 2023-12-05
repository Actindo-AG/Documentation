# Manage BigCommerce settings


## Manage API settings

As the driver creates automatically the necessary API settings during creating the connection, you have no need for further actions. See the *Store-level API account* in your *BigCommerce* store under *Settings > API*. 

![Store-level API accounts](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/StoreLevelApiAccount.png "[BigCommerce settings]")


## Manage multiple shipping addresses

Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only. Any orders that use multiple shipping addresses cannot be imported and will fail during the import.  
To avoid failures during the import, you must check a specific setting in *BigCommerce*. 

#### Prerequisites

- A *BigCommerce* connection has been created.
- You have a valid user account in *BigCommerce*.

#### Procedure

*BigCommerce store > Settings*

![BigCommerce settings](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/BigCommerceSettings.png "[BigCommerce settings]")

1. Display the *Advanced* section and click the *Checkout* entry.

   ![BigCommerce advanced settings](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/BigCommerceSettings2.png "[BigCommerce advanced settings]")

2. Display the *Optimized one-page checkout settings > Shipping* section.

   ![Check multiple shipment addresses](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/CheckMultipleAddress.png "[Check multiple shipment addresses]")

3. Ensure that the *Allow customers to select multiple shipping addresses for an order* setting is not selected.
