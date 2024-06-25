[!!Create a store in POS](./06_CreateStore.md)
[!!Manage the POS warehouse](./08_ManageWarehouse.md)
[!!Handle an out-of-stock order](../Troubleshooting/01_OutOfStockOrder.md)
[!!configure the warehouse groups](../../RetailSuiteWarehousing/Integration/01_ConfigureWarehouseGroups.md)
[!!Configure the warehouses](../../RetailSuiteWarehousing/Integration/02_ConfigureWarehouses.md)


# Configure the warehouse for POS

As a POS system usually has its own warehouse and is separated from the main warehouse, a new POS warehouse should be created in advance.
Therefore, it is recommended to create a new warehouse group and integrate all warehouses made specifically for POS into this group.


## Create a warehouse group

Create a warehouse group to which you can assign all specific warehouses for your POS store, for instance a sales warehouse, a returns warehouse, and a storage area for blocked stock.

#### Prerequisites

The *Warehouse groups* plugin must be installed. 

#### Procedure

For detailed information, see [Create a warehouse group](../../RetailSuiteWarehousing/Integration/01_ConfigureWarehouseGroups.md#create-a-warehouse-group) in the *Warehousing* documentation.


## Create a warehouse

Create one or more specific warehouses for your POS store from which the stock is taken.

#### Prerequisites

A warehouse group has been created.

#### Procedure

For detailed information, see [Create a warehouse](../../RetailSuiteWarehousing/Integration/02_ConfigureWarehouses.md#create-a-warehouse) in the *Warehousing* documentation.