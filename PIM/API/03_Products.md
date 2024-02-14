# Products


## Create a product  

**Endpoint**: /Actindo.Modules.Actindo.PIM.PIM.create  

**Method**: POST

### Definitions / Parameters

The required fields are marked in bold.

| Field      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **sku**      | string    |  Product SKU |
| **attributeSetId**   | integer  | DataHub attribute set  |


### Request sample



## Edit a product



## Delete a product



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



