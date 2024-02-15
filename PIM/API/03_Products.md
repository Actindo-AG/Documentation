# Products

Create, edit, delete, and list PIM products via API. 

## Create a product  

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.create

**Method**: POST

[comment]: <> (Evtl. method weglassen, alle POST in Actindo)

### Parameters

The required attributes are marked in bold.

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string   |  Product SKU |
| **attributeSetId**   | integer  | DataHub attribute set identification number |
| pim_art_name | string | ... |
| pim_price | PIM price field | ... |
| pim_size_l | Number with unit | ... |
| pim_size_b | Number with unit | ... |
| pim_size_h | Number with unit | ... |
| pim_images | string | ... |

You have to include all required attributes in the JSON file and provide them with a value. The *attributeSetId* value must be an already existing value in *DataHub*.  

Depending on the information you want to add, you have to add the corresponding attribute. For a complete list of the attributes relevant for the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute set*. Alternatively, you can find a list of all existing PIM attributes in *DataHub > Settings > Attributes*.

[comment]: <> (Stimmt das? In API Request sample gibt es viel mehr? PIM Basic set + ...?)

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).


### Request sample  

Create a PIM product with an SKU and assign an attribute set to it.


    {
        "product": {
            "sku": "IP13-Test",
            "attributeSetId": 592
        }
    }

Create a PIM product with an SKU, price, and dimensions (length, width, height), assign an attribute set to it, and add an image.  

    {
        "product": {
            "sku": "IP13-Test",
            "attributeSetId": 592,
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
              "pim_images": "1234.jpg"
        }
    }

[comment]: <> (Andere Attribute hinzufügen, die sinnvoll sein können. Oder unterschiedliche Samples angeben, z.B. mit _pim_size_l/b/h, ... s. PIM basic set)



## Edit a product

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.save

**Method**: POST

### Parameters

The required fields are marked in bold.

| Field      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string    |  Product SKU |
| **attributeSetId**   | integer  | DataHub attribute set  |


### Request sample



## Delete a product


**Endpoint**: /Actindo.Modules.Actindo.PIM.PIM.create  

**Method**: POST

### Parameters

The required fields are marked in bold.

| Field      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string    |  Product SKU |
| **attributeSetId**   | integer  | DataHub attribute set  |


### Request sample



## List products

**Endpoint**: /Actindo.Modules.Actindo.PIM.PIM.listProducts

**Method**: POST


### Definitions / Parameters

The required fields are marked in bold.

| Field      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string    |  Product SKU |
| **attributeSetId**   | integer  | DataHub attribute set  |


### Request sample  

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



