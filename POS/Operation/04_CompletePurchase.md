[!!Venduo POS](POS)

# Complete a purchase

To complete a purchase, you need to initiate the payment. At the Venduo POS pay desk, you have several options to complete the payment process, for instance by cash payment, by cashless payment or by voucher. You can also assign a discount to one or more items on the bill list or park a payment for a later time.

## Pay cash

If a customer wishes to pay in cash, the payment process in the pay desk must be completed as follows.

### Prerequisites

At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the [PAY] button at the bottom of the bill list.   
  The payment view is displayed in the bill list.

   ![Pay](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/Pay.png "[Pay]")

2. In the *Select Payment* section you can complete the cash payment by two different ways:   

   a. Use Quick Select to select the cash payment amount   

  1. Click one of the buttons in the *Quick Select* section. The offered amounts on the buttons vary depending on the amount of the purchase and the denomination of the currency defined in the global settings.   
   The *Payment Pending* view is displayed while the payment is being processed.   

     ![Payment Pending](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentPending.png "[Payment Pending]")

     The *Payment successful* view is displayed when the payment is completed.   

     ![Payment Successful](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentSuccessful.png "[Payment Successful]")

  2. Click the [Done] button.   
     The purchase is completed. The bill list is displayed again.


  b. Select the cash payment amount

  1. Click the [Cash] button.   
     The *Cash payment* view is displayed.

     ![Cash payment](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/CashPayment.png "[Cash payment]")

  2. Enter the cash payment amount in the *Amount* field or select an amount by clicking the number buttons in the lower area.

  3. Click the [Pay] button in the bottom right corner.   
     The *Payment Pending* view is displayed while the payment is being processed.   

     ![Payment Pending](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentPending.png "[Payment Pending]")

     The *Payment successful* view is displayed when the payment is completed.   

     ![Payment Successful](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentSuccessful.png "[Payment Successful]")

  4. Click the [Done] button.   
     The purchase is completed. The bill list is displayed again.

### Next steps

- [Open the drawer](#open-the-drawer)
- [Pay cashless at the terminal](#pay-cashless-at-the-terminal)
- [Pay with voucher](#pay-with-voucher)
- [Manage a parked bill](#manage-a-parked-bill)
- [Cancel a purchase](#cancel-a-purchase)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)



## Open the drawer

Generally, you open the cash drawer when you accept a cash payment or when you want to store the receipt in the drawer for a cashless payment.
In case of cash or cashless payment, the option to open the drawer can be activated or deactivated in the settings.
If you want to open the drawer independently of a payment process, for instance to change money, you can do so as follows.

### Prerequisites

- A pay desk is opened, see [Open a pay desk](01_OpenPayDesk.md).

### Procedure

*Venduo POS > Sales > Select Store and Pay Desk*

1. Click the *CASHPOINT* tab.   
   The *CASHPOINT* tab is displayed.

   ![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

2. Click the [ ![Open Drawer](/Assets/Icons/Drawer.png "[Open Drawer]") Open Drawer] button at the bottom part of the bill list.   
   The drawer opens.

or

1. Click the *CASH REGISTER* tab.   
   The *CASH REGISTER* tab is displayed.

   ![Cash Register](/Assets/Screenshots/POS/Sales/CashRegister/CashRegister.png "[Cash Register]")

2. Click the [ ![Open drawer](/Assets/Icons/Drawer.png "[Open drawer]") Open drawer] button at the top of the *Cash In/Out* section.   
   The drawer opens.

### Next steps

- [Pay cashless at the terminal](#pay-cashless-at-the-terminal)
- [Pay with voucher](#pay-with-voucher)
- [Manage a parked bill](#manage-a-parked-bill)
- [Cancel a purchase](#cancel-a-purchase)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)
- [Pay cash](#pay-cash)



## Pay cashless at the terminal

[comment]: <> (need more information!)

If a customer wishes to pay cashless, the payment process in the pay desk must be completed as follows. Currently, it's not possible to connect an external terminal to POS. The payment process itself has to be completed at the external terminal. Nevertheless, you can book the payment in your pay desk for the statistic and to transfer it in your accounts.  

### Prerequisites

At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the [PAY] button at the bottom of the bill list.   
   The payment view is displayed in the bill list.

   ![Pay](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/Pay.png "[Pay]")

2. Click the [ ![Terminal](/Assets/Icons/Terminal.png "[Terminal]") MANUAL PAYMENT AT TERMINAL] button at the right side of the *Select Payment* section.   
   The *Cashless payment* view is displayed.

   ![Cashless payment](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/CashlessPayment.png "[Cashless payment]")

3. Select the card type in the drop-down list *Card type*.
  The selected card type is displayed in the drop-down list.

[comment]: <> (Is card type correct? It could also be Paypal, or another cardless method...)

4. Click the [Finalize payment process] button.   
   The *Payment at teminal* view is displayed when the payment is completed.

   ![Payment at teminal](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentTerminal.png "[Payment at terminal]")


5. Click the [Done] button.   
   The purchase is completed. The bill list is displayed again.

### Next steps

- [Pay with voucher](#pay-with-voucher)
- [Manage a parked bill](#manage-a-parked-bill)
- [Cancel a purchase](#cancel-a-purchase)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)
- [Pay cash](#pay-cash)
- [Open the drawer](#open-the-drawer)



## Pay with voucher

In addition to cash and cashless payment, customers can also pay with vouchers.

### Prerequisites

At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the [PAY] button at the bottom of the bill list.   
   The payment view is displayed in the bill list.

   ![Pay](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/Pay.png "[Pay]")

2. Click the *Voucher code* field at the top in the *Vouchers* section and enter the voucher code.   

3. Click the [REDEEM] button to the right of the *Voucher code* field.   
   The voucher is indicated in the *Settlement* section of the bill list.

    > [Info] The current value of the voucher is displayed on the left side, the amount that will be redeemed at purchase is displayed on the right side. The remaining total of the purchase is indicated below. If the voucher amount is higher than the purchase amount, the voucher is reduced by the purchase amount and the remaining total 0.00 € is displayed on the bill list.

   ![Pay voucher](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PayVoucher.png "[Pay voucher]")

      > [Info] To the right of the indicated voucher amount, on the edge of the bill list, the ![Remove](/Assets/Icons/Cross06.png "[Remove]") (Remove) flag is displayed. Click the flag to remove the voucher from the payment.

  [comment]: <> (Is there a predefined way how to complete the purchase when total = 0?)

4. Complete the purchase by paying the remaining total either by cash or cashless payment:
  - For cash payment, see [Pay cash](#pay-cash).
  - For cashless payment, see [Pay cashless at the terminal](#pay-cashless-at-the-terminal).

### Next steps

- [Manage a parked bill](#manage-a-parked-bill)
- [Cancel a purchase](#cancel-a-purchase)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)
- [Pay cash](#pay-cash)
- [Open the drawer](#open-the-drawer)
- [Pay cashless at the terminal](#pay-cashless-at-the-terminal)


## Manage a parked bill

You can park a purchase, for instance if a customer has forgotten the wallet and resume it at a later time.

### Prerequisites

At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

#### Park a bill

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the [ ![Park](/Assets/Icons/Park.png "[Park]") Park] button at the bottom of the bill list.   
   A window to enter a title for the purchase is displayed in the bill list.

   ![Park bill](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ProductParkBill.png "[Park bill]")

2. Enter a descriptive name for the purchase in the *Title* field.

  > [Info] If you want to resume the purchase, you should be able to recognize the purchase by this title.

3. Click the [Park] button.   
   The purchase is parked. The [ ![Park](/Assets/Icons/Park.png "[Park]") PARKED] flag is displayed in the upper part to the right of the bill list. The bill list is empty.

   ![Parked bill](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ProductParkedBill.png "[Parked bill]")

  > [Info] The number on the flag indicates the numbers of parked purchases.

#### Resume a parked bill

If you have parked a purchase, you can resume it as follows.

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/ParkedBill.png "[Cashpoint]")

1. Click the [ ![Park](/Assets/Icons/Park.png "[Park]") PARKED] flag in the upper part to the right of the bill list.   
   The *Parked bills* window is displayed.

   ![Parked bills](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ParkedBills01.png "[Parked bills]")

2. Click the appropriate bill.   
   The [Cancel] and the [Resume] buttons are displayed in the window.

   ![Parked bills](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ParkedBills02.png "[Parked bills]")

3. Click the [Resume] button.   
   The purchase is resumed. The parked bill list is displayed again.

   ![Bill List Product](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/Product.png "[Bill List Product]")

4. Complete the purchase by editing the bill list or paying the remaining total either by cash or cashless payment:
  - For cash payment, see [Pay cash](#pay-cash).
  - For cashless payment, see [Pay cashless at the terminal](#pay-cashless-at-the-terminal).
  - For payment with voucher, see [Pay with voucher](#pay-with-voucher).


### Next steps

- [Cancel a purchase](#cancel-a-purchase)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)
- [Pay cash](#pay-cash)
- [Open the drawer](#open-the-drawer)
- [Pay cashless at the terminal](#pay-cashless-at-the-terminal)
- [Pay with voucher](#pay-with-voucher)



## Cancel a purchase

You can cancel a purchase, for instance if a customer decides against the purchase at short notice.   

### Prerequisites

At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the ![Delete](/Assets/Icons/Trash02.png "[Delete]") (Delete) button at the bottom of the bill list.   
   The current purchase is canceled. The bill list is empty.

  > [Info] If you click the ![Delete](/Assets/Icons/Trash02.png "[Delete]") (Delete) button the entire purchase is canceled without further query. The cancellation cannot be undone.

### Next steps

- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)
- [Pay cash](#pay-cash)
- [Open the drawer](#open-the-drawer)
- [Pay cashless at the terminal](#pay-cashless-at-the-terminal)
- [Pay with voucher](#pay-with-voucher)
- [Manage a parked bill](#manage-a-parked-bill)
