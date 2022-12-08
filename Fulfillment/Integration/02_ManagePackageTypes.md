[!!User Interface Package types](../UserInterface/03b_PackageTypes.md)

## Manage the package types

Package types serve as suggestion for the fulfiller about the type of packaging and carrier which may be applied for a shipment. Package types can be defined using many different parameters. All relevant fields (attributes) used are mapped via ETL from the business document.  

[comment]: <> (I may not be applicable for all customers, e.g. in case of non-physical shipments or the fulfiller has his own package types defined.)

### Create a package type

Create a package type to define ...

#### Prerequisites

No prerequisite to fulfill. 

[comment]: <> (ETL basic mapping in Sandbox, in NoE test account Kd-spezifisches Mapping)

#### Procedure

*Fulfillment > Settings > Tab PACKAGE TYPES*

![Package types](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/ListPackageTypes.png "[Package types]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create package type* view is displayed.

  ![Create package type](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/CreatePackageType.png "[Create package type]")

2. Enter a name for the connection in the *Name* field.

3. Enter the maximal dimensions allowed for the package type:
    - In the *Max height* box, enter the maximal value in the *Quantity* field and click the *Unit* drop-down list to select the applicable unit.  
    - In the *Max width* box, enter the maximal value in the *Quantity* field and click the *Unit* drop-down list to select the applicable unit.  
    - In the *Max length* box, enter the maximal value in the *Quantity* field and click the *Unit* drop-down list to select the applicable unit.  
    - In the *Max weight* box, enter the maximal value in the *Quantity* field and click the *Unit* drop-down list to select the applicable unit.  
   
4. Enter the maximal monetary value for the items contained in the package type in the *Max value* box. To do so, follow the instructions below:
    - Click the [ADD PRICE] button.  
        The *Edit price* window is displayed. 

        ![Edit price](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/EditPrice.png "[Edit price]")

    - Enter the item price in the *Base price* field.

    - If desired, scale prices can be added. Click the [ADD SCALE PRICE] button.  
        The *Edit scale price* window is displayed.  

        ![Edit scale price](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/EditScalePrice.png "[Edit scale price]")

    - Enter the applicable price in the *Price* field and applicable number of units in the *From* field. 

    - Click the [SAVE] button.  
        The *Edit scale price* window is closed. The scale prices are displayed in the *Scale prices* box in the *Edit price* window. 

    - Click the [SAVE] button at the bottom of the window.  
        The *Edit price* window is closed. The entered prices are displayed in the *Max value* box.

[comment]: <> (Check ob alles default, also ob Beschreibung nötig; evtl. Verweis auf Attributes in DataHub?)

5. Carrier (Name)

6. Express toggle

7. Package type identifier

8. Ship-to country drop-down list

9. Priority

10. Additional services (shipping method)

11. Connection drop-down list



### Edit a package type

Edit a package type to update any set parameters.

#### Prerequisites

A package type has been created, see [Create a package type](#create-a-package-type).

#### Procedure

*Fulfillment > Settings > Tab PACKAGE TYPES*

![Package types](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/ListPackageTypes.png "[Package types]")

1. Click the package type to be edited. Alternatively, click the checkbox of the package type to be edited and the [EDIT] button in the editing toolbar.
    The *Edit package type* view is displayed.

2. 

[comment]: <> (Check standard Sätze!)


### Delete a package type

Delete a package type that is no longer applicable.

#### Prerequisites

A package type has been created, see [Create a package type](#create-a-package-type).

#### Procedure

*Fulfillment > Settings > Tab PACKAGE TYPES*

![Package types](../../Assets/Screenshots/Fulfillment/Settings/PackageTypes/ListPackageTypes.png "[Package types]")

1. Click the checkbox of the package type to be deleted.  
    The editing toolbar is displayed.

2. Click the [EDIT] button.
    The selected package type is deleted.

[comment]: <> (Notice displayed?)



