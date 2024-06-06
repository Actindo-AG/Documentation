# Manage variant products

You can create a single or multiple variant products to an existing master or a master-to-be single product via API addressing the endpoint */Actindo.Modules.Actindo.PIM.Products.createVariants*. 

To edit and delete *PIM* variant products via API, see [Manage products](./05_ManageProducts.md). 

> [Caution] In the latest version of the *PIM* and *DataHub* modules, it is possible to modify the attribute key. Bear in mind, though, that attribute keys are used for API access. Changing the attribute key, which is strongly discouraged, has an impact on the API naming for all affected entities where this attribute is included. This means that all external API consumers, workflows, webhooks, or other custom code need to be adjusted accordingly in case any of them address this attribute.

[comment]: <> (Evtl. Manage variant products in Manage products integrieren)

## Create a variant product

Create a single or multiple variant products at once to a existing master product.

**Endpoint**: /Actindo.Modules.Actindo.PIM.Products.createVariants

#### Definitions

The required fields are marked in bold.

| Attribute key     | Data type | Description | Comments | 
| ----------- | ----------- | ---------- | ------ | 
| **parentProduct**  | object |  Master product identification number | It contains the required field **id** (integer). |
| **variantSet**   | object  | Variant set identification number | It contains the required field **id** (integer). |
| **variants** | array of objects | Variant product definition | It contains the required field **sku** (string), the required object **definingAttributeValues**, and the optional object *differingAttributeValues*. The objects **defining AttributeValues** and *differingAttributeValues* contain the attributes configured in the variant set. | 


All entity ID values must be existing values in *DataHub*. To find out the entity ID, see [Retrieve entity data](./04_RetrieveEntityData.md). 

Depending on the data you want to specify, you need to add the corresponding attribute keys in your request. For a complete list of the attributes contained in the variant set of the variant product you want to add, you can check the corresponding variant set in the *PIM* module under *PIM > Settings > Variant sets*. Alternatively, you can find a list of the existing variant products, if any, and the assigned variant set for a specific master product under *PIM > Products > Select a master product > Tab Variants*.


### Sample: Create a single variant product

    {
        "parentProduct": {
              "id": 1171
        },
        "variantSet": {
            "id": 91
        },
        "variants": [
            {
                "sku": 1111,
                "definingAttributeValues": {
                    "_pim_ean": "123456789"
                },
                "differingAttributeValues": null
            }
        ]
    }


### Sample: Create multiple variant products


        {
            "parentProduct": {
                "id": 111
            },
            "variantSet": {
                "id": 11
            },
            "variants": [
                {
                    "sku": "variant-1",
                    "definingAttributeValues": {
                        "_pim_ean": "1234"
                    },
                    "differingAttributeValues": null
                },
                {
                    "sku": "variant-2",
                    "definingAttributeValues": {
                        "_pim_ean": "5678"
                    },
                    "differingAttributeValues": null
                }
            ]
        }



## Edit a variant product

You can edit a single or multiple variant products at once via API, for example, to add an image or update the price. 
To edit a variant product, see [Edit a product](./05_ManageProducts.md#edit-a-product).

Bear in mind that only variant-specific attributes such as EAN code, image, color, or size, can be modified in the variants. Values that are inherited from the master product, such as product name, description, or tax class, can only be updated in the parent product. 

The variant-specific attributes must be included in the variant set.



## Delete a variant product

To delete a variant product, see [Delete a product](./05_ManageProducts.md#delete-a-product).



## List variant products

To get a list of variant products, see [List products](./05_ManageProducts.md#list-products).



[comment]: <> (Kann man Variants to ein Master auflisten? Sinnvoll? Bisher nur via PIM.PIM.Get -> entityId geschafft)








