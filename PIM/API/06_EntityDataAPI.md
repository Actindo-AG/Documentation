# Entity data via API

You can get all entity data you need via API. All entity data are provided in the response to your requests. Depending on the entity data you need, the endpoint you have to address may vary. 

In the following, a few request samples for the most usual use cases are provided.

## Get entity data

Get all data stored in the database for a specific entity, for example, a product. If desired, you can also set filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.PIM.get
**Endpoint**: /Actindo.Modules.Actindo.PIM.PIM.getEntityData

[comment]: <> (Unterschiedliche Info - warum?)

### Definitions

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| **entityId** | integer | Entity identification number |

### Request sample  

    {
        "entityId": 12
    }


## Attribute sets ID

**Endpoint:** /Actindo.Modules.Actindo.PIM.AttributeController.getListOfAttributeSets

Frage: wie für Attribute ID Kein Endpoint in AttributeController? 

### Definitions

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|


### Request sample
 
    {
       
    }


## Get a list of attributes in an attribute set

Get a list of all attributes contained in an attribute set. If desired, you can also set filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.AttributeController.getList
 
### Definitions

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| **attributeSetId** | integer | Attribute set identification number |

### Request sample

    {
      "attributeSetId": 592,
      "start": 0,
      "limit": 100
    }



## Product ID

## Variant set ID

## Attributes in variant set

