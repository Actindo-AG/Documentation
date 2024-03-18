[!!Configure the warehouse groups](./01_ConfigureWarehouseGroups.md)
[!!Configure the warehouses](./02_ConfigureWarehouses.md)
[!!User interface Warehouse](../UserInterface/03a_Warehouse.md)


# Configure the stock withdrawal matrix

The stock withdrawal matrix is designed to determine automatically from which warehouse and under which conditions stock is withdrawn. You can configure the following parameters: 

- Country of delivery: The country where the order is to be delivered.  
- Sales channel: The output channel via which you want to create offers, for example, the *Omni-Channel* module.  
- Account: The connection used in the *Omni-Channel* module, for example, Salesforce Commerce Cloud or POS.  
- Sub-account: The shop where the order is placed, for example, the online store in Germany or in the US.  
- Shipping provider: The shipping service provided, for example, in case of express delivery, the material can be taken from a warehouse, and in case of standard delivery, from a different one.  
- Warehouse: The specific warehouse from which the stock should be withdrawn.  
- Warehouse group: The warehouse group from which the stock should be withdrawn. This information is optional. If both warehouse and warehouse group are specified, the warehouse must be included in the warehouse group.

The stock withdrawal matrix is a so-called priority list, that is, a list of criteria arranged in descending order based on their priority. Therefore, the correct order of these criteria is crucial, as the system goes through them in the order they are listed, starting from the top, and stops checking them as soon as a matching criterion is found. For example, if two entries have the same matching criteria, the system withdraws the stock from the warehouse that comes first until there is no more materials in stock, and then it goes to the next one.   



## Create an entry

Create an entry to determine a set of criteria to withdraw stock from a specific warehouse.

#### Prerequisites  

At least one warehouse has been created, see [Create a warehouse](./02_ConfigureWarehouses.md#create-a-warehouse).

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Click the [ADD] button in the bottom left corner.   
    A new data input line is displayed.

2. Double-click the field in the *Delivery address country* column and select the desired country from the drop-down list.  

    > [Info] The small red triangle in the left upper corner of the field indicates that the marked field has been changed.  
    
3. Leave the fields in the *Product group* column unchanged. The default setting is **all**. 

    > [Info] This function is no longer supported. Therefore, it is not described in this documentation.

4. Double-click the field in the *Sales channel* column and select the channel where the order originates. The following options are available: 

    - **All**  
        Select this option for all sales channels.
    - **None**  
        Select this option for orders that are manually created via the *Order Management* module.
    - **Core 1 Channels**  
        Select this option for all sales channels connected via the *Omni-Channel* module. 
    - **Shop**   
        Select this option for orders imported via the *Multimarkets* module. This module is currently being replaced by *Omni-Channel*.  

[comment]: <> (Julian: Bitte Shop/Multimarkets-Info prüfen)

5. Double-click the field in the *Account* column and select a connection. All connections available in the *Omni-Channel* module are displayed in the list.

6. If necessary, double-click the field in the *Sub-account* column and select the appropriate sub-account, that is, the specific sub-shop where the order has been placed.

7. If desired, double-click the field in the *Shipping provider* column and select a shipping provider. You can configure the shipping providers in the *Order Management* module under *Settings > Tab SHIPPING PROVIDER > Shipping*.

8. Double-click the field in the *Warehouse* column and select the warehouse from which the stock should be withdrawn. All available warehouses are displayed in the list.

9. If desired, double-click the field in the *Warehouse group* column and select the warehouse group from which the stock should be withdrawn. All available warehouses are displayed in the list. 

    > [Info] You can indicate the warehouse group generally or specify more precisely the exact warehouse within a warehouse group where the stock has to be taken from. When both warehouse and warehouse group are specified, the warehouse must be included in the warehouse group.

10. Click the [SAVE ASSIGNMENTS] button in the bottom right corner.   
    The entry in the stock withdrawal matrix is saved.

    > [Info] Repeat steps **1** to **10** to add further entries.



## Edit an entry

Once you have created an entry, you can edit it.

#### Prerequisites  

An entry has been created, see [Create an entry](#create-an-entry). 

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Select the entry you want to edit.

2. Edit the settings as necessary by double-clicking in the corresponding field.  
    
    > [Info] The small red triangle in the left upper corner of the field indicates that the marked field has been changed.
    
3. Click the [SAVE ASSIGNMENTS] button in the bottom right corner.   
    The new assignment in the stock withdrawal matrix has been saved.



## Delete an entry

Once you have created an entry, you can delete it.

#### Prerequisites  

An entry has been created, see [Create an entry](#create-an-entry). 

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Select the entry you want to delete.

2. Click the [DELETE] button in the bottom right corner.   
    The entry has been removed from the stock withdrawal matrix.




