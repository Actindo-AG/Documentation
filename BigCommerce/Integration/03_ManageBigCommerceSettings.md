# Manage BigCommerce settings

Make sure that you do not allow using multiple shipping addresses.

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
    The *Advanced* section is displayed.

   ![BigCommerce advanced settings](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/BigCommerceSettings2.png "[BigCommerce advanced settings]")

2. Display the *Optimized one-page checkout settings* section.
    The *Optimized one-page checkout settings* section is displayed.

   ![Check multiple shipment addresses](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/CheckMultipleAddress.png "[Check multiple shipment addresses]")

3. Ensure that the *Allow customers to select multiple shipping addresses for an order* setting in the *Shipping* section is not selected.
