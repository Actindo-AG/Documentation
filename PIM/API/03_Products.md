# Products

You can create, edit, delete, and list PIM products via API. 

The keys are customer-defined in *DataHub*. Therefore, the fields displayed in the request samples should just serve as an example.   

> [Caution] If you modify a key in the *DataHub* or *PIM* modules, which is strongly discouraged, the key in the API changes as well. This means that you also have to update the key, that is, the field, in your request body. Otherwise, the field will not be found when sending a request. 


## Create a product

Create a product in the *PIM* module. 

**Endpoint:** /Actindo.Modules.Actindo.PIM.Products.create

**Method:** POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

[comment]: <> (sinnvoll diese Info hier oder eher in Introduction, da immer gleich? Method ist auch immer POST for Actindo. Es ist schon in Introduction erklärt. Hier weglassen?)

### Definitions

The following table displays a list of all attributes contained in the *PIM basic set* (pim_attribute_name) with their default data types and configuration. Additional attributes, such as created and modified, are available in all entities and can be used to set filters. The required fields are marked in bold. 

| Attribute       | Data type   | Description |  
| ----------- | ----------- | ----------- | 
| **sku**      | string   |  Product SKU |
| **attributeSetId**   | integer  | Attribute set identification number |
| created	 | string | Date and time of creation <br> Format: YYYY-MM-DD HH:mm:ss |
| createdBy | integer | User ID |
| modified	| string | Date and time of last modification <br> Format: YYYY-MM-DD HH:mm:ss |
| modifiedBy |integer| User ID |
| attributeSet | object | Product attribute set. It contains required field **id**. |
| variantStatus | string | It indicates whether a product is a **master** or a **variant**. |
| pim_variants | object | It defines the variant product to a master product. It contains the required fields **variantSetId**, **masterId** and **definingValues**. |
| pim_art_name | string | Product name |
| pim_art_name__scope__language | string | Product name in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_catalog | array of objects | Product category. It contains the required field **id**. |
| pim_long_text | string | Product description <!-- Frage: Unterschied zu product description? --> |
| pim_long_text__language | string | Product description in a specific language (if attribute multi-language) |
| pim_ean | string | EAN code |
| pim_customs_number | string | Customs tariff number |
| pim_origin | object | Country of origin. It contains the required field **code3digit**. Country code format: ISO 3166-A3, e.g. DEU for Germany. <!-- Frage: gibt es auch code2digit? Wovon abhängig? --> |
| pim_valid_until | string | Expiration date <br> Format: YYYY-MM-DD HH:mm:ss |
| pim_is_sale | boolean | The product is a sale item. Options are **true** or **false**. |
| pim_fsk18 | boolean | Suitable for persons above 18. Options are **true** or **false**. |
| pim_product_digital | boolean | The product is a digital item. Options are **true** or **false**. |
| pim_stock_value | number | Stock level in warehouse |
| pim_salesunit | object <!-- oder string, wie in payload? --> | Sale unit <!-- Frage: Unterschied zu is_sale? --> It contains the required fields **unitId** and **dimensionId**. |
| pim_size_l | object | Product length. It contains required fields **value** and **unitId**. |
| pim_size_b | object | Product width. It contains required fields **value** and **unitId**. |
| pim_size_h | object | Product depth. It contains required fields **value** and **unitId**. |
| pim_weight | object | Product weight. It contains required fields **value** and **unitId**. |
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
| pim_products_bundle | object | It adds products that can be sold in a bundle with the selected product. It contains required fields **entity** and **quantity**. |
| pim_products_relations | string | Adds related products, e.g. for product recommendation. |
| pim_completeness | string | Required attributes completeness. This attribute is for internal use only. |
| pim_images | object | It allows to upload images. It contains the required field **id**. |
| pim_files | object | It allows to upload files. It contains the required field **id**. |
| pim_channels_connection | string, number, integer, boolean, object | It allows to connect a *PIM* product to an *Omni-Channel* offer. |
| pim_stock_germany | number | Stock level in warehouse (Germany) |
| pim_stock_foreign | number | Stock level in warehouse (other countries) |


You have to include all required fields in the JSON file and provide them with a value. The **attributeSetId** value must be an existing value in *DataHub*. You can find out an entity ID via user interface or via API, see [Entity ID](./02_Basics.md#entity-id).

Depending on the data you want to specify, you have to add the corresponding field in your request. For a complete list of the attributes relevant for the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute sets*. Alternatively, you can find a list of all existing PIM attributes under *DataHub > Settings > Attributes > Search for pim_*.

[comment]: <> (Stimmt das so?)

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).


### Request samples

####  Create a single product


    {
        "product": {
            "sku": "ABC_1234",
            "attributeSetId": 592
        }
    }


#### Create a product in two languages

    {
        "product": {
            "sku": "ABC_1234",
            "attributeSetId": 123,
            "_pim_art_name__actindo_basic__en_US": "Shirt",
            "_pim_art_name__actindo_basic__de_DE": "Hemd",
            "_pim_products_description__actindo_basic__en_US": "This is a product description.",
            "_pim_products_description__actindo_basic__de_DE": "Das ist eine Produktbeschreibung.",
        }
    }


#### Create a product with different prices pro scope

    {
        "product": {
            "sku": "ABC_1234",
            "attributeSetId": 123,
            "_pim_price__webshop": "50.00",
            "_pim_price__retailer_platform": "60.00",
        }
    }

  
#### Create a master product

      {
          "product": {
              "sku": "MASTER1",
              "attributeSetId": 612,
              "variantStatus": "master"
          }
      }

#### Create a variant

      {
          "product": {
              "sku": "CHILD1",
              "attributeSetId": 752,
              "variantStatus": "child",
              "variantSet": [
                  {
                      "id": 2
                  }
              ]
          }
      }

#### Create several variant products

    {
      "product": {
        "sku": "CHILD1",
        "attributeSetId": 612,
        "variantStatus": "child"
        "variantSet": [
                  {
                      "id": 2
    },
      "product": {
        "sku": "CHILD2",
        "attributeSetId": 612,
        "variantStatus": "child"
        "variantSet": [
                  {
                      "id": 2
      }
    }
  


#### Add variants to master product

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.changeVariantMaster


      {
        "variantProduct": {
          "id": 82
        },
        "parentProduct": {
          "id": 72
        },
        "variantSet": {
          "id": 22
        }
      }

You can get all needed ID from the request response.




## Edit a product

You can edit a product via API to modify any number of field values at a time. You can also add attributes to an existing product.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

### Definitions

The required fields are marked in bold. For a list of *PIM* attributes, see [Create a product](#create-a-product). 

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number  |

### Request samples

#### Update SKU and add dimension

    {
        "product": {
            "id": 456,
            "sku": "ABC_1234",
            "_pim_size_h": {
                "value": 10,
                "unitId": 432
            }
        }
    }


#### Add the product name in different languages

    {
        "product": {
            "id": 456,
            "_pim_art_name__actindo_basic__en_US": "Product name",
            "_pim_art_name__actindo_basic__de_DE": "Produktname"
            }
        }
    }


#### Add a single variant to a product


#### Add multiple variants to a product

[comment]: <> (Sinnvolle use cases?)


## Delete a product permanently

You can delete a product if it is no longer needed. 

> [Caution] If it is a master product, that is, with product variants, all variants will also be deleted. If it is a product variant, only the variant will be deleted.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.delete

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number |


### Request sample

#### Delete a product (and its variants, if any) permanently

    {
      "product": {
        "id": 456
      }
    }


## Delete a product temporarily 

### Move a product to recycle bin

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.moveToRecycleBin

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number |


### Request sample

...


### Move a product to archive

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.moveToArchive

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

### Definitions

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number |


### Request sample

...

## List products

Get a list of all products including the ones in the archive or recycle bin. You can set one or more filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.getList

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json


### Definitions

The required fields are marked in bold.

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| scopeId | integer | Filter for multi-scope attributes |
| languageId | integer | Filter for multi-language attributes |
| query | string | Quick search for a query string |
| fields | array of strings | Quick Search for query fields; null to search for all fields |
| filter | array of objects | To set a filter. It contains the required fields **property** (field to filter), **operator**, and **value**. |
| hints | array of objects | It contains the required fields **name** (name of the hint) and **value** (value of the hint). |
| sort | array of objects | It contains  the required fields **field** (field to sort) and **order** ("ASC" for ascending and "DESC" for descending).  |
| start | integer | Pagination: Pagination start (from 0) |
| limit | integer | Pagination: Pagination limit |
| serializeOptionals | array of strings | <!-- Was ist das --> |

[comment]: <> (Check non-authoritative sources -> Query hints: You may set query hints to modify the execution of the query, for example get data from non-authoritative sources.)

[comment]: <> (type: "numeric"|"date": "<", "<=", ">", ">=", "=", "!="; type="list": "in"; type="string": "like"; type="all": "isNull","isNotNull")

### Request sample  

#### Get a list of products setting a filter

    {
      "scopeId": 0,
      "languageId": 0,
      "query": "string",
      "fields": [
        "string"
      ],
      "filter": [
        {
          "property": "string",
          "operator": "string",
          "value": "string"
        }
      ],
      "hints": [
        {
          "name": "string",
          "value": "string"
        }
      ],
      "sort": [
        {
          "field": "string",
          "order": "string"
        }
      ],
      "start": 0,
      "limit": 0,
      "serializeOptionals": [
        "string"
      ]
    }


## Get product details

Get all details stored in the database for a specific product. You can set one or more filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.PIM.get

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

### Request sample  

{
    "entityId": 12,
    "freezeEntityIfPossible": false
}


## Set filters



## Get attributes in an attribute set

    {
      "attributeSetId": 752,
      "start": 0,
      "limit": 15
    }
