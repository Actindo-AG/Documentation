# Variant products

You can create, edit, delete, and list *PIM* variant products via API. The endpoint */Actindo.Modules.Actindo.PIM.Variants.create* allows you to manage variant products within an existing master product. 

The keys are customer-defined in *PIM*. Therefore, the fields displayed in the request samples should just serve as an example.   

> [Caution] If you modify a key in the *DataHub* or *PIM* modules, which is strongly discouraged, the key in the API changes as well. This means that the field may not be found when sending a request. In this case, you have to update the key, that is, the field, in your request body as well.


## Create a variant product

Create a single or multiple variant products at once to a existing master product.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Variants.create

### Definitions

The required fields are marked in bold.

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **masterId**      | integer   |  Master product identification number |
| **variantSetId**   | integer  | Variant set identification number |
| **variants** | array of objects | It contains the required field **definingAttributeValues**, and the optional *differingAttributeValues* and *additionalFields*. | 


You have to include all required fields in the JSON file and provide them with a value. The **masterId** and **variantSetId** values must be existing values in *DataHub*. To find out the entity ID, see [Entity ID](./02_Basics.md#entity-id). 

Depending on the data you want to specify, you have to add the corresponding fields in your request. For a complete list of the fields relevant for the variant set of the variant product you want to add, you can check the corresponding variant set in the *PIM* module under *PIM > Settings > Variant sets*. Alternatively, you can find a list of the existing variant products, if any, and the assigned variant set for a specific master product under *PIM > Products > Select a master product > Tab Variants*.

[comment]: <> (Stimmt das? Sinnvoll zu erklären?)

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).


### Sample: Create a single variant product

    {
        "masterId": 881,
        "variantSetId": 91,
        "variants": [
            {
                "definingAttributeValues": {
                    "_pim_ean": 123456789
                },
                "additionalFields": null
            }
        ]
    }


### Sample: Create multiple variant products 


    {
        "masterId": 881,
        "variantSetId": 91,
        "variants": [
            {
                "definingAttributeValues": {
                    "_pim_ean": 234567890
                },
                "additionalFields": null
            },
            {
                "definingAttributeValues": {
                    "_pim_ean": 345678912
                },
                "additionalFields": null
            }
        ]
    }



## Edit a variant product

You can edit a single o multiple variant products at once via API, for example, to add an image or update the price. 
To edit a variant product, see [Edit a product](./03_Products.md#edit-a-product).

Bear in mind that only variant-specific attributes, such as EAN code, image, color, or size, can be modified in the variants. Values that are inherited from the master product, such as product name, description, or tax class, can only be updated in the parent product. 

The variant-specific attributes must be included in the variant set.


## Delete a variant product

To delete a variant product, see [Delete a product](./05_Products.md#delete-a-product).


## List variants to a master product

[comment]: <> (Überhaupt möglich???)

Get a list of variants to a master product. You can set one or more filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.getList


### Definitions

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| ids | array of integer (?) | Bedeutung ? |
| query | string | Quick search for a query string |
| fields | array of strings | Quick Search for query fields; null to search for all fields |
| filter | array of objects | To set a filter. It contains the required fields **property** (field to filter), **operator**, and **value**. |
| hints | array of objects | It contains the required fields **name** (name of the hint) and **value** (value of the hint). |
| sort | array of objects | It contains  the required fields **field** (field to sort) and **order** ("ASC" for ascending and "DESC" for descending).  |
| start | integer | Pagination: Pagination start (from 0) |
| limit | integer | Pagination: Pagination limit |


### Request sample  

#### Get a list of variants setting a filter

    {
      "ids": 0,
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
      "limit": 0
    }









