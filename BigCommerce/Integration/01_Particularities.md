# BigCommerce particularities

There are several particularities regarding the *BigCommerce* product data that must be taking into account when establishing and using the *BigCommerce* connection. These particularities are described in detail below.
For detailed information on product data, refer to the *BigCommerce* documentation.


## Offer handling

You have two options for exchanging offer data between *Actindo* and *BigCommerce*:
- If you start with *BigCommerce* and have created already all offers in *Actindo*, you can export your offers to your *BigCommerce* storefront.
- If you start with *Actindo* after you have started with *BigCommerce*, you can import the offers created in *BigCommerce* to *Actindo*.   
  Note, if you choose this way, you will not be able to import offer changes again from *BigCommerce* to *Actindo*. In this case, you must change the offers on the *Actindo* side and export them to *BigCommerce*.  
  For this reason, it is recommended to hold offer data at *Actindo*.



## Export of offers

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

Color Swatch Variant Option (Defining Attribute):

Since *BigCommerce* allows multiple types for variant options, the driver needs a way to determine the intended type for a variant option. You can handle types like dropdowns, radio buttons, or rectangles by the connection settings. For detailed information on these types, see [Check product images](../Integration/02_ManageBigCommerceConnection.md#configure-the-bigcommerce-connection).

Additionally, the “color-swatch type” is available and determined in a specific way.  A color swatch is simply a palette showing a variety of shades of the same color. In the physical world, they would be presented as small pieces of fabric with the name and identification number for a specific color on it.

- To add a variant option as a color swatch, the defining attribute needs to be a “Single Select Tree”. Each entry in said tree has the following values:
- Name: The name determines the name of the option value shown to the customer. 
- Key: The key determines the actual value of that option. In case of a color swatch“, this value needs to be a ‘#' followed by a Color-Hex-Code (e.g. '#FF00AA’). BigCommerce supports up to three colors per “Color-Swatch” value, so a possible option value could look like this: 

Name

Key

Red, Green & Blue

#FF0000,#00FF00,#0000FF

Each additional color added is separated by a comma. The color codes need to be valid Hex-Codes.



## Import of orders

The import of offers has the following particularities:
- Offers are imported into the system in a configurable order status. That means, that you can.... 
- The *BigCommerce* connection enables parallel imports to handle larger loads.

## Order status updates


## Shipments





#### Import of offers



- During importing orders to *Omni-Channel*, the orders are filtered by order status and the last modification date/time. <!--- All orders that are matched but not yet imported will be put into a message queue and parallel jobs will import the orders into Omni-Channel-->

- The offer import contains the following information:

    - Contained products
    - Billing address
    - Shipping address       
       > [Info] Note: Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only.   
       For detailed information, see [Manage multiple shipping addresses](../Integration/02_ManageBigCommerceSettings#manage-multiple-shipping-addresses).
    - Channels. All channels that you connect via *BigCommerce* are handled as sub sales channels. This architecture enables you to run multiple stores in *BigCommerce*.

Information that is not in the list above, is not contained in the order import. For example, the following ones that are not part of the order import, might be interesting for you:  
- Gift wraps
- Multiple shipping addresses   
   > [Info] Note: Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only.   
    For detailed information, see 
- Customer IDs. *Actindo* does not use the customer IDs of *BigCommerce* to avoid inconsistencies with already existing customer IDs. Instead, *Actindo* automatically creates a new customer, if the import data does not match an existing *Actindo* customer. 


#### Importing product data

 
You have two options for handling the product data:
- You export the product data created in *Actindo* to your *BigCommerce* storefront.
- You import the product data created in *BigCommerce* to *Actindo*. Note, if you choose this way, you will not be able to import product changes again from *BigCommerce* to *Actindo*. In this case, you must change product data on the *Actindo* side and export them to *BigCommerce*.  
  For this reason, it is recommended to hold product data on Actindo.


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

#### Multidimensional Variations

The BigCommerce API allows to create variations using variation options and values. While creating an offer with more than one defining attribute, it is possible to create less variations than are actually possible with the options and values you created. If that happens, you are able to select and order products in the BigCommerce Shopfront which are non existent. 
E.g:
You create a product with two defining attributes (size and color). You create two variations for this product. The variations you created are V1(S, Red) and V2(M, Green). Following options and values are created by the driver:
Size(S, M),
Color(Green, Red)
 While the driver only creates these variants, the shopfront will display all possible combinations of options and values. Including products like V(S, Green). Not only are these product variations displayed, but you are also able to order these non existent products.
!This issue needs to be handled by the shopfront it self!
Via /v3/catalog/products/{productId}/variations you can access all variations the driver created and only the ones the driver created!

#### Variation Thumbnails

If a variation should display a thumbnail in BigCommerce, the Images Attribute in Channels should be declared as changeable and the variation should include different images than the master offer. 
If these conditions are given, the first image in the image attribute of the variation is uploaded as the thumbnail. If the variation holds the same images as the master offer or no images at all, no thumbnail will be uploaded.

#### Shipments
Note that *BigCommerce* only allows specific values for tracking the carrier of a shipment. You can only use one of these values, otherwise the export of the shipment will fail! 

Ref. https://github.com/bigcommerce/dev-docs/blob/main/assets/csv/tracking_carrier_values.csv 

