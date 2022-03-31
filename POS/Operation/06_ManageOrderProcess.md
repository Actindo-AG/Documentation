[!!Omni-Channel](Channels)
[!!Invoicing](RetailSuiteFaktBase)
[!!Venduo POS](POS)

# Manage the POS order process

Trace the POS order process by checking the order status, the cash invoice and the payment of an order.


## Check the POS order status

Check the POS order in Omni-Channel to see its current status.

### Prerequisites

An order has been completed in POS, see [Complete a purchase](04_CompletePurchase.md).

### Procedure

*Omni-Channel > Orders and Returns > Tab ORDERS*

![Omni-Channel Orders](/Assets/Screenshots/Channels/OrdersReturns/Orders/Orders.png "[Omni-Channel Orders]")

 > [Info] The ordering process is performed asynchronously. That means that it may take a few minutes until the POS order is displayed in the order list in the *Omni-Channel* module. If the POS order is not yet displayed, click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the upper right corner to update the order list.

1. Check the *Status of Import from Channel* column.   
    The following table shows the possible statuses and their meaning.

    | Status         | Meaning               |
    |----------------|-----------------------|
    | Imported       | The order is imported from the specified channel, but it is still pending completion. |
    | Order complete | The order is fully completed in the specified channel and successfully imported. |
    | Canceled       | The order was canceled in the specified channel and will not be imported. |

[comment]: <> (Are there other statuses? Meaning?)

2. Check the *Status of Export to Channel* column.   
    The following table shows the possible statuses and their meaning.

    | Status         | Meaning               |
    |----------------|-----------------------|
    | Exported       | to be completed |
    | No Changes to sync |to be completed |

[comment]: <> (Are there other statuses? Meaning?)

3. Check the *Status of Export to OMS* column.   
    The following table shows the possible statuses and their meaning.

    | Status         | Meaning               |
    |----------------|-----------------------|
    | Exported       | The order is successfully exported to invoicing. The receipt number in invoicing is displayed in the *ID in OMS* column|
    | Not exported   | The order is still pending export to invoicing. |
    | Error! followed by the error description | The export failed. An error occurred. Check the error description and go to the [*Troubleshooting*](/POS/Troubleshooting/00_Troubleshooting.md) chapter for help.|

[comment]: <> (Are there other statuses? Meaning?)

4. Check the column *ID in OMS* column.    
    If the order has been successfully exported to invoicing, the receipt number of the order in invoicing is displayed in this column.

[comment]: <> (Are there other important columns to check?)

### Next steps

- [Check the cash invoice](#check-the-cash-invoice)
- [Check the payment](#check-the-payment)

### See also

- [User Interface Omni-Channel](/Channels/UserInterface/00_UserInterface.md)
- [Manage offers for POS](07_ManageOffers.md)



## Check the cash invoice

Check the cash invoice in invoicing to see its current status.

### Prerequisites

An order has been completed in POS, see [Complete a purchase](04_CompletePurchase.md).

### Procedure

*Invoicing > Overview > Tab OVERVIEW*

![Overview](/Assets/Screenshots/RetailSuiteFaktBase/Overview/Overview.png "[Overview]")

 > [Info] The invoicing process is performed asynchronously. That means that it may take a few minutes until the invoice is displayed in the invoicing list in the *Invoicing* module. If the invoice is not yet displayed, click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the bottom to update the invoicing list.

1. Right-click the row with the appropriate document number.   
    The context menu is displayed.

    ![Context Menu](/Assets/Screenshots/RetailSuiteFaktBase/ContextMenu.png "[Context Menu]")

2. Click the *Edit document* entry.   
    The *Last document* menu entry is opened. The *LAST DOCUMENT* tab with the selected document is displayed.

    ![Last document](/Assets/Screenshots/RetailSuiteFaktBase/LastDocument/Customer.png "[Last document]")

3. Click first the *Customer* tab, then the *Billing address* sub-tab and check the billing address of the document.

4. Click the *Delivery address* sub-tab and check the delivery address of the document.

5. Click the *Positions* tab and check the products of the order.

![Last document](/Assets/Screenshots/RetailSuiteFaktBase/LastDocument/Positions.png "[Last document]")

6. Select a product in the *Positions* tab.   
  The details to the selected product are displayed in the sub-tabs in the bottom part of the *Positions* tab.

7. Click the *Stock location* sub-tab in the bottom part of the *Positions* tab and check the details of the stock.

 > [Info] Note that changes you made in the documents are not synced back to the *Venduo POS* module.


### Next steps

- [Check the payment](#check-the-payment)

### See also

- [User Interface Invoicing](/RetailSuiteFaktBase/UserInterface/00_UserInterface.md)
- [Check the POS order status](#check-the-pos-order-status)
- [Manage offers for POS](07_ManageOffers.md)



## Check the payment

Check the current status of the booking and its payment.

### Prerequisites

An order has been completed in POS, see [Complete a purchase](04_CompletePurchase.md).

### Procedure

*Venduo POS > Management > Tab ACCOUNTING SYNC*

![Accounting Sync](/Assets/Screenshots/POS/Management/AccountingSync/AccountingSync.png "[Accounting Sync]")

1. Check the order status for the order in the *Status* column.   

  > [Info] The payment process is performed asynchronously. That means that it may take a few minutes until the payment is synchronized with the invoicing. If the status of the order is still **Pending**, click the [KICK JOB] button in the upper left corner of the list to start a new synchronization with invoicing.

2. When the order status of the order is **Sync successful**, switch to the *Invoicing* module: *Invoicing > Overview* .   
    The *Overview* menu entry is opened. The *OVERVIEW* tab with the invoicing list is displayed.

    ![Overview](/Assets/Screenshots/RetailSuiteFaktBase/Overview/Overview.png "[Overview]")

3. Click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button in the bottom of the invoicing list.
    The invoicing list is updated.

4. Check the payment status of the invoice in the *Paid* column.

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [User Interface Invoicing](/RetailSuiteFaktBase/UserInterface/00_UserInterface.md)
- [Check the POS order status](#check-the-pos-order-status)
- [Manage offers for POS](07_ManageOffers.md)
- [Check the cash invoice](#check-the-cash-invoice)
