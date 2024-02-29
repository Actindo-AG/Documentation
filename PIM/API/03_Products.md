# Products

You can create, edit, delete, and list PIM products via API. 

The attribute key is customer-defined in *DataHub*. Therefore, the fields displayed in the request samples should just serve as an example.   

[comment]: <> (Richtiges Wort? Field, attribute/attribute key, parameter??)

> [Caution] If you modify an attribute key in the *DataHub* or *PIM* modules, which is strongly discouraged, the key in the API changes as well. That means, that the field may not be found when sending a request. In this case, you have to update the attribute key in your request body as well.

How to find out entity ID?
  - via UI
  - via API

## Create a product

Create a product in the *PIM* module.

**Endpoint:** /Actindo.Modules.Actindo.PIM.Products.create

**Method:** POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

[comment]: <> (sinnvoll diese Info hier oder eher in Introduction, da immer gleich? Method ist auch immer POST for Actindo. Es ist schon in Introduction erklärt. Hier weglassen?)

### Definitions

[comment]: <> (Oder Parameters? Was ist das richtige Fachwort hier?)

The following table displays a list of all attributes contained in the *PIM basic set* (_pim_attribute name) with their default data types and configuration. The required attributes are marked in bold. 

[comment]: <> (Evtl. übergeordneter Header mit der Tabelle und nur required attributes pro Call unter dem jeweiligen Header. sku bis compareOldValue -> sind diese Attribute "system-intern"? Nicht in DataHub angezeigt)

| Attribute      | Data type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string   |  Product SKU |
| **attributeSetId**   | integer  | Attribute set identification number |
| created	 | string | Date and time of creation <br> Format: YYYY-MM-DD HH:mm:ss |
| createdBy | integer | Frage: Warum an integer? User ID? |
| modified	| string | Date and time of last modification <br> Format: YYYY-MM-DD HH:mm:ss |
| modifiedBy |integer| Frage: Warum an integer? User ID?  |
| attributeSet | object | Attribute set. It contains required field **id**. Frage: Same as field attributeSetId? |
| variantStatus | string | Frage: Example? Master or variant? Vgl. pim_variants |
| lifecycleStatus | string | Frage: Example? |
| synchronousSync | boolean | Frage: Was machst das? Options are **true** or **false**. |
| compareOldValue | boolean | Frage: Was machst das? Options are **true** or **false**. |
| pim_variants | string, number, integer, boolean, object | It indicates if the product is a master or a variant. - Frage: Stimmt das? Unterschied zu VariantStatus oben? Warum so viele Datentypen möglich? Internal use only? S. Data types list |
| pim_art_name | string | Product name |
| pim_art_name__scope__language | string | Product name in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_catalog | array of objects | Product category. It contains the required field **id**. |
| pim_long_text | string | Product description - Frage: Unterschied zu product description? |
| pim_long_text__language | string | Product description in a specific language (if attribute multi-language) |
| pim_ean | string | EAN code |
| pim_customs_number | string | Customs tariff number |
| pim_origin | object | Country of origin. It contains the required field **code3digit**. Frage: ISO 3166-A3 damit gemeint? |
| pim_valid_until | string | Expiration date <br> Format: YYYY-MM-DD HH:mm:ss |
| pim_is_sale | boolean | The product is a sale item. Options are **true** or **false**. |
| pim_fsk18 | boolean | Suitable for persons above 18. Options are **true** or **false**. |
| pim_product_digital | boolean | The product is a digital item. Options are **true** or **false**. |
| pim_stock_value | number | Stock level in warehouse |
| pim_salesunit | string, number, integer, boolean, object | Sale unit - Frage: Unterschied zu is_sale? |
| pim_size_l | object | Product length. It contains required fields **value** and **unitId**. |
| pim_size_b | object | Product width. It contains required fields **value** and **unitId**. |
| pim_size_h | object | Product depth. It contains required fields **value** and **unitId**. |
| pim_weight | object | Product weight. It contains required fields **value** and **unitId**. |
| pim_price | string, number, integer, boolean, object | Product price |
| pim_baseprice | string, number, integer, boolean, object | Price per unit |
| pim_products_url | string | Supplier link |
| pim_products_keywords | string | Additional terms for search |
| pim_products_keywords__scope__language | string | Additional terms for search in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_products_tags | string | Tags - Frage: Unterschied zwischen Tags und Keywords? |
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
| pim_products_relations | string, number, integer, boolean, object | Adds related products, e.g. for product recommendation |
| pim_completeness | string, number, integer, boolean, object | Completeness (Frage: Internal use only?) |
| pim_images | object | It allows to upload images. It contains the required field **id**. |
| pim_files | object | It allows to upload files. It contains the required field **id**. |
| pim_channels_connection | string, number, integer, boolean, object | It allows to connect a *PIM* product to an *Omni-Channel* offer. |
| pim_stock_germany | number | Stock level in warehouse (Germany) |
| pim_stock_foreign | number | Stock level in warehouse (other countries) |


[comment]: <> (Tabelle oben hat nur die Attribute aus PIM basic set. Sinnvoll, mehr dazu zu erklären? Die ersten created, modified, etc. nicht sinnvoll zum Erstellen aber schon zum filter, oder?)

[comment]: <> (Was bedeutet string, number, integer, boolean, object? Alle möglich?)

[comment]: <> (Unterschied zwischen number und integer data type?)

You have to include all required attributes in the JSON file and provide them with a value. The *attributeSetId* value must be an already existing value in *DataHub*. You can find out an entity ID via user interface or via API, see [Link](#to-be-determined). 

Depending on the data you want to specify, you have to add the corresponding attribute in your request. For a complete list of the attributes relevant for the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute set*. Alternatively, you can find a list of all existing PIM attributes under *DataHub > Settings > Attributes*.

[comment]: <> (Stimmt das so?)

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).


### Request samples

####  Create a basic product


    {
        "product": {
            "sku": "ABC_1234",
            "attributeSetId": 592
        }
    }


[comment]: <> (Braucht man auch responses samples oder standard/selbstverständlich? Standard HTTP codes erwähnt in Intro. Mehr dazu? S. API Dokus als Referenz.)

#### Create a product with price, dimensions and image

    {
        "product": {
            "sku": "ABC_1234",
            "attributeSetId": 123,
            "_pim_price": "100",
              "_pim_size_l": {
                  "value": 15,
                  "unitId": 432
              "_pim_size_b": {
                  "value": 8,
                  "unitId": 432,
              "_pim_size_h": {
                  "value": 2,
                  "unitId": 432,
              "pim_images": "ABC_1234.jpg"
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


#### Create a product with a single variant

#### Create a product with multiple variants

[comment]: <> (Ist das überhaupt möglich oder eher via Create variants? Sinnvolle use cases?)


## Edit a product

You can edit a product via API to modify any number of field values at a time. You can also add attributes to an existing product.

[comment]: <> (Stimmt das so? Use case?)

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

### Definitions

The required attributes are marked in bold. For a list of *PIM* attributes, see [Create a product](#create-a-product). 

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product identification number  |

### Request samples

#### Update SKU and add dimension

    {
        "product": {
            "id": "456",
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
            "id": "456",
            "_pim_art_name__actindo_basic__en_US": "Product name",
            "_pim_art_name__actindo_basic__de_DE": "Produktname"
            }
        }
    }


#### Add a single variant to a product


#### Add multiple variants to a product

[comment]: <> (Sinnvolle use cases?)


## Delete a product

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

    {
      "product": {
        "id": "456"
      }
    }


## List products

Get a list of all products including the ones in the archive or recycle bin. You can set one or more filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.getList

**Method**: POST

**Authorization:** oauth2Auth

**Request body schema:** application/json


### Definitions

The required fields are marked in bold.

[comment]: <> (Keine required? Wenn man filter, hints, sort objects setzen will, dann mit required Felder) 

| Field      | Type | Description |  
| ----------- | ----------- | ---------- | 
| filter      | Array of objects    |  ... |
| hint   | integer  | ...  |


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



[comment]: <> (0, -> ohne Anführungszeichen? Was bedeutet es? Not set?)

