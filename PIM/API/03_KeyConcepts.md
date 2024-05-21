[!!DataHub Basics](../../DataHub/Overview/04_Basics.md)
[!!Data types](../../DataHub/UserInterface/04_DataTypeList.md)

# Key concepts

To be able to communicate via API with the *Actindo Core1 Platform*, you need to have a clear overview of the data structure that lies behind it.

For an overview of the Actindo data model, see [Data model](../../DataHub/Overview/04_Basics.md) in the *DataHub* documentation.



## Attributes

An attribute defines a characteristic to describe an entity, for example, a product in the case of the *PIM* module. All attributes can be created and maintained in the *DataHub* module. Therefore, all attributes available in the system are displayed in *DataHub*. Besides, some entity-specific attributes, such as product-related attributes or offer-related attributes, can be created and maintained in the corresponding module, that is, in *PIM* or *Omni-Channel* respectively. If you install additional plugins to communicate with third-party systems, such as external sales channels or service providers, other attributes may be created via driver.

All attributes have a key. This key is required for API access and therefore must be system-wide unique. 

You can define your own attribute keys, but we strongly recommend that you follow consistent naming conventions for the sake of clarity, such as follows: 

**_plugin_attribute_short_name__scope__language**

| Key | Meaning |
| :------- | :------- |
| **Plugin** | Plugin or module where the attribute originates from. If an attribute originates in the *PIM* module, its key should start with *_pim*. |
| **Attribute short name** | Any descriptive name you want to give to an attribute, such as *attributeSetId* or *art_name*. No spaces are allowed here, therefore you have to write the attribute name in one word or join the different parts with a **single** underscore. |
| **Scope** | For multi-scope attributes, key of the scope in which the attribute is used. You can use an attribute, e.g. *_pim_products_description*, in different scopes, for instance, in your web shop and in a reseller platform, such as Amazon. This way, your product description can be different in your web shop and in the reseller platform. In this case, the attribute is multi-scope and must be accordingly defined in its key. Note that the scope is separated with a **double** underscore in the attribute key. The attribute key would therefore be *_pim_products_description__webshop* and *_pim_products_description__reseller_platform*. For detailed information, see [Configure the scopes settings](../Integration/05_ConfigureChannels.md) and [Manage the scopes in DataHub](../../DataHub/Integration/04_ManageChannels.md). |
| **Language** | For multi-language attributes, key of the language (ISO language code) in which the attribute is maintained. You can maintain an attribute, e.g. *_pim_products_description* in different languages, for instance, in English (United States) and in German (Germany). In this case, the attribute is multi-language and must be accordingly defined in its key. The attribute key would therefore be *_pim_products_description__en-US* and *_pim_products_description__de-DE*. Note that the language is separated with a **double** underscore in the attribute key. For detailed information, see [Configure the language settings](../Integration/05_ConfigureLanguages.md) and [Manage the languages in DataHub](../../DataHub/Integration/04_ManageChannels.md). |

Depending on the nature of your products, you will need to create different attributes. For example, if you are selling shirts, you will need to define the material, type of fit or the collar size (example attribute keys: *_pim_material*, *_pim_fit*, *_pim_collar_size*). However, if you sell smartphones, you need to specify the storage, the screen size, or the case color (example attribute keys: *_pim_storage*, *_pim_screen_size*, *_pim_case_color*). 

Some attributes apply to all products, as every product needs to have a name, a price, an applicable tax class, and a description. These common attributes are included by default in the so-called *PIM basic set* in the *PIM* module. Product-specific attributes, however, need to be included additionally in other sets. For detailed information on attribute sets, see [Attribute sets](#attribute-sets).

Every attribute has a defined data type, which determines the type of value the attribute may contain, for example, a series of characters (data type: string) or a whole number (data type: integer). For detailed information about the data types, see [Data type list](../../DataHub/UserInterface/04_DataTypeList.md).

You can create your own attributes in your instance via user interface, as well as edit or deactivate existing attributes. For detailed information, see [Manage the attributes](../../DataHub/Integration/01_ManageAttributes.md) in the *DataHub* documentation.


The following examples are based on predefined *PIM* attributes. If you have created your own attributes in your system, the names and keys may differ.

| Attribute        | Attribute key               | Data type |
|------------------|-----------------------------|-----------|
| Name             | *_pim_art_name*             | string    |
| Price                                             | *_pim_price*                                        | PIM price field   |
| Tax class                                         | *_taxes_tax_class*                                  | taxclass |
| Product description                               | *_pim_products_description*                         | textfield    |
| Product description (multi-scope, multi-language) | *_pim_products_description__scope__language_code*   | textfield    |


[comment]: <> (Frage: Tax class can be data type "tax class" and "tree node", i.e. Standard, ermäßigt. Was ist data type taxclass? Wieso ist es nicht zu finden in API products? Owning module ist Taxes? Ähnlich wie pim_price and PIM price field data type. Warum nicht data type number?)

The following graphic visualizes a series of attributes, within an attribute set, maintained in different scopes and languages, and how these attributes define a specific product: 

![Attribute](../../Assets/Screenshots/PIM/API/Attribute.png "[Attribute]")



## Attribute sets

An attribute set includes a number of attributes that define an entity type, for example, a specific type of product in the case of the *PIM* module. All attribute sets can be created and maintained in the *DataHub* module. Therefore, all attribute sets available in the system are displayed in *DataHub*. Besides, some entity-specific attribute sets, such as a product-related attribute sets or offer-related attribute sets, can be created and maintained in the corresponding module, that is, in *PIM* or *Omni-Channel* respectively. If you install additional plugins to communicate with third-party systems, such as external sales channels or service providers, other attribute sets may be created via driver.

All attribute sets have a key. This key is required for API access and therefore must be system-wide unique. 

You can define your own attribute set keys, but we strongly recommend that you follow consistent naming conventions for the sake of clarity, such as follows: 

**_plugin_attribute_set_short_name**


| Key | Meaning |
| :------- | :------- |
| **Plugin** | Plugin or module where the attribute originates from. If an attribute set originates in the *PIM* module, its key should start with *_pim*. |
| **Attribute set short name** | Any descriptive name you want to give to an attribute set, such as *electronics*, *trousers*, or *notebooks*. No spaces are allowed here, therefore you have to write the attribute name in one word or join the different parts with an underscore. |

The following examples are based on predefined *PIM* attribute sets. If you have created your own attributes sets in your system, the names and keys may differ.

| Attribute set      | Attribute set key   |
|--------------------|---------------------|
| PIM basic set      | *_pim_base_set*     |
| PIM electronics    | *_pim_electronics*  |
| PIM shirts         | *_pim_shirts*       |

Apart from the *PIM basic set*, you can create other sets to define other types of products, such as shirts or notebooks. These product-specific attribute sets will usually be based on the *PIM basic set*, that is, will inherit the attributes included in it, and contain additional attributes needed to define the specific product type, such as a piece of clothing or a computer.  

You can create your own attribute sets in your instance via user interface, as well as edit or deactivate existing attribute sets. For detailed information, see [Manage the attribute sets](../../DataHub/Integration/02_ManageAttributeSets.md) in the *DataHub* documentation.


The following graphic visualizes the attribute set structure and the inheritance principle, and how the attributes in different attribute sets define different types of products:

![Attribute set](../../Assets/Screenshots/PIM/API/AttributeSet.png "[Attribute set]")



## Master and variant products 

In the *PIM* module, you can create three sort of products:

- *Single product*: A standalone product with no variations to it, for example, a computer game. 
- *Master product*: A product that has variations to it, for example, a shirt, which has different options in size and color. A master product is the "parent" entity to a family of products.
- *Variant product*: A product with a special characteristic that differentiates it from other products of the same type, for example, color or size. A shirt, for instance, is usually sold in different colors. A blue shirt and a red shirt are variant products of a shirt master product, which is just an abstract definition of the shirt product type. 

All thee sort of products are created and managed in the *PIM* module. You can create single products, with no variations, and master products with their corresponding variants. To be able to create variant products to a master product, you have to create a so-called variant set first to determine the attributes that will define the variant product. For detailed information, see [Variant sets](#variant-sets).

You can create any number of variant products in your instance via user interface, as well as edit existing variant products. For detailed information, see [Manage the variants](../Operation/02_ManageVariants.md).

The following graphic visualizes a series of attributes, within an attribute set and a variant set, maintained in different scopes and languages, and how these attributes define specific variants: 

![Variant](../../Assets/Screenshots/PIM/API/Variant.png "[Variant]")



## Variant sets

A variant set includes the attributes needed to define a variant product. A variant set must be therefore assigned to an attribute set, that is, to the type of product to which you want to create the variants. For example, if you want to create color variants for the product "shirt", you have to create the variant set *Color* containing the defining attribute *_pim_color* and assign it to the attribute set *_pim_shirts*. 

Like the variant products, variant sets are created and managed in the *PIM* module. You can create variant sets for a product type in your instance via user interface, as well as edit existing variant sets. For detailed information, see [Manage the variant sets](../Integration/07_ManageVariantSets.md).

The following graphic visualizes the attribute and variant set structure, the inheritance principle, and how the attribute set and variant set attributes define a specific product:

![Variant set](../../Assets/Screenshots/PIM/API/VariantSet.png "[Variant set]")



## Entities

An entity is an object containing data, for instance, a *PIM* product, an *Omni-Channel* offer, a *DataHub* attribute, or an attribute set. Every entity has a unique ID, which is automatically assigned by the system for internal purposes. When accessing the system via API, you need the entity ID of all the fields that are required in your request for the system to be able to recognize the entity. 

You can find out the ID via user interface or via API:

- To find out the entity via user interface, see [Discover an entity ID via user interface](./04_RetrieveEntityData.md#discover-an-entity-id-via-user-interface).  
- To find out the entity ID, and other entity information, via API, see [Discover an entity ID via API](./04_RetrieveEntityData.md#discover-an-entity-id-via-api).



## Mapping

To be able to exchange data among the different entity types in your system, you need to map the different entities. This way, you can convert the data contained in an entity to make it available to another entity.

For instance, you can use a *PIM* product to create an *Omni-Channel* offer and export it subsequently into all your sales channels. The data structure in the different sales channels will most surely differ. This data structure conversion can be managed through the so-called *ETL* function. For detailed information, see [DataHub ETL process](../../DataHub/Overview/04_Basics.md#etl-process) and [Manage the ETL mappings](../../DataHub/Operation/01_ManageETLMappings.md).