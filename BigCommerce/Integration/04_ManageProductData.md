# Manage product and offer data

Before you start exchanging data with *BigCommerce*, you must check your product and offer data.
You must check the images assigned to a product in *PIM* as well as the changeable attributes assigned to your variant sets in *Omni-Channel*.


## Check product images

Check if the desired product data image is on the right position and the correct text field is maintained.  
It is recommended for a good presentation of the offers in your store that the desired images are displayed for each variant. *BigCommerce* supports the import of one thumbnail per variant only. The first image in the corresponding attribute is marked as thumbnail image for the offer. Additionally, the alt-text of that image will be added as description.   
The following procedure describes how to check the images in the *PIM* module. If you only have the *Omni-Channel* module in use, you can check the image accordingly via *Offers > Select variant set > Edit offer*.


#### Prerequisites

You have assigned more than one image per product variant.

#### Procedure

*PIM > Products > Tab LIST*

![Product images](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMCheckImages.png "[Product images]")

1. Click the product variant you want to check and click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button.   
  The *Edit product* view is displayed. The *Attributes* tab is preselected.

    ![Edit product](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/EditProduct.png "[Edit product]")

2. Click the *Files and Images* entry of the *Basic Data* attribute group, or the customer-specific attribute group in which you have defined the images.   
   The *Files and images* section is displayed. 

   ![Files and images](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMImageAndFiles.png "[Files and images]")

3. Click the image at the first position, if it is suitable for your *BigCommerce* store. Check additionally if the *Alt text* field is filled. If you must change the existing entry, you have the following options: 
    - You can change the entry. This might have impact on other connections you have in use.
    - If and want to keep the product data in this scope unchanged, copy your products to a specific *BigCommerce* scope. <!---Stimmt das, sollte man das so tun?-->

## Check variant sets

Check your existing *Omni-Channel* variant sets if they are suitable for the *BigCommerce* connection or create new ones.   
For detailed information on *BigCommerce* product variants, see the following *BigCommerce* documentation: [https://developer.bigcommerce.com/docs/rest-catalog/product-variants#create-a-product-variant](https://developer.bigcommerce.com/docs/rest-catalog/product-variants#create-a-product-variant).

*BigCommerce* allows only certain attributes to be changeable per variant. The following attributes are declared as changeable in *BigCommerce*:
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

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

Check your existing variant sets or create new ones. For detailed information, see [Manage variants](../../PIM/Operation/02_ManageVariants.md). 



## Configure color-swatch variant option

A color-swatch is simply a palette that displays a variety of shades of the same color. In the physical world, they would be presented as small pieces of fabric with the name and identification number for a specific color on it.   
You can use the color-swatch option for your *BigCommerce* connection, if the options provided in the driver settings are not suitable for you. For detailed information on the standard color options, see 

#### Prerequisites

- To add a variant option as a color-swatch, the defining attribute in the variant set needs to be of the *Tree node* data type.
- If you have the *PIM* module not in use, you can check or create the attribute in the *DataHub* module.

#### Procedure

*PIM > Settings > Tab Attributes*

 ![PIM attributes](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMattribute.png "[PIM attributes]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create attribute* view is displayed.

    ![Create attribute](../../Assets/Screenshots/PIM/Settings/Attributes/CreateAttribute.png "[Create attribute]")

3. Enter a name for the attribute in the *Name* field and, if desired, add an attribute description in the *Description* field.

4. Select the *Tree node* data type in the *Data type* drop-down list.  
   The ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add) button in the *Assigned sets* field is unlocked. Depending on the selected data type, the *CONFIGURATION* section is displayed.    

5. Select the attribute sets you want to assign the attribute.

6. 





- To add a variant option as a color swatch, the defining attribute needs to be a “Single Select Tree”. Each entry in said tree has the following values:
- Name: The name determines the name of the option value shown to the customer. 
- Key: The key determines the actual value of that option. In case of a color swatch“, this value needs to be a ‘#' followed by a Color-Hex-Code (e.g. '#FF00AA’). BigCommerce supports up to three colors per “Color-Swatch” value, so a possible option value could look like this: 

Name

Key

Red, Green & Blue

#FF0000,#00FF00,#0000FF

Each additional color added is separated by a comma. The color codes need to be valid Hex-Codes.
