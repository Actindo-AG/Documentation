# Products

You can create, edit, delete, and list PIM products via API. 

The attribute key is customer-defined in *DataHub*. Therefore, the fields displayed in the request samples should just serve as an example.   

[comment]: <> (Richtiges Wort? Field, attribute/attribute key, parameter??)

> [Caution] If you modify an attribute key in the *DataHub* or *PIM* modules, which is strongly discouraged, the key in the API changes as well. That means, that the field may not be found when sending a request. In this case, you have to update the attribute key in your request body as well.

How to find out entity ID?
  - via UI
  - via API

## Create a product

**Endpoint:** /Actindo.Modules.Actindo.PIM.Products.create

**Method:** POST

**Authorization:** oauth2Auth

**Request body schema:** application/json

[comment]: <> (sinnvoll diese Info hier oder eher in Introduction, da immer gleich? Method ist auch immer POST for Actindo. Es ist schon in Introduction erklärt. Hier weglassen?)

### Parameters

The following table displays a list of all attributes contained in the *PIM basic set* with their default data types and configuration. The required attributes are marked in bold. 

| Attribute      | Data type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string   |  Product SKU |
| **attributeSetId**   | integer  | Attribute set identification number |
| created	 | string | Date and time of creation. Format: YYYY-MM-DD HH:mm:ss |
| createdBy | integer | Frage: Warum an integer? User ID? |
| modified	| string | Date and time of last modification. Format: YYYY-MM-DD HH:mm:ss |
| modifiedBy |integer| Frage: Warum an integer? User ID?  |
| attributeSet | object | Attribute set. It contains required field **id**. Frage: Same as field attributeSetId? |
| variantStatus | string | Frage: Example? Master or variant? |
| lifecycleStatus | string | Frage: Example? |
| synchronousSync | boolean | Was ist das? Options are **true** or **false**. |
| compareOldValue | boolean | Was ist das? Options are **true** or **false**. |
| pim_variants | string, number, integer, boolean, object | Product variants - Frage: Unterschied zu VariantStatus oben? Warum so viele Datentypen möglich? |
| pim_art_name | string | Product name |
| pim_art_name__scope__language | string | Product name in a specific scope and language (if attribute multi-scope and multi-language) |
| pim_catalog | array of objects | Product categories |
| pim_long_text | string | Product description |
| pim_long_text__language | string | Product description in a specific language (if attribute multi-language) |
| pim_ean | string | EAN code |
| pim_customs_number | string | Customs tariff number |
| pim_origin | object | Country of origin |
| pim_valid_until | string | Expiration date. Format: YYYY-MM-DD HH:mm:ss |
| pim_is_sale | boolean | The product is a sale item. Options are **true** or **false**. |
| pim_fsk18 | boolean | Suitable for persons above 18. Options are **true** or **false**. |
| pim_product_digital | boolean | The product is a digital item. Options are **true** or **false**. |
| pim_stock_value | number | Stock level in warehouse |
| pim_salesunit | string, number, integer, boolean, object | Sale unit - Frage: Unterschied zu is_sale? |
| pim_size_l | object | Product length. If you want to specify this attribute, you need to specify the required fields **value** and **unitId**. |
| pim_size_b | object | Product width. If you want to specify this attribute, you need to specify the required fields **value** and **unitId**. |
| pim_size_h | object | Product depth. If you want to specify this attribute, you need to specify the required fields **value** and **unitId**. |
| pim_weight | object | Product weight. If you want to specify this attribute, you need to specify the required fields **value** and **unitId**. |
| pim_price |string, number, integer, boolean, object | Product price |
| pim_baseprice |string, number, integer, boolean, object | Product basic price - Frage: price vs. basic price |
| pim_products_url | string | Supplier link |
| pim_products_keywords__actindo_basic__en_US | string | Additional terms for search in a specific scope and language |
| pim_products_keywords__actindo_basic__de_DE | string | Additional terms for search in a specific scope and language |
| pim_products_tags__actindo_basic__en_US | string | Tags/keywords in a specific scope and language |
| pim_products_tags__actindo_basic__de_DE | string | Tags / Keywords in a specific scope and language |
| pim_products_meta_title__actindo_basic__en_US | string | Meta title in a specific scope and language |
| pim_products_meta_title__actindo_basic__de_DE | string | Meta title in a specific scope and language|
| pim_products_meta_keywords__actindo_basic__en_US | string | Meta keywords in a specific scope and language |
| pim_products_meta_keywords__actindo_basic__de_DE | string | Meta keywords in a specific scope and language |
| pim_products_description__actindo_basic__en_US | string | Product description in a specific scope and language|
| pim_products_description__actindo_basic__de_DE | string | Product description in a specific scope and language |
| pim_products_meta_description__actindo_basic__en_US | string |Meta description in a specific scope and language |
| pim_products_meta_description__actindo_basic__de_DE | string | Meta description in a specific scope and language |
| pim_products_short_description__actindo_basic__en_US | string | Product short description in a specific scope and language |
| pim_products_short_description__actindo_basic__de_DE | string | Product short description in a specific scope and language|
| pim_products_bundle | object | --- |
| pim_products_relations | string, number, integer, boolean, object | Product relations |
| pim_completeness | string, number, integer, boolean, object | Completeness |
| pim_images | object | --- |
| pim_files | object | --- |
| pim_channels_connection | string, number, integer, boolean, object | PIM to Omni-Channel connection |
| pim_stock_germany | number | Stock Germany |
| pim_stock_foreign | number | Stock Foreign Countries |


[comment]: <> (Tabelle oben hat nur die Attribute aus PIM basic set. Sinnvoll, mehr dazu zu erklären? Die ersten created, modified, etc. nicht sinnvoll zum Erstellen aber schon zum filter, oder?)

[comment]: <> (Was bedeutet string, number, integer, boolean, object? Alle möglich?)

You have to include all required attributes in the JSON file and provide them with a value. The *attributeSetId* value must be an already existing value in *DataHub*. You can find out an entity ID via user interface or via API, see [Link](#to-be-determined). 

Depending on the data you want to specify, you have to add the corresponding attribute in your request. For a complete list of the attributes relevant for the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute set*. Alternatively, you can find a list of all existing PIM attributes under *DataHub > Settings > Attributes*.

[comment]: <> (Stimmt das? In API Request sample gibt es mehr? 54 vs. 64 -> PIM Basic set + zusätzliche Attributen in den anderen sets?)

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

#### Create a product, specify price and dimensions (length, width, height), and add an image  

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


#### Create a product maintained in two languages  

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

[comment]: <> (Sinnvolle use cases?)

#### Create a product with a single variant

#### Create a product with multiple variants



## Edit a product

You can edit a product via API to modify any number of field values at a time. You can also add attributes to an existing product.

[comment]: <> (Stimmt das so? Use case?)

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

**Method**: POST


### Parameters

The required fields are marked in bold.

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product ID  |
| (attribute)   | ...  | ...  |



### Request samples

Edit a product to update the SKU and add dimensions (here height/depth).

    {
        "product": {
            "id": "662",
            "sku": "IP13-Test2",
            "_pim_size_h": {
                "value": 10,
                "unitId": 432
            }
        }
    }


Edit a product to update the SKU and add the product name both in English and German.

    {
        "product": {
            "id": "662",
            "sku": "IP13-Test3",
            "_pim_size_h": {
                "value": 10,
                "unitId": 432,
            "_pim_art_name__actindo_basic__en_US": "Smartphone",
            "_pim_art_name__actindo_basic__de_DE": "Cooles Handy"
            }
        }
    }

[comment]: <> (Komischerweise hat das nicht funktioniert. Wieso?)



## Delete a product

You can delete a product if it is no longer needed. 

> [Caution] If it is a master product, that is, with product variants, all variants will also be deleted. If it is a product variant, only the variant will be deleted.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.delete

**Method**: POST

### Parameters

The required fields are marked in bold.

| Attribute   | Type | Description |  
| ----------- | ----------- | ---------- | 
| **id**      | integer    |  Product ID |
| (attribute) | (type) | ... |


### Request sample



## List products

Get a list of all products including the ones in the archive or recycle bin. You can set one or more filters to 

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.getList

**Method**: POST

### Definitions / Parameters

The required fields are marked in bold.

[comment]: <> (Keine required? Wenn man filter, hints, sort objects setzen will, dann mit required Felder) 

| Field      | Type | Description |  
| ----------- | ----------- | ---------- | 
| filter      | Array of objects    |  ... |
| hint   | integer  | ...  |



### Request sample  

Get a list setting a filter.

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


Other use cases

Add Images
