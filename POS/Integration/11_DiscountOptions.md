# Discount options

This section provides you with an overview on the various discount options that are available for the *POS* module.

> [Info] A combination of several discount options is not allowed. For example, you cannot give a discount on a single offer and a discount on the purchase. If a customer has a customer-specific discount that is automatically added to the pay bill list, manually applied discounts are not allowed.


## Automatic discount

Discount that is automatically applied if the total of the bill exceeds a certain amount.  

For detailed information, see [Automatic discount](../UserInterface/02a_GlobalSettings.md#automatic-discount).



## Manually granted discount

Discount that the cashier grants when editing the bill list or completing the purchase.

For detailed information, see the following:
- [Add a discount to the purchase](../Operation/04_CompletePurchase.md#add-a-discount-to-the-purchase)
- [Add a discount to a single offer](../Operation/03_EditBillList.md#add-a-discount-to-a-single-offer)



## Customer-specific discount

Customer-specific discount that is automatically added to the pay bill list when a customer, for whom a discount is defined in the customer's master data, purchases an offer.   

For detailed information, see the following:
- Configuration: [Customer-specific discount](../UserInterface/02a_GlobalSettings.md#customer-specific-discount)
- Use: [Check the customer-specific discount](../Operation/04_CompletePurchase.md#check-the-customer-specific-discount)

<!---Error-->


## Discount based on price group

Discount that is automatically added to the pay bill list when a customer who has been assigned a price group in the customer's master data purchases an offer in which a price group price is stored.

For detailed information, see the following:
- Configuration:   
    - [Create a price group for POS](../Integration/07_ManageOffers.md#create-a-price-group-for-pos)
    - [Active price groups](../UserInterface/02a_GlobalSettings.md#active-price-groups)
    - [Field for price group](../UserInterface/02a_GlobalSettings.md#field-for-price-group)

- Use: [Assign a price group](../Operation/04_CompletePurchase.md#assign-a-price-group)


## Discount based on promotion prices 

Discount that is automatically added to the bill list when the cashier has selected an offer, for which a promotion price has been assigned.  

For detailed information, see the following:

- Configuration: [Define promotions for POS](../Integration/07_ManageOffers.md#define-promotions-for-pos)


