# ETL extensions list

The ETL (Extract Transform Load) is used to extract data from a certain source, transform it in a specific way and load it into a defined destination. In the *DataHub* module, the attribute sets are mapped via ETL. The attributes of the source attribute set are mapped to the attributes of the destination attribute set.   
The ETL extensions are used to define how the data is transformed from the source attribute to the destination attribute. The ETL extensions provided for a mapping differ depending on the destination attribute. The data type of the destination attribute determines the available ETL extensions. The selected extension, in turn, determines the available source attributes by defining the data type of the source attribute. In addition, further settings can be defined for some ETL extensions.    
The list below describes in detail all available ETL extensions and, if available, their specific configurations.


## Add prefix/suffix -



### Configuration
- Prefix
- Suffix


## Arithmetic Extension -

### Configuration
- Equation 1
- Equation x (possible to add modifiers)


## Basic Mapping -
The basic mapping adopts the value from the source attribute to the destination attribute without any change.

Example:
- Source attribute: String with the value **abc**
- Destination attribute: String with the value **abc**

### Configuration
This ETL extension has no further configuration settings.

-> 1 zu 1 Übertragung; keine Transformation


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



## Cloudinary-to-String -

Nintendo spezifisch



## Constant value

![Constant value](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/ConstantValue.png "[Constant value]")

This extension is used to map a constant value to a random destination attribute. The fixed source value is defined in the configurations and never changes. This extension is often used according to receipts, for instance to define the receipt type.

[comment]: <> (Is that right? random destination attribute? or only string?)

### Configuration
- *Destination attribute name*   
   Enter a value that is always mapped to the destination attribute.


## Copy packaging units

### Configuration
This ETL extension has no further configuration settings.


## Country-To-X -

### Configuration
This ETL extension has no further configuration settings.


## Date Converter

![Date Converter](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/DateConverter.png "[Date Converter]")

This extension is used to map a date attribute to another date attribute of a different format or to a string attribute. The destination date format is defined in the configuration. Further, modifiers can be defined to change the date by a defined time value.

[comment]: <> (Is that right? destination = string or date?)

### Configuration
- *Destination Format*   
  Enter the destination format of the date, for instance **Y-m-d**. The date must be entered in the php format, see https://www.php.net/manual/de/datetime.format.php.

- *Modifier 1*   
  Enter a value for the modifier to change the source date by a certain time value. For instance, enter **+ 7 days** to predate the date in the source attribute always by 7 days in the destination attribute. You can predate a date by using a plus sign, or backdate a date by using a minus sign.

  [comment]: <> (modifier format? ausgeschrieben oder abkürzungen wie in destination format feld?)

- ![Add](/Assets/Icons/Plus03.png "[Add]") (Add)   
  Click this button to add another modifier. You can add an unlimited number of modifiers.

  [comment]: <> (pro modifier nur ein wert ändern? oder warum brauche ich davon mehrere?)


## EAN zu Artikelnummer ???


## Entity Id to Generic Property Extension -

### Configuration
- *Empty drop-down list*
  - Beleg
  - Beleg-Position
  - Kunde


- Field Name


## ETLPIMToUCSBundleExtension

### Configuration
This ETL extension has no further configuration settings.



## Html-Template -

### Configuration

- *Html-Template*

-> plugin installieren!


## Identity-Mapping

### Configuration

This ETL extension has no further configuration settings.



## Image-To-Download-Link -

### Configuration
- Enter the image number
- Enter image validity (days)
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Is the image downloadable only once?


## Image-To-ImageTags -

### Configuration
- Enter the image number


## Import special price

### Configuration
This ETL extension has no further configuration settings.


## Language-To-X -

### Configuration
- languageValue:
  - 3 digit code
  - 2 digit code
  - Name (english)
  - Name (french)
  - Name (german)


## Mapping Table -

### Configuration

| Source Value   | Destination Value     |
|----------------|-----------------------|
|to be completed |  to be completed      |

possible to add more source values


## Mysql query -

### Configuration

-> sehr neu


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

nimm wert x0 - wenn nicht gefüllt, nimm wert x1 etc.

### Configuration

- Relevant Language



## Number-To-String

![Number to String](/Assets/Screenshots/DataHub/Settings/ETL/Extensions/NumberToString.png "[Number to String]")

This extension is used to map a number attribute to a string attribute.

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


## Pricing to float -

### Configuration
- Country: dropdown with all available countries
- Currency: dropdown with all available currencies
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Destination gross


## Pricing to float with fallback price

### Configuration
- Country: dropdown with all available countries
- Currency: dropdown with all available currencies
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Destination gross


## RMA-Extension ???


## RMAExtension PosId Extensions ???



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
This extension is often used for csv-imports where only data input as string data type is allowed but the data should result in a tree node data type.  

### Configuration

- *Separator*   
  Enter a separator sign by which a lower level in the string attribute is indicated. For instance, to indicate several gradations for a color (Red|Coral).

- *Destination Field*   
  Select the field of the tree node attribute whose value will be used for the mapping. The drop-down down list is only displayed when the destination attribute is a tree node attribute.
  - **Key**: The key value of the tree node attribute is used for the mapping.
  - **Title**: The title value of the tree node attribute is used for the mapping.


- *Relevant locale (applies for single language attributes)*   
  Select the language of the attribute whose value will be used for the mapping. This setting only applies to single language attributes.

  [comment]: <> (Anwendungsbeispiel? Verstehe den Einsatz nicht so richtig...)



## String and Value to Unit

### Configuration
This ETL extension has no further configuration settings.


## String Date Converter -

### Configuration
- Destination Format
- Modifier 1
- Modifier x (possible to add modifiers)


## String to Image

### Configuration
This ETL extension has no further configuration settings.


## String-Concat-To-String -

### Configuration
- Glue


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


- *Separator*
- *Decimal Separator*
- *Decimal Places*


## UnitValue-To-UnitValue

### Configuration
- Choose the unit mapping mode:
  - Keep Unit  
  - Configured Unit
  - Destination Unit

- Configured unit (if option **Configured Unit** is selected): dropdown with all available units


## Variant-To-String -

### Configuration
![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Include attribute name

-> Produktinformationen übergeben


## Variant-Value-To-Master-Sku ???

### Configuration
This ETL extension has no further configuration settings.


## Variante auf Variante (Variant to variant) -

### Configuration
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Automatically generate all child entities when main entity is created
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Automatically map variant sets
- Source variant sets (when toggle *Automatically map variant sets* is inactive): dropdown of all available variant sets.
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Automatically create variant set if no suiting variant set can be found
- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") Automatically add not mapped defining attributes to destination set when creating variant set


-------

wie wird eine Info zu einem Zielattribut übertragen

Datentyp Zielattribut definiert Auswahl der Mappings

Kombi aus Datentyp und Mapping definiert Auswahl des Quellattributs
