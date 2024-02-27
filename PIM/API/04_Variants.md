# Variants

You can create, edit, delete, and list PIM variants via API. 

---
The attribute key is customer-defined in *DataHub*. Therefore, the fields displayed in the request samples should just serve as an example.   

> [Caution] If you modify an attribute key in the *DataHub* or *PIM* modules, which is not recommended in principle, the key in the API changes as well. That means, that the field may not be found when sending a request. In this case, you have to update the attribute key in your request body as well.


## Create a variant  

You can create a product via API if you want to... 

[comment]: <> (Use case?)

**Endpoint**: /Actindo.Modules.Actindo.PIM.Variants.create

**Method**: POST

### Parameters

The required attributes are marked in bold.

[comment]: <> (product is immer als Objekt required in PIM-Doku, aber ist es nicht selbstverständlich? Muss man es in der Tabelle unten angeben?)

| Attribute      | Type | Description |  
| ----------- | ----------- | ---------- | 
| **masterId**      | integer   |  Master product identification number |
| **variantSetId**   | integer  | PIM variant set identification number |
| **variants** | array of objects | 

You have to include all required attributes in the JSON file and provide them with a value. The *...* value must be an already existing value in *DataHub*.  

Depending on the information you want to add, you have to add the corresponding ... For a complete list of the attributes relevant for the attribute set of the product you want to add, you can check the corresponding attribute set in the *DataHub* module under *DataHub > Settings > Attribute set*. Alternatively, you can find a list of all existing PIM attributes under *DataHub > Settings > Attributes*.

[comment]: <> (Stimmt das? In API Request sample gibt es mehr? 54 vs. 64 -> PIM Basic set + zusätzliche Attributen in den anderen sets?)

For detailed information on the data types, see [Data types](../../DataHub/UserInterface/04_DataTypeList.md).


### Request samples  

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

[comment]: <> (Andere Attribute hinzufügen, die sinnvoll sein können. Oder unterschiedliche Samples angeben, z.B. mit _pim_size_l/b/h...)



## Edit a variant

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



## Delete a variant

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



## List variants

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

## List children?

## 
