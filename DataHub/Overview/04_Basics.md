# Basics

## Our Data Model
Each of our entity types - like an Omni-Channel Order, Omni-Channel Line Item, Product Information Management Product - 
provides a very sparse set of fixed fields that are needed in order to a have functional entity type like primary identifier or stock keeping unit.
A list of available entities can be seen in under "DevTool->API->Data Models". Not all listed entities are already based on DataHub.

Data Hub allows tho extend the pre-defined fixed fields with additional fields that can store the data you need. 
In the context of DataHub we call these fields *Attributes*.

Each attribute comes with a *name*, *key* and *data type*. The latter defines the type of data an attribute can store ranging from simple string to complex price fields.
The variety of data types can be different for each tenant as every installed plugin can add their own data types.

*Attributes* can be *multi language* and/or *multi channel* which means that they can store are value for each language and scope combination.
*Channels* and *Languages* can be created to your needs.

*Attributes* are collected in so-called *Attribute Sets*. Each entity, which is the concrete instance of a given entity type, has exactly one *Attribute Set* which defines the available *Attributes*.
An *Attribute Set* can only be used for a single *entity type*.

*Attributes* are grouped in so-called *Attribute Groups*. Each attribute is assigned to exactly one *Attribute Group*.
*Attribute groups* are responsible to arrange and group the available *Attributes* when editing an entity. They do not have any other functional meaning.



## ETL
When providing fully an adjustable data models an adjustable way of data exchange is required which is our *ETL*.
ETL connects 1-N *Source Attribute(s)* to a *Destination Attribute* using a so-called *Extension*. The values of the *Source Attributes*
are extracted, transformed by the *Extension* and loaded into the *Destination Attribute*. This connection is called *Attribute Set Map*.

This process can be configured based on each connection of a *Source Attribute Set* with *Destination Attribute Set* that is needed.
This connection is called *Attribute Set Map* and contains a collection of multiple *Attribute Set Maps*.