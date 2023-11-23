# BigCommerce particularities

There are several particularities regarding the *BigCommerce* product data that must be taking into account when establishing and using the *BigCommerce* connection. These particularities are described in detail below.
For detailed information on product data, refer to the *BigCommerce* documentation.


## Offer handling

You have two options for exchanging offer data between *Actindo* and *BigCommerce*:
- If you start with *BigCommerce* and have created already all offers in *Actindo*, you can export your offers to your *BigCommerce* storefront.
- If you start with *Actindo* after you have started with *BigCommerce*, you can import the offers created in *BigCommerce* to *Actindo*.   
  Note, if you choose this way, you will not be able to import offer changes again from *BigCommerce* to *Actindo*. In this case, you must change the offers on the *Actindo* side and export them to *BigCommerce*.  
  For this reason, it is recommended to hold offer data at *Actindo*.



## Export of offers (Actindo > BigCommerce)

### Variant options

*BigCommerce* supports multiple types for the selection of variant options on the UI.  For detailed information, see [Configure the BigCommerce connection](../Integration/01_ManageBigCommerceConnection.md#configure-the-bigcommerce-connection).  


### Custom fields

*BigCommerce* supports simple string values only. For this reason, only the following *Actindo* data types are supported as possible custom field values for attributes:

- Text field
- String
- Float 
- Integer
- Date time

All data types that are no string values are converted to string. 
The length of a custom field string is limited to 255 characters. 

### Images

The first image in the corresponding attribute is marked as thumbnail image for the offer. The alt-text of an image will be added as description for that image. Every other field is not supported.
For detailed information, see [Check product images](../Integration/04_ManageProductData#check-product-images).  
 

### Videos
Product videos are not supported by the driver. If you have a strong need to have videos available, ask your *Actindo* contact person for support.


### Related Offers

You can select related offers in the corresponding attribute. Offers can only be selected as related, if they exist as channels offers. These offers are shown in *BigCommerce* as related if they are uploaded and available in the shop.

### Variants

#### Variant options

Since *BigCommerce* allows multiple types for variant options, the driver needs a way to determine the intended type for a variant option. You can handle types such as dropdowns, radio buttons, or rectangles by the connection settings. For detailed information on these types, see [Configure BigCommerce connection](../Integration/02_ManageBigCommerceConnection.md#configure-bigcommerce-connection).

Alternatively, the “color-swatch type” is available which must be configured in a specific way. For detailed information, see [Configure color-swatch variant option](../Integration/04_ManageProductData.md#add-color-swatch-variant-option).

### Omni-Channel attributes to BigCommerce attributes

In variant sets, the *Omni-channel* module allows to select any attribute as changeable, but *BigCommerce* allows only certain attributes to be changeable per variant.  
Note that only attributes that are changeable in *BigCommerce* are changed on creation or update of a variant. Others are skipped. For detailed information, see [Check variant sets](../Integration/04_ManageProductData.md#check-variant-sets).

### Multi-dimensional variants
Multi-dimensional variants are variant sets that contain more than one variant option as defining attribute, for example size and color for clothes.   

The *BigCommerce* API allows creating variants by using variant options (defining attributes) and values (changeable attributes). However, during creating an offer, the API makes it possible to create more variants than would be possible with the options and values created by *Actindo*. In this case, customers can select and order products in the *BigCommerce* shopfront that does not exist.   

**Example**   
An offer is created by using the two defining attributes size and color. By using these attributes two variants are created t-shirt-s-red (S, red) and t-shirt-m-green (M, green). The driver creates the following options and values:
- Size (S, M),
- Color (Green, Red)  

While the Actindo *BigCommerce driver* creates the variants "t-shirt-s-red" and "t-shirt-m-green" only, the *BigCommerce* shopfront displays all possible combinations of options and values. This includes products such as t-shirt-s-green (S, green), which do not exist. The issue is that these product variants are not only displayed to the customers, but that they are also able to order these non-existent products!  

Note that you must manage this issue by the shopfront itself.
You can access via /v3/catalog/products/{productId}/variants all variations the driver has created and only the ones the driver created.

## Import of offers (BigCommerce > Actindo)


### Shared variant options

*BigCommerce* has shared variant options that cannot be modified in any way using the API: 
- The driver can import offers with shared variant options, but you are not able to edit them after the import.   
- In addition, the driver cannot manage any changes after the import in the *BigCommerce* UI. Changing shared variant options after an import will cause *Omni-Channel* offer updates to fail.   

Before the first import of offers, check your variant options in *BigCommerce*. It is strongly recommended not to use shared variant options. 



## Import of orders (BigCommerce > Actindo)

The import of offers is supported by the *BigCommerce* driver.
- Offers are imported into the system in a configurable order status. That means, that you can.... 
- The *BigCommerce* connection enables parallel imports to handle larger loads.

The following data are managed by the driver:
- Contained products
- Billing address
- Shipping address       
   > [Info] Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only.   
   For detailed information, see [Manage multiple shipping addresses](../Integration/02_ManageBigCommerceSettings#manage-multiple-shipping-addresses).
- Channels    
  All channels that you connect via *BigCommerce* are handled as sub sales channels. This architecture enables you to run multiple stores in *BigCommerce*.

Data that is not included in the above list is not included in the order import. For example, you may be interested in the following data, which is not part of the order import: 
- Gift wraps
- Multiple shipping addresses   
- Customer IDs   
   *Actindo* does not use the customer IDs of *BigCommerce* to avoid inconsistencies with already existing customer IDs. Instead, *Actindo* automatically creates a new customer, if the import data does not match an existing *Actindo* customer.  

If you have a strong need to have this data available, ask your *Actindo* contact person for support.


#### Multiple Shipping Addresses

Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only.  Any orders that use multiple shipping addresses cannot be imported and will fail during the import.  
For detailed information, see [Manage multiple shipping addresses](../Integration/02_ManageBigCommerceSettings#manage-multiple-shipping-addresses).

#### Discounts

*BigCommerce* supports one single discount coupon per order only.

> [INFO] *BigCommerce* processes discounts before taxes. To manage this case, the driver splits discounts on each line item, add them, and calculates a net discount value using the line items tax rate. Because of that even “discount in percent” discounts will be shown as absolute values on each line item. 

Used discount coupons (name and code) are displayed in Onmi-Channel as custom attributes on each line item. 



## Order status updates

#### Order Delivery Statuses

The driver supports updates on the order statuses, but *BigCommerce* can only manage a few *Omni-Channel* statuses. The order statuses are assigned as follows:

| Status in Omni-Channel | Status in BigCommerce   
   |-----|-------   
   |Partially shipped|Partially shipped
   |Ready for shipping|Awaiting shipment
   |Shipped| Shipped   
  

#### Order payment statuses
This feature is not supported, as *BigCommerce* does not allow an update of a payment status.



## Shipments

Note that *BigCommerce* allows only specific values to for tracking the carrier of a shipment. You can only use one of these values, otherwise the export of the shipment will fail!   
For detailed information on the supported carriers, see the *BigCommerce* documentation in *GitHub* under https://github.com/bigcommerce/dev-docs/blob/main/assets/csv/tracking_carrier_values.csv.



#### Import of offers



- During importing orders to *Omni-Channel*, the orders are filtered by order status and the last modification date/time. <!--- All orders that are matched but not yet imported will be put into a message queue and parallel jobs will import the orders into Omni-Channel-->

- The offer import contains the following information:

    - Contained products
    - Billing address
    - Shipping address       
       > [Info] Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only.   
       For detailed information, see [Manage multiple shipping addresses](../Integration/02_ManageBigCommerceSettings#manage-multiple-shipping-addresses).
    - Channels. All channels that you connect via *BigCommerce* are handled as sub sales channels. This architecture enables you to run multiple stores in *BigCommerce*.





##### Exporting product data 

The export of the following product data is not supported: 
- Upload of videos
- Bulk prices  
- Product variants can only be mapped using a TreeNodeValue

If you have a strong need to have this data available, ask your *Actindo* contact person for support.


Images are handled as follows:
- Import from *BigCommerce* to *Actindo*
   - Per variant, you can import one image only
- Export from *Actindo* to *BigCommerce*
   - Even if you have defined several images per variant, the first image is automatically marked as thumbnail
   - Alt-text is used as description
   - Other image specific fields are not supported

#### Product variant:
Channels Attributes to BigCommerce Attributes:

*BigCommerce* only allows certain attributes to be changeable per variation. *Omni-Channel* allows you to select any attribute as changeable. 
Only attributes that are changeable in *Bigcommerce* are changed on creation or update of a variation. Others are skipped.   
For detailed information on product variants, see [Check product variants](../Integration/04_ManageProductData.md#check-variant-sets)




For detailed information on BigCommerce product variants, refer to the following *BigCommerce* documentation: [https://developer.bigcommerce.com/docs/rest-catalog/product-variants#create-a-product-variant](https://developer.bigcommerce.com/docs/rest-catalog/product-variants#create-a-product-variant).



#### Variation Thumbnails

If a variation should display a thumbnail in BigCommerce, the Images Attribute in Channels should be declared as changeable and the variation should include different images than the master offer. 
If these conditions are given, the first image in the image attribute of the variation is uploaded as the thumbnail. If the variation holds the same images as the master offer or no images at all, no thumbnail will be uploaded.

#### Shipments
Note that *BigCommerce* only allows specific values for tracking the carrier of a shipment. You can only use one of these values, otherwise the export of the shipment will fail! 

Ref. https://github.com/bigcommerce/dev-docs/blob/main/assets/csv/tracking_carrier_values.csv 

