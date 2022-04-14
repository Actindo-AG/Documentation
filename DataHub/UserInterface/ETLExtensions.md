# ETL extensions list

The ETL (Extract Transform Load) is used to extract data from a certain source, transform it in a specific way and load it into a defined destination. In the *DataHub* module, the attribute sets are mapped via ETL. The attributes of the source attribute set are mapped to the attributes of the destination attribute set.   
The ETL extensions are used to define how the data is transformed from the source attribute to the destination attribute. The ETL extensions provided for a mapping differ depending on the destination attribute. The data type of the destination attribute determines the available ETL extensions. The selected extension, in turn, determines the available source attributes by defining the data type of the source attribute. In addition, further settings can be defined for some ETL extensions.    
The list below describes in detail all available ETL extensions and, if available, their specific configurations.


## Add prefix/suffix

![Add prefix suffix](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/AddPrefixSuffix.png "[Add prefix suffix]")

This extension is used to add a specific prefix and/or suffix to the destination attribute. The prefix and/or suffix to be added is defined in the configuration.

### Configuration
- *Prefix*    
  Enter the prefix to be added before the value of the destination attribute.

- *Suffix*   
  Enter the suffix to be added after the value of the destination attribute.


## Arithmetic Extension

![Arithmetic extension](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ArithmeticExtension.png "[Arithmetic extension]")

This mapping is used to specify one or more fallback attributes to be mapped if the first attribute is not available. At least one source attribute must be selected in the *x1* drop-down list. Up to eight attributes can be selected in the drop-down lists. Enter the function to be applied in the configuration.  

### Configuration
- *Equation 1*   
  Enter the function to be applied to the selected source attributes. You have to follow the syntax below: ???

[comment]: <> (funktioniert nicht - welche Syntax muss in der Equation genutzt werden? Muss immer eine Equation angegeben sein? )

- ![Add](/Assets/Icons/Plus03.png "[Add]") (Add)   
  Click this button to add another equation. You can add an unlimited number of equations.

[comment]: <> (pro modifier nur ein wert ändern? oder warum brauche ich davon mehrere?)


## Basic Mapping

![Basic mapping](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NumberToString.png "[Basic mapping]")

This mapping is used to adopt the value from a source attribute to a destination attribute without any change. The basic mapping is the most commonly used mapping and can be applied to all data types.

[comment]: <> (stimmt das?)

### Configuration
This ETL extension has no further configuration settings.


## Boolean-To-String

![Number to String](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NumberToString.png "[Number to String]")

This extension is used to map a boolean attribute (checkbox or toggle) to a string attribute. The content that is mapped to the string depending on the boolean value is defined in the configuration.

### Configuration
- *Content for value true*   
  Enter the content that is mapped to the string attribute when the boolean value equals true, which means that the checkbox is selected or the toggle is active.
- *Content for value false*   
  Enter the content that is mapped to the string attribute when the boolean value equals false, which means that the checkbox is not selected or the toggle is inactive.


## Catalog Tree to Tree value mapping

![Catalog tree to tree value mapping](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/CatalogTreeToTreeValueMapping.png "[Catalog tree to tree value mapping]")

This extension is used to map a catalog attribute to a tree node attribute. It is mainly used to map the Actindo specific categories.

### Configuration
This ETL extension has no further configuration settings.



## Cloudinary-to-String

This extension is used to map a Cloudinary attribute to a string attribute. Select at least one and up to four Cloudinary source attributes in the *Image* drop-down lists. If required, you can select a transformation.

[comment]: <> (wofür ist die Liste Transformation? Was mache ich damit?)

### Configuration

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Export public ID*   
  Activate the toggle to export both, the Cloudinary URL but also its public ID. Deactivate the toggle to export only the Cloudinary URL.

  [comment]: <> (wozu ist die public ID gut?)


## Constant value

![Constant value](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ConstantValue.png "[Constant value]")

This extension is used to map a constant value to a destination attribute of a random data type. The fixed source value is defined in the configurations and never changes. This extension is often used according to receipts, for instance to define the receipt type.

[comment]: <> (Is that right? random destination attribute? or only string?)

### Configuration
- *Destination attribute name*   
   Enter a value that is always mapped to the destination attribute.


## Copy cloudinary image value
destination attribute: Cloudinary images

### Configuration

This ETL extension has no further configuration settings.


## Copy packaging units

### Configuration
This ETL extension has no further configuration settings.


## Country-To-X

![Country to X](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/CountryToX.png "[Country to X]")

This extension is used to map a country attribute to a string attribute. It is mainly used to map the Actindo *Country of Origin* attribute.

[comment]: <> (Is that right? only string?)

### Configuration
This ETL extension has no further configuration settings.


## Date Converter

![Date Converter](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/DateConverter.png "[Date Converter]")

This extension is used to map a date attribute to another date attribute of a different format or to a string attribute. The destination date format is defined in the configuration. Further, additional modifiers can be defined to change the date by a defined time value.

[comment]: <> (Is that right? destination = string or date?)

### Configuration
- *Destination Format*   
  Enter the destination format of the date, for instance **Y-m-d**. The date must be entered in the php format, see https://www.php.net/manual/de/datetime.format.php.

- *Modifier 1*   
  Enter a value for the modifier to change the source date by a certain time value. For instance, enter **+ 7 days** to predate the date in the source attribute always by 7 days in the destination attribute. You can predate a date by using a plus sign, or backdate a date by using a minus sign.

  [comment]: <> (modifier format? ausgeschrieben oder abkürzungen wie in destination format feld? What format is taken if nothing is defined in the configuration?)

- ![Add](/Assets/Icons/Plus03.png "[Add]") (Add)   
  Click this button to add another modifier. You can add an unlimited number of modifiers.

  [comment]: <> (pro modifier nur ein wert ändern? oder warum brauche ich davon mehrere? Fehler in UI?)


## EAN zu Artikelnummer ???

### Configuration


## Entity Id to Generic Property Extension -

![Entity ID to generic property extension](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/EntityIDToGenericPropertyExtension.png "[Entity ID to generic property extension]")

This extension is used to map the generic property of an entity attribute to a string attribute. It is often used for the data export.

[comment]: <> (Finde kein Source attribut bei dme die Konfiguration angezeigt wird. Anwendungsfall aufzeigen!)

### Configuration
- *Empty drop-down list*
  - Beleg
  - Beleg-Position
  - Kunde


- *Field Name*   
  Enter the name of the field assigned to the entity attribute whose value should be mapped to the destination attribute.



## ETLPIMToUCSBundleExtension

![ETL PIM to UCS bundle extension](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ETLPIMToUCSBundleExtension.png "[ETL PIM to UCS bundle extension]")

This extension is used to map a PIM product bundle attribute to a UCS bundle attribute. This extension is Actindo specific and is only used in the mapping from the PIM to the RetailSuite. It is mainly used to manage the stock of sets.

### Configuration
This ETL extension has no further configuration settings.



## Html-Template

![HTML template](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/HTMLTemplate.png "[HTML template]")

This extension is used to map a HTML template attribute to a random destination attribute. The HTML template to be applied is selected in the configuration. This extension is selected for mappings requiring more logical assignments which cannot be mapped with the other extensions, for instance it is often used for the document export. This extension is only available when the *HTML Templates for ETL* plugin is installed.  
For detailed information about HTML templates, see [Manage the HTML templates](/PIM/Operation/03_ManageHTMLTemplates.md).

### Configuration

- *Html-Template*   
  Select the HTML template to be applied to the mapping. The HTML templates can be created in the *HTML TEMPLATES* tab.



## Identity-Mapping

### Configuration
This ETL extension has no further configuration settings.


## Image-To-Download-Link

![Image to download link](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ImageToDownloadLink.png "[Image to download link]")

This extension is used to map the download link of an image attribute to a string attribute, for instance for csv exports. The image number must be indicated in the configuration.

### Configuration

- *Enter the image number*    
  Enter the number of the image whose download link should be mapped. The image number must be entered regardless of whether one or more images are assigned to the image attribute.

- *Enter image validity (days)*   
  Enter the period in days for which the image can be downloaded by the link. If the field is left empty, the link will be valid for an unlimited period of time.  

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Is the image downloadable only once?*   
  Activate the toggle to allow only a single download of the image. After that, the link will be invalid. Deactivate the toggle to allow an unlimited number of downloads.  



## Image-To-ImageTags

![Image to image tags](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ImageToImageTags.png "[Image to image tags]")

This extension is used to map the image tags of an image attribute to a string attribute. The image number must be indicated in the configuration.

### Configuration

- *Enter the image number*   
  Enter the number of the image whose tags should be mapped. The image number must be entered regardless of whether one or more images are assigned to the image attribute.


## Import Base price
destination attribute: Stock
### Configuration


## Import from cloudinary folder
destination attribute: Cloudinary images

### Configuration

- *Folder*



## Import special price

![Import special price](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ImportSpecialPrice.png "[Import special price]")

This extension is used to map a promotion price to a price attribute. The promotion price to be mapped is composed of different source attributes. By the source attributes, define:  
  - whether the discount is a percent discount or an absolute discount
  - the amount of the discount
  - the currency
  - the start quantity from which the promotion price is applied
  - the start date of the promotion price
  - the end date of the promotion price

Beside the dates, all attributes are required for the mapping.

[comment]: <> (Is that right?)

### Configuration
This ETL extension has no further configuration settings.


## Language-To-X

![Language to x](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/LanguageToX.png "[Language to x]")

This extension is used to map a language attribute to a string attribute. It is mainly used to map the Actindo language attributes.

[comment]: <> (Is that right? only string?)

### Configuration

- *languageValue*   
  Select the appropriate display type for the language attribute. The following types are available:
  - **3 digit code**: The three-letter language code according to ISO 639-2 is used. For languages with a bibliographic (B) and a terminological (T) code, both codes are indicated, for instance *ger (B), deu (T)*.
  - **2 digit code**: The two-letter language code according to ISO 639-1 is used, for instance *de*.
  - **Name (english)**: The english language name is used, for instance *german*.
  - **Name (french)**: The french language name is used, for instance *allemand*.
  - **Name (german)**: The german language name is used, for instance *deutsch*.


## Mapping Table

![Mapping table](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/MappingTable.png "[Mapping table]")

This extension is used to map a fixed set of source attribute values to fixed destination attribute values differing from the source values. The destination values are assigned in the configuration. This extension is often used in the order import, for instance with the different shipping providers names in the store and Actindo.

### Configuration

| Source Value   | Destination Value     |
|----------------|-----------------------|
| All available values for the selected source attribute are automatically displayed in this column. | Click the row in this column to enter or select a destination value for the corresponding source value. When a tree node attribute is selected as a destination attribute, all predefined values for this attribute are available in a drop-down list. |

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)    
  Click this button to manually add a source value to the mapping table.


## Mysql query

![MySQL query](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/MySQLQuery.png "[MySQL query]")

This extension is used to map a MySQL query to a random destination attribute. The MySQL query to be applied is selected in the configuration. Mainly, this extension is selected for mappings requiring more logical assignments which cannot be mapped with the other extensions. This extension is only available when the *Database and Reporting* module is installed.  

### Configuration

- *Query*   
  Select the MySQL query to be applied to the mapping. The MySQL query can be created in the *DB and Reporting* module: *DB and Reporting > Managed queries > Tab QUERIES*.

- *Column*   
  ???

  [comment]: <> (was wird hier gewählt? Bild fehlt! Modul installieren? TEST button -> wofür? No change tracking?)


## Next Promotion Base Price to Float

### Configuration
- Country: dropdown with all available countries
- Currency: dropdown with all available currencies
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Destination gross*   



## Next special base price to date time

![Next special base price to date time](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NextSpecialBasePriceToDateTime.png "[Next special base price to date time]")

This extension is used to map the promotion date of a PIM price field attribute to a date attribute. The PIM price field is Actindo specific and contains not only the simple price, but also the base price, scale prices, promotion prices, the tax class including the tax rate and supported currencies. Each of this data is extracted from the price attribute by the corresponding extension. In this case, the date of the next promotion is mapped by the *Next special base price to date time* extension. Further settings are defined in the configuration.

### Configuration
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Get from date*   
  Activate the toggle to map the start date of the promotion. Otherwise the end date of the promotion is mapped to the destination attribute.

[comment]: <> (Ist das hier genau andersherum wie im deutschen? Da aktiviert man den Toggle, um das bis-datum zu bekommen - oder ist das nen Übersetzungsfehler?)

- *Currency*   
  Select the appropriate currency in the drop-down list. Only those currencies that are defined as a supported currency in the PIM price field attribute configuration are mapped. in All available currencies are displayed in the list.

  [comment]: <> (Is that right? what currencies are mapped?)


## Null Coalescence Extension

![Null coalescence extension](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NullCoalescenceExtension.png "[Null coalescence extension]")

This extension is used to specify one or more fallback attributes to be mapped if the first attribute is not available. At least one source attribute must be selected in the *x0* drop-down list and one fallback attribute in the *x1* drop-down list. If the value of the source attribute in the *x0* drop-down list is empty, the value of the source attribute in the *x1* drop-down list is applied and so on. Up to four source attributes can be selected in the drop-down lists. Note that a blank space is also considered as an input.

[comment]: <> (Unterschied zu Arithmetic Extension?)

### Configuration

- *Relevant Language*   
  Select the language of the attribute value used for the mapping. This setting only applies when a tree node attribute is mapped to a single language attribute. All active languages are displayed in the drop-down list.

  [comment]: <> (Was ist, wenn ich keine Sprache wähle?)


## Number-To-String

![Number to String](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NumberToString.png "[Number to String]")

This extension is used to map a number attribute to a string attribute. The value is mapped unchanged, only the data type of the attribute changes.

### Configuration
This ETL extension has no further configuration settings.


## Number-To-UnitValue

![Number to unit value](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NumberToUnitValue.png "[Number to unit value]")

This extension is used to map a number attribute to an unit attribute. This mapping is used when the source value is always maintained in a certain unit that is not included in the source attribute but must be mapped to an unit attribute, which always includes both, the quantity and the unit. Define the unit settings in the configuration.

### Configuration
- *SourceUnit*   
  Select the appropriate unit of the source attribute to calculate the quantity value into the correct unit. All units corresponding to the dimension of the destination attribute are displayed in the drop-down list.

- *Mode destination unit*   
  Select the appropriate unit mapping mode. The following modes are available:
  - **Configure manually**: The unit to be mapped to the destination attribute must be selected in the *Unit to convert to* drop-down list. The quantity value is calculated into the correct destination unit.
  - **Keep unit**: The unit selected in the *SourceUnit* drop-down list is mapped to the destination attribute.
  - **Default unit of destination attribute**: The configured default destination unit is kept in the destination attribute. The quantity value is calculated into the correct destination unit.

- *Unit to convert to*   
  Select the appropriate unit of the destination attribute to calculate the quantity value into the correct unit. All units corresponding to the dimension of the destination attribute are displayed in the drop-down list.


## PIM BasePrice to Amount (VPE Value)

![PIM base price to amount](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PIMBasePriceToAmount.png "[PIM base price to amount]")

This extension is used to map a PIM base price attribute to a number or stock value attribute. The base price is Actindo specific and contains the dimension, the unit and the relevant amount for the base price. Each of this data is extracted from the base price attribute by the corresponding extension. In this case, the amount is mapped by the *PIM BasePrice to Amount (VPE Value)* extension.

[comment]: <> (Is the destination attribute right- number/stock value attribute?)

### Configuration
This ETL extension has no further configuration settings.


## PIM BasePrice to Boolean (VPE Active)

![PIM base price to boolean](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PIMBasePriceToBoolean.png "[PIM base price to unit]")

This extension is used to map a PIM base price attribute to a boolean attribute, for instance to define whether or not a base price is available. If the PIM base price attribute is empty, the false value is mapped to the boolean attribute. Otherwise, the true value is mapped to the boolean attribute.

[comment]: <> (Is that right? Anwendungsfall?)

### Configuration
This ETL extension has no further configuration settings.


## PIM BasePrice to Unit

![PIM base price to unit](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PIMBasePriceToUnit.png "[PIM base price to unit]")

This extension is used to map a PIM base price attribute to a tree node attribute. The PIM base price is Actindo specific and contains the dimension, the unit and the relevant amount for the base price. Each of this data is extracted from the PIM base price attribute by the corresponding extension. In this case, the unit is mapped by the *PIM BasePrice to Unit* extension.

[comment]: <> (Is that right- tree node attribute?)

### Configuration
This ETL extension has no further configuration settings.


## PIM BasePrice to VPE Reference Unit

![PIM base price to VPE reference unit](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PIMBasePriceToVPEReferenceUnit.png "[PIM base price to VPE reference unit]")

This extension is used to map a PIM base price attribute to a number or stock value attribute. The PIM base price is Actindo specific and contains the dimension, the unit and the relevant amount for the base price. Each of this data is extracted from the PIM base price attribute by the corresponding extension. In this case, the amount is mapped by the *PIM BasePrice to VPE Reference Unit* extension as a reference amount.

[comment]: <> (Doesn't make sense - why/how mapping a unit to a number/stock value attribute???)

### Configuration
This ETL extension has no further configuration settings.



## PIM Price to Simple Price

This extension is used to map a PIM base price attribute to a tree node attribute. The PIM base price is Actindo specific and contains the dimension, the unit and the relevant amount for the base price. Each of this data is extracted from the PIM base price attribute by the corresponding extension. In this case, the unit is mapped by the *PIM BasePrice to Unit* extension.

### Configuration
- *Country*   

- *Mapping mode*   



## Preg Replace Extension

### Configuration
- Pattern
- Replacement


## PriceBuilder

![Price builder](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PriceBuilder.png "[Price builder]")

This extension is used to map an individual price to a price attribute. The price to be mapped is composed of different source attributes. By the source attributes, define:  
  - the tax class
  - the base price
  - the currency
  - whether the price is gross or net
  - the MSRP

Beside the MSRP, all attributes are required for the mapping.

[comment]: <> (Is that right?)

### Configuration
This ETL extension has no further configuration settings.


## Price to price with discount

![Price to price with discount](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PriceToPriceWithDiscount.png "[Price to price with discount]")

This extension is used to map a PIM price field attribute including a defined discount to another PIM price field attribute. In the discount attribute, a number for the percentage discount is defined. The source price field attribute less the selected disount is mapped to the destination price attribute.

### Configuration
This ETL extension has no further configuration settings.


## Price to Tax

![Price to tax](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PriceToTax.png "[Price to tax]")

This extension is used to map a PIM price field attribute to a number attribute. The PIM price field is Actindo specific and contains not only the simple price, but also the base price, scale prices, promotion prices, the tax class including the tax rate and supported currencies. Each of this data is extracted from the price attribute by the corresponding extension. In this case, the tax rate is mapped by the *Price to Tax* extension. The tax rate settings are defined in the configuration.

[comment]: <> (Is that right- number attribute?)

### Configuration
- *Country*   
  Select the appropriate country in the drop-down list to apply the corresponding tax rate. All available countries are displayed in the list.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *In percent*   
  Activate the toggle to indicate the tax rate as a percentage. Otherwise, the tax rate is indicated as a decimal number.

[comment]: <> (Is that right?)


## Price to Tax Class

![Price to tax class](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PriceToTaxClass.png "[Price to tax class]")

This extension is used to map a PIM price field attribute to a tree node attribute. The PIM price field is Actindo specific and contains not only the simple price, but also the base price, scale prices, promotion prices, the tax class including the tax rate and supported currencies. Each of this data is extracted from the price attribute by the corresponding extension. In this case, the tax class is mapped by the *Price to Tax Class* extension.

[comment]: <> (Is that right- tree node attribute?)

### Configuration

**Map PIM-Taxclasses to corresponding Tree Nodes**

For each tax class defined in Actindo, a single drop-down list is displayed:

- *Standardsatz*   
  Select the tax rate to be mapped to the standard rate in the destination attribute. All available tax rates from the destination attribute are displayed in the drop-down list.

- *Ermäßigt*   
  Select the tax rate to be mapped to the reduced rate in the destination attribute. All available tax rates from the destination attribute are displayed in the drop-down list.

[comment]: <> (Stimmt das? When is the configuration displayed?)



## Pricing to float

![Pricing to float](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PricingToFloat.png "[Pricing to float]")

This extension is used to map a PIM price field attribute to a random destination attribute. The PIM price field is Actindo specific and contains not only the simple price, but also the base price, scale prices, promotion prices, the tax class including the tax rate and supported currencies. Each of this data is extracted from the price attribute by the corresponding extension. In this case, the price itself is mapped by the *Pricing to float* extension. A discount to the price can be entered in the *Discount in percent* drop-down list. Further price settings are defined in the configuration.

[comment]: <> (random destination attribute)


### Configuration

- *Country*     
  Select the appropriate country in the drop-down list to apply the correct tax rate to the price. All available countries are displayed in the list.

- *Currency*   
  Select the appropriate currency in the drop-down list. Only those currencies that are defined as a supported currency in the PIM price field attribute configuration are mapped. in All available currencies are displayed in the list.

  [comment]: <> (Is that right? what currencies are mapped?)

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Destination gross*   
  Activate the toggle to map the gross price of the source attribute. Deactivate the toggle to map the net price.


## Pricing to float with fallback price

![Pricing to float with fallback price](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PricingToFloatWithFallbackPrice.png "[Pricing to float with fallback price]")

This extension is used to map a PIM price field attribute with a fallback PIM price field attribute to a number attribute. This mapping is similar to the *Pricing to float* extension with an additional fallback price. The *Special Price* attribute is always considered first when mapping. The *Fallback Price* attribute is only used as a fallback price that will be mapped when no other price is available. The fallback price attribute is mandatory. This mapping is used when at least two PIM price field attributes with different prices are maintained. Further price settings are defined in the configuration.

[comment]: <> (Is that right? number destination attribute?)

### Configuration

- *Country*     
  Select the appropriate country in the drop-down list to apply the correct tax rate to the price. All available countries are displayed in the list.

- *Currency*   
  Select the appropriate currency in the drop-down list. Only those currencies that are defined as a supported currency in the PIM price field attribute configuration are mapped. in All available currencies are displayed in the list.

  [comment]: <> (Is that right? what currencies are mapped?)

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Destination gross*   
  Activate the toggle to map the gross price of the source attribute. Deactivate the toggle to map the net price.


## RMA-Extension ???

### Configuration


## RMAExtension PosId Extensions ???

### Configuration


## Simple-Pricing-To-Float

![Simple pricing to float](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/SimplePricingToFloat.png "[Simple pricing to float]")

This extension is used to map a simple price attribute to a number attribute. The simple price attribute is Actindo specific and therefore needs a special extension for mapping. As the simple price attribute is not often used, also this extension is rarely needed.  

### Configuration

- *Empty Value*
  Select what will be mapped to the destination attribute if the source attribute value is empty. The following options are available:
  - **null**: The destination attribute value is empty.
  - **0**: The destination attribute value is 0.

  [comment]: <> (Is that right?)


## Special price with default fallback

![Special price with default fallback](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/SpecialPriceWithDefaultFallback.png "[Special price with default fallback]")

This extension is used to map a PIM price field attribute with a fallback PIM price field attribute to a price attribute. The *Special Price* attribute is used for the promotion price. This attribute is always considered first when mapping. The *Fallback Price* attribute is used as a fallback price that will be mapped when no promotion price is available. The fallback price attribute is mandatory. This mapping is used when promotion prices and regular prices are maintained in different price field attributes. Further price settings are defined in the configuration.

### Configuration

- *Country*     
  Select the appropriate country in the drop-down list to apply the correct tax rate to the price. All available countries are displayed in the list.

- *Mapping mode*   
  Select the appropriate mapping mode for the source price attributes. The following modes are available:   
    - **Consider all prices**: All prices in the PIM price field attribute are mapped to the destination attribute.
    - **Consider only promotions**: Only the promotion prices in the PIM price field attribute are mapped to the destination attribute.
    - **Ignore promotions**: All prices beside the promotion prices in the PIM price field attribute are mapped to the destination attribute.



## Stock-To-Integer

![Stock to integer](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StockToInteger.png "[Stock to integer]")

This extension is used map a stock attribute to an integer attribute. The stock attribute is Actindo specific and therefore needs a special extension to map to an integer attribute. This extension is mainly used to map the stock from Actindo to another channel.  

### Configuration
This ETL extension has no further configuration settings.


## (String|Tree)-To-(String|Tree)

![String tree to string tree](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringTreeToStringTree.png "[String tree to string tree]")

This extension is used to either map a string to a tree node attribute or a tree node to string attribute. This extension is often used for csv imports where only data input as string data type is allowed but the data should result in a tree node data type.  

### Configuration

- *Separator*   
  Enter a separator sign by which a lower level in the string attribute is indicated. For instance, to indicate several gradations for a color (Red|Coral).

- *Destination Field*   
  Select the field of the tree node attribute whose value will be used for the mapping. The drop-down down list is only displayed when the destination attribute is a tree node attribute.
  - **Key**: The key value of the tree node attribute is used for the mapping.
  - **Title**: The title value of the tree node attribute is used for the mapping.


- *Relevant locale (applies for single language attributes)*   
  Select the language of the attribute value used for the mapping. This setting only applies to single language attributes. All active languages are displayed in the drop-down list.

  [comment]: <> (Anwendungsbeispiel? Verstehe den Einsatz nicht so richtig...)



## String and Value to Unit

![String and value to unit](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringValueToUnit.png "[String and value to unit]")

This extension is used to map two attributes including a unit and a unit value to a unit attribute. A unit attribute always includes a unit and a quantity. The unit to be mapped is defined in the *Unit* attribute, the quantity in the *Value* attribute.

### Configuration
This ETL extension has no further configuration settings.


## String Date Converter

![String date converter](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringDateConverter.png "[String date converter]")

This extension is used to map a string attribute containing a date to another string attribute containing a date. The source as well as the destination date format are defined in the configuration. Further, additional modifiers can be defined to change the date by a defined time value.

[comment]: <> (Is that right? destination = string)

### Configuration

- *Source Format*   
  Enter the source format of the date, for instance **Y-m-d**. The date must be entered in the php format, see https://www.php.net/manual/de/datetime.format.php.

- *Destination Format*   
  Enter the destination format of the date, for instance **Y-m-d**. The date must be entered in the php format, see https://www.php.net/manual/de/datetime.format.php.

- *Modifier 1*   
  Enter a value for the modifier to change the source date by a certain time value. For instance, enter **+ 7 days** to predate the date in the source attribute always by 7 days in the destination attribute. You can predate a date by using a plus sign, or backdate a date by using a minus sign.

  [comment]: <> (modifier format? ausgeschrieben oder abkürzungen wie in destination format feld? What format is taken if nothing is defined in the configuration?)

- ![Add](/Assets/Icons/Plus03.png "[Add]") (Add)   
  Click this button to add another modifier. You can add an unlimited number of modifiers.

  [comment]: <> (pro modifier nur ein wert ändern? oder warum brauche ich davon mehrere?)



## String to Image

![String to image](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringToImage.png "[String to image]")

This extension is used to map multiple string attributes to an image attribute. At least one string attribute containing an image must be selected for mapping and up to eight source attributes can be mapped. To each image you can define one or several tags.  Define the tags separator in the configuration.

[comment]: <> (Was wähle ich im  String attribut aus? die url vom Bild? oder wie wird das zu nem image attribut?)

### Configuration

- *Separator*   
  Enter a separator that is used between multiple image tags.
[comment]: <> (Separator correct?)


## String-Concat-To-String

![String concat to string](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringConcatToString.png "[String concat to string]")

This extension is used to map multiple string attributes to a single string attribute. This extension is often used in the receipt management, for instance to combine the receipt type and the number number, which are stored in different source attributes, in a single destination attribute. At least two source attributes must be selected and up to ten attributes can be selected. The source attribute values are written one after the other in the destination attribute without separation. Define a connector in the configuration.

### Configuration

- *Glue*   
  Enter a connector which is added before each source attribute value.

  [comment]: <> (Glue - warum wird das auch vors erste attribut geschrieben? Ist das nicht sinnfrei?)


## String-To-Absolute-Number

![String to absolute number](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringToAbsoluteNumber.png "[String to absolute number]")

This extension is used to map a string attribute to an integer attribute. The value is mapped unchanged, only the data type of the attribute changes. Only absolute numbers can be mapped to the destination attribute. To map deimal numbers, use the *String-To-Number* extension.

[comment]: <> (What happens if a string attribute contains a floating number? Is it rounded?)

### Configuration

- *separator*
  Select the appropriate separator for decimal numbers. The following signs are available:  
  - **,**: By default, the comma is used as a decimal separator in German.
  - **.**: By default, the point is used as a decimal separator in English.

  [comment]: <> (separator for absolute numbers? where is an absolute number separated?)

- *emptyString*
  Select what will be mapped to the destination attribute if the source attribute value is empty. The following options are available:
  - **leer**: The destination attribute value is empty.
  - **0**: The destination attribute value is 0.


## String-To-Boolean

![String to boolean](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringToBoolean.png "[String to boolean]")

This extension is used to map a string attribute to a boolean attribute. If the string attribute value equals 0, the false value is mapped to the boolean attribute. If the string attribute value equals 1, the true value is mapped to the boolean attribute.

### Configuration
This ETL extension has no further configuration settings.


## String-To-Country

![String to country](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringToCountry.png "[String to country]")

This extension is used to map a string attribute to a country attribute. This mapping is often used for the import. Define how the country is indicated in the configuration.

### Configuration
- *fieldToSearch*
  Select the appropriate information about how the country is entered in the source attribute, so that the system can map the country correctly to the destination attribute. The following options are available:
  - **Numerischer Ländercode**: Three-digit country code according to ISO 3166-1 numeric, for instance *840*.
  - **Dreibuchstabiger Ländercode**: Three-letter country code according to ISO 3166-1 alpha-3, for instance *USA*.
  - **Zweibuchstabiger Ländercode**: Two-letter country code according to ISO 3166-1 alpha-2, for instance *US*.
  - **Kfz Ländercode**: International vehicle registration code, for instance *USA*.
  - **Name**: Country name (in the national language), for instance *United States*.
  - **FusionMaps Ländercode**: ???

  [comment]: <> (Was ist FusionMaps?)


## String-To-Number

![String to number](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringToNumber.png "[String to number]")

This extension is used to map a string attribute to a floating point number attribute. The value is mapped unchanged, only the data type of the attribute changes. In contrast to the *String-To-Absolute-Number* extension, both, decimal and absolute numbers can be mapped to the destination attribute.

### Configuration

- *separator*
  Select the appropriate separator for decimal numbers. The following signs are available:  
  - **,**: By default, the comma is used as a decimal separator in German.
  - **.**: By default, the point is used as a decimal separator in English.

  - *emptyString*
    Select what will be mapped to the destination attribute if the source attribute value is empty. The following options are available:
    - **leer**: The destination attribute value is empty.
    - **0**: The destination attribute value is 0.


## Tax class and basic price to PIM price

### Configuration
This ETL extension has no further configuration settings.


## Tax class to Tax class

### Configuration
'This extensions cannot be configured'


## Tax zone to VAT id

### Configuration
This ETL extension has no further configuration settings.


## Text-To-UnitValue

### Configuration
This ETL extension has no further configuration settings.


## Tree and Number to base price

### Configuration
The configuration is depending on the selected source attributes:


## Tree node and basic price to PIM price

### Configuration
'Set a valid attribute for tax class to configure the mapping'


## Tree(Key)-To-String

![TreeKey to String](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/TreeKeyToString.png "[TreeKey to String]")

This extension is used to either map a tree node attribute to a string attribute. The key value of the source tree node attribute is mapped to the string destination attribute.

### Configuration

This ETL extension has no further configuration settings.


## Tree/String-to-Tax-Class

### Configuration
- Standardsatz:

- Ermäßigt:


## Tree-To-Boolean

### Configuration
This ETL extension has no further configuration settings.


## Tree-To-Float

### Configuration
This ETL extension has no further configuration settings.


## Tree-to-Tree

![Tree to tree](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/TreeToTree.png "[Tree to tree]")

This extension is used to map a tree node attribute to another tree node attribute. Further settings to the tree node are defined in the configuration.

### Configuration
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Create node if not existing*   
  Activate the toggle to automatically create a tree node in the destination attribute if no tree node exists. Otherwise, you have to manually create a tree node.

  [comment]: <> (is that right? or does the mapping fail then?)

- *Match destination node by*   
  Select the field of the tree node attribute whose value will be used for the mapping.
  - **Key**: The key value of the tree node attribute is used for the mapping.
  - **Title**: The title value of the tree node attribute is used for the mapping.


- *Relevant Language*   
  Select the language of the attribute value used for the mapping. All active languages are displayed in the drop-down list. The drop-down list is only displayed, when the **Title** option is selected in the *Match destination node by* drop-down list.


## Tree value mapping

![Tree value mapping](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/TreeValueMapping.png "[Tree value mapping]")

This extension is used to map a string attribute to a tree node attribute where the corresponding value of the string attribute must be accessed to map it to correctly the tree node attribute. For instance, this extension is often used to map the Actindo payment method from an order. All payment methods and their IDs are defined in the *Invoicing* module. These values must be accessed to map both, the payment methods and their IDs to the destination tree node attribute.

### Configuration
This ETL extension has no further configuration settings.


## UnitValue-To-Number

![Unit value to number](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/UnitValueToNumber.png "[Unit value to number]")

This extension is used to map an unit attribute to a number attribute. A unit attribute always includes a unit and a quantity. Only the quantity value is mapped to the destination attribute. To map the quantity value in the correct unit, the quantity is calculated into the unit of the destination attribute. Define the unit in the configuration.

[comment]: <> (Is that right? If not - how can a unit be mapped to a number attribute?)

### Configuration
- *Unit to convert to*   
  Select the appropriate unit of the destination attribute to calculate the quantity value into the correct unit. All units corresponding to the dimension of the source attribute are displayed in the drop-down list.


## UnitValue-To-Text

![Unit value to text](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/UnitValueToText.png "[Unit value to text]")

This extension is used to map an unit attribute to a string attribute. A unit attribute always includes a unit and a quantity. The settings how to display both values in the string attribute are defined in the configuration.

### Configuration
- *Mode*     
  Select the unit mapping mode. The following modes are available:
  - **Keep Unit**: The source unit is mapped to the destination attribute.
  - **Configured Unit**: The unit to be mapped to the destination attribute must be selected in the *Configured unit* drop-down list.
  - **Destination Unit**: The destination unit is kept in the destination attribute.

  [comment]: <> (Destination Unit -> error; Configured Unit -> not working and no drop-down list displayed; ergibt auch irgendwie beides keinen sinn, oder?)

- *Suffix Mode*   
  Select the suffix display mode for the unit. The following options are available:
  - **Suffix Symbol**: The unit is displayed by its symbol or abbreviation, for instance *cm*.
  - **Suffix Name**: The unit is displayed by its name, for instance *centimeter*.
  - **Suffix Empty**: The unit is hidden.


- *Separator*   
  Enter the separator sign placed between quantity and unit. If the field is left empty, the unit and quantity are written directly one after the other.

- *Decimal Separator*   
  Enter the decimal separator for the quantity value. If the number of decimal places is greater than 0, you should enter a separator sign to avoid that the value is displayed incorrectly. By default, the point is used as a decimal separator in English, the comma in German.

- *Decimal Places*   
  Enter the number of decimal places for the quantity value. This field is mandatory. Depending on the decimal places, the quantity is rounded.

  [comment]: <> (Verwirrend: warum wird bei der unitvalue-to-number erweiterung nur der mengenwert, bei der unitvalue-to-string erweiterung aber menge inklusive einheit übertragen?)


## UnitValue-To-UnitValue

![Unit value to unit value](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/UnitValueToUnitValue.png "[Unit value to unit value]")

This extension is used to map an unit attribute to a another unit attribute. A unit attribute always includes a unit and a quantity. Define in the configuration which of the units should be mapped in the destination attribute.

### Configuration

- *Choose the unit mapping mode*     
  Select the appropriate unit mapping mode. The following options are available:
  - **Keep Unit**: The source unit is mapped to the destination attribute.
  - **Configured Unit**: The unit to be mapped to the destination attribute must be selected in the *Configured unit* drop-down list.
  - **Destination Unit**: The destination unit is kept in the destination attribute.


- *Configured unit*    
  Select the unit that will be mapped in the destination unit. All units corresponding to the dimension of the destination attribute are displayed in the drop-down list. The drop-down list is only displayed when the  **Configured Unit** option is selected in the *Choose the unit mapping mode* drop-down list.


## Variant-To-String

![Variant to string](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/VariantToString.png "[Variant to string]")

This extension is used to map a variant attribute to a string attribute, for instance to provide the product information. The values of the defining attributes of a variant are mapped to the destination attribute. Define if certain attributes should be excluded and if the attribute names should be included in the configuration.

### Configuration

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Include attribute name*     
  Activate the toggle to map both, the attribute names and their values. Deactivate the toggle to map the attribute values only.

- *Excluded Attribute Keys*  
  Enter the attribute keys of those attributes that should not be mapped to the destination attribute.

- *Language for values from a tree node*   
  Select the language of the source attribute value used for the mapping. This setting only applies to values from a tree node. All active languages are displayed in the drop-down list.

[comment]: <> (when is the language setting displayed?)


## Variant-Value-To-Master-Sku ???

### Configuration
This ETL extension has no further configuration settings.


## Variante auf Variante (Variant to variant)

![Variant to variant](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/VariantToVariant.png "[Variant to variant]")

This extension is used to map a variant attribute to a variant attribute. The variant mapping is used to define the handling of product variants in relation to their master product. The settings about the variant handling are defined in the configuration.

### Configuration
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically generate all child entities when main entity is created*   
  All variants to a master product are automatically created in the destination when the master product is created. This toggle is read-only.

  [comment]: <> (Welchen Sinn ergibt ein Toggle, der nicht umgeschaltet werden kann?)

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically map variant sets*   
  Activate the toggle to automatically map the assigned variant sets of the source variant attribute and the destination variant attribute. It is recommended to Activate the toggle. Otherwise, the variant sets must be mapped manually. By default, the toggle is active.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically create variant set if no suiting variant set can be found*   
  Activate the toggle to automatically create a variant set if the assigned variant sets of the source variant attribute and the destination variant attribute do not match. It is recommended to Activate the toggle. Otherwise, the variant set must be created manually. By default, the toggle is active. This toggle is only displayed when the *Automatically map variant sets* toggle is active.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically add not mapped defining attributes to destination set when creating variant set*   
  Activate the toggle to automatically add unmapped defining attributes to the created destination variant set. It is recommended to Activate the toggle. Otherwise, the defining attributes must be added manually to the attribute set. By default, the toggle is active. This toggle is only displayed when the *Automatically map variant sets* toggle is active.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Sync variant set in case they do not match to each other*   
  Activate the toggle to sync the source variant set and the destination variant set if they do not match. By default, the toggle is inactive. This toggle is only displayed when the *Automatically map variant sets* toggle is inactive.

  [comment]: <> (Verstehe ich nicht, was diese Option macht...)

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Do not apply master product status to children*      
  Activate the toggle to manage the status of all variants independently of their master product. Otherwise, the status of the main product is automatically applied to all variants in the destination attribute. By default, the toggle is inactive.



-------

wie wird eine Info zu einem Zielattribut übertragen

Datentyp Zielattribut definiert Auswahl der Mappings

Kombi aus Datentyp und Mapping definiert Auswahl des Quellattributs
