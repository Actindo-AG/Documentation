[!!Omni-Channel](Actindo/Omni-Channel)
[!!Fakturierung](Actindo/Fakturierung)
[!!Venduo POS](Actindo/Venduo POS)

# Manage the POS order process


## Check the POS order status

Check the POS order in Omni-Channel to see its current status.

### Prerequisites

An order has been completed in POS, see [Complete a purchase](04_CompletePurchase.md).

### Procedure

*Omni-Channel > Orders and Returns > Tab ORDERS*

![Omni-Channel Orders](/Assets/Screenshots/OmniChannel/OrdersReturns/Orders/Orders.png "[Omni-Channel Orders]")

 > [Info] The ordering process is performed asynchronously. That means that it may take a few minutes until the POS order is displayed in the order list in the *Omni-Channel* module. If the POS order is not yet displayed, click the button ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) in the upper right corner to update the order list.

1. Check the column *Status of Import from Channel* .   
    The following table shows the possible statuses and their meaning.

    | Status         | Meaning               |
    |----------------|-----------------------|
    | Imported       | The order is imported from the specified channel, but it is still pending completion. |
    | Order complete | The order is fully completed in the specified channel and successfully imported. |
    | Canceled       | The order was canceled in the specified channel and will not be imported. |

[comment]: <> (Are there other statuses? Meaning?)

2. Check the column *Status of Export to Channel* .   
    The following table shows the possible statuses and their meaning.

    | Status         | Meaning               |
    |----------------|-----------------------|
    | Exported       | to be completed |
    | No Changes to sync |to be completed |

[comment]: <> (Are there other statuses? Meaning?)

3. Check the column *Status of Export to OMS* .   
    The following table shows the possible statuses and their meaning.

    | Status         | Meaning               |
    |----------------|-----------------------|
    | Exported       | The order is successfully exported to invoicing. The receipt number in invoicing is displayed in the column *ID in OMS* |
    | Not exported   | The order is still pending export to invoicing. |
    | Error! followed by the error description | The export failed. An error occurred. Check the error description and go to the chapter [*Troubleshooting*](VenduoPOS/Troubleshooting/00_Troubleshooting.md) for help.|

[comment]: <> (Are there other statuses? Meaning?)

4. Check the column *ID in OMS* .    
    If the order has been successfully exported to invoicing, the receipt number of the order in invoicing is displayed in this column.

[comment]: <> (Are there other important columns to check?)

### Next steps

- [Check the cash invoice](#check-the-cash-invoice)
- [Check the payment](#check-the-payment)

### See also

- [User Interface Omni-Channel](/OmniChannel/UserInterface/00_UserInterface.md)
- [Manage offers for POS](07_ManageOffers.md)



## Check the cash invoice

Check the cash invoice in invoicing to see its current status.

### Prerequisites

An order has been completed in POS, see [Complete a purchase](04_CompletePurchase.md).

### Procedure

*Fakturierung > Übersicht > Tab ÜBERSICHT*

![Fakturierung Übersicht](/Assets/Screenshots/Fakturierung/Uebersicht/Uebersicht.png "[Invoicing Overview]")

 > [Info] The invoicing process is performed asynchronously. That means that it may take a few minutes until the invoice is displayed in the invoicing list in the *Fakturierung* module. If the invoice is not yet displayed, click the button ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) in the bottom to update the invoicing list.

1. Right-click the row with the appropriate receipt number.   
    The context menu is displayed.

    ![Context Menu](/Assets/Screenshots/Fakturierung/ContextMenu.png "[Context Menu]")

2. Click the menu entry *Beleg bearbeiten* .   
    The menu entry *Last Receipt* is opened. The tab *LETZTER BELEG (RB Number)* with the selected receipt is displayed.

    ![Last Receipt](/Assets/Screenshots/Fakturierung/LetzterBeleg/Kunde01.png "[Last Receipt]")

3. Click first the tab *Kunde*, then the sub tab *Rechnungs-Adresse* and check the invoice address of the receipt.

4. Click the sub tab *Liefer-Adresse* and check the delivery address of the receipt.

5. Click the tab *Positionen* and check the articles of the order.

![Last Receipt](/Assets/Screenshots/Fakturierung/LetzterBeleg/Positionen03.png "[Last Receipt]")

6. Select an article in the tab *Positionen* .   
  The details to the selected article are displayed in the sub tabs in the bottom part of the tab *Positionen*.

7. Click the sub tab *Lager* in the bottom part of the tab *Positionen* and check the details of the warehouse withdrawal.

 > [Info] Note that changes you made in the receipt are not synced back to the *Venduo POS* module.


### Next steps

- [Check the payment](#check-the-payment)

### See also

- [User Interface Fakturierung](/Fakturierung/UserInterface/00_UserInterface.md)
- [Check the POS order status](#check-the-pos-order-status)
- [Manage offers for POS](07_ManageOffers.md)



## Check the payment

Check the current status of the booking and its payment.

### Prerequisites

An order has been completed in POS, see [Complete a purchase](04_CompletePurchase.md).

### Procedure

*Venduo POS > Management > Tab BUCHHALTUNGS-SYNC*

![Buchhaltungs-Sync](/Assets/Screenshots/VenduoPOS/Management/BuchhaltungsSync/BuchhaltungsSync.png "[Buchhaltungs-Sync]")

1. Check the order status for the order in the column *Status*.   

  > [Info] The payment process is performed asynchronously. That means that it may take a few minutes until the payment is synchronized with the invoicing. If the status of the order is still **Pending**, click the button [KICK JOB] in the upper left corner of the list to start a new synchronization with invoicing.

2. When the order status of the order is **Sync successful**, switch to the *Fakturierung* module: *Fakturierung > Übersicht* .   
    The menu entry *Übersicht* is opened. The tab *ÜBERSICHT* with the invoicing list is displayed.

    ![Fakturierung Übersicht](/Assets/Screenshots/Fakturierung/Uebersicht/Uebersicht.png "[Invoicing Overview]")

3. Click the button ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) in the bottom of the invoicing list.
    The invoicing list is updated.

4. Check the payment status of the invoice in the column *Bezahlt*.

### See also

- [User Interface Venduo POS](VenduoPOS/UserInterface/00_UserInterface.md)
- [Check the POS order status](#check-the-pos-order-status)
- [Manage offers for POS](07_ManageOffers.md)
- [Check the cash invoice](#check-the-cash-invoice)
