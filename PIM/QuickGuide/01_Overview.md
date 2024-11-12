# Overview

This quick guide gives an short overview over the steps to take to configure the basic data model in the *PIM* module. All steps are illustrated with examples and graphics.

For detailed information about the certain steps, please refer to the corresponding chapters in the *PIM* module documentation.

## PIM data model

The data model of the *PIM* module is composed of the following important elements:
- Attributes
- Attribute sets
- Attribute groups
- Variants
- Variant sets

### Attributes and attribute sets

An attribute is a single data field that contains the stored data and is used to maintain the products. Each attribute is a single data field with a certain data type. The different data types are described in details in the *DataHub* module, see [Data type list](../../DataHub/UserInterface/05_DataTypeList.md).

If you have different product types, you have to handle a huge amount of attributes for all products, but not all attributes are used for each product. Therefore, the attributes are organized in attribute sets that reflect the different product types. When maintaining the different products, only the attributes that are assigned to the corresponding attribute set are displayed in the product view. 

> Example: Your product range includes different shirts, trousers and dresses as well as smartphones and tablets. Therefore, you have to maintain attributes such as *collar size*, *sleeve length*, *fit*, but also *storage*, *screen size* and *ports*.   
> You create the *Clothing* and the *Mobile devices* attribute sets and assign the *collar size*, *sleeve length* and *fit* attributes to the *Clothing* attribute set and the *storage*, *screen size* and *ports* attributes to the *Mobile devices* attribute set. This way, products that are assigned to the *Clothing* attribute set only contain the clothing specific attributes and products that are assigned to the *Mobile devices* attribute set contain the mobile devices specific attributes.        

[comment]: <> (Grafik zu Beispiel einfügen)


### Attribute groups

Attribute groups are used to organize and group related attributes in the product. This structure allows for clear management of product characteristics and facilitates their assignment to products.

The hierarchy of attribute groups is limited to two levels:

1. Attribute groups: These are the main attribute groups.
2. Attribute subgroups: Each main attribute group can contain an unlimited number of subgroups.

    > [Info] Subgroups cannot have any further subgroups. The hierarchy ends at this level. 

