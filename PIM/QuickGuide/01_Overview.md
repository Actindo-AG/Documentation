# Overview

This quick guide gives an short overview over the steps to take to configure the basic data model of the *PIM* module. All steps are illustrated with examples and graphics.

For detailed information about the certain steps, please refer to the corresponding chapters in the *PIM* module documentation.


## PIM data model

The *PIM* module is based on a structured data model that enables efficient management and organization of product data. This model consists of various components that together form a flexible and powerful system.


### Attributes

Attributes are the building blocks of product data and form the foundation of the PIM data model. They represent individual data fields where specific product information is stored and maintained. Each attribute represents a single data field and can has a certain data type in order to capture different types of information. The different data types are described in details in the *DataHub* module, see [Data type list](../../DataHub/UserInterface/05_DataTypeList.md).


### Attribute sets

Since different product types often require a multitude of attributes, but not every product needs all of these attributes, attributes are organized in so-called attribute sets. These attribute sets allow the definition and maintenance of specific attributes for certain product types. When a product is created within an attribute set, only the attributes assigned to that set are displayed during data maintenance for that product. This ensures a clear and efficient data entry process.

> Example: Your product range includes different shirts, trousers and dresses as well as smartphones and tablets. Therefore, you have to maintain attributes such as *collar size*, *sleeve length*, *fit*, but also *storage*, *screen size* and *ports*.   
> You create the *Clothing* and the *Mobile devices* attribute sets and assign the *collar size*, *sleeve length* and *fit* attributes to the *Clothing* attribute set and the *storage*, *screen size* and *ports* attributes to the *Mobile devices* attribute set. This way, products that are assigned to the *Clothing* attribute set only contain the clothing specific attributes and products that are assigned to the *Mobile devices* attribute set contain the mobile devices specific attributes.        

[comment]: <> (Grafik zu Beispiel einfügen)


### Attribute groups

For better structuring attributes within the product, attributes are organized into groups. These groups are used to organize and group related attributes in the product. An attribute can only belong to one attribute group.

The hierarchy of attribute groups is limited to two levels:

1. Attribute groups: These are the main attribute groups. Users can quickly switch between different attribute groups by clicking them.
2. Attribute subgroups: Each main attribute group can contain an unlimited number of subgroups. Users can seamlessly scroll between attribute subgroups.

    > [Info] Subgroups cannot have any further subgroups. The hierarchy ends at the second level. 


### Variant sets

Variant sets are intricately linked to attribute sets. The system must be aware of which attributes are available for variation, ensuring a clear structure for product differentiation. This connection between variant sets and attribute sets forms the foundation for effective product variation.

Within the *Actindo Core1 Platform*, attributes are categorized into two main types:
    - *Defining attributes*: These are core characteristics that distinguish one variant from another, for example the color.
    - *Changeable attributes*: These attributes are not characteristic for a variant but also distinguish one variant from another, for example a product image. 


### Variants

Variants are created in the master product itself. Therefore, it is important to consider the correct attribute set and variant set when creating a variant to a product. Variants inherit most of their data from their master product. By default, data from the master product is passed down to its variants and cannot be directly edited in the variant itself. This inheritance model ensures consistency across product variations. 
However, certain attributes need to be managed differently for variants. These are the defining attributes on the one hand, which are already set when creating the variants and the changeable attributes on the other hand, which must be maintained specifically for each variant. 


## Sample scenario

In the following chapters, you will encounter examples that consistently refer to the following initial scenario:

The product catalog of company *ABC* primarily includes shirts, pants, dresses, smartphones, and tablets. As the company is adopting the *Actindo Core1 PLatform*, they need to develop a data model that efficiently captures their products with minimal maintenance effort. 
This scenario will serve as a foundation for illustrating various concepts and techniques related to data modeling, ensuring a practical understanding of how these principles can be applied in the *Actindo Core1 Platform*.
