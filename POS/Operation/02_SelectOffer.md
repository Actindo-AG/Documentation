[!!Manage offers for POS](../Integration/07_ManageOffers.md)
[!!User interface Cashpoint](../UserInterface/01a_Cashpoint.md)

# Select an offer

The *Venduo POS* module offers several ways to select an offer or to search for it.
You may select an offer:
- by Quickselect, see [Select by QuickSelect](#select-by-quickselect)
- by name, see [Select by name](#select-by-name)
- by number, see [Select by number](#select-by-number)

The different options are described in the following.

## Select by QuickSelect

The QuickSelect option offers you the possibility to select an offer by clicking a predefined button. This option is often used for popular offers or permanent favorites.

#### Prerequisites

- Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).
- A QuickSelect Category for POS is created, see [Create a QuickSelect Category](../Integration/07_ManageOffers.md#create-a-quickselect-category).

#### Procedure

*Venduo POS > Sales > Select store and pay desk > Tab CASHPOINT*

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Select the desired category by clicking the corresponding tab below the search bar.  
    All offers assigned to the selected category are displayed.

2. Select the desired offer by clicking the corresponding product button.   
    The offer is added to the bill list.



## Select by name

You may select an offer or search for it by entering its name in the search bar. To find an offer, you must enter at least three characters in the search bar. All offers that correspond to your entry are automatically displayed.

#### Prerequisites

Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).

#### Procedure

*Venduo POS > Sales > Select store and pay desk > Tab CASHPOINT*

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Click the *Find offer by nam...* search bar in the upper left part of the tab.  
    The cursor is displayed in the search bar.

2. Enter the name of the offer or the keyword you are searching for in the search bar.
    The offers that match the search are displayed in a list below the search bar.

    > [Info] The search already provides you with proposals for your keyword as you type.


3. Select the desired offer by clicking the corresponding product in the list.   
    The offer is added to the bill list on the right side.

    > [Info] The keyword remains in the search bar when you add a product to the bill list. When you click the search bar with that keyword again, the search results list for this keyword is displayed again.



## Select by number

You may select an offer or search for it by entering its offer number in the search bar. To find an offer, you must enter at least three numbers in the search bar. All offers that correspond to your entry are automatically displayed.

#### Prerequisites

Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).

#### Procedure

*Venduo POS > Sales > Select store and pay desk > Tab CASHPOINT*

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Click the *Find offer by nam...* search bar in the upper left part of the tab.  
    The cursor is displayed in the search bar.

2. Enter the number of the offer you are searching for in the search bar.
    The offers that match the search are displayed in a list below the search bar.

    > [Info] The search already provides you with proposals for your number as you type.


3. Select the desired offer by clicking the corresponding product in the list.   
    The offer is added to the bill list on the right side.

    > [Info] The number remains in the search bar when you add a product to the bill list. When you click the search bar with that number again, the search results list for this number is displayed again.



## Use single scan

If the same offer is selected more than once, it is displayed in the bill list as one product with the corresponding quantity indication. By using the single scan feature, each offer is listed as a single product in the bill list, even if it is the same offer. This allows you to treat each product in the booking individually, for instance to apply an individual discount.

#### Prerequisites

Offers for POS are created, see [Manage offers for POS](../Integration/07_ManageOffers.md).

#### Procedure

*Venduo POS > Sales > Select store and pay desk > Tab CASHPOINT*

![Cashpoint](../../Assets/Screenshots/POS/Sales/Cashpoint/Cashpoint.png "[Cashpoint]")

1. Activate the *Single scan* toggle in the bill list on the right side of the pay desk interface.   

    > [Info] The single scan works from the moment it is toggled on. It does not apply backwards to products that were already on the bill list at the time of activation.   
    Even if the single scan function is active, you can edit the quantity of products manually in the bill list, see [Edit the quantity of a product](./03_EditBillList.md#edit-the-quantity-of-a-product).

2. Select an offer.   
    The product is listed in the bill list.

3. Select the same offer again.   
    The same product is listed in an own entry in the bill list.
