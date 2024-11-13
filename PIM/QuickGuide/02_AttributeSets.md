# Attribute sets

Attribute sets are a fundamental component in organizing product data efficiently. The process of creating and managing these sets involves several key steps and considerations.

> [Info] By default, the *PIM Basic Set* is already created.


## Create an attribute set

*PIM > Settings > Tab ATTRIBUTE SETS > Button [Add]*

1. Complete the following fields:
    - *Name*: Enter a clear, descriptive name for the attribute set.
    - *Description*: If desired, enter an attribute set description to provide additional context.
    - *Key*: Enter a key for the attribute set. The key serves as a unique identifier at the database level and is mandatory. It is recommended to use a consistent naming structure for keys, such as including a prefix like **pim_set_**. This practice helps to identify the origin of attribute sets within the *DataHub* module.

2. Configure the following toggles:
    - *Active*: Enable the toggle to set the attribute set active and available for selection when creating attributes.
    - *Locked*: Disable the toggle to unlock the attribute set. When enabled, the attribute set is locked, for example to prevent further modifications to the attribute structure.

3. Configure the inheritance and copying features:
    - *Inherit/Copy values from*: Select the appropriate attribute set in the drop-down list.
    - *Inherit configuration*: Enable the toggle to inherit not only the attributes from the selected attribute set, but also their configuration.
    - *Inherit/Copy values*: Select the appropriate option in the drop-down list. The following options are available:
        - *Inherit*: Subsequent changes in the selected attribute set will be automatically adopted.
        - *Copy once*: The current attribute list from the selected attribute set is copied once, without adopting future changes.

    > [Info] These features significantly simplify the maintenance and administration of attributes and attribute sets, leading to more efficient management processes.


## Sample scenario &ndash; Create an attribute set

The product catalog of company *ABC* includes shirts, pants, dresses, smartphones, and tablets. These products can be classified in two product types:
- Clothes
- Mobile devices

 For each product type, a single attribute set is created:

[comment]: <> (add screenshot for both attribute sets)