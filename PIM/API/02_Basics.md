# Basics on Actindo Core1 OpenAPI

## Attribute keys  

All attributes defined in the *DataHub* module have a key. This key is required for API access and therefore must be system wide unique. 

An attribute key must fulfill the following criteria:
    - valid characters are **a-z** (upper and lower case), **0-9** and the underscore ( **_** )
    - the key must not start with a number
    - a double underscore ( **___** ) and a trailing underscore are forbidden

[comment]: <> (Das stimmt nicht, mit dem double underscore, oder?)

Attribute key structure:

\_owning module_

For detailed information on how to create an attribute, see [Create an attribute](../../DataHub/Integration/01_ManageAttributes.md#create-an-attribute).




The attribute key is customer-defined in *DataHub*. Therefore, the fields displayed in the request samples should just serve as an example.   

If you modify a key in *DataHub*, which is not recommended, the key in the API changes as well. That means, that the field may not be found when sending a request.

## Required attributes  

Attributes can be required or optional. Required attributes must always be provided when sending a request

## Data types  



## Format  

The *Actindo Core1 OpenAPI* endpoints accept requests in JSON format. 

