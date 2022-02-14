# Data type list

To create a new attribute, you have to define a data type. In the following, all available data types, their use and their configuration is described in detail.

## Textfield

![Textfield](/Assets/Screenshots/PIM/Settings/Attributes/Textfield.png "[Textfield]")

The data type *Textfield* is used for long texts, e. g. for descriptions. You can configure the text length an the editor you use.
In the PIM basic product set, the following attributes have the data type *Textfield*:
- Article short description
- Article description
- Long text

### Configuration

![Textfield](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/Textfield.png "[Textfield]")

- *Min length*   
  Enter a minimal length of the textfield.

- *Max length*   
  Enter a maximal length of the textfield.

- *Rows*   
  Enter the number of rows in the textfield. By default the number of rows is set to **5**.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *HTML Editor*   
  Activate this toggle to enable the HTML editor for the textfield. A WYSIWIG-editor is displayed to edit the textfield. Deactivate the toggle to disable the HTML editor for the textfield. By default, this toggle is inactive.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Activate this toggle to set the textfield read-only. Deactivate the toggle to set the textfield editable. By default, this toggle is inactive.


## Checkbox

![Checkbox](/Assets/Screenshots/PIM/Settings/Attributes/Checkbox.png "[Checkbox]")

The data type *Checkbox* is used to indicate a statement that is either true or false, e. g. if a product is a digital or real product. The checkbox is displayed by a toggle. In the PIM basic product set, the following attributes have the data type *Checkbox*:
- Sale items
- FSK18
- Digital product

> [Info] Note that the date type *Checkbox* also has the third value **not set**. When creating or importing a product, the value **not set** is set for the corresponding attribute. After saving, the value switches automatically to **false** if it was not manually changed to **true**. This may cause problems when connecting to other systems, e.g. shops or marketplaces, with different default settings for checkboxes.   

### Configuration

This data type has no further configuration settings.


## Floating point number

![Floating point number](/Assets/Screenshots/PIM/Settings/Attributes/FloatingPointNumber.png "[Floating point number]")

The data type *Floating point number* is used to indicate decimal numbers without a unit. You can configure the number of decimal places and the number range.

### Configuration

![Floating point number](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/FloatingPointNumber.png "[Floating point number]")

- *Precision*   
  Enter the number of decimal places for the floating point number. By default the number of decimals is set to **4**.  

- *Min value*   
  Enter a minimum value for the floating point number.  

- *Max value*   
  Enter a maximum value for the floating point number.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Activate this toggle to set the floating point number read-only. Deactivate the toggle to set the floating point number editable. By default, this toggle is inactive.


## Integer

![Integer](/Assets/Screenshots/PIM/Settings/Attributes/Integer.png "[Integer]")

The data type *Integer* is used to indicate whole numbers without a unit. You can configure the number range.

### Configuration

![Integer](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/Integer.png "[Integer]")

- *Min value*   
  Enter a minimum value for the integer.  

- *Max value*   
  Enter a maximum value for the integer.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Activate this toggle to set the integer read-only. Deactivate the toggle to set the integer editable. By default, this toggle is inactive.


## String

![String](/Assets/Screenshots/PIM/Settings/Attributes/String.png "[String]")

The data type *String* is used for short texts or alphanumeric information, e. g. keywords. You can configure the string length and define regular expressions for the string. In the PIM basic product set, the following attributes have the data type *String*:
- Article name
- EAN-code
- Digital product
- Customs tariff number
- Manufacturer link
- Additional search terms
- Tags/Keywords
- Meta title
- Meta description
- Meta keywords
- Volume

### Configuration

![String](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/String.png "[String]")

- *Min length*   
  Enter a minimal length of the string.

- *Max length*   
  Enter a maximal length of the string.

- *Regex*   
  Enter a regular expression for the string. For detailed information about regular expressions, see https://regex101.com/.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*   
  Activate this toggle to set the string read-only. Deactivate the toggle to set the string editable. By default, this toggle is inactive.


## Currency

![Currency](/Assets/Screenshots/PIM/Settings/Attributes/Currency.png "[Currency]")

The data type *Currency* is used to indicate a currency. A drop-down list with all currencies in the system is displayed in the product view.

### Configuration

This data type has no further configuration settings.


## Language

![Language](/Assets/Screenshots/PIM/Settings/Attributes/Language.png "[Language]")

The data type *Language* is used to indicate a language. A drop-down list with all languages in the system is displayed in the product view.

### Configuration

This data type has no further configuration settings.


## Country

![Country](/Assets/Screenshots/PIM/Settings/Attributes/Country.png "[Country]")

The data type *Country* is used to indicate a country. A drop-down list with all countries in the system is displayed in the product view. In the PIM basic product set, the following attributes have the data type *Country*:
- Country of origin

### Configuration

This data type has no further configuration settings.


## TreeNode

The data type *TreeNode* is used for indications with multiple, predefined selection options. You have to define the different selection options in the configuration. Additionally you can configure whether the selection of values will be a multiple or single selection.

[comment]: <> (to be edited)

![TreeNode](/Assets/Screenshots/PIM/Settings/Attributes/TreeNode.png "[TreeNode]")

### Configuration

![TreeNode](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/TreeNode.png "[TreeNode]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi Select*   
  Activate this toggle to enable a multiple selection of values. Deactivate the toggle to allow only a single selection of values. By default, this toggle is inactive.

> [Info] In the product view, the data type *TreeNode* is displayed either by a drop-down list or a a box with all created options. The drop-down list is only displayed for one dimensional single select trees.

**Edit tree**

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click first this button and then the plus sign displayed in the left column of the *Edit tree* table to add an attribute value. The *Add Element* window is displayed.

### Add Element

![Add element](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/AddElement.png "[Add element]")

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


## Number with Unit

![Number with Unit](/Assets/Screenshots/PIM/Settings/Attributes/NumberUnit.png "[Number with Unit]")

The data type *Number with Unit* is used for numerical specifications of a certain unit of measurement, e. g. weight specifications. You can can define the unit of measurement. In the PIM basic product set, the following attributes have the data type *Number with Unit*:
- Length
- Width
- Depth
- Article weight

### Configuration

![Number with Unit](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/NumberUnit.png "[Number with Unit]")

[comment]: <> (Configuration missing)


## DateTime

![DateTime](/Assets/Screenshots/PIM/Settings/Attributes/DateTime.png "[DateTime]")

The data type *DateTime* is used to indicate a date and/or a time. You can configure whether to display or not the date and the time and you can select a date and time format. A calendar widget to select the date is displayed in the product view. In the PIM basic product set, the following attributes have the data type *DateTime*:
- Expiration date

### Configuration

![DateTime](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/DateTime.png "[DateTime]")

- *Date*
  Click the drop-down list to select a date format. The formats below are available. By default, the date format **Short** is selected.
  - **Do not show date**: hidden date
  - **Short**: short format, e.g. 02/11/2021
  - **Medium**: medium format, writing out the month, e.g. February 11, 2021
  - **Long**: long format, adding the weekday and writing out the month, e.g. Monday, February 11, 2021


- *Time*    
  Click the drop-down list to select a time format. The formats below are available. By default, the time format **Medium** is selected.
  - **Do not show time**: hidden time
  - **Short**: short format, e.g. 09:00 PM
  - **Medium**: medium format, including seconds, e.g. 09:00:00 PM


## Sales Unit Value

![Sales Unit Value](/Assets/Screenshots/PIM/Settings/Attributes/SalesUnitValue.png "[Sales Unit Value]")

The data type *Sales Unit Value* is used to define a dimension and a unit. Two drop-down lists to select the applicable dimension and unit are displayed in the product view. Depending on the selected dimension, the options for the unit are adapted. In the PIM basic product set, the following attributes have the data type *Sales Unit Value*:
- Sales unit

### Configuration

This data type has no further configuration settings.


## Simple price field

![Simple price field](/Assets/Screenshots/PIM/Settings/Attributes/SimplePriceField.png "[Simple price field]")

The data type *Simple price field* is used to indicate a price. You can configure the use of gross or net price, the display of an MSRP field and promotion prices and the currency to be used. Additionally, you can create scale prices in the product view. Unlike the data type *Preise*, the data type *Simple price field* requires less information to indicate the price.

### Configuration

![Simple price field](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/SimplePriceField.png "[Simple price field]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Gross prices*   
  Activate this toggle to display gross prices. Deactivate the toggle to display net prices. By default, this toggle is active.

  > [Info] Note that it is especially for the ETL-mapping very important if prices are net or gross.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Show MSRP field*   
  Activate this toggle to display the MSRP field. Deactivate the toggle to hide the MSRP field. By default, this toggle is inactive.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Use Promotions*    
  Activate this toggle to enable to enter a promotion period for prices. Deactivate the toggle to not allow promotion prices. By default, this toggle is inactive.

- *Currency*   
  Click the drop-down list to select the currency to be used. All available currencies are displayed in the drop-down list.

[comment]: <> (Not working -> MSRP field is displayed even when the toggle is not active -> to be fixed)


## Stock Value

![Stock Value](/Assets/Screenshots/PIM/Settings/Attributes/StockValue.png "[Stock Value]")

The data type *Stock Value* is used to indicate the number of stocks. You can configure the number of decimal places. A new target channel for this stock is created in the *Stock* module for the inventory assignment. In the PIM basic product set, the following attributes have the data type *Stock Value*:
- Stock  

### Configuration

![Stock Value](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/StockValue.png "[Stock Value]")

- *Precision*
  Enter the number of decimals for the stock value. By default the number of decimals is set to **4**.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Read only*
  Activate this toggle to set the stock value read-only. Deactivate the toggle to set the stock value editable. By default, this toggle is active.

  > [Info] If the warehouse logistic for an product is active and the *Invoicing* module is correctly connected, the stocks are transferred from the invoicing and automatically written into this attribute value. It is only recommended to deactivate the toggle *Read only* if the warehouse logistic is inactive and a stock value is needed.


## EntityCollectionValue (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## IntegerCollectionValue (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## StringCollectionValue (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Taxclass

![Taxclass](/Assets/Screenshots/PIM/Settings/Attributes/Taxclass.png "[Taxclass]")

The data type *Taxclass* is used to indicate the tax class. A drop-down list with all available tax classes is displayed in the product view.

  > [Info] For detailed information about creating a tax class, see [Create a tax class](to_be_completed_#create-a-tax-class).

### Configuration

This data type has no further configuration settings.


## Images

![Images](/Assets/Screenshots/PIM/Settings/Attributes/Images.png "[Images]")

The data type *Images* is used to attach images. You can configure the filename prefix of the uploaded image, the allowed number of images and the file extensions. A preview of the uploaded images is displayed in the product view. In the PIM basic product set, the following attributes have the data type *Images*:
- Images    

### Configuration

![Images](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/Images.png "[Images]")

- *Field for filename prefix*   
  Enter a fixed field name whose value will be used as filename prefix for the uploaded image, e. g. **id** or **sku**.

- *Min number of images*     
  Enter the minimum number of images.

- *Max number of images*     
  Enter the maximum number of images.

- *Allowed file extensions.*     
  Enter the allowed file extensions for the image format. If you want to allow several extensions, separate them with a comma. If no file extension is entered, all file extensions are allowed.


## Files

![Files](/Assets/Screenshots/PIM/Settings/Attributes/Files.png "[Files]")

The data type *Files* is used to attach files. You can configure the filename prefix of the uploaded file, the allowed number of files and the file extensions. The uploaded files are displayed in a list in the product view. In the PIM basic product set, the following attributes have the data type *Files*:
- Files    

### Configuration

![Files](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/Files.png "[Files]")

- *Field for filename prefix*   
  Enter a fixed field name whose value will be used as filename prefix for the uploaded file , e. g. **id** or **sku**.

- *Min number of files*     
  Enter the minimum number of files.

- *Max number of files*     
  Enter the maximum number of files.

- *Allowed file extensions.*     
  Enter the allowed file extensions for the file format. If you want to allow several extensions, separate them with a comma. If no file extension is entered, all file extensions are allowed.



## Verbindung PIM zu Channels (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## UCS Product bundle (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## URLs (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## XML (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Encrypted Value (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Related products

![Related products](/Assets/Screenshots/PIM/Settings/Attributes/RelatedProducts.png "[Related products]")

The data type *Related products* is used to connect other products to the selected product, e. g. for product recommendations. You can configure the allowed number of related products. You can select each created product as a related product in the product view. In the PIM basic product set, the following attributes have the data type *Related products*:
- Cross Selling

### Configuration

![Related products](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/RelatedProducts.png "[Related products]")

- *Min relations*     
  Enter the minimum number of products that must be related to the selected product.

- *Max relations*    
  Enter the maximum number of products that can be related to the selected product.


## Preise

![Preise](/Assets/Screenshots/PIM/Settings/Attributes/Preise.png "[Preise]")

The data type *Preise* is used to indicate a price. You can configure the number of decimals for the price and the supported currencies. In the product view, you must select a tax class for price calculation. Additionally, you can define a MSRP, scale prices and promotion periods. Unlike the data type *Simple price field*, the data type *Preise* offers more setting options and therefore also a more detailed and extended price specification. In the PIM basic product set, the following attributes have the data type *Preise*:
- Price

### Configuration

![Preise](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/Preise.png "[Preise]")

- *Precision*   
  Enter the number of decimals for the price. By default the number of decimals is set to **2**.  

**SUPPORTED CURRENCIES**

- *Currency*    
  Click the drop-down list to select a currency. All available currencies are displayed in the drop-down list.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the currency left to this button.

- ![Add](/Assets/Icons/Plus06.png "[Add]") (Add)   
  Click this button to add another currency to the list of supported currencies. A new row with the drop-down list *Currency* is displayed below.


## Produktvarianten (internal, not editable)

This data type is for internal use only. It is strongly advised not to use this data type without the required knowledge.


## Grundpreisangabe

![Grundpreisangabe](/Assets/Screenshots/PIM/Settings/Attributes/Grundpreisangabe.png "[Grundpreisangabe]")

The data type *Grundpreisangabe* is used to indicate a base price. The base price is necessary to calculate the price per unit which is mandatory in th EU. Two drop-down lists to select the applicable dimension and unit and a field to enter the corresponding amount of the product are displayed in the product view. In the PIM basic product set, the following attributes have the data type *Grundpreisangabe*:
- Base unit (base price)

### Configuration

This data type has no further configuration settings.


## Product bundle

![Product bundle](/Assets/Screenshots/PIM/Settings/Attributes/ProductBundle.png "[Product bundle]")

The data type *Product bundle* is used to define products that can be sold in a bundle with the selected product. In a product bundle, several different products are sold together, e. g. at a promotional price, without forming a packaging unit. That means, that each product has still its own EAN-code and can also be purchased by itself. You can configure the number of allowed products in a product bundle. In the PIM basic product set, the following attributes have the data type *Product bundle*:
- Bill of materials

### Configuration

![Product bundle](/Assets/Screenshots/PIM/Settings/Attributes/Configuration/ProductBundle.png "[Product bundle]")

- *Min relations*     
  Enter the minimum number of products that must be related for a product bundle.

- *Max relations*    
  Enter the maximum number of products that can be related for a product bundle.


## Packaging Unit

![Packaging Unit](/Assets/Screenshots/PIM/Settings/Attributes/PackagingUnit.png "[Packaging Unit]")

The data type *Packaging Unit* is used to define packaging units. In a packaging unit, several same products are sold together in one fixed package. This package has its own EAN code and is handled as an own product. You can create multiple packaging units for a product in the product view.

### Configuration

This data type has no further configuration settings.
