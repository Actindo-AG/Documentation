# Manage product and offer data

Before you start exchanging data with *BigCommerce*, you must check your product and offer data.
You must check the images assigned to a product in *PIM* as well as the changeable attributes assigned to your variant sets in *Omni-Channel*.


## Check product images

Check if the desired product data image is on the right position and the correct text field is maintained.  
IF you have the *PIM* module in use, it is recommended for a good presentation of the offers in your store that the desired images are displayed for each variant. *BigCommerce* supports the import of one thumbnail per variant only. The first image in the corresponding attribute is marked as thumbnail image for the offer. Additionally, the alt-text of that image will be added as description.


#### Prerequisites

You have assigned more than one image per product variant.

#### Procedure

*PIM > Products > Tab LIST*

![Product images](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMCheckImages.png "[Product images]")

1. Click the product variant you want to check and click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button.   
  The *Edit product* view is displayed. The *Attributes* tab is preselected.

    ![Edit product](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/EditProduct.png "[Edit product]")

2. Click the *Files and Images* entry of the *Basic Data* attribute group, or the customer-specific attribute group in which you have defined the images.   
   The *Files and images* section is displayed. The image attributes are displayed on the right.

   ![Files and images](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMImageAndFiles.png "[Files and images]")

3. Check the image at the first position and if the *Alt text* field is filled. If you must change the existing entry, you have the following options: 
    - You can change the entry. This might have impact on other connections you have in use.
    - If and want to keep the product data in this scope unchanged, copy your products to a specific *BigCommerce* scope. <!---Stimmt das, sollte man das so tun?-->

## Check variant sets


For detailed information on *BigCommerce* product variants, refer to the following *BigCommerce* documentation: [https://developer.bigcommerce.com/docs/rest-catalog/product-variants#create-a-product-variant](https://developer.bigcommerce.com/docs/rest-catalog/product-variants#create-a-product-variant).

The following attributes are declared as changeable in *BigCommerce*:
- Cost price   
- Price   
- Sale price   
- Retail price  
- Weight   
- Width   
- Height   
- Depth   
- Is free shipping   
- Fixed cost shipping price   
- UPC   
- Inventory level   
- Inventory warning level   
- BIN   
- GTIN   
- MPN   
- Image URL (only one thumbnail per variant)   
- SKU   
