# Manage product and offer data

Before you start exchanging data with *BigCommerce*, you must check your product and offer data.
You must check the images assigned to an offer in the *PIM* or the *Omni-Channel* module. In addition, you can define the color-swatch variant option.


## Check product images

Verify that the desired product data image is in the correct position and that the correct text field is maintained.   

For a good presentation of the offers in your store, it is recommended that the desired images are displayed for each variant. *BigCommerce* supports the import of one thumbnail per variant only. The first image in the corresponding attribute is marked as thumbnail image for the offer. Additionally, the alt text of that image will be added as description.   

The following procedure describes how to check the images in the *PIM* module. If you only have the *Omni-Channel* module in use, you can check the images accordingly via *Offers > Select offer > Edit offer*.


#### Prerequisites

You have assigned more than one image per product variant.

#### Procedure

*PIM > Products > Tab LIST*

![Product images](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMCheckImages.png "[Product images]")

1. Click the product variant you want to check and click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button.   
  The *Edit product* view is displayed. The *Attributes* tab is preselected.

    ![Edit product](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/EditProduct.png "[Edit product]")

2. Click the *Files and images* entry of the *Basic data* attribute group or the customer-specific attribute group in which you have defined the images.   
   The *Files and images* section is displayed. 

   ![Files and images](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMImageAndFiles.png "[Files and images]")

3. Verify that the image at the first position is suitable for your *BigCommerce* store. If not, drag and drop the desired image to the first position.

4. Verify that the *Alt text* field is filled for the image on first position. If you must change the existing entry, you have the following options: 
    - You can change the entry. This may have an impact on other connections you have in use.
    - If you want to keep the product data in this scope unchanged, copy your products to a specific *BigCommerce* sales channel. <!---Stimmt das, sollte man das so tun?-->

5. If applicable, click the [SAVE] button to save your changes.



## Configure color&dash;swatch variant option

Configure the color-swatch variant option for the *BigCommerce* products for which the options provided in the connection settings are not suitable.    
A color-swatch option in *BigCommerce* is an option with which the store customers can select a color combination in the *BigCommerce* storefront. For example, you want to offer T-shirts that are available with the color combinations black/white, white/green, and black/green. *BigCommerce* supports up to three colors per color-swatch value.   
 For detailed information on the standard selection options, see [Configure BigCommerce connection](../Integration/01_ManageBigCommerceConnection.md#configure-bigcommerce-connection).

To add a variant option as a color-swatch, the defining attribute in the variant set needs to be of the *Tree node* data type. If you do not have the *PIM* module in use, you can check or create the attribute in the *DataHub* module.


#### Prerequisites

You are permitted to create attributes.
 
#### Procedure

*PIM > Settings > Tab Attributes*

 ![PIM attributes](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/PIMattribute.png "[PIM attributes]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create attribute* view is displayed.

    ![Create attribute](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/CreateAttribute.png "[Create attribute]")

2. Enter a name for the attribute in the *Name* field and, if desired, add an attribute description in the *Description* field.

3. Select the *Tree node* data type in the *Data type* drop-down list.  
   The ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add) button in the *Assigned sets* field is unlocked. The *CONFIGURATION* section is displayed.    

4. Ensure that the *Multi-language* and *Multi-channel* toggles are disabled.

    > [Info] Be aware that only attributes which are neither multi-language nor multi-channel can be used as defining attributes for variants. For detailed information, see [Create a variant set](../../PIM/Integration/07_ManageVariantSets.md#create-a-variant-set) in the documentation of the *PIM* module.

5. Click the ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add) button in the *Assigned sets* field.      
    A drop-down list with all active attribute sets is displayed.

6. Enable the *Flat* toggle in the *CONFIGURATION* section. Since *BigCommerce* only supports string values, the tree must be flat to be output as a string. For this reason, you cannot use a multi-select tree node.

7. Click the ![Add](../../Assets/Icons/Plus04.png "[Add]") button in the bottom right corner and then the plus sign displayed in the left column of the *Edit tree* section.   
  The *Add element* window is displayed.

   ![Add element](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TreeNodeAddElement.png "[Add element]")

8. Enter the name of the option value to be shown to the *BigCommerce* customer in the *Name* field.

9. Enter the key of the actual value of that option in the *Key* field. This value needs to be a hash key (#) followed by a color hex code, for example #FF00AA. Each additional color added is separated by a comma. The color codes need to be valid hex codes. Enter a maximum of three colors.   
  For example, a feasible option value could look like this:   
  Name: Red, Green & Blue   
  Key: #FF0000,#00FF00,#0000FF

10. Click the [SAVE] button in the bottom right corner of the *Add element* window.

12. Click the [SAVE] button in the upper right corner of the *Create attribute* view.      
  The *Submitting data* notice is displayed. The *Attribute list* view is displayed.