# Entity data

## Entity ID via user interface

You can find out any entity ID via user interface as follows:

1. Go to the module where the entity "lives", for example *DataHub > Data models > Attribute sets* to find out an attribute set ID.

2. Locate the entity whose ID you need.

3. Check the ID in the *ID* column. 

    > [Info] If the *ID* column is hidden, see [Add or remove columns](../../Core1Platform//UsingCore1/05_WorkWithLists.md#add-or-remove-columns) to display it. 


    ![Entity ID in user interface](../../Assets/Screenshots/PIM/API/EntityID_UI.png "[Entity ID in user interface]")

Alternatively, you can find out the entity ID in the URL as follows:

1. Click the entity whose ID you need.  
    The *Edit "entity"* view is displayed.

2. Check the site URL in your browser.  
    The selected entity ID is located at the end of the URL, as in the following example: 

    ![Entity ID in URL](../../Assets/Screenshots/PIM/API/EntityID_URL.png "[Entity ID in URL]")


## Entity ID via API

You can get all entity data you need via API. All entity data are provided in the response to your requests. Depending on the entity data you need, the endpoint you have to address may vary. 

In the following, a few request samples for the most common use cases are provided.

Required fields:

attributeSetId 
variantSetId 
Product ID
Attributes ID


## Get product data

Get all data stored in the database for a specific entity, for example, a product. If desired, you can also set filters. For detailed information on how to set a filter, see []()

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.get

### Definitions

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| **Id** | integer | Entity identification number |

### Request sample  

        {
            "product": {
                "id": "862"
            }
        }




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


## List attributes in attribute set

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

## List variant sets

Get a list of variant sets. You can set one or more filters.

**Endpoint**: /Actindo.Modules.Actindo.PIM.VariantSetController.getList

### Definitions

The required fields are marked in bold.

| Attribute      | Data type | Description |  
| ---------------|-----------|-------------|
| **attributeSetId** | array of integer | Attribute set identification number |
| query | string | Quick search for a query string |
| fields | array of strings | Quick Search for query fields; null to search for all fields |
| filter | array of objects | To set a filter. It contains the required fields **property** (field to filter), **operator**, and **value**. |
| hints | array of objects | It contains the required fields **name** (name of the hint) and **value** (value of the hint). |
| sort | array of objects | It contains  the required fields **field** (field to sort) and **order** ("ASC" for ascending and "DESC" for descending).  |
| start | integer | Pagination: Pagination start (from 0) |
| limit | integer | Pagination: Pagination limit |


### List variant sets request

    {
      "attributeSetId": 622,
      "start": 0,
      "limit": 5
    }


### List variant sets response

[comment]: <> (Response ist absurd lang... Abstract oder ohne response?)



