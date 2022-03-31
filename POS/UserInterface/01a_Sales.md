# Cashpoint

*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

- *Find offer by nam... ![Search](/Assets/Icons/Search.png "[Search]")*   
  Enter the product name, the keyword or the (EAN) number you search for in the search bar. Click a product in the list of search results to add it to the bill list.

  > [Info] The search already provides you with proposals for your keyword as you type.

- *QuickSelect Category*    
  Click a QuickSelect category tab to display the associated QuickSelect elements. The tabs are only displayed if a QuickSelect category with an element has been created before. The categories are named individually.

- *QuickSelect Element*   
  Click a QuickSelect element to add it to the bill list. The QuickSelect element is only displayed if a QuickSelect category with an element has been created before. The elements are named individually.

  > [Info] For detailed information, see [Create a QuickSelect Category](VenduoPOS/Integration/07_ManageOffers.md#create-a-quickselect-category).


## Bill List

![Bill List](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/BillList.png "[Bill List]")

- ![Add Customer](/Assets/Icons/Customer02.png "[Add Customer]") (Add Customer)   
  Click this button to assign the bill to a certain customer. The *Add Customer* view is displayed.

- *Customer Name and Address*   
  The customer name and address is displayed, when the bill list is assigned to a customer. This field is read-only.

- ![Unassign Customer](/Assets/Icons/Trash01.png "[Unassign Customer]") (Unassign Customer)  
  Click this button to unassign the customer from the bill list. The button is only displayed when the bill list is already assigned to a customer.

- *Quantity x*    
  Quantity of the product in the bill list. This field is displayed only when a product is added to the bill list.

- *Name*   
  Product name. This field is displayed only when a product is added to the bill list.

- *Price*   
  Total net price of the product(s). This field is displayed only when a product is added to the bill list.   
  By default, the price is displayed in black. If the price has been modified, it is displayed differently.
    - Price is written in red and followed by an amount/a percentage in brackets: The red price is a discount price, the discount is indicated in brackets, either as a fixed discount or percentage.
    - Price is written in italics: The price itself has been modified.


- ![Remove Product](/Assets/Icons/Cross02.png "[Remove Product]") (Remove Product)   
  Click this button to remove a product entry from the bill list. This field is displayed only when a product is added to the bill list.

- *![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Single Scan*   
  Activate this toggle to use the single scan feature.

  > [Info]   If the same offer is selected more than once and you use the single scan feature, each offer is listed as a single product in the bill list. This allows you to treat each product in the booking individually.

- *Sub total*   
  Gross amount of all products in the bill list. This field is read-only.

- *Tax*   
  Tax amount of all products in the bill list. This field is read-only.

- *Add Sale Note*   
  Enter a sale note to add any additional information to the bill list.

- [ ![Drawer](/Assets/Icons/Drawer.png "[Drawer]") Open Drawer]   
  Click this button to open the drawer.

- [ ![Park](/Assets/Icons/Park.png "[Park]") Park]   
  Click this button to park the current bill list to a later time.

- ![Delete Bill List](/Assets/Icons/Trash02.png "[Delete Bill List]") (Delete Bill List)   
  Click this button to delete the current bill list.

- [PAY]   
  Click this button to start the payment process. The payment view is displayed in the bill list. The total net amount of the purchase is displayed at the right of the [PAY] button.


## Pay Bill List
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > [PAY]*

![Pay](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/Pay.png "[Pay]")   

- *Customer Name and Address*   
  The customer name and address is displayed, when the bill list is assigned to a customer. This field is read-only.


**Vouchers**

This section is only displayed when no voucher has been redeemed.

- *Gutscheincode*   
  Enter a voucher code to apply the voucher to the invoice.

- [REDEEM]   
  Click this button to redeem the voucher. A voucher can only be redeemed with a correct voucher code.


**Settlement**

- *Sub total*   
  Gross amount of all products in the bill list. This field is read-only.

- *Tax*   
  Tax amount of all products in the bill list. This field is read-only.

- [+ DISCOUNT]   
  Click this button to apply a discount to the bill. The *Discount on bill* view is displayed. This button is only displayed when no discount has been selected.

- [Discount ![Calculator](/Assets/Icons/Calculator02.png "[Calculator]") ]      
  Selected discount. Click this button to edit the discount. This button is only displayed when a discount is selected.

- ![Remove Discount](/Assets/Icons/Cross06.png "[Remove Discount]") (Remove Discount)    
  Click this button to remove the discount. The button is only displayed when a discount is selected.

- *Voucher (xxxxxxx)*   
  Redeemed voucher with the voucher code in brackets. The remaining amount of the voucher is displayed on the left, the amount of the voucher to be credited on the right. This field is read-only.

- ![Remove Voucher](/Assets/Icons/Cross06.png "[Remove Voucher]") (Remove Voucher)    
  Click this button to remove the voucher. The button is only displayed when a voucher is redeemed.

- *Total:*   
  Total net amount of the bill. This field is read-only.


**Select Payment**

- [EUR]   
  Default currency that is used for the payment.
  [comment]: <> (Is it possible to add a second currency? Why is this a button when I cannot choose?)

- [Cash]   
  Click this button to pay cash. The *Cash payment* view is displayed.

**Quick Select**

- [Amount]   
  Click a button with a proposed cash amount. The offered amounts on the buttons vary depending on the amount of the purchase and the denomination of the currency defined in the global settings.  

**-- or --**

- [ ![Terminal](/Assets/Icons/Terminal.png "[Terminal]") MANUELLES ZAHLEN AM TERMINAL]   
  Click this button to pay cashless. The *Cashless payment* view is displayed.

## Cash Payment
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > [PAY] > [CASH]*

![Cash payment](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/CashPayment.png "[Cash payment]")

- *Amount*   
  Enter the cash amount given by the customer using the number buttons or typing the amount directly into the field.

- *Number field*   
  Use the number buttons to enter the cash amount given by the customer.
  - ![Delete entry](/Assets/Icons/Trash05.png "[Delete entry]") (Delete entry)   
    Click this button to delete the entered amount.

  - ![Delete last character](/Assets/Icons/Back03.png "[Delete last character]") (Delete last character)   
    Click this button to delete the last number (or character) entered in the field *Amount*.

- ![Back](/Assets/Icons/Back01.png "[Back]") (Back)   
  Click this button to cancel the cash payment and return to the payment view.

- [Pay]   
  Click this button to finalize the cash payment process. The *Payment Pending* view is displayed.   
  The payment can be finalized only if an amount equal or higher than the bill amount is entered in the field *Amount*.
  If an amount smaller than the bill amount or no amount at all is entered, an error message is displayed.


### Payment Pending   

The *Payment Pending* view is displayed when the cash payment has been confirmed. When the cash payment process has been completed, the *Payment Successful* view is automatically displayed.

![Payment Pending](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentPending.png "[Payment Pending]")

- *Total*   
  Total bill amount. This field is read-only.

- *Paid*   
  Amount given by the customer. This field is read-only.

- *Change*   
  Amount of change to be given to the customer. This field is read-only.


### Payment Successful   

The *Payment Successful* view is automatically displayed when the cash payment process has been successfully completed.

![Payment Successful](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentSuccessful.png "[Payment Successful]")

- *Total*   
  Total bill amount. This field is read-only.

- *Paid*   
  Amount given by the customer. This field is read-only.

- *Change*   
  Amount of change to be given to the customer. This field is read-only.

- [Done]   
  Click this button to confirm the completion of the payment process and return to the bill list.


## Cashless Payment
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > [PAY] > [MANUELLES ZAHLEN AM TERMINAL]*

![Cashless payment](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/CashlessPayment.png "[Cashless payment]")  

- *Card type*   
  Click the drop-down list to select the used card type or payment method. By default, the payment methods below are available. Additional cashless payment methods can be defined in the Global Settings, see [Zahlungsweisen (manuelle Zahlung Terminal)](02a_Management.md#zahlungsweisen-manuelle-zahlung-terminal).  
  - **Debit card**
  - **Credit card**
  - **Paypal**    


- [Cancel]
  Click this button to cancel the cashless payment process and return to the payment view.

- [Finalize payment process]
  Click this button to finalize the cashless payment process. The *Payment at terminal* view is displayed.   
  The payment can be finalized only if a payment method is selected in the drop-down list *Card type*.

### Payment at Terminal   

The *Payment at terminal* view is automatically displayed when the cash payment process has been successfully completed.

![Payment at terminal](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PaymentTerminal.png "[Payment at terminal]")

- *Total*   
  Total bill amount. This field is read-only.

- *Paid*   
  Amount given by the customer. This field is read-only.

- *Change*   
  Amount of change to be given to the customer. This field is read-only.

- [Done]   
  Click this button to confirm the completion of the payment process and return to the bill list.



## Add Customer
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > Button Add Customer*

![Add Customer](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/AddCustomer01.png "[Add Customer]")

- ![Cancel](/Assets/Icons/Cross02.png "[Cancel]") (Cancel)   
  Click this button to cancel the operation and close the *Add Customer* view.

- *Find existing customer... ![Search](/Assets/Icons/Search.png "[Search]")*    
  Enter the customer name you search for in the search bar. Click a customer in the list of search results to assign the bill to the customer.

- [ ![Create Customer](/Assets/Icons/Customer01.png "[Create Customer]") Create Customer]   
  Click this button to register a customer. The *Create Customer* view is displayed.


## Create Customer
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > Button Add Customer > Button Create Customer*

![Create Customer](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/AddCustomer02.png "[Create Customer]")

- ![Cancel](/Assets/Icons/Cross02.png "[Cancel]") (Cancel)   
  Click this button to cancel the operation and close the *Add Customer* view.

- *Title*   
  Enter the title of the customer.

- *First name*   
  Enter the first name of the customer.

- *Last name*   
  Enter the last name of the customer.

- *Company*   
  Enter the company name of the customer.

- *Email*   
  Enter the email address of the customer.

- *Street*   
  Enter the street of the customer's address.

- *House Number*   
  Enter the house number of the customer's address.

- *ZIP*   
  Enter the ZIP code of the customer's address.

- *City*   
  Enter the city of the customer's address.

- *Country*   
  Enter the country of the customer's address.


- ![Arrow Back](/Assets/Icons/Back01.png "[Arrow Back]") (Back)   
  Click this button to cancel the registration of the customer and close the current view.

- [ ![Create Customer](/Assets/Icons/Customer01.png "[Create Customer]") Create Customer]   
  Click this button to register the customer and assign the bill to the customer. The *Add Customer* view is closed and the bill list is displayed again.


## Discount on bill
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > [PAY] > [+ DISCOUNT]*

![Discount on bill](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/DiscountBill.png "[Discount on bill]")

- ![Percent](/Assets/Icons/Percent.png "[Percent]") (Percent)   
  Click this button to select percentage as the type of discount. By default, the percentage discount is preselected.

- *Description*   
  Enter a description of the discount.

- *Discount*   
  This field displays the selected amount and type of discount. The field is read-only.

- *(Pay XX.XX €)*   
  This field displays the current amount of the bill less the discount entered. If you enter or edit a discount, the amount is automatically adjusted.

- - *Number field*   
  Use the number buttons to enter the discount.
  - ![Delete entry](/Assets/Icons/Trash05.png "[Delete entry]") (Delete entry)   
    Click this button to delete the entered discount.

  - ![Delete last character](/Assets/Icons/Back03.png "[Delete last character]") (Delete last character)   
    Click this button to delete the last number (or character) of the discount entered.

- ![Back](/Assets/Icons/Back01.png "[Back]") (Back)   
  Click this button to cancel the discount on the bill and return to the payment view.

- [APPLY DISCOUNT]   
  Click this button to apply the entered discount. The payment view with the entered discount is displayed.


## Product Details
*Venduo POS > Sales > Select Store and Pay Desk > Tab CASHPOINT > Select Product in the Bill List*

![Product Details](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ProductDetails.png "[Product Details]")

- *Quantity*
  Quantity of the selected product in the bill list.

- ![Minus](/Assets/Icons/Minus.png "[Minus]") (Minus)  
  Click this button to decrease the quantity in the field *Quantity* by 1. The button is locked, when the quantity equals 1.

- ![Plus](/Assets/Icons/Plus03.png "[Plus]") (Plus)  
  Click this button to increase the quantity in the field *Quantity* by 1.

- *Discount*   
  Discount on the selected product in the bill list.

- *%/Currency*   
  Click this drop-down list and select the type of discount. The following options are available:
  - **%**:  A percentage discount is applied.
  - **EUR** (currency): A fixed price discount in the selected currency is applied.


- *Price*   
  Price of the selected product in the bill list.

-  ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to unlock the price field and edit the price of the selected product.

- ![Back](/Assets/Icons/Back01.png "[Back]") (Back)   
  Click this button to cancel the changes to the product and return to the bill list.

- [Save]   
  Click this button to save the changes to the product and return to the bill list.
