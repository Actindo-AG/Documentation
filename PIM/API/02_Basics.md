[!!DataHub Basics](../../DataHub/Overview/04_Basics.md)
[!!Data types](../../DataHub/UserInterface/04_DataTypeList.md)


# Basics on Actindo Core1 OpenAPI

To be able to communicate via API with the *Actindo Core1 Platform*, you need to have a clear overview of the data structure that lies behind it.

For an overview of the Actindo data model, see [Data model](../../DataHub/Overview/04_Basics.md).


## Attributes

- Attribute
    - Managed in DataHub
    - Attribute structure
    - Data types
    - ID
        - via UI
        - via API

An attribute defines a characteristic to describe a product. All attributes are created and maintained in the *DataHub* module. Therefore, all attributes available in the system are displayed in *DataHub*. Besides, product-specific attributes can be created and maintained in the *PIM* module. If you install additional plugins to communicate with third-party systems, such as external sales channels or service providers, other attributes may be created via driver.

All attributes have a key. This key is required for API access and therefore must be system wide unique. 

You can define your own attribute keys, but we strongly recommend that you follow consistent naming conventions for the sake of clarity, such as follows: 

**plugin_attribute short name__scope__language**

| Key part  | Meaning  |
| --------- | -------- |
| Plugin    | Plugin or module where the attribute originates from. |
| Scope     | For multi-scope attributes, key of scope in which the attribute is used. | 
| Language | For multi-language attributes, code of the language in which te attribute is maintained. |

The following examples are based on predefined *PIM* attributes. If you have created your own attributes in your system, the names and keys may differ.

| Attribute      | Attribute key |
|----------------|---------------|
| Product name   | pim_art_name |
| Product name | pim_art_name__actindo_basic__en_US |
| Product name | pim_art_name__actindo_basic__de_DE |
| EAN code       | pim_ean      |
| Product description | pim_products_description |
| Price          | pim_price  |   

An example data structure an attribute is displayed in the following graphic:

![Attribute](../../Assets/Screenshots/PIM/API/Attributes.png "[Attribute]")

Depending on the nature of your products, you will need to create different attributes. For example, if you are selling clothes, you will need to define the material, type of fit or the collar size (example attribute keys: pim_material, pim_fit, pim_collar_size). However, if you sell smartphones, you need to specify the storage, the screen size, or the case color (example attribute keys: pim_storage, pim_screen_size, pim_case_color). 

Some attributes apply to all products, as every product needs to have a name, an EAN or SKU code, or a product description. These common attributes are included in the so-called *PIM basic set* in the *PIM* module. Product-specific attributes, however, are include in a other additional sets. For detailed information on attribute sets, see [Attribute sets](#attribute-sets).

You can create you own attributes in your Core1 system via the user interface. For detailed information on how to create an attribute, see [Create an attribute](../../DataHub/Integration/01_ManageAttributes.md#create-an-attribute).



## Attribute sets

- Attribute set
    - Managed in DataHub
    - Assign/add attribute to a set
    - Mapping
    - ID
        - via UI
        - via API

![Attribute sets](../../Assets/Screenshots/PIM/API/AttributeSets_ActindoColors.png "[Attribute sets]")

Attributes are collected in so-called *Attribute sets*. An attribute set includes therefore a number of attributes that define an entity type, for example, a specific type of product in the case of the *PIM* module. 

All attribute sets have a key. This key is required for API access and therefore must be system wide unique. 

You can define your own attribute key sets, but we strongly recommend that you follow consistent naming conventions for the sake of clarity, such as follows: 

**plugin_attribute set short name**

| Key part  | Meaning  |
| --------- | -------- |
| Plugin    | Plugin or module where the attribute originates from. |

The following examples are based on predefined *PIM* attributes. If you have created your own attributes in your system, the names and keys may differ.

| Attribute set      | Attribute set key |
|--------------------|-------------------|
| PIM basic set      | pim_basic_set    |
| PIM electronics    | pim_electronics  |

You can create you own attribute sets in your Core1 system via the user interface. For detailed information on how to create an attribute set, see [Create an attribute set](../../DataHub/Integration/01_ManageAttributeSets.md#create-an-attribute-set).


Define concepts 
- entity
- inheritance



## Variant  
    - Managed in PIM

## Variant set




## Inheritance

## Data types  

For detailed information on the different data types available in the *DataHub* module, see [Data type list](../../DataHub/UserInterface/04_DataTypeList.md).


Further information:

[Assign an attribute to an attribute set](../../DataHub/Integration/02_ManageAttributeSets.md#add-an-attribute-to-the-set). 

## Required attributes  

Attributes can be required or optional. Required attributes must always be provided when sending a request

## Format  

The *Actindo Core1 OpenAPI* endpoints accept requests in JSON format. 

