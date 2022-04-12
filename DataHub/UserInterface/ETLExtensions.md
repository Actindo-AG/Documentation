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


## Catalog Tree to Tree value mapping -

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


## Import from cloudinary folder
destination attribute: Cloudinary images

### Configuration

- *Folder*


## Import special price

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
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Destination gross


## Next special base price to date time

### Configuration
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Get from date
- Currency: dropdown witth all available currencies


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

### Configuration
- SourceUnit: dropdown with all available units
- Mode destination unit:
  - Configure manually
  - Keep unit
  - Default unit of destination attribute


- Unit to convert to (if option **Configure manually** is selected): drop-down with all configured units.


## PIM BasePrice to Amount (VPE Value)

### Configuration
This ETL extension has no further configuration settings.


## PIM BasePrice to Boolean (VPE Active)

### Configuration
This ETL extension has no further configuration settings.


## PIM BasePrice to Unit -

### Configuration
This ETL extension has no further configuration settings.


## PIM BasePrice to VPE Reference Unit

### Configuration
This ETL extension has no further configuration settings.


## Preg Replace Extension

### Configuration
- Pattern
- Replacement


## PriceBuilder

### Configuration
This ETL extension has no further configuration settings.


## Price to price with discount

### Configuration
This ETL extension has no further configuration settings.


## Price to Tax

### Configuration
- Country: dropdown with all available countries
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") In percent


## Price to Tax Class -

### Configuration
This ETL extension has no further configuration settings.


## Pricing to float

![Pricing to float](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/PricingToFloat.png "[Pricing to float]")

This extension is used to map a price field attribute to a string attribute. A discount to the price can be entered in the *Discount in percent* drop-down list. Further price settings are defined in the configuration.

### Configuration

- *Country*     
  Select the appropriate country in the drop-down list to apply the correct tax rate to the price. All available countries are displayed in the list.

- *Currency*   
  Select the appropriate currency in the drop-down list. Only those currencies that are defined as a supported currency in the price attribute configuration are mapped. in All available currencies are displayed in the list.

  [comment]: <> (Is that right? what currencies are mapped?)

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Destination gross*   
  Activate the toggle to map the gross price of the source attribute. Deactivate the toggle to map the net price.


## Pricing to float with fallback price

### Configuration

- *Country*     
  Select the appropriate country in the drop-down list to apply the correct tax rate to the price. All available countries are displayed in the list.

- *Currency*   
  Select the appropriate currency in the drop-down list. Only those currencies that are defined as a supported currency in the price attribute configuration are mapped. in All available currencies are displayed in the list.

  [comment]: <> (Is that right? what currencies are mapped?)

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Destination gross*   
  Activate the toggle to map the gross price of the source attribute. Deactivate the toggle to map the net price.


## RMA-Extension ???

### Configuration


## RMAExtension PosId Extensions ???

### Configuration


## Simple-Pricing-To-Float

### Configuration
- Empty Value:
  - null
  - 0


## Special price with default fallback

### Configuration
This ETL extension has no further configuration settings.


## Stock-To-Integer

### Configuration
This ETL extension has no further configuration settings.


## (String|Tree)-To-(String|Tree)

![StringTree to StringTree](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringTreeToStringTree.png "[StringTree to StringTree]")

This extension is used to either map a string to a tree node attribute or a tree node to string attribute.
This extension is often used for csv imports where only data input as string data type is allowed but the data should result in a tree node data type.  

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

### Configuration
This ETL extension has no further configuration settings.


## String Date Converter

This extension is used to map a string attribute containing a date to another string attribute or a date attribute. The source as well as the destination date format are defined in the configuration. Further, additional modifiers can be defined to change the date by a defined time value.

[comment]: <> (Is that right? destination = string or date?)

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



### Configuration
- Destination Format
- Modifier 1
- Modifier x (possible to add modifiers)


## String to Image

### Configuration
This ETL extension has no further configuration settings.


## String-Concat-To-String

![String concat to string](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/StringConcatToString.png "[String concat to string]")

This extension is used to map multiple string attributes to a single string attribute. This extension is often used in the receipt management, for instance to combine the receipt type and the number number, which are stored in different source attributes, in a single destination attribute. At least two source attributes must be selected and up to ten attributes can be selected. The source attribute values are written one after the other in the destination attribute without separation. Define a connector in the configuration.

### Configuration

- *Glue*   
  Enter a connector which is added before each source attribute value.

  [comment]: <> (Glue - warum wird das auch vors erste attribut geschrieben? Ist das nicht sinnfrei?)


## String-To-Absolute-Number

### Configuration
- separator:
  - ,
  - .


- emptyString:
  - leer
  - 0


## String-To-Boolean

### Configuration
This ETL extension has no further configuration settings.


## String-To-Country

### Configuration
- fieldToSearch:
  - Numerischer Ländercode
  - Dreibuchstabiger Ländercode
  - Zweibuchstabiger Ländercode
  - Kfz Ländercode
  - Name
  - FusionMaps Ländercode


## String-To-Number

### Configuration
- separator:
  - ,
  - .


- emptyString:
  - leer
  - 0


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


## Tree-to-Tree -

### Configuration
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Create node if not existing
- Match destination node by:
  - Key
  - Title



## Tree value mapping -

### Configuration
This ETL extension has no further configuration settings.


## UnitValue-To-Number -


### Configuration
- Unit to convert to: drop-down with the unit values of the selected source attribute


## UnitValue-To-Text

![UnitValue to text](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/UnitValueToText.png "[UnitValue to text]")

This extension is used to map an unit attribute to a string attribute. A unit attribute always includes a dimension and a unit, for instance, the dimension *Length* and the unit *m*.

### Configuration
- *Mode*    

  - **Keep Unit**
  - **Configured Unit**
  - **Destination Unit**


- *Suffix Mode*

  - **Suffix Symbol**
  - **Suffix Name**
  - **Suffix Empty**


- *Separator* zwischen Zahl und Einheit
- *Decimal Separator*
- *Decimal Places*


## UnitValue-To-UnitValue

### Configuration
- Choose the unit mapping mode:
  - Keep Unit  
  - Configured Unit
  - Destination Unit

- Configured unit (if option **Configured Unit** is selected): dropdown with all available units


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

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Status des Hauptartikels nicht auf Kindartikel übertragen*      
  Activate the toggle to apply the status of the main product to all variants in the destination attribute. Deactivate the toggle to manage the status of all variants independently of their master product. By default, the toggle is inactive.


  [comment]: <> (Existiert der letzte Toggle noch?)


-------

wie wird eine Info zu einem Zielattribut übertragen

Datentyp Zielattribut definiert Auswahl der Mappings

Kombi aus Datentyp und Mapping definiert Auswahl des Quellattributs
