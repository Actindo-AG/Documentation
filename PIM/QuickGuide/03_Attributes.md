# Attributes

When creating attributes for attribute sets, several key steps and considerations are involved.

## Create an attribute

*PIM > Settings > Tab ATTRIBUTE > Button [Add]*

1. Complete the following fields:
    - *Name*: Enter a clear, descriptive name for the attribute.
    - *Description*: If desired, enter an attribute description to provide additional context.
    - *Data type*: Select the appropriate data type, which determines: 
        - How data must be imported via API
        - The format for CSV imports
        - How the attribute is displayed in the UI 
    - *Key*: Enter a key for the attribute set. The key serves as a unique identifier at the database level and is mandatory. It is recommended to use a consistent naming structure for keys, such as including a prefix like **pim_**. This practice helps to identify the origin of attributes within the *DataHub* module. 
        > [Info] The key name be updated when modifying an attribute. Nevertheless, you should only rename the key in exceptional cases in order to avoid problems with existing references.

2. Configure the following toggles:
    - *Multi-language*: Enable the toggle to determine the attribute as multi-language. This setting is useful for attributes that vary by language. 
    - *Multi-scope*: Enable the toggle to determine the attribute as multi-scope. This setting is useful for attributes that vary by scope, for example for different product names in various sales channels (Amazon, Shopware, eBay) 
        > [Info] The use of multi-language and multi-scope attributes helps to keeps the attribute structure lean by avoiding multiple attributes.
    - *Active*: Enable the toggle to set the attribute active and available for selection when adding to attribute sets.
    - *Contains sensitive data*: Enable the toggle to indicate that the attribute contains data that should not always be visible to everyone.

    [Comment]: <> (Welche Auswirkungen hat es, wenn ich das Feld aktiviere?)


3. Configure the attribute set assignment:
    - *Assigned attribute sets*: Add the attribute set(s) to which the attribute should be assigned by clicking the [Add] button.
        > [Info] You can assign the attribute to an unlimited number of attribute sets. An attribute can be used for completely different products, for example the *battery capacity* attribute can be used for mobile devices as well as for e-bikes. 
        When inheritance is turned on for an attribute set, its attributes are automatically inherited to all linked attribute sets. This means you only need to add an attribute to the top level attribute set, and it will automatically appear in all the attribute sets below it.

4. Configure the type-specific fields.
    > [Info] Based on the selected data type, you can set further configurations for the attribute. For example, for a string attribute, you can set the minimum/maximum length, an regex, or bad words filter. For a tree node attribute, you have to create the corresponding drop-down fields.   
    > The most used data types are the following:
    > - String: Free textfield
    > - Textfield: Larger version of string attribute, selection of HTML editor possible
    > - Checkbox: On/off selection 
    > -	Floating point number: Decimal number
    > - Currency: Currency selection
    > -	Language/Countries: Fixed data types with dropdown menus, all languages and countries are preset in the system
    > - Tree node: Fixed selection of configured values
    > - Number with unit: Number and a configured unit
    > - Date/time: Date with or without time
    > - Stock value: stock value from the *Warehousing* module
    > - PIM price field: Complex data type for pricing information containing tax class, currency, promotion price, scale price  
    > Find a detailed list of all data types and their configurations in the *Datahub* module, see [Data type list](../../DataHub/UserInterface/05_DataTypeList.md).



## Sample scenario &ndash; Create an attribute

You have already created the two attribute sets *Clothes* and *Mobile devices*. 
In the following, you create specific attributes and assign them to the corresponding attribute sets. The attributes you want to create are the following:
- collar size
- sleeve length
- storage
- screen size

