# BigCommerce particularities

There are several particularities regarding the *BigCommerce* product data that must be taking into account when establishing and using the *BigCommerce* connection. These particularities are described in detail below.

## Import of orders

The import of orders has the following particularities:
- All channels that you connect via *BigCommerce* are handled as sub sales channels.   
- Orders are imported into the system in a configurable order status. That means, that you can.... 
- The *BigCommerce* connection enables parallel imports to handle larger loads.

- During importing orders to *Omni-Channel*, the orders are filtered by order status and the last modification date/time. <!... All orders that are matched but not yet imported will be put into a message queue and parallel jobs will import the orders into Omni-Channel ...>

- The order import contains the following information:

    - Contained products
    - Billing address
    - Shipping address       
       > [Info] Note: Although *BigCommerce* allows multiple shipping addresses, *Actindo* supports the import of one shipping address only.
    - Channels. All channels that you connect via *BigCommerce* are handled as sub sales channels. 

Information that is not in the list above, is not contained in the order import. For example, the following ones that are not part of the order import, might be interesting for you:  
- Gift wraps
- Multiple shipping addresses
- Customer IDs. *Actindo* does not use the customer IDs of *BigCommerce* to avoid inconsistencies with already existing customer IDs. Instead, *Actindo* automatically creates a new customer, if the import data does not match an existing *Actindo* customer. 

## Order Export
coming soon

## Importing product data

You have two options for handling the product data:
- You export the product data created in *Actindo* to your *BigCommerce* storefront.
- You import the product data created in *BigCommerce* to *Actindo*. Note, if you choose this way, you will not be able to import product changes again from *BigCommerce* to *Actindo*. In this case, you must change product data on the *Actindo* side and export them to *BigCommerce*.


## Exporting product data 

The export of the following product data is not supported: 
- Upload of videos
- Bulk prices  
- Product variants can only be mapped using a TreeNodeValue

If you have a strong need to have this data available, ask your *Actindo* contact person for support.


Images are handled as follows:
- The first image is automatically marked as thumbnail
- Alt-text is used as description
- Other image specific fields are not supported

## Variations:
Channels Attributes to BigCommerce Attributes:

BigCommerce only allows certain attributes to be changeable per variation. Channels allows you to select any attribute as changeable. 
Only attributes that are changeable in bigcommerce are changed on creation or update of a variation. Others are skipped.
 Product Variants | BigCommerce Dev Center 

## Multidimensional Variations

The BigCommerce API allows to create variations using variation options and values. While creating an offer with more than one defining attribute, it is possible to create less variations than are actually possible with the options and values you created. If that happens, you are able to select and order products in the BigCommerce Shopfront which are non existent. 
E.g:
You create a product with two defining attributes (size and color). You create two variations for this product. The variations you created are V1(S, Red) and V2(M, Green). Following options and values are created by the driver:
Size(S, M),
Color(Green, Red)
 While the driver only creates these variants, the shopfront will display all possible combinations of options and values. Including products like V(S, Green). Not only are these product variations displayed, but you are also able to order these non existent products.
!This issue needs to be handled by the shopfront it self!
Via /v3/catalog/products/{productId}/variations you can access all variations the driver created and only the ones the driver created!

## Variation Thumbnails

If a variation should display a thumbnail in BigCommerce, the Images Attribute in Channels should be declared as changeable and the variation should include different images than the master offer. 
If these conditions are given, the first image in the Image Attribute of the variation is uploaded as the thumbnail. If the variation holds the same images as the master offer or no images at all, no thumbnail will be uploaded.

## Shipments
Note that *BigCommerce* only allows specific values for tracking the carrier of a shipment. You can only use one of these values, otherwise the export of the shipment will fail! 

Ref. https://github.com/bigcommerce/dev-docs/blob/main/assets/csv/tracking_carrier_values.csv 