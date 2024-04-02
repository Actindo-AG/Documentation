# Products

You can manage your products via API. You can create, edit, delete, both permanently and temporary, and list *PIM* products via API. 

The keys are customer-defined. Therefore, the fields displayed in the request samples should just serve as an example. You have to include all required fields in the JSON file and provide them with a value. Any ID values you need, for example, the **attributeSetId**, must be an existing value in the *DataHub* module.  

You can find out an entity ID via user interface or via API, see [Entities](./03_KeyConcepts.md#entities).

Depending on the data you want to specify, you have to add the corresponding field to your request. For a complete list of the attributes relevant for the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute sets*. Alternatively, you can find a list of all existing PIM attributes under *DataHub > Settings > Attributes > Search for pim_*.

If necessary, you can get a list of all attributes you have created in the *DataHub* module, both in the user interface and via API. To obtain a list in the user interface, go to *DataHub > Attributes* and filter the attribute list by any criteria you wish, e.g. by attribute name starting with *"pim_"*. To get a list of all pim attributes via API, see [Get a list of attributes in an attribute set](./04_EntityData.md#get-a-list-of-attributes-in-an-attribute-set).

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).

> [Caution] In the latest version of the *DataHub* module, it is possible to modify the attribute key. However, this is strongly discouraged and has far-reaching consequences. If you modify a key in the *DataHub* or *PIM* modules, the key in the API changes as well. This means that you also have to update the key, that is, the field, in your request body. Otherwise, the field will not be found when sending a request. 


## The product object

Products represent the goods and services you offer to your customer. They are defined through a set of attributes. 

The following table displays a list of all attributes contained in the *PIM basic set* (pim_attribute_name) with their default data types and configuration. Additional attributes, such as created and modified, are available in all entities and can be used to set filters. The required fields are marked in bold. 

| Attribute       | Data type   | Description |
| ----------- | ----------- | ----------- | 
| **sku**      | string   |  Product SKU | 
| **attributeSetId**   | integer  | Attribute set identification number |
| created	 | string | Date and time of creation <br> Format: YYYY-MM-DD HH:MM:SS |
| createdBy | integer | User ID | 
| modified	| string | Date and time of last modification <br> Format: YYYY-MM-DD HH:MM:SS |
| modifiedBy |integer| User ID |
| attributeSet | object | Product attribute set. It contains the required field **id**. |
| variantStatus | string | Product status. It indicates whether a product is a *single*, *master* or a *variant*. |
| pim_variants | object | It defines a variant product to a master product. It contains the required fields **variantSetId**, **masterId** and **definingValues**. |
| pim_art_name | string | Product name |
| pim_art_name__scope__language | string | Product name in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_catalog | string <!-- Frage: Stimmt so? --> | Product category. It contains the required field **id**. <!-- Frage: In Payload nur string, in product object Tabelle Any of...? --> |
| pim_long_text | string | Product description <!-- Frage: Unterschied zu product description? --> |
| pim_long_text__language | string | Product description in a specific language (if attribute multi-language) |
| pim_ean | string | EAN code |
| pim_customs_number | string | Customs tariff number |
| pim_origin | object | Country of origin. It contains the required field **code3digit**. <br> Country code format: ISO 3166-A3, e.g. DEU for Germany. <!-- Frage: gibt es auch code2digit? Wovon abhängig? --> |
| pim_valid_until | string | Expiration date <br> Format: YYYY-MM-DD HH:MM:SS |
| pim_is_sale | boolean | The product is a sale item. Options are *true* or *false*. |
| pim_fsk18 | boolean | Suitable for persons above 18. Options are *true* or *false*. |
| pim_product_digital | boolean | The product is a digital item. Options are *true* or *false*. |
| pim_stock_value | number | Stock level in warehouse |
| pim_salesunit | object <!-- oder string, wie in payload? --> | Sale unit. <!-- Frage: Unterschied zu is_sale? --> |
| pim_size_l | object | Product length. It contains the required fields **value** and **unitId**. |
| pim_size_b | object | Product width. It contains the required fields **value** and **unitId**. |
| pim_size_h | object | Product depth. It contains the required fields **value** and **unitId**. |
| pim_weight | object | Product weight. It contains the required fields **value** and **unitId**. |
| pim_price | string | Product price |
| pim_baseprice | string | Price per unit |
| pim_products_url | string | Supplier link |
| pim_products_keywords | string | Additional terms for search |
| pim_products_keywords__scope__language | string | Additional terms for search in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_tags | string | Tags <!-- Frage: Unterschied zwischen Tags und Keywords? --> |
| pim_products_tags__scope__language | string | Tags in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_meta_title | string | Meta title |
| pim_products_meta_title__scope__language | string | Meta title in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_meta_keywords | string | Meta keywords |
| pim_products_meta_keywords__scope__language | string | Meta keywords in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_description | string | Product description |
| pim_products_description__scope__language | string | Product description in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_meta_description | string | Meta description |
| pim_products_meta_description__scope__language | string | Meta description in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_short_description | string | Product short description |
| pim_products_short_description__scope__language | string | Product short description in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_bundle | object | It adds products that can be sold in a bundle with the selected product. It contains the required fields **entity** and **quantity**. |
| pim_products_relations | string | Adds related products, e.g. for product recommendation. |
| pim_completeness | string | Required attributes completeness. This attribute is for internal use only. |
| pim_images | string | It allows to upload images. |
| pim_files | string | It allows to upload files. |
| pim_channels_connection | string, number, integer, boolean, object | It allows to connect a *PIM* product to an *Omni-Channel* offer. <-- Any of -- Bedeutung? --> |
| pim_stock_germany | number | Stock level in warehouse (Germany) |
| pim_stock_foreign | number | Stock level in warehouse (other countries) |


## Create a product

Create a new product. 

You can create thee types of product:
 - a single product
 - a master product
 - a variant product

Depending on the type of product, the required fields vary.

### Definitions

| Attribute       | Data type   | Description |
| ----------- | ----------- | ----------- | 
| **sku**      | string   |  Product SKU | 
| **attributeSetId**   | integer  | Attribute set identification number |
| **variantStatus**   | string  | Indicates whether it is a *single*, *master* or *child*  |
| **variantSet**   | object  | It contains the required field **id**.  |

### Sample: Single product

    {
        "product": {
            "sku": "Shirt_123",
            "attributeSetId": 622
        }
    }


### Sample: Single product in two languages


    {
        "product": {
            "sku": "Shirt_456",
            "attributeSetId": 622,
            "_pim_art_name__actindo_basic__en_US": "Shirt",
            "_pim_art_name__actindo_basic__de_DE": "Hemd",
            "_pim_products_description__actindo_basic__en_US": "This is a product description.",
            "_pim_products_description__actindo_basic__de_DE": "Das ist eine Produktbeschreibung."
        }
    }

### Sample: Single product with different prices pro scope

    {
        "product": {
            "sku": "ABC_1234",
            "attributeSetId": 123,
            "_pim_price__webshop": "50.00",
            "_pim_price__retailer_platform": "60.00",
        }
    }


### Sample: Master product


      {
          "product": {
              "sku": "MASTER1",
              "attributeSetId": 622,
              "variantStatus": "master"
          }
      }


### Sample: Variant product

    {
      "product": 
        {
          "sku": "VARIANT-Shirt_38",
          "attributeSetId": 622,
          "variantStatus": "child",
          "variantSet": {
            "id": 32
          }
        }
    }



## Edit a product

You can edit a product via API to modify any number of field values at a time. You can also add attributes to an existing product.

[comment]: <> (Modify single to master possible? How?)

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

### Definitions

For a list of standard *PIM* attributes, see [The product object](#the-product-object). The required fields are marked in bold. 

To get a list of all your attributes, see [List of all attributes](#to-be-determined).

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number  |


### Sample: Update price and add images request

    {
        "product": {
            "id": 456,
            "price": "65.00",
            "pim_images": "string",
            }
    }

[comment]: <> (Wie werden die images hochgeladen/verbunden? Wo befinden sich die images?)


### Sample: Add the product name in different languages request

    {
        "product": {
            "id": 456,
            "_pim_art_name__actindo_basic__en_US": "Product name",
            "_pim_art_name__actindo_basic__de_DE": "Produktname"
            }
    }


### Sample: Add variant defining attributes request

    {
        "product": {
            "id": 782,
            "pim_variants": {
                "3,892": "Pink",
                "3,902": "256",
                "149": "1,989"
            }
        }
    }

  [comment]: <> (Response: success, aber keine Änderung in CHILD1. Warum?)



## Add variants to master product

Once you have created variant products, you can add them to the corresponding master product. You ca also move a variant product to another master product. The *variantSet* parameter is only necessary if the master-to-be is not a master product yet.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.changeVariantMaster

### Definitions

The required fields are marked in bold. For a list of *PIM* attributes, see [The product object](#the-product-object). 

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **variantProduct**      | object    |  It contains the required field **id**.  |
| **parentProduct**       | object    |  It contains the required field **id**.  |
| **variantSet**          | object    |  It contains the required field **id**.  |


### Sample: Add a variant to master product request

      {
        "variantProduct": {
          "id": 852
        },
        "parentProduct": {
          "id": 842
        },
        "variantSet": {
          "id": 32
        }
      }

[comment]: <> ("error": "Call to a member function getVariantSet() on a non-object (null)",)

### Sample: Add a variant to master product response

[comment]: <> (Add multiple variants to a master product at a time?)


## Delete a product

You can delete a product if it is no longer needed. If it is a master product, that is, with a product with variants, all variants will also be deleted. If it is a variant product, only the addressed variant will be deleted.

> [Caution] **Loss of data**   
  Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored. Problems may occur due to unresolved dependencies. Make sure you really want to delete the selected data.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.delete

### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number |


### Sample: Delete a product request

    {
      "product": {
        "id": 456
      }
    }


## Move a product to recycle bin

You can delete a product temporarily by archiving it of moving it to the recycle bin. These products can be subsequently restored if necessary. If it is a master product, that is, with a product with variants, all variants will also be archived/moved. If it is a variant product, only the addressed variant will be archived/moved.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.moveToRecycleBin

### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number |


### Sample: Move product to recycle bin request

    {
      "product": {
        "id": 456
      }
    }

> [Info] You can restore the product sending the same request to the following API endpoint: /Actindo.Modules.Actindo.PIM.Products.restoreFromRecycleBin


## Move a product to archive

You can delete a product temporarily by archiving it of moving it to the recycle bin. These products can be subsequently restored if necessary. If it is a master product, that is, with a product with variants, all variants will also be archived/moved. If it is a variant product, only the addressed variant will be archived/moved.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.moveToArchive

### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number |


### Sample: Move product to archive request

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

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| scopeId | integer | Filter for multi-scope attributes |
| languageId | integer | Filter for multi-language attributes |
| query | string | Quick search for a query string |
| fields | array of strings | Quick search for query fields; null to search for all fields |
| filter | array of objects | To set a filter. It contains the required fields **property** (field to filter), **operator**, and **value**. |
| hints | array of objects | It contains the required fields **name** (name of the hint) and **value** (value of the hint). |
| sort | array of objects | It contains  the required fields **field** (field to sort) and **order** ("ASC" for ascending and "DESC" for descending).  |
| start | integer | Pagination: Pagination start (from 0) |
| limit | integer | Pagination: Pagination limit |


### Sample: List products by creation date request

    {
      "filter": [
        {
          "property": "created",
          "operator": ">",
          "value": "2024-03-26 00:00:00"
        }
      ],
      "start": 0,
      "limit": 10
    }

### Sample: List products by create date response

    {
        "data": [
            {
                "id": 822,
                "sku": "Shirt_123",
                "created": "2024-03-26 13:38:39",
                "createdBy": 220741,
                "createdByUsername": "User Name (username)",
                "modified": "2024-03-26 13:38:39",
                "modifiedBy": 220741,
                "modifiedByUsername": "User Name (username)",
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 622,
                "attributeSetName": "Hemden",
                "mappedAttributeSetIds": null,
                "variantStatus": "single",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            },
            {
                "id": 832,
                "sku": "Shirt_456",
                "created": "2024-03-26 13:43:37",
                "createdBy": 220741,
                "createdByUsername": "User Name (username)",
                "modified": "2024-03-26 13:43:37",
                "modifiedBy": 220741,
                "modifiedByUsername": "User Name (username)",
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 622,
                "attributeSetName": "Hemden",
                "mappedAttributeSetIds": null,
                "variantStatus": "single",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            },
            {
                "id": 852,
                "sku": "VARIANT-Shirt_38",
                "created": "2024-03-26 13:51:25",
                "createdBy": 220741,
                "createdByUsername": "User Name (username)",
                "modified": "2024-03-26 14:46:51",
                "modifiedBy": 220741,
                "modifiedByUsername": "User Name (username)",
                "lifecycleStatusChangedAt": "2024-03-26 14:46:51",
                "lifecycleStatusChangedBy": 220741,
                "lifecycleStatusChangedByUsername": "User Name (username)",
                "attributeSetId": 622,
                "attributeSetName": "Hemden",
                "mappedAttributeSetIds": null,
                "variantStatus": "single",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            }
        ],
        "n_rows": 3,
        "success": true,
        "displayMessage": null,
        "displayMessageTitle": null,
        "error": null,
        "job_id": null
    }

  
[comment]: <> (Komisch! Alle als single, obwohl ein single, ein master und ein child)

### Sample: List variant products request

    {
     "filter": [
        {
            "property": "variantStatus",
            "operator": "like",
            "value": "child"
        }
    ],
    "start": 0,
    "limit": 5
}


### Sample: List variant products response


    {
        "data": [
            {
                "id": 12,
                "sku": "IP13-pink-128GB",
                "created": "2022-12-02 14:23:08",
                "createdBy": 225622,
                "createdByUsername": null,
                "modified": "2022-12-02 14:32:15",
                "modifiedBy": 225622,
                "modifiedByUsername": null,
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 592,
                "attributeSetName": "Smartphones",
                "mappedAttributeSetIds": null,
                "variantStatus": "child",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            },
            {
                "id": 22,
                "sku": "IP13-pink-256GB",
                "created": "2022-12-02 14:23:10",
                "createdBy": 225622,
                "createdByUsername": null,
                "modified": "2022-12-02 14:32:22",
                "modifiedBy": 225622,
                "modifiedByUsername": null,
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 592,
                "attributeSetName": "Smartphones",
                "mappedAttributeSetIds": null,
                "variantStatus": "child",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            },
            {
                "id": 32,
                "sku": "IP13-pink-512GB",
                "created": "2022-12-02 14:23:11",
                "createdBy": 225622,
                "createdByUsername": null,
                "modified": "2022-12-02 14:32:22",
                "modifiedBy": 225622,
                "modifiedByUsername": null,
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 592,
                "attributeSetName": "Smartphones",
                "mappedAttributeSetIds": null,
                "variantStatus": "child",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            },
            {
                "id": 42,
                "sku": "IP13-blue-128GB",
                "created": "2022-12-02 14:23:12",
                "createdBy": 225622,
                "createdByUsername": null,
                "modified": "2022-12-02 14:32:23",
                "modifiedBy": 225622,
                "modifiedByUsername": null,
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 592,
                "attributeSetName": "Smartphones",
                "mappedAttributeSetIds": null,
                "variantStatus": "child",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            },
            {
                "id": 52,
                "sku": "IP13-blue-256GB",
                "created": "2022-12-02 14:23:14",
                "createdBy": 225622,
                "createdByUsername": null,
                "modified": "2022-12-02 14:32:23",
                "modifiedBy": 225622,
                "modifiedByUsername": null,
                "lifecycleStatusChangedAt": null,
                "lifecycleStatusChangedBy": null,
                "lifecycleStatusChangedByUsername": null,
                "attributeSetId": 592,
                "attributeSetName": "Smartphones",
                "mappedAttributeSetIds": null,
                "variantStatus": "child",
                "lifecycleStatus": "active",
                "isFrozenByMe": false,
                "frozenDate": null,
                "frozenByUid": null,
                "frozenByName": null,
                "frozenSesskey": null,
                "frozenRequestId": null,
                "entityId": 2617111665,
                "_E": 2617111665
            }
        ],
        "n_rows": 63,
        "success": true,
        "displayMessage": null,
        "displayMessageTitle": null,
        "error": null,
        "job_id": null
    }