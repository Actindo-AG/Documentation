# Data type list

To [create an attribute](/PIM/Integration/01_ManageAttributes.md#create-an-attribute), you have to define a data type.   
In the *DataHub* module, a few more data types are available than in the *PIM* module. The data types that are available in both, the *DataHub* and the *PIM* module are described in the *PIM* module, see [Data type List PIM](/PIM/UserInterface/04_DataTypeList.md). In the following, all additional data types in the *DataHub* module, their use and their configuration are described in detail.

[comment]: <> (Zusammenhang Datentyp und assigned Sets?)


## Offer variants

The data type *Offer variant* is used to  

[comment]: <> (Unterschied zu product variants attribut in PIM?)

### Configuration

This data type has no further configuration settings.



## Feed-Angebotsvarianten

The data type *Feed-Angebotsvarianten* is used to

[comment]: <> (Warum kann ich kein Attributset zuordnen?)

### Configuration

This data type has no further configuration settings.



## Multiple errors

The data type *Multiple Errors* is used to

[comment]: <> (internal?)

### Configuration

This data type has no further configuration settings.



--------
[comment]: <> (ab hier PIM data types)

## Textfield

![Textfield](/Assets/Screenshots/PIM/DataTypes/Textfield.png "[Textfield]")

The data type *Textfield* is used for long texts, for example for descriptions. You can configure the text length an the editor you use.
In the *PIM Basic Set*, the following attributes have the data type *Textfield*:
- Product short description
- Product description
- Long text

### Configuration

![Textfield](/Assets/Screenshots/PIM/DataTypes/Configuration/Textfield.png "[Textfield]")

- *Min length*   
  Enter a minimal length of the textfield.

- *Max length*   
  Enter a maximal length of the textfield.

- *Rows*   
  Enter the number of rows in the textfield. By default the number of rows is set to **5**.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *HTML Editor*   
  Enable this toggle to enable the HTML editor for the textfield. A WYSIWIG-editor is displayed to edit the textfield. Disable the toggle to disable the HTML editor for the textfield. By default, this toggle is disabled.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Enable this toggle to set the textfield read-only. Disable the toggle to set the textfield editable. By default, this toggle is disabled.


## Checkbox

![Checkbox](/Assets/Screenshots/PIM/DataTypes/Checkbox.png "[Checkbox]")

The data type *Checkbox* is used to indicate a statement that is either true or false, for example if a product is a digital or real product. The checkbox is displayed by a toggle. In the *PIM Basic Set*, the following attributes have the data type *Checkbox*:
- Sale item
- 18+
- Digital item

> [Info] Note that the date type *Checkbox* also has the third value **not set**. When creating or importing a product, the value **not set** is set for the corresponding attribute. After saving, the value switches automatically to **false** if it was not manually changed to **true**. This may cause problems when connecting to other systems, for example shops or marketplaces, with different default settings for checkboxes.   

### Configuration

This data type has no further configuration settings.


## Floating point number

![Floating point number](/Assets/Screenshots/PIM/DataTypes/FloatingPointNumber.png "[Floating point number]")

The data type *Floating point number* is used to indicate decimal numbers without a unit. You can configure the number of decimal places and the number range.

### Configuration

![Floating point number](/Assets/Screenshots/PIM/DataTypes/Configuration/FloatingPointNumber.png "[Floating point number]")

- *Precision*   
  Enter the number of decimal places for the floating point number. By default the number of decimals is set to **4**.  

  > [Info] Note that when you enter more than the defined number of decimal places for the attribute value, the number is commercially rounded to the defined number of decimal places after saving.

- *Min value*   
  Enter a minimum value for the floating point number.  

- *Max value*   
  Enter a maximum value for the floating point number.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Enable this toggle to set the floating point number read-only. Disable the toggle to set the floating point number editable. By default, this toggle is disabled.


## Integer

![Integer](/Assets/Screenshots/PIM/DataTypes/Integer.png "[Integer]")

The data type *Integer* is used to indicate whole numbers without a unit. You can configure the number range.

### Configuration

![Integer](/Assets/Screenshots/PIM/DataTypes/Configuration/Integer.png "[Integer]")

- *Min value*   
  Enter a minimum value for the integer.  

- *Max value*   
  Enter a maximum value for the integer.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Enable this toggle to set the integer read-only. Disable the toggle to set the integer editable. By default, this toggle is disabled.


## String

![String](/Assets/Screenshots/PIM/DataTypes/String.png "[String]")

The data type *String* is used for short texts or alphanumeric information, for example keywords. You can configure the string length and define regular expressions for the string. In the *PIM Basic Set*, the following attributes have the data type *String*:
- Product name
- EAN-code
- Customs tariff number
- Supplier link
- Additional terms for search
- Tags/Keywords
- Meta title
- Meta description
- Meta keywords

### Configuration

![String](/Assets/Screenshots/PIM/DataTypes/Configuration/String.png "[String]")

- *Min length*   
  Enter a minimal length of the string.

- *Max length*   
  Enter a maximal length of the string.

- *Regex*   
  Enter a regular expression for the string. For detailed information about regular expressions, see https://regex101.com/.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Enable this toggle to set the string read-only. Disable the toggle to set the string editable. By default, this toggle is disabled.


## Currency

![Currency](/Assets/Screenshots/PIM/DataTypes/Currency.png "[Currency]")

The data type *Currency* is used to indicate a currency. A drop-down list with all currencies in the system is displayed in the product view.

### Configuration

This data type has no further configuration settings.


## Language

![Language](/Assets/Screenshots/PIM/DataTypes/Language.png "[Language]")

The data type *Language* is used to indicate a language. A drop-down list with all languages in the system is displayed in the product view.

### Configuration

This data type has no further configuration settings.


## Country

![Country](/Assets/Screenshots/PIM/DataTypes/Country.png "[Country]")

The data type *Country* is used to indicate a country. A drop-down list with all countries in the system is displayed in the product view. In the *PIM Basic Set*, the following attributes have the data type *Country*:
- Country of origin

### Configuration

This data type has no further configuration settings.


## TreeNode

The data type *TreeNode* is used for indications with multiple, predefined selection options. You have to define the different selection options in the configuration. Additionally you can configure whether the selection of values will be a multiple or single selection.

[comment]: <> (to be edited)

![TreeNode](/Assets/Screenshots/PIM/DataTypes/TreeNode.png "[TreeNode]")

### Configuration

![TreeNode](/Assets/Screenshots/PIM/DataTypes/Configuration/TreeNode.png "[TreeNode]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi Select*   
  Enable this toggle to enable a multiple selection of values. Disable the toggle to allow only a single selection of values. By default, this toggle is disabled.

> [Info] In the product view, the data type *TreeNode* is displayed either by a drop-down list or a a box with all created options. The drop-down list is only displayed for one dimensional single select trees.

**Edit tree**

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click first this button and then the plus sign displayed in the left column of the *Edit tree* table to add an attribute value. The *Add Element* window is displayed.

### Add Element

![Add element](/Assets/Screenshots/PIM/DataTypes/Configuration/AddElement.png "[Add element]")

- *Name*   
  Enter the attribute value name.

- *Key*   
  Enter the attribute value key.

- [CANCEL]   
  Click this button to cancel adding a value.

- [SAVE]   
  Click this button to save the value and add it to the table.


## Completeness (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.   
In the *PIM Basic Set*, the following attributes have the data type *Completeness*:
- Completeness



## Number with Unit

![Number with Unit](/Assets/Screenshots/PIM/DataTypes/NumberUnit.png "[Number with Unit]")

The data type *Number with Unit* is used for numerical specifications of a certain unit of measurement, for example weight specifications. You can configure the applicable dimension and unit of measurement. Depending on the selected dimension, the options for the unit are adapted. In the *PIM Basic Set*, the following attributes have the data type *Number with Unit*:
- Length
- Width
- Depth
- Weight

### Configuration

![Number with Unit](/Assets/Screenshots/PIM/DataTypes/Configuration/NumberUnit.png "[Number with Unit]")

- *Dimension*   
  Click the drop-down list to select the dimension to be used. All active dimensions are displayed in the drop-down list.

- *Default unit*   
  Click the drop-down list to select the dimension to be used. All units that are assigned to the selected dimension are displayed in the drop-down list.


## DateTime

![DateTime](/Assets/Screenshots/PIM/DataTypes/DateTime.png "[DateTime]")

The data type *DateTime* is used to indicate a date and/or a time. You can configure whether to display or not the date and the time and you can select a date and time format. A calendar widget to select the date is displayed in the product view. In the *PIM Basic Set*, the following attributes have the data type *DateTime*:
- Expiration date

### Configuration

![DateTime](/Assets/Screenshots/PIM/DataTypes/Configuration/DateTime.png "[DateTime]")

- *Date*
  Click the drop-down list to select a date format. The formats below are available. By default, the date format **Short** is selected.
  - **Do not show date**: hidden date
  - **Short**: short format, for example 02/11/2021
  - **Medium**: medium format, writing out the month, for example February 11, 2021
  - **Long**: long format, adding the weekday and writing out the month, for example Monday, February 11, 2021


- *Time*    
  Click the drop-down list to select a time format. The formats below are available. By default, the time format **Medium** is selected.
  - **Do not show time**: hidden time
  - **Short**: short format, for example 09:00 PM
  - **Medium**: medium format, including seconds, for example 09:00:00 PM


## Sales Unit Value

![Sales Unit Value](/Assets/Screenshots/PIM/DataTypes/SalesUnitValue.png "[Sales Unit Value]")

The data type *Sales Unit Value* is used to define a dimension and a unit. Two drop-down lists to select the applicable dimension and unit are displayed in the product view. Depending on the selected dimension, the options for the unit are adapted. In the *PIM Basic Set*, the following attributes have the data type *Sales Unit Value*:
- Sale unit

### Configuration

This data type has no further configuration settings.


## Simple price field

![Simple price field](/Assets/Screenshots/PIM/DataTypes/SimplePriceField.png "[Simple price field]")

The data type *Simple price field* is used to indicate a price. You can configure the use of gross or net price, the display of an MSRP field and promotion prices and the currency to be used. Additionally, you can create scale prices in the product view. Unlike the data type *Preise*, the data type *Simple price field* requires less information to indicate the price.

### Configuration

![Simple price field](/Assets/Screenshots/PIM/DataTypes/Configuration/SimplePriceField.png "[Simple price field]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Gross prices*   
  Enable this toggle to display gross prices. Disable the toggle to display net prices. By default, this toggle is enabled.

  > [Info] Note that it is especially for the ETL-mapping very important if prices are net or gross.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Show MSRP field*   
  Enable this toggle to display the MSRP field. Disable the toggle to hide the MSRP field. By default, this toggle is disabled.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use Promotions*    
  Enable this toggle to enable to enter a promotion period for prices. Disable the toggle to not allow promotion prices. By default, this toggle is disabled.

- *Currency*   
  Click the drop-down list to select the currency to be used. All available currencies are displayed in the drop-down list. By default, the default currency is preselected.

[comment]: <> (Not working -> MSRP field is displayed even when the toggle is disabled -> to be fixed)


## Stock Value

![Stock Value](/Assets/Screenshots/PIM/DataTypes/StockValue.png "[Stock Value]")

The data type *Stock Value* is used to indicate the number of stocks. You can configure the number of decimal places. A new target channel for this stock is created in the *Stock* module for the inventory assignment. In the *PIM Basic Set*, the following attributes have the data type *Stock Value*:
- Stock  

### Configuration

![Stock Value](/Assets/Screenshots/PIM/DataTypes/Configuration/StockValue.png "[Stock Value]")

- *Precision*
  Enter the number of decimals for the stock value. By default the number of decimals is set to **4**.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*
  Enable this toggle to set the stock value read-only. Disable the toggle to set the stock value editable. By default, this toggle is enabled.

  > [Info] If the warehouse logistic for an product is active and the *Invoicing* module is correctly connected, the stocks are transferred from the invoicing and automatically written into this attribute value. It is only recommended to deactivate the toggle *Read only* if the warehouse logistic is inactive and a stock value is needed.


## EntityCollectionValue (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## IntegerCollectionValue (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## StringCollectionValue (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## JSON (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Taxclass

![Taxclass](/Assets/Screenshots/PIM/DataTypes/Taxclass.png "[Taxclass]")

The data type *Taxclass* is used to indicate the tax class. A drop-down list with all available tax classes is displayed in the product view.

  > [Info] For detailed information about creating a tax class, see [Create a tax class](to_be_completed_#create-a-tax-class).

### Configuration

This data type has no further configuration settings.


## Taxzone

![Taxzone](/Assets/Screenshots/PIM/DataTypes/Taxzone.png "[Taxzone]")

The data type *Taxzone* is used to indicate the tax zone. A drop-down list with all available tax zones is displayed in the product view.

  > [Info] For detailed information about creating a tax zone, see [Create a tax zone](to_be_completed_#create-a-tax-zone).

### Configuration

This data type has no further configuration settings.



## Images

![Images](/Assets/Screenshots/PIM/DataTypes/Images.png "[Images]")

The data type *Images* is used to attach images. You can configure the filename prefix of the uploaded image, the allowed number of images and the file extensions. A preview of the uploaded images is displayed in the product view. In the *PIM Basic Set*, the following attributes have the data type *Images*:
- Images    

### Configuration

![Images](/Assets/Screenshots/PIM/DataTypes/Configuration/Images.png "[Images]")

- *Field for filename prefix*   
  Enter a fixed field name whose value will be used as filename prefix for the uploaded image, for example **id** or **sku**.

- *Min number of images*     
  Enter the minimum number of images.

- *Max number of images*     
  Enter the maximum number of images.

- *Allowed file extensions.*     
  Enter the allowed file extensions for the image format. If you want to allow several extensions, separate them with a comma. If no file extension is entered, all file extensions are allowed.


## Files

![Files](/Assets/Screenshots/PIM/DataTypes/Files.png "[Files]")

The data type *Files* is used to attach files. You can configure the filename prefix of the uploaded file, the allowed number of files and the file extensions. The uploaded files are displayed in a list in the product view. In the *PIM Basic Set*, the following attributes have the data type *Files*:
- Files    

### Configuration

![Files](/Assets/Screenshots/PIM/DataTypes/Configuration/Files.png "[Files]")

- *Field for filename prefix*   
  Enter a fixed field name whose value will be used as filename prefix for the uploaded file , for example **id** or **sku**.

- *Min number of files*     
  Enter the minimum number of files.

- *Max number of files*     
  Enter the maximum number of files.

- *Allowed file extensions.*     
  Enter the allowed file extensions for the file format. If you want to allow several extensions, separate them with a comma. If no file extension is entered, all file extensions are allowed.



## PIM-Channels Connection (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.   
In the *PIM Basic Set*, the following attributes have the data type *PIM-Channels Connection*:
- PIM Omni-Channel Connection


## UCS Product bundle (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## URLs (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Cloudinary Image

![Cloudinary image](/Assets/Screenshots/PIM/DataTypes/CloudinaryImage.png "[Cloudinary image]")

The data type *Cloudinary Image* is used to attach image files from Cloudinary. You can configure further data exchange settings for the image files. You can import image files from Cloudinary or upload image files to Cloudinary in the product view. This data type is only available when the *Cloudinary* module is installed.

### Configuration

![Cloudinary image](/Assets/Screenshots/PIM/DataTypes/Configuration/CloudinaryImage.png "[Cloudinary image]")

- *Folder*   
  Enter a folder name where the images are put into. If the folder is not yet created in Cloudinary, it is automatically created when uploading the first image. Use placeholders to define product specific folder, for instance **{sku}**.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*
  Enable this toggle to set the C*loudinary Image* value read-only. Disable the toggle to set the *Cloudinary Image* value editable. By default, this toggle is disabled.

- *Import Regex*     
  Enter a regular expression to restrict the listed items for the import of images from Cloudinary. The restriction is applied to the filename. If the field is left blank, no restriction is applied. For detailed information about regular expressions, see https://regex101.com/.

- *Meta Data Fields*     
  Enter names for additional contextual meta data fields. Use commas to separate the field names. A separate meta data field is created for each field name. By default, the *Title (caption)* and the *Description (alt)* contextual meta data fields are automatically created for each image and do not need to be added manually.

- *Connection*     
  Click the drop-down list and select the appropriate connection. All connections created in the *Cloudinary* module are displayed in the list.

**Structured Meta Data Fields**

In this section all structured meta data fields from the selected Cloudinary connection are displayed. Enable the meta data fields in the *PIM* module by activating the corresponding toggle. All inactive fields are not displayed in the *PIM* module and consequently cannot be edited in the *Cloudinary Image* attribute.


## Cloudinary Video

![Cloudinary video](/Assets/Screenshots/PIM/DataTypes/CloudinaryVideo.png "[Cloudinary video]")

The data type *Cloudinary Video* is used to attach video files from Cloudinary. You can configure further data exchange settings for the video files. You can import video files from Cloudinary or upload video files to Cloudinary in the product view. This data type is only available when the *Cloudinary* module is installed.

### Configuration

![Cloudinary video](/Assets/Screenshots/PIM/DataTypes/Configuration/CloudinaryVideo.png "[Cloudinary video]")

- *Folder*   
  Enter a folder name where the videos are put into. If the folder is not yet created in Cloudinary, it is automatically created when uploading the first video file. Use placeholders to define product specific folder, for instance **{sku}**.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*
  Enable this toggle to set the *Cloudinary Video* value read-only. Disable the toggle to set the *Cloudinary Video* value editable. By default, this toggle is disabled.

- *Import Regex*     
  Enter a regular expression to restrict the listed items for the import of videos from Cloudinary. The restriction is applied to the filename. If the field is left blank, no restriction is applied. For detailed information about regular expressions, see https://regex101.com/.

- *Meta Data Fields*     
  Enter names for additional contextual meta data fields. Use commas to separate the field names. A separate meta data field is created for each field name. By default, the *Title (caption)* and the *Description (alt)* contextual meta data fields are automatically created for each video and do not need to be added manually.

- *Connection*     
  Click the drop-down list and select the appropriate connection. All connections created in the *Cloudinary* module are displayed in the list.

**Structured Meta Data Fields**

In this section all structured meta data fields from the selected Cloudinary connection are displayed. Enable the meta data fields in the *PIM* module by activating the corresponding toggle. All inactive fields are not displayed in the *PIM* module and consequently cannot be edited in the *Cloudinary Video* attribute.


## XML (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Offer bundle

![Offer bundle](/Assets/Screenshots/PIM/DataTypes/OfferBundle.png "[Offer bundle]")

The data type *Offer bundle* is used to

[comment]: <> (For what?)

### Configuration

![Offer bundle](/Assets/Screenshots/PIM/DataTypes/Configuration/OfferBundle.png "[Offer bundle]")


- *Min relations*     
  Enter the minimum number of offers that must be related for an offer bundle.

- *Max relations*    
  Enter the maximum number of offers that can be related for an offer bundle.


## Object (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.

[comment]: <> (Check this - "No Data" displayed in the field in the product view)


## Encrypted Value (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Related products

![Related products](/Assets/Screenshots/PIM/DataTypes/RelatedProducts.png "[Related products]")

The data type *Related products* is used to connect other products to the selected product, for example for product recommendations. You can configure the allowed number of related products. You can select each created product as a related product in the product view. In the *PIM Basic Set*, the following attributes have the data type *Related products*:
- Product relations

### Configuration

![Related products](/Assets/Screenshots/PIM/DataTypes/Configuration/RelatedProducts.png "[Related products]")

- *Min relations*     
  Enter the minimum number of products that must be related to the selected product.

- *Max relations*    
  Enter the maximum number of products that can be related to the selected product.


## PIM Price Field

![PIM Price Field](/Assets/Screenshots/PIM/DataTypes/PIMPriceField.png "[PIM Price Field]")

The data type *PIM Price Field* is used to indicate a price. You can configure the number of decimals for the price and the supported currencies. In the product view, you must select a tax class for price calculation. Additionally, you can define a MSRP, scale prices and promotion periods. Unlike the data type *Simple price field*, the data type *PIM Price Field* offers more setting options and therefore also a more detailed and extended price specification. In the *PIM Basic Set*, the following attributes have the data type *PIM Price Field*:
- Price

### Configuration

![PIM Price Field](/Assets/Screenshots/PIM/DataTypes/Configuration/PIMPriceField.png "[PIM Price Field]")

- *Precision*   
  Enter the number of decimals for the price. By default the number of decimals is set to **2**.  

**SUPPORTED CURRENCIES**

- *Currency*    
  Click the drop-down list to select a currency. All available currencies are displayed in the drop-down list.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the currency left to this button.

- ![Add](/Assets/Icons/Plus06.png "[Add]") (Add)   
  Click this button to add another currency to the list of supported currencies. A new row with the drop-down list *Currency* is displayed below.


## Product Variants (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.   
In the *PIM Basic Set*, the following attributes have the data type *Product Variants*:
- Product variants



## Base price

![Base price](/Assets/Screenshots/PIM/DataTypes/BasePrice.png "[Base price]")

The data type *Base price* is used to indicate a base price. The base price is necessary to calculate the price per unit which is mandatory in th EU. Two drop-down lists to select the applicable dimension and unit and a field to enter the corresponding amount of the product are displayed in the product view. In the *PIM Basic Set*, the following attributes have the data type *Base price*:
- Base unit (Base price)

### Configuration

This data type has no further configuration settings.


## Product bundle

![Product bundle](/Assets/Screenshots/PIM/DataTypes/ProductBundle.png "[Product bundle]")

The data type *Product bundle* is used to define products that can be sold in a bundle with the selected product. In a product bundle, several different products are sold together, for example at a promotional price, without forming a packaging unit. That means, that each product has still its own EAN-code and can also be purchased by itself. You can configure the number of allowed products in a product bundle. In the *PIM Basic Set*, the following attributes have the data type *Product bundle*:
- Bundle

### Configuration

![Product bundle](/Assets/Screenshots/PIM/DataTypes/Configuration/ProductBundle.png "[Product bundle]")

- *Min relations*     
  Enter the minimum number of products that must be related for a product bundle.

- *Max relations*    
  Enter the maximum number of products that can be related for a product bundle.


## Packaging Unit

![Packaging Unit](/Assets/Screenshots/PIM/DataTypes/PackagingUnit.png "[Packaging Unit]")

The data type *Packaging Unit* is used to define packaging units. In a packaging unit, several same products are sold together in one fixed package. This package has its own EAN code and is handled as an own product. You can create multiple packaging units for a product in the product view.

### Configuration

This data type has no further configuration settings.
