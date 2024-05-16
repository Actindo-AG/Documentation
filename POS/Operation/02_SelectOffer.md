[!!Manage offers for POS](../Integration/07_ManageOffers.md)
[!!User interface Cashpoint](../UserInterface/01a_Cashpoint.md)

# Record the purchase

The *POS* module offers several ways to select an offer and to search for it. Additionally, you can prepare further actions for editing the bill list &ndash; and to ensure the protection of minors.  



## Use single scan

If the same offer is selected more than once, it is displayed in the bill list as one line item with the corresponding quantity indication.     
Optionally, you can activate the single scan feature before you select the offers. By using it, each offer is listed as a single line item in the bill list, even if it is the same offer. This allows you to treat each offer in the bill list individually, for instance, to apply an individual discount.

#### Prerequisites

Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT*

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Enable the ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]")*Single scan* toggle in the bill list on the right side of the pay desk interface.   

    > [Info] The single scan works from the moment it is enabled. It does not apply backwards to offers that were already on the bill list at the time of activation.

    Even if the single scan function is active, you can edit the quantity of offers manually in the bill list, see [Edit the quantity of a product](./03_EditBillList.md#edit-the-quantity-of-a-product).

2. Select an offer, see [Select an offer](02_SelectOffer.md#select-an-offer).   
    The product is listed in the bill list.

3. Select the same offer again.   
    The same product is listed in an own entry in the bill list.

    ![Product single scan](../../Assets/Screenshots/POS/Sales/Cashpoint/ProductSingleScan.png "[Product single scan]")


## Select an offer

You may select an offer by the following:
- Quickselect, see [Select an offer by QuickSelect](#select-an-offer-by-quickselect).
- Name, see [Select an offer by name](#select-an-offer-by-name).
- Number, see [Select and offer by number](#select-an-offer-by-number).


### Select an offer by QuickSelect

The QuickSelect option offers you the possibility to select an offer by clicking a predefined button. This option is often used for popular offers or permanent favorites.

#### Prerequisites

- Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).
- A QuickSelect Category for POS is created, see [Create a QuickSelect Category](../Integration/07_ManageOffers.md#create-a-quickselect-category).

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT*
![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Select the desired category by clicking the corresponding tab below the search bar.  
    All offers assigned to the selected category are displayed.

2. Select the desired offer by clicking the corresponding button.   
    The offer is added to the bill list if no age rating prevents this, see [Verify the age](#verify-the-age).   
    


### Select an offer by name

You may select an offer or search for it by entering its name in the search bar. To find an offer, you must enter at least three characters in the search bar. All offers that correspond to your entry are automatically displayed.

#### Prerequisites

Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT*

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Click the *Find offer by nam...* search bar in the upper left part of the tab.  
    The cursor is displayed in the search bar.

2. Enter the name of the offer or the keyword you are searching for in the search bar.
    The offers that match the search are displayed in a list below the search bar.

    > [Info] The search already provides you with proposals for your keyword as you type.

3. Select the desired offer by clicking the corresponding product in the list.   
    The offer is added to the bill list on the right side if no age rating prevents this, see [Verify the age](#verify-the-age). 
     
    > [Info] The keyword remains in the search bar when you add a product to the bill list. When you click the search bar with that keyword again, the search results list for this keyword is displayed again.



### Select an offer by number

You may select an offer or search for it by entering its offer number in the search bar. To find an offer, you must enter at least three numbers in the search bar. All offers that correspond to your entry are automatically displayed.
<!---Ist das die Offer ID, SKU  oder was ist das für eine Nummer?-->

#### Prerequisites

Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT* 

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Click the *Find offer by nam...* search bar in the upper left part of the tab.  
    The cursor is displayed in the search bar.

2. Enter the number of the offer you are searching for in the search bar.
    The offers that match the search are displayed in a list below the search bar.

    > [Info] The search already provides you with proposals for your number as you type.


3. Select the desired offer by clicking the corresponding offer in the list.   
    The offer is added to the bill list on the right side if no age rating prevents this, see [Verify the age](#verify-the-age).   
    
    > [Info] The number remains in the search bar when you add an offer to the bill list. When you click the search bar with that number again, the search results list for this number is displayed again.


### Select a pre&dash;printed voucher offer 

Select a voucher offer that allows you to identify and charge a pre-printed voucher. You can then scan the voucher code with a barcode scanner or add the card code manually. 

#### Prerequisites

- Your company uses the KNISTR integration or another integration, with which vouchers can be pre-printed.

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT* 

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Click the *Find offer by nam...* search bar in the upper left part of the tab.  
    The cursor is displayed in the search bar.

2. Enter the name or the SKU of the voucher you are searching for in the search bar.
    The offers that match the search are displayed in a list below the search bar.

    > [Info] The search already provides you with proposals as you type.

3. Select the desired voucher by clicking the corresponding offer in the list.   
    The *Voucher details* window is displayed.

    ![Voucher details](../../Assets/Screenshots/POS/Sales/Cashpoint/VoucherDetails.png "[Voucher details]")

4. Scan the voucher code with the barcode scanner or enter the code manually.     
    If the barcode was successfully scanned or the code manually entered, the voucher code is automatically added to the *Voucher code* field. The cursor is placed in the *Amount* field, where a default value is provided, which you can overwrite.

5. Enter the amount in the *Amount* field. Note that this amount will be added to any amount already on the voucher.

6. Click the [SAVE] button.   
    The entered amount is added to the bill list.


<!--- NEU-->
## Verify the age

Some offers are not suitable for children and young people, for example offers such as alcoholic beverages, cigarettes, or energy drinks. When you select an offer, Actindo checks whether an age verification is necessary before the offer is added to the bill list.

#### Prerequisites

- Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).
- An age restriction for the offer is defined, for example 18 or 16.    
- The *Display age rating* setting is activated. For detailed information, see [Display age rating](../UserInterface/02a_GlobalSettings.md#display-age-rating).

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT* 

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Select an offer.   
    If the offer requires an age verification, the *Age verification* window is displayed.

    ![Age verification](../../Assets/Screenshots/POS/Sales/Cashpoint/AgeVerification.png "[Age verification]")

2. Check the age of the customer. The *Age verification* window provides you with both the minimum age required and the date of birth that the customer must meet or fall below. Eventually, an explanatory text has been added.

    ![Age verification](../../Assets/Screenshots/POS/Sales/Cashpoint/AgeVerification.png "[Age verification]")
    

3. Click the [AGE OF BUYER CONFIRMED] button if the customer is allowed to buy this offer.  
    The offer is added to the bill list.

4. Click the [CANCEL] button if the customer is too young to buy this offer.   
    The offer is not added to the bill list.


## Add a product option

There are products where the buyer has the option of customizing them. If a store has the appropriate technical capabilities, this could be shirts with optional flocking, for example, or photos that a customer can have printed on mugs or other items. In these cases, a specific service is associated to an offer. This service is optional for customers and can be purchased additionally.

#### Prerequisites

- Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).
- Offers relevant to product options have been associated to the offers to which they are related, see [Create a product option](../Integration/07_ManageOffers.md#create-a-product-option).

#### Procedure

*POS > Sales > Select store and pay desk > Tab CASHPOINT* 

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Select an offer.   
    If a product option is associated to the offer and your store offers this service, the *Choose options* window is displayed.

    ![Choose options](../../Assets/Screenshots/POS/Sales/Cashpoint/ChooseOption.png "[Choose options]")

2. Present the various options to the customer.   
    + If the customer does not want to use the service, click the [CANCEL] button.   
    The *Choose options* window is closed.
    + If the customer wants to use the service, continue.  
        Depending on the service option, additional information might be required, for example, if a customer wants to have his/her name printed on a shirt. 

3. If applicable, enter the name or other information that might be required.

4. Click the [SAVE] button.  
    The *Choose options* window is closed. The product option and the additionally edited information are added to the bill list.

    ![Bill list](../../Assets/Screenshots/POS/Sales/Cashpoint/ProductOptionBillList.png "[Bill list]")


