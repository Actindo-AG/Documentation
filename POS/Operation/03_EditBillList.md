[!!Venduo POS](POS)

# Edit the bill list

## Add a discount

You can add a discount to [single products](#add-a-discount-to-a-single-product) or to the [whole purchase](#add-a-discount-to-the-purchase), for instance because of a campaign, defects in the products, for loyal customers or from a certain quantity of products.

### Prerequisites

- Offers for POS are created, see [Manage offers for POS](/POS/Integration/07_ManageOffers.md).
- At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

#### Add a discount to a single product

You can add a customized discount to single products in your bill list.

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the product in the bill list on which you want to apply a discount.   
  The detail view of the product is displayed in the bill list.

  ![Product Detail](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ProductDetails.png "[Product Detail]")

2. Click on the drop-down list to the right of the *Discount* field and select the **%** option if you want to apply a percentage discount or select the **EUR** option to apply a fixed amount discount to the product.   
  The selected option is displayed in the drop-down list.

  > [Info] The currency displayed in the drop-down list corresponds to the default currency in the tab *Global Settings*.

3. Enter a number in the text field to the right of the *Discount* field. The number indicates the amount of the discount, depending on the selection in the drop-down list as a percentage or as a fixed amount.

4. Click the [SAVE] button in the upper right corner to apply the discount.   
  The detail view of the product is closed. The bill list is displayed again. The reduced price of the product is displayed in red, the discount is indicated below the price.

  > [Info] You can apply an individual discount to each product in your bill list. The discount is applied to the product entry in the bill list. That means, if the quantity of a product in the bill list is greater than 1, the discount will apply to all products of this entry. If you want to apply a discount to a single one of several products in an entry, you have to use the [single scan function](02_SelectOffer.md#use-single-scan) first to add the product as a single entry in the bill list.


#### Add a discount to the purchase

Additional or alternative to the single discount, you can add a customized discount to the whole purchase in your bill list.

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the [PAY] button at the bottom of the bill list.   
  The payment view is displayed in the bill list.

  ![Pay](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/Pay.png "[Pay]")

2. Click the [+ DISCOUNT] button above the total.   
  The *Discount on bill* view is displayed.

  ![Discount on bill](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/DiscountBill.png "[Discount on bill]")

3. Enter a description in the *Description* field to specify the discount, for instance campaign, defect.

  > [Info] The discount to the purchase is always a percentage discount.

  [comment]: <> (is that right? Why is there the percentage button but no other selection?)

4. Enter a percentage in the text field to the right of the *Description* field or select a percentage by clicking the number buttons in the lower area.   
  The reduced price of the purchase is displayed below the percentage field.

5. Click the [APPLY DISCOUNT] button in the upper right corner.   
  The bill discount view is closed. The payment view is displayed again. The discount is indicated both as a percentage and as a fixed amount above the reduced total.

  ![Pay Discount](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/PayDiscount.png "[Pay Discount]")

  > [Info] To the right of the indicated discount, on the edge of the bill list, the ![Remove](/Assets/Icons/Cross06.png "[Remove]") (Remove) flag is displayed. Click the flag to delete the discount.

### Next steps

- [Edit the price of a product](#edit-the-price-of-a-product)
- [Edit the quantity of a product](#edit-the-quantity-of-a-product)
- [Delete a product from the bill list](#delete-a-product-from-the-bill-list)
- [Add a Sale Note](#add-a-sale-note)
- [Assign a purchase to a customer](#assign-a-purchase-to-a-customer)
- [Complete a purchase](04_CompletePurchase.md)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)



## Edit the price of a product

You can manually change the price of a product in your bill list, for instance if a price is not correctly in the system.

### Prerequisites

- Offers for POS are created, see [Manage offers for POS](/POS/Integration/07_ManageOffers.md).
- At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the product in the bill list whose quantity you want to change.   
  The detail view of the product is displayed in the bill list.

  ![Product Detail](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ProductDetails.png "[Product Detail]")

2. To the right of the *Price* field, click the ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit) button.   
  The price text field becomes editable. The field name changes to *Price (mod.)*.

  > [Info] If you enter a changed price for a product, you will not be able to apply an additional single discount to that product. The discount field will be locked.

3.  Enter a price in the text field to the right of the *Price (mod.)* field.   

> [Info] If you want to restore the original price, click the ![Reject](/Assets/Icons/Cross03.png "[Reject]") (Reject) button in the *Price (mod.)* field.

4. Click the [Save] button in the bottom right corner to apply the price change.   
  The detail view of the product is closed. The bill list is displayed again. The modified price is displayed in italics to the right of the product.

### Next steps

- [Edit the quantity of a product](#edit-the-quantity-of-a-product)
- [Delete a product from the bill list](#delete-a-product-from-the-bill-list)
- [Add a Sale Note](#add-a-sale-note)
- [Assign a purchase to a customer](#assign-a-purchase-to-a-customer)
- [Complete a purchase](04_CompletePurchase.md)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Add a discount](#add-a-discount)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)



## Edit the quantity of a product

You can change the quantity of a product in your bill list by increasing or decreasing it.

### Prerequisites

- Offers for POS are created, see [Manage offers for POS](/POS/Integration/07_ManageOffers.md).
- At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the product in the bill list whose quantity you want to change.   
  The detail view of the product is displayed in the bill list.

  ![Product Detail](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/ProductDetails.png "[Product Detail]")

2. To the right of the *Quantity* field, click the ![Plus](/Assets/Icons/Plus03.png "[Plus]") (Plus) button to increase the quantity or click the ![Minus](/Assets/Icons/Minus.png "[Minus]") (Minus) button to decrease the quantity of the selected product. Alternatively, you can directly enter a number in the text field to the left of the buttons.

  > [Info] You have to enter a quantity higher than 0. The ![Minus](/Assets/Icons/Minus.png "[Minus]") (Minus) button is only active if the quantity is higher than 1.

3. Click the [SAVE] button in the bottom right corner to apply the quantity change.   
  The detail view of the product is closed. The bill list is displayed again. The selected quantity is displayed to the left of the product.


### Next steps

- [Delete a product from the bill list](#delete-a-product-from-the-bill-list)
- [Add a Sale Note](#add-a-sale-note)
- [Assign a purchase to a customer](#assign-a-purchase-to-a-customer)
- [Complete a purchase](04_CompletePurchase.md)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Add a discount](#add-a-discount)
- [Edit the price of a product](#edit-the-price-of-a-product)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)



## Delete a product from the bill list

You can delete a product from your bill list, for instance if you accidentally added it to the list.

### Prerequisites

- Offers for POS are created, see [Manage offers for POS](/POS/Integration/07_ManageOffers.md).
- At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to the right of the product you want to delete from the bill list.   
  The product entry is deleted from the list.

  > [Info] If you click the ![Delete Product](/Assets/Icons/Cross02.png "[Delete Product]") (Delete Product) button the whole product entry regardless of its quantity is deleted. The deletion cannot be undone.

### Next steps

- [Add a Sale Note](#add-a-sale-note)
- [Assign a purchase to a customer](#assign-a-purchase-to-a-customer)
- [Complete a purchase](04_CompletePurchase.md)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Add a discount](#add-a-discount)
- [Edit the price of a product](#edit-the-price-of-a-product)
- [Edit the quantity of a product](#edit-the-quantity-of-a-product)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)


## Add a Sale Note

You can add a note to the purchase in your bill list to indicate if you have made any changes to the products or want to save any other information about the purchase.

### Prerequisites

- Offers for POS are created, see [Manage offers for POS](/POS/Integration/07_ManageOffers.md).
- At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the *Add Sale Note* field at the bottom part of the bill list.   
  The cursor is displayed in the field.

2. Enter the note you want to add to the bill list.   
  The note is displayed in the text field.

[comment]: <> (Is there any restriction concerning the length of the note? Where is the note displayed after the purchase has been completed?)

### Next steps

- [Assign a purchase to a customer](#assign-a-purchase-to-a-customer)
- [Complete a purchase](04_CompletePurchase.md)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Add a discount](#add-a-discount)
- [Edit the price of a product](#edit-the-price-of-a-product)
- [Edit the quantity of a product](#edit-the-quantity-of-a-product)
- [Delete a product from the bill list](#delete-a-product-from-the-bill-list)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)



## Assign a purchase to a customer

You can assign a customer to a purchase in order to track customer buying behavior or loyalty.   
You can either assign the purchase to an [existing customer](#assign-a-purchase-to-a-customer) or [register a new customer](#register-a-customer) if the customer is not yet registered in the system.

### Prerequisites

- Offers for POS are created, see [Manage offers for POS](/POS/Integration/07_ManageOffers.md).
- At least one product is added to the bill list, see [Select an offer](02_SelectOffer.md).

### Procedure

#### Assign a purchase to an existing customer

Assign the current purchase to an registered customer.

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the ![Add Customer](/Assets/Icons/Customer02.png "[Add Customer]") (Add Customer) button in the upper right corner of the bill list.   
  The search view is displayed in the bill list.

  ![Add Customer](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/AddCustomer01.png "[AddCustomer]")

2. Click the *Find existing customer...* search bar and enter the customer name. You must enter at least three characters in the search bar to start the search. All customers that correspond to your entry are automatically displayed.

  > [Info] The search already provides you with proposals for your entry as you type.

  The customers that match the entered name are displayed in a list below the search bar. If no customer with the entered name is displayed, you have to [register the customer](#register-a-customer) first.

3. Click the appropriate customer name in the list.   
  The search view is closed. The bill list is displayed again. The selected customer name and its address is displayed in the upper left corner of the bill list.

  > [Info] If you want to unassign the customer from the purchase, click the ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete) button to the right of the selected customer in the upper right corner of the bill list.

#### Register a customer

If you want to assign purchase to a customer who does not yet exist in the system, you must first register that customer.

*Venduo POS > Sales > Tab CASHPOINT > Select Store and Pay Desk*

![Cashpoint](/Assets/Screenshots/POS/Sales/Cashpoint/Product.png "[Cashpoint]")

1. Click the ![Add Customer](/Assets/Icons/Customer02.png "[Add Customer]") (Add Customer) button in the upper right corner of the bill list.   
  The search view is displayed in the bill list.

  ![Add Customer](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/AddCustomer01.png "[AddCustomer]")

2. Click the [ ![Create Customer](/Assets/Icons/Customer01.png "[Create Customer]") Create Customer] button.    
  A view to enter the customer data is displayed.

  ![Create Customer](/Assets/Screenshots/POS/Sales/Cashpoint/BillList/AddCustomer02.png "[Create Customer]")

3. Enter the customer data in the corresponding fields and click the [ ![Create Customer](/Assets/Icons/Customer01.png "[Create Customer]") Create Customer] button.   
  The customer is registered. The customer data view is closed. The bill list is displayed again. The created customer name and its address is displayed in the upper left corner of the bill list.

  > [Info] If you want to unassign the customer from the purchase, click the ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete) button in the upper right corner of the bill list.

### Next steps

- [Complete a purchase](04_CompletePurchase.md)
- [Manage the cash register](05_ManageCashRegister.md)
- [Manage the POS order process](06_ManageOrderProcess.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Add a discount](#add-a-discount)
- [Edit the price of a product](#edit-the-price-of-a-product)
- [Edit the quantity of a product](#edit-the-quantity-of-a-product)
- [Delete a product from the bill list](#delete-a-product-from-the-bill-list)
- [Add a Sale Note](#add-a-sale-note)
- [Manage offers for POS](/POS/Integration/07_ManageOffers.md)
