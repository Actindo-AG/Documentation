# Variants

You can create, edit, delete, and list *PIM* variants via API. You can also create, edit, delete, and list variant sets. 

[comment]: <> (Edit und delete geht es übers UI aber ich finde es in API-Doku delete unter Variant nicht. S. Delete product! Variant sets via API auch sinnvoll für Kunden?)

The keys are customer-defined in *PIM*. Therefore, the fields displayed in the request samples should just serve as an example.   

> [Caution] If you modify a key in the *DataHub* or *PIM* modules, which is strongly discouraged, the key in the API changes as well. This means that the field may not be found when sending a request. In this case, you have to update the key, that is, the field, in your request body as well.


## Create a variant

[comment]: <> (Use case?)

Create one of several variants at once via API to an existing product.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Variants.create

### Definitions

The required fields are marked in bold.

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **masterId**      | integer   |  Master product identification number |
| **variantSetId**   | integer  | Variant set identification number |
| **variants** | array of objects | It contains the fields *definingAttributeValues*, *differingAttributeValues*, and *additionalFields*. | 

[comment]: <> (Kann man so viele defining und differing attribute values hinzufügen, wie man möchte? Keine als required, aber man muss mindestens ein defining attribute haben, oder? Info fehlt.)

You have to include all required fields in the JSON file and provide them with a value. The **masterId** and **variantSetId** values must be existing values in *DataHub*. To find out the entity ID, see [Entity ID](./02_Basics.md#entity-id). 

Depending on the data you want to specify, you have to add the corresponding fields in your request. For a complete list of the fields relevant for the variant set of the variant you want to add, you can check the corresponding variant set in the *PIM* module under *PIM > Settings > Variant sets*. Alternatively, you can find a list of the existing variants, if any, and the assigned variant set for a specific product under *PIM > Products > Select a master product > Tab Variants*.

[comment]: <> (Stimmt das? Sinnvoll zu erklären?)

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).


### Request samples  

#### Create a single variant


    {
      "masterId": 0,
      "variantSetId": 0,
      "variants": [
        {
          "definingAttributeValues": {},
          "differingAttributeValues": {},
          "additionalFields": "string"
        }
      ]
    }

#### Create multiple variants 


    {
      "masterId": 0,
      "variantSetId": 0,
      "variants": [
        {
          "definingAttributeValues": {},
          "differingAttributeValues": {},
          "additionalFields": "string"
        }
        {
          "definingAttributeValues": {},
          "differingAttributeValues": {},
          "additionalFields": "string"
        }
        {
          "definingAttributeValues": {},
          "differingAttributeValues": {},
          "additionalFields": "string"
        }
      ]
    }


[comment]: <> (Überhaupt möglich???)



## Edit a variant

To edit a variant, see [Edit a product](./03_Products.md#edit-a-product).

[comment]: <> (Stimmt das so?)

---

You can edit a variant via API, for example to add an image or update a value.

> [Info] Bear in mind that only variant-specific attributes, such as EAN code, image, color, or size, can be modified in the variants. Values that have been inherited from the master product, such as product name, description, or tax class, can only be updated in the parent product. 

[comment]: <> (Überhaupt möglich? Stimmt das so? Use case?)

**Endpoint**: /Actindo.Modules.Actindo.PIM.Variants.save

[comment]: <> (Gibt es das überhaupt? In meiner API-Doku in DOP nicht gefunden! Oder ist es eher via Create product?)


### Definitions

The required fields are marked in bold.

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **masterId**      | integer   |  Master product identification number |
| **variantSetId**   | integer  | PIM variant set identification number |
| **variants** | array of objects | It contains the fields *definingAttributeValues*, *differingAttributeValues*, and *additionalFields*. | 

### Request samples

#### Edit a variant to add an image


    {
      "masterId": 0,
      "variantSetId": 0,
      "variants": [
        {
          "definingAttributeValues": {},
          "differingAttributeValues": {},
          "additionalFields": "string"
        }
      ]
    }


[comment]: <> (Sinnvolle use cases?)


## List variants

Get a list of variants. You can set one or more filters.

[comment]: <> (Sinnvoll für Kunden?)

**Endpoint**: /Actindo.Modules.Actindo.PIM.Variants.listChildren

[comment]: <> (oder /Actindo.Modules.Actindo.PIM.PIM.listProducts?)


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



{
/*    "filter": [
        {
            "property": "variantStatus",
            "operator": "like",
            "value": "child"
        }
    ],*/
    "start": 0,
    "limit": 5000
}







