# Products

You can manage your products via API. You can create, edit, delete, both permanently and temporary, and list *PIM* products. 

Keys are customer-defined. Therefore, the fields displayed in the following request samples should just serve as an example. You have to include all required fields in your request and provide them with a value. Any ID values you need, for example, the **attributeSetId**, must be an existing value in the *DataHub* module.  

You can find out an entity ID via user interface or via API, see [Entity data](./04_EntityData.md).

Depending on the data you want to specify, you have to add the corresponding field to your request. For a complete list of the attributes included in the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute sets*. Alternatively, you can find a list of all existing PIM attributes under *DataHub > Settings > Attributes*.

If necessary, you can get a list of all attributes you have created in the *DataHub* module, both in the user interface and via API. To obtain a list in the user interface, go to *DataHub > Attributes* and filter the attribute list by any criteria you wish, e.g. by attribute name starting with *"pim_"*. To get a list of all pim attributes via API, see [List the attributes in an attribute set](./04_EntityData.md#list-the-attributes-in-an-attribute-set).

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).

> [Caution] In the latest version of the *DataHub* and *PIM* modules, it is possible to modify the attribute key. However, this is strongly discouraged and has far-reaching consequences. If you modify a key in the *DataHub* or *PIM* modules, the key in the API changes as well. This means that you also have to update the key, that is, the field, in your request body. Otherwise, the field will not be found when sending a request. 



## The product object

Products represent the goods and services you offer to your customer. They are defined through a set of attributes. 

The following table displays a list of all attributes contained in the *PIM basic set* (_pim_attribute_name) with their default data types and configuration. Additional fields, such as created and modified, are set by default in all entities and can be used to set filters. The required fields are marked in bold. 

| Attribute   | Data type   | Description | Comments |
| ----------- | ----------- | ----------- | -------- | 
| **sku**      | string   |  Product SKU |          |
| **attributeSetId**   | integer  | Attribute set identification number | |
| created	 | string | Date and time of creation | Format: YYYY-MM-DD HH:MM:SS |
| createdBy | integer | User ID |  To find a user ID, go to *Settings > Users and groups > User management*. |
| modified	| string | Date and time of last modification | Format: YYYY-MM-DD HH:MM:SS |
| modifiedBy |integer | User ID | To find a user ID, go to *Settings > Users and groups > User management*. |
| attributeSet | object | Product attribute set | It contains the required field **id**. |
| variantStatus | string | Product status | It indicates whether a product is a *single*, *master* or a *variant*. This field is updated automatically when a variant is added to a master product, that is, it cannot be manually updated. |
| _pim_variants | object | It defines variant product(s) to a master product. | It contains the following fields: <br> **variantSetId** (integer), isMasterEntity (true/false), **masterId** (integer) and the object **definingValues**. The object **definingValues** is an array of objects, where at least an **attributeName** and a **value** must be defined. |
| _pim_art_name | string | Product name | |
| _pim_art_name__scope__language | string | Product name in a specific scope and language | If attribute is multi-scope and multi-language |
| _pim_catalog | string / object ? | Product categories | It contains the required field **id**. <!-- Frage: In Payload nur string, in product object Tabelle Any of...? --> |
| _pim_long_text | string | Product long name | |
| _pim_long_text__language | string | Product long name in a specific language | If attribute is multi-language |
| _pim_ean | string | Product EAN code | |
| _pim_customs_number | string | Customs tariff number | |
| _pim_origin | object / Country ? | Country of origin | It contains the required field **code3digit**. <br> Country code format: ISO 3166-A3, e.g. DEU for Germany. |
| _pim_valid_until | string | Expiration date | Format: YYYY-MM-DD HH:MM:SS |
| _pim_is_sale | boolean | The product is a sale item. | Options are *true* or *false*. |
| _pim_fsk18 | boolean | Suitable for persons above 18 | Options are *true* or *false*. |
| _pim_product_digital | boolean | The product is a digital item. | Options are *true* or *false*. |
| _pim_stock_value | number | Stock level in warehouse | |
| _pim_salesunit | object | Product sale unit | It contains the required fields **unitId** and **dimensionId**. | |
| _pim_size_l | object | Product length | It contains the required fields **value** and **unitId**. | |
| _pim_size_b | object | Product width | It contains the required fields **value** and **unitId**. | |
| _pim_size_h | object | Product depth | It contains the required fields **value** and **unitId**. | |
| _pim_weight | object | Product weight | It contains the required fields **value** and **unitId**. | |
| _pim_price | string | Product price | |
| _pim_baseprice | object | Price per unit | It contains the required fields **amount**, **unitId** and **dimensionId**. |
| _pim_products_url | string | Supplier link | |
| _pim_products_keywords | string | Additional terms for search | |
| _pim_products_keywords__scope__language | string | Additional terms for search in a specific scope and language | If attribute is multi-scope and multi-language |
| _pim_products_tags | string | Product tags | |
| _pim_products_tags__scope__language | string | Product tags in a specific scope and language | If attribute is multi-scope and multi-language | 
| _pim_products_meta_title | string | Meta title | |
| _pim_products_meta_title__scope__language | string | Meta title in a specific scope and language | If attribute is multi-scope and multi-language | 
| _pim_products_meta_keywords | string | Meta keywords | |
| _pim_products_meta_keywords__scope__language | string | Meta keywords in a specific scope and language | If attribute is multi-scope and multi-language | 
| _pim_products_description | string | Product description | |
| _pim_products_description__scope__language | string | Product description in a specific scope and language | If attribute is multi-scope and multi-language | 
| _pim_products_meta_description | string | Meta description | |
| _pim_products_meta_description__scope__language | string | Meta description in a specific scope and language | If attribute is multi-scope and multi-language | 
| _pim_products_short_description | string | Product short description | |
| _pim_products_short_description__scope__language | string | Product short description in a specific scope and language | If attribute is multi-scope and multi-language | 
| _pim_products_bundle | object / array of objects ? | It adds products that can be sold in a bundle with the selected product. | It contains the required fields/objects? **entity** and **quantity**.  |
| _pim_products_relations | string | Adds related products, e.g. for product recommendation. | |
| _pim_completeness | string | Required attributes completeness | This attribute is for internal use only. |
| _pim_images | object | It allows to upload images. | It contains the required field **id**. You need the path to the file location. | 
| _pim_files | string | It allows to upload files. | It contains the required field **id**. You need the path to the file location. |
| _pim_channels_connection | string, number, integer, boolean, object | It allows to connect a *PIM* product to an *Omni-Channel* offer. <-- Any of -- Bedeutung? --> | |
| _pim_stock_germany | number | Stock level in warehouse (Germany) | |
| _pim_stock_foreign | number | Stock level in warehouse (other countries) | |

[comment]: <> (_pim_origin: id and/or code3digit required? Es funktioniert nicht. Andere Felder: _pim_product_relations ist wahrscheinlich ein Objekt, _pim_products_bundle ist object/array of objects?, _pim_catalogs ist object? _pim_channels_connection weglassen hier?)

## Create a product

In the *PIM* module, you can create three types of product:
 - a single product, that is, a product without variations, such as a game 
 - a master product, that is, a product with variations, for example, in size or color
 - a variant product, that is, each of the variations of a master product 

There are two possible ways to create a master-variant product structure:

1. Create all products independently first and then link them all at once, as described below: 

    - Create a single or master product, see [Sample: Simple product](#sample-single-product) or [Sample: Master product](#sample-master-product).
    - Add relevant information to variant products, see [Sample: Add variant defining attributes](#sample-add-variant-defining-attributes).
    - Create a variant-master product structure, see [Create a variant-master product structure](#create-a-variant-master-product-structure). 

2. Create a single or master product first and then add to it any numbers of variants at once. For detailed information, see [Create a variant product](./06_Variants.md#create-a-variant-product).

Depending on the type of product, the required fields vary.

#### Definitions

| Attribute       | Data type   | Description | Comments |
| ----------- | ----------- | ----------- | ------------ |
| **sku**      | string   |  Product SKU | |
| **attributeSetId**   | integer  | Attribute set identification number | |
| variantStatus | string | Product status | It indicates whether a product is a *single*, *master* or a *variant*. This field is updated automatically when a variant is added to a master product, that is, it cannot be manually updated. |
| **variantSet**    | object  | Set containing the attributes for product variation | It contains the required field **id**.  |
| **_pim_variants** | object | It defines variant product(s) to a master product. | It contains the following fields: <br> **variantSetId** (integer), *isMasterEntity* (true/false), **masterId** (integer) and the object **definingValues**. The object **definingValues** is an array of objects, where at least an **attributeName** and a **value** must be defined. |


### Sample: Single product

    {
        "product": {
            "sku": "Single-product",
            "attributeSetId": 102
        }
    }

### Sample: Single product in two languages

    {
        "product": {
            "sku": "Single-product",
            "attributeSetId": 102,
            "_pim_art_name__actindo_basic__en_US": "Single product",
            "_pim_art_name__actindo_basic__de_DE": "Einzelprodukt",
            "_pim_products_description__actindo_basic__en_US": "This is a product description.",
            "_pim_products_description__actindo_basic__de_DE": "Das ist eine Produktbeschreibung."
        }
    }

### Sample: Single product with different prices pro scope

    {
        "product": {
            "sku": "Single-product",
            "attributeSetId": 102,
            "_pim_price__webshop": "50.00",
            "_pim_price__retailer_platform": "60.00",
        }
    }

### Sample: Master product

    {
        "product": {
            "sku": "Master-product",
            "attributeSetId": 102,
            "variantStatus": "master",
            "_pim_variants": {
                "isMasterEntity": true,
                "variantSetId": 91
            }
        }
    }

If you want to create one or multiple variant products to a master product at once, see [Create a variant product](./06_Variants.md#create-a-variant-product).



## Edit a product

You can edit a product via API to modify any number of field values at a time. You can also add attributes to an existing product.  

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

#### Definitions

For a list of standard *PIM* attributes, see [The product object](#the-product-object). The required fields are marked in bold. 

To get a list of all your attributes, see [List the attributes in an attribute set](./04_EntityData.md#list-the-attributes-in-an-attribute-set).

| Attribute      | Type | Description | Comments | 
| ----------- | ----------- | ---------- |-------| 
| **id**      | integer    |  Product identification number  | 
| **attributeSetId**   | integer  | Attribute set identification number | |
| variantStatus   | string  | Product status | Indicates whether it is a *single*, *master* or *child*. This field is updated automatically when a variant is added to a master product, that is, it cannot be manually updated. |
| **variantSet**    | object | Set containing the attributes for product variation | It contains the required field **id**.  |
| **_pim_variants** | object | It defines variant product(s) to a master product. | It contains the following fields: <br> **variantSetId** (integer), *isMasterEntity* (true/false), **masterId** (integer) and the object **definingValues**. The object **definingValues** is an array of objects, where at least an **attributeName** and a **value** must be defined. |


### Sample: Add an image to a product

    {
        "product": {
            "id": 891,
            "_pim_images": {
                "images": [
                    {
                        "id": "/EcmFileImage/PIM Product/Hosen/IDS_FROM_1_TO_500/632_actindotrousers-blue"
                    }
                ]
            }
        }
    }    

> [Info] The images are stored in the *ECM* module. To upload images via API, you need to provide the path (file location) to the image you want to upload. If you are uploading an image to a variant product, the "_pim_images" attribute must be included in the variant set. 


### Sample: Add variant defining attributes

    {
        "product": {
            "id": "961",
            "_pim_ean": "Variant-2"
        }
    }

[comment]: <> (variant-to-be single, oder master-to-be single: Felder VariantSetId and definingAttributes müssen definiert sein, um Verknüpfen zu können)


## Create a variant-master product structure

Once you have created your products, you can create a variant-master structure between them. You can also move a variant product to another master product. 

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.changeVariantMaster

#### Definitions

The required fields are marked in bold. For a list of standard *PIM* attributes, see [The product object](#the-product-object). 

| Attribute      | Type | Description | Comments | 
| ----------- | ----------- | ---------- | ----- |
| **variantProduct**      | object    | Variant-to-be product | It contains the required field **id**.  |
| **parentProduct**       | object    | Master-to-be product | It contains the required field **id**.  |
| **variantSet**          | object    | Variant set | It contains the required field **id**.  |

> [Info] The *variantSet* parameter is only necessary if the master-to-be is not a master product yet.

### Sample: Link a single variant to master product

      {
        "variantProduct": {
          "id": 951
        },
        "parentProduct": {
          "id": 941
        },
        "variantSet": {
          "id": 91
        }
      }

### Sample: Link multiple variants to master product

        [
            {
                "variantProduct": {
                    "id": 1161
                },
                "parentProduct": {
                    "id": 1121
                },
                "variantSet": {
                    "id": 91
                }
            },
                {
                "variantProduct": {
                    "id": 1141
                },
                "parentProduct": {
                    "id": 1121
                },
                "variantSet": {
                    "id": 91
                }
            }
        ]


## Delete a product

You can delete a product if it is no longer needed. If it is a master product, that is, with a product with variants, all variants will also be deleted. If it is a variant product, only the addressed variant will be deleted.

> [Caution] **Loss of data**   
  Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored. Problems may occur due to unresolved dependencies. Make sure you really want to delete the selected data.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.delete

#### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description | Comments |  
| ----------- | ----------- | ---------- | ---- |
| **id**      | integer    |  Product identification number | |


### Sample: Delete a product

    {
      "product": {
        "id": 456
      }
    }


## Move a product to recycle bin

You can delete a product temporarily by archiving it of moving it to the recycle bin. These products can be subsequently restored if necessary. If it is a master product, that is, with a product with variants, all variants will also be archived/moved. If it is a variant product, only the addressed variant will be archived/moved.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.moveToRecycleBin

#### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description | Comments |  
| ----------- | ----------- | ---------- | ---- |
| **id**      | integer    |  Product identification number | |


### Sample: Move product to recycle bin

    {
      "product": {
        "id": 456
      }
    }

> [Info] You can restore the product sending the same request to the following API endpoint: /Actindo.Modules.Actindo.PIM.Products.restoreFromRecycleBin


## Move a product to archive

You can delete a product temporarily by archiving it of moving it to the recycle bin. These products can be subsequently restored if necessary. If it is a master product, that is, with a product with variants, all variants will also be archived/moved. If it is a variant product, only the addressed variant will be archived/moved.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.moveToArchive

#### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description | Comments |  
| ----------- | ----------- | ---------- | --- |
| **id**      | integer    |  Product identification number | | 


### Sample: Move product to archive

    {
      "product": {
        "id": 456
      }
    }

> [Info] You can restore the product sending the same request to the following API endpoint: /Actindo.Modules.Actindo.PIM.Products.restoreFromArchive



## List products

Get a list of all products including the ones in the archive or recycle bin. You can set one or more filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.getList

#### Definitions

The required fields are marked in bold.

| Attribute      | Data type | Description | Comments | 
| ---------------|-----------|-------------|--------- |
| scopeId | integer | Scope identification number | Filter for multi-scope attributes |
| languageId | integer | Language key/code | Filter for multi-language attributes <br> The language key must fulfill the criteria of the language codes according to [RFC 4646](https://www.heise.de/netze/rfc/rfcs/rfc4646.shtml), e.g. en, en_US, en-US. |
| query | string | Query string | Quick search for a string |
| fields | array of strings | Query field | Quick search for a field <br> Enter null to search for all fields |
| filter | array of objects | Property value filter | It contains the required fields **property** (field to filter), **operator**, and **value**. Usual filter operators are allowed, e.g. >, <, like, and so on.  |
| hints | array of objects | Query hint | Set query hints to modify the execution of the query, e.g. get data from non-authoritative resources. It contains the required fields **name** (name of the hint) and **value** (value of the hint). |
| sort | array of objects | Results sorting order  | It contains  the required fields **field** (field to sort) and **order** ("ASC" for ascending and "DESC" for descending). |
| start | integer | Pagination start | From 0 |
| limit | integer | Pagination limit |   |

[comment]: <> (Useful? Was für filter sinnvoll? Hints and query Beispiele?)

### Sample: List products by creation date

    {
      "filter": [
        {
          "property": "created",
          "operator": ">",
          "value": "2024-03-26 00:00:00"
        }
      ],
      "start": 0,
      "limit": 500
    }



### Sample: List products by status

    {
     "filter": [
        {
            "property": "variantStatus",
            "operator": "like",
            "value": "child"
        }
    ],
    "start": 0,
    "limit": 500
    }

> [Info] Similarly, you can list all master and all single products by changing the value to "master" and "single" respectively. 



