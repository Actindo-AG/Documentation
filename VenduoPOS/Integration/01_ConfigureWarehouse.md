[!!Lager](Actindo/Lager)
# Configure the warehouse for POS

As a POS system usually has its own warehouse and is separated from the main warehouse, a new POS warehouse should be created in advance.
Therefore, it is recommended to create a new warehouse group and integrate all warehouses made specifically for POS into this group.


## Create a warehouse group

Create a warehouse group to which you can assign all specific warehouses for your POS store, e.g. a sales warehouse, a returns warehouse and a quarantine warehouse.

### Prerequisites

No prerequisites to fulfill.

### Procedure
*Lager > Einstellungen > Tab LAGER > Tab Lagerstammdaten*

![Neue Lagergruppe](/Assets/Screenshots/Lager/Einstellungen/Lager/Lagerstammdaten/NeueGruppe_Basisdaten01.png "[Neue Lagergruppe]")

| (1) |**Button [NEUE GRUPPE]**|
|-----|---------------------|
|**(2)**|**Button Refresh**|
|**(3)**|**Button [SPEICHERN]**|

1. Click the button [NEUE GRUPPE].   
  The Tab *Basisdaten* is displayed on the right side.

2. Enter a unique number for the warehouse group in the field *Warehouse number*.

3. Enter a name for the new warehouse group in the field *Warehouse name*.

4. Select a group type in the drop-down list *Group type*.   
  For detailed information, see [User Interface Lager](/Lager/UserInterface/00_UserInterface.md).

5. Click the button [SPEICHERN].

6. Click the button ![Refresh Icon](/Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) at the top of the left column.   
  The new warehouse group is displayed in the left column.

### Next steps

  - [Create a warehouse](#create-a-warehouse)
  - [Manage the accounts for POS](02_ManageAccounts.md)
  - [Configure the printer for POS](03_ConfigurePrinter.md)
  - [Assign users to the POS groups](04_AssignUsers.md)
  - [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
  - [Create a store in POS](06_CreateStore.md)
  - [Manage offers for POS](07_ManageOffers.md)
  - [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

  - [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
  - [Handle an out-of-stock order](VenduoPOS/Troubleshooting/01_OutOfStockOrder.md)


## Create a warehouse

Create one or more specific warehouses for your POS store from which the stock is taken.

### Prerequisites
A warehouse group is created, see [Create a warehouse group](#create-a-warehouse-group).

### Procedure
*Lager > Einstellungen > Tab LAGER > Tab Lagerstammdaten*

![Neues Lager](/Assets/Screenshots/Lager/Einstellungen/Lager/Lagerstammdaten/NeuesLager_Basisdaten01.png "[Neues Lager]")

| (1) | **Button [NEUES LAGER]** |
|-----|---------------------|
|**(2)**|**Button Refresh**|
|**(3)**|**Button [SPEICHERN]**|

1. Click the button [NEUES LAGER].   
  The Tab *Basisdaten* is displayed on the right side.

2. Enter a number for the warehouse in the field *Warehouse number*.

  > [Info] If the warehouse is part of a warehouse group, it is recommended to enter a number corresponding to the number range of the warehouse group.

3. Select the warehouse group in the drop-down list *Warehouse group*.

4. Enter a name for the new warehouse in the field *Warehouse name*.

5. Select the items per shelf in the drop-down list *Items per shelf*.

  > [Info] If you create a warehouse for POS, it is recommended to select the option **Multiple items per shelf** .   
  For detailed information, see [User Interface Lager](/Lager/UserInterface/00_UserInterface.md).

6. Click the button [SPEICHERN].

7. Click the button ![Refresh Icon](/Assets/Icons/Refresh01.png "[Refresh Icon]") (Refresh) at the top of the left column.   
  The new warehouse is displayed in the left column.

### Next steps

- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [Handle an out-of-stock order](VenduoPOS/Troubleshooting/01_OutOfStockOrder.md)
