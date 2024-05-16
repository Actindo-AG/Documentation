# Manage products 

You can manage your products via API. You can create, edit, delete, both permanently and temporary, and list *PIM* products. 

To manage your products via API, you need to provide the required key-value pairs in your requests. The following elements are essential in a request: 

**Attribute key**

Depending on the data you want to specify, you have to add the corresponding attribute, in its form as attribute key, to your request. For detailed information on the attribute key structure, see [Attributes](./03_KeyConcepts.md#attributes). 

For a complete list of the attributes included in the attribute set of the product you want to address, you can check the corresponding *PIM* attribute set under *PIM > Settings > Attribute sets*. Alternatively, you can find a list of all existing *PIM* attributes under *PIM > Settings > Attributes*. Alternatively, you can get a list of attributes via API, see [List the attributes in an attribute set](./04_RetrieveEntityData.md#list-the-attributes-in-an-attribute-set).

Bear in mind that keys are customer-defined. Therefore, the fields displayed in the following request samples should just serve as an example. For a practical example on how to use the request samples, see [How to use the request samples](./02_GetStarted.md#how-to-use-the-request-samples). 

> [Caution] In the latest version of the *PIM* and *DataHub* modules, it is possible to modify the attribute key. However, this is strongly discouraged and has far-reaching consequences. If you modify a key in the *PIM* or *DataHub* modules, the key in the API changes as well. This means that you also have to update the key, that is, the field, in your request body. Otherwise, the field will not be found when sending a request. 

**Entity IDs**

You may need to provide an entity ID value to a specific attribute key. Any ID values you need, for example, the **attributeSetId**, must be an existing value in the *DataHub* module. You can find out an entity ID via user interface or via API. For detailed information, see [Retrieve entity data](./04_RetrieveEntityData.md).

**Data type**

The value you can give a specific attribute depends on the attribute's data type. For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).



## The product object

Products represent the goods and services you offer to your customers. They are defined through a set of attributes. 

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
| _pim_variants | object | Master or variant product definition | Depending on the product status (master or variant product), the fields contained vary. <br> A master product contains the following fields: <br> **variantSetId** (integer), **isMasterEntity** (true), and, if variants already available,  **childrenIds** and **numberOfChildren**. <br> A variant product contains the following fields: <br>  **variantSetId** (integer), **isMasterEntity** (false), **masterId** (integer), and the object **definingValues**. The object **definingValues** is an array of objects, where at least one **attributeName** and one **value** must be defined, e.g. *_pim_ean* and *child-1* respectively. |
| _pim_art_name | string | Product name | |
| _pim_art_name__scope__language | string | Product name in a specific scope and language | If attribute is multi-scope and multi-language |
| _pim_catalog | string / object ? | Product categories | It contains the required field **id**. <!-- Frage: In Payload nur string, in product object Tabelle Any of...? --> |
| _pim_long_text | string | Product long name | |
| _pim_long_text__language | string | Product long name in a specific language | If attribute is multi-language |
| _pim_ean | string | Product EAN code | |
| _pim_customs_number | string | Customs tariff number | |
| _pim_origin | object | Country of origin | It contains the required field **code3digit**. <br> Country code format: ISO 3166-A3, e.g. DEU for Germany. |
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
| _pim_products_relations | string / object ? | Adds related products, e.g. for product recommendation. | |
| _pim_completeness | object | Required attributes completeness | This attribute is for internal use only. |
| _pim_images | object | It allows to upload images. | It contains the required field **id**. You need the path to the file location. | 
| _pim_files | string | It allows to upload files. | It contains the required field **id**. You need the path to the file location. |
| _pim_channels_connection | Object ? | Connection definition from *PIM* to *Omni-Channel* | It allows to connect a *PIM* product to an *Omni-Channel* offer. |
| _pim_stock_germany | number | Stock level in warehouse (Germany) | |
| _pim_stock_foreign | number | Stock level in warehouse (other countries) | |

[comment]: <> (_pim_origin: id and/or code3digit required? Es funktioniert nicht. Andere Felder: _pim_product_relations ist wahrscheinlich ein Objekt, _pim_products_bundle ist object/array of objects?, _pim_catalogs ist object? _pim_channels_connection weglassen hier?)

[comment]: <> (_pim_variants: fields vary depending on product status, i.e. variant or master. S. unten - in Doku übernehmen! If parent, isMasterEntity true, variantSetId, childrenIds, and numberOfChildren, if variants available. If variant... )

--- Bitte ignorieren. Ich muss es noch in Doku evtl. übernehmen. ---


Master/Variant (geerbt) pim_origin:

        "_pim_origin": {
                        "id": 76,
                        "codeNumeric": 76,
                        "code3digit": "BRA",
                        "code2digit": "BR",
                        "codeKfz": "BR",
                        "continentCode": "SA",
                        "isEu": false,
                        "name": "Brasilien",
                        "_E": 2905170383
                    },


_pim_product_relations: 

        "_pim_products_relations": {
                                    "id": "8b1989c738d4b489ffcef0d3a93e9448",
                                    "ids": [],
                                    "entityData": [],
                                    "stringRepresentation": "",
                                    "_E": 4049651496
                                },

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

2. Create a single or master product first and then add to it any numbers of variants at once. For detailed information, see [Create a variant product](./06_ManageVariantProducts.md#create-a-variant-product).

Depending on the type of product, the required fields vary.

#### Definitions

| Attribute       | Data type   | Description | Comments |
| ----------- | ----------- | ----------- | ------------ |
| **sku**      | string   |  Product SKU | |
| **attributeSetId**   | integer  | Attribute set identification number | |
| variantStatus | string | Product status | It indicates whether a product is a *single*, *master* or a *variant*. This field is updated automatically when a variant is added to a master product, that is, it cannot be manually updated. |
| **variantSet**    | object  | Set containing the attributes for product variation | It contains the required field **id**.  |
| **_pim_variants** | object | Master of variant product definition | It contains the following fields: <br> **variantSetId** (integer), *isMasterEntity* (true/false), **masterId** (integer) and the object **definingValues**. The object **definingValues** is an array of objects, where at least an **attributeName** and a **value** must be defined. |


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

If you want to create one or multiple variant products to a master product at once, see [Create a variant product](./06_ManageVariantProducts.md#create-a-variant-product).



## Edit a product

You can edit a product via API to modify any number of field values at a time. You can also add attributes to an existing product.  

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

#### Definitions

For a list of standard *PIM* attributes, see [The product object](#the-product-object). The required fields are marked in bold. 

To get a list of all your attributes, see [List the attributes in an attribute set](./04_RetrieveEntityData.md#list-the-attributes-in-an-attribute-set).

| Attribute      | Type | Description | Comments | 
| ----------- | ----------- | ---------- |-------| 
| **id**      | integer    |  Product identification number  | 
| **attributeSetId**   | integer  | Attribute set identification number | |
| variantStatus   | string  | Product status | Indicates whether it is a *single*, *master* or *child*. This field is updated automatically when a variant is added to a master product, that is, it cannot be manually updated. |
| **variantSet**    | object | Set containing the attributes for product variation | It contains the required field **id**.  |
| **_pim_variants** | object | Master or variant product definition | It contains the following fields: <br> **variantSetId** (integer), *isMasterEntity* (true/false), **masterId** (integer) and the object **definingValues**. The object **definingValues** is an array of objects, where at least an **attributeName** and a **value** must be defined. |


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


## Create a product family

[comment]: <> (Oder Create a variant-master product structure?)

Once you have created your products, you can link them together to create a product family. A product family is a group of products comprising a master product and its variant products. You can also move a variant product to another product family, that is, link it to a different master product. 

A product family reflects your product structure...

[comment]: <> (Wozu brauche ich das?)

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

---

Filter all products
PIM.Products.getList

{


}


PIM.AttributeSetController.getList

filter
property: key
operation: (gleich)
value: _pim_base_set