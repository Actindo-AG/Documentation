[!!Configure the printer for POS](./03_ConfigurePrinter.md)
[!!Open a pay desk](../Operation/01_OpenPayDesk.md)
[!!User interface Stores](../UserInterface/02b_Stores.md)
[!!User interface PIM Attributes](../../PIM/UserInterface/03a_Attributes.md)
[!!User interface DataHub ETL](../../DataHub/UserInterface/02a_Mappings.md)

# Create a POS store manually

Alternatively to using the [store wizard](./06_CreateStore.md#create-a-store-using-the-wizard), you can create a store manually. Be aware that to use the store and its full functionality, it is necessary to configure the following settings manually:
- [Configure the store details](#configure-the-store-details)
- [Create a pay desk](#create-a-pay-desk)
- [Configure the pay desk details](#configure-the-pay-desk-details)
- [Define a printer](#define-a-printer)
- [Define the store address](#define-the-store-address)
- [Assign the POS warehouse](#assign-the-pos-warehouse)
- [Configure the stock withdrawal matrix](#configure-the-stock-withdrawal-matrix)
- [Assign the stock source](#assign-the-stock-source)
- [Assign the accounts](#assign-the-accounts)  

In addition, you can use these procedures to edit the store settings if you need to make changes to the settings you created when you used the wizard for store creation. <!---Ist das richtig?-->



## Create a store manually

Create a store manually, if you do not want to use the wizard.

#### Prerequisites

- A warehouse for POS is configured, see [Configure the warehouse for POS](./01_ConfigureWarehouse.md).
- The accounts for POS are configured, see [Manage the accounts for POS](./02_ManageAccounts.md).
- The printer for POS is configured, see [Configure the printer for POS](./03_ConfigurePrinter.md).
- The users are assigned to the POS groups, see [Assign users to the POS groups](./04_AssignUsers.md).
- The global settings for POS are configured, see [Configure the global settings for POS](./05_ConfigureGlobalSettings.md).


#### Procedure

*Venduo POS > Management > Tab STORES*

![Create Store](../../Assets/Screenshots/POS/Management/Stores/Stores.png "[Create Store]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The [Create store via wizard (recommended) ![Store Wizard](../../Assets/Icons/Tool.png "[Store Wizard]") ] button and the [Create Store ![Store Manual](../../Assets/Icons/Plus02.png "[Store Manual]") ] button are displayed.

2. Click the [Create Store ![Store Manual](../../Assets/Icons/Plus02.png "[Store Manual]")] button to add a new store manually.   
    The *Create Store* window is displayed.

    ![Create Store](../../Assets/Screenshots/POS/Management/Stores/CreateStore.png "[Create Store]")

3. Enter a store name in the *Name* field.

4. Click the [CREATE] button.   
    The *Creating Store...* message is displayed. It may take several minutes until the creation is completed. The new store is displayed in the *STORES* tab. The *Basic data* tab is displayed by default.

    ![Store Details](../../Assets/Screenshots/POS/Management/Stores/Store/BasicData/BasicData.png "[Store Details]")

    The following entities have been automatically created:
    - *DataHub* module:   
        The following attribute sets have been created<!--- Ist das richtig?-->:
        - Orders channel POS Store "Name of new store"
        - Line items channel POS Store "Name of new store"
        - Payment items channel POS Store "Name of new store"
        - Discount items channel POS Store "Name of new store" 
        - Returns connection POS Store "Name of the new store"
        - Return line items channel POS Store "Name of the new store"
        - Redeem voucher item channel POS Store "Name of the new store"
        - Service items channel POS Store "Name of the new store"  
        - Set for POS store "Name of new store"
        - Offer option set for POS store "Name of the new store" 
    - *PIM* module   
        Your customer-specific PIM attribute sets have been created for the new store with a destination attribute set *Set for POS store "Name of the new store"*
    - *Omni-Channel* module   
    The following attribute sets have been created:    
        - A connection *POS store "Name of new store"*
        - A variant set *Set for POS for "Name of the new store"* 
        - A variant set *Offer option set for POS store "Name of the new store"* 


## Configure the store details

In the store details, you give some detailed information about your store. Further, you assign a store manager.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- The users are assigned to the POS groups, see [Assign users to the POS groups](./04_AssignUsers.md).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Store Details](../../Assets/Screenshots/POS/Management/Stores/Store/BasicData/BasicData.png "[Store Details]")

1. Enter a short description of the store in the *Short description* field.

2. Click the *TSS connection* drop-down list and select the required TSS connection. For detailed information on TSS connections, see [Create connection to TSS Provider](./10_TSSProviderConnection.md).

2. Click the [ADD] button in the *Store manager* box.   
    The *Store managers* window is displayed.

3. Select a store manager from the list by selecting the corresponding checkbox.

    > [Info] The store managers list displays all users who are assigned to the POS store manager group. You may select multiple users as store managers.    
    For detailed information, see [Assign users to the POS groups](./04_AssignUsers.md).

4. Click the [Add] button in the upper right corner of the window.

5. Click the [SAVE] button left below the *Store manager* box.   
    The store manager is saved. The *Stores* view is displayed and the *STORES* tab is preselected.




## Create a pay desk

Create at least one pay desk to be able to process any type of transaction via *Venduo POS*.

A pay desk can be used in different manners. You can consider a pay desk as a physical unit and consequently create one pay desk per physically existing pay desk.   
However, you can also create one pay desk per user, so that each pay desk is assigned to one specific cashier and can only be used by that cashier. In this way, you can also create several pay desks in the POS system for one physically existing pay desk.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Store Details](../../Assets/Screenshots/POS/Management/Stores/Store/BasicData/BasicData.png "[Store Details]")

1. Click the [ADD] button in the *Pay desks* box.    
    The *Create pay desk* window is displayed.

    ![Create Pay Desk](../../Assets/Screenshots/POS/Management/Stores/Store/BasicData/CreatePayDesk.png "[Create Pay Desk]")

2. Enter a pay desk name in the *Name* field.

3. Click the [SAVE] button.   
    The new pay desk is displayed in the *Pay desks* box.

    > [Info] Repeat step 1 to 3 to add further pay desks. You can add as many pay desks as you need.

4. Click the [SAVE] button left below the *Store manager* section.   
    The pay desk is saved. The *Stores view* view is displayed, and the *STORES* tab is preselected.

[comment]: <> (Is it a feature or is it a bug?)


## Configure the pay desk details

In the pay desk details, you give some detailed information about the pay desk. Further, you assign one or several cashiers to prevent the pay desk from unauthorized access.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- At least one pay desk has been created, see [Create a pay desk](#create-a-pay-desk).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data > Select pay desk for editing*

![Basic Data](../../Assets/Screenshots/POS/Management/Stores/PayDesk/BasicData/BasicData.png "[Basic Data]")

1. If desired, enter a short description of the pay desk in the *Short Description* field.

2. Click the [ADD] button in the *Cashiers* box.    
    The *Cashiers* window is displayed.

    ![Pay Desk Cashiers](../../Assets/Screenshots/POS/Management/Stores/PayDesk/BasicData/Cashiers.png "[Pay Desk Cashiers]")

3. Select a cashier from the list by selecting the corresponding checkbox.

    > [Info] The cashiers list displays all users who are assigned to the POS cashier group. You may select multiple users as cashiers. Only cashiers who are assigned to a certain pay desk can use the pay desk.  

    For detailed information, see [Assign users to the POS groups](./04_AssignUsers.md)

4. Click the [Add] button in the upper right corner of the window.   
    The selected cashier is added to the box.

5. Click the [SAVE] button left below the *Cashiers* box.   
    The *Submitting data...* message is displayed. The cashier is saved when the *Store* view is displayed.

[comment]: <> (Is it a feature or is it a bug?)



## Define a printer

You have to define a printer for the printing of receipts.  

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- At least one pay desk has been created, see [Create a pay desk](#create-a-pay-desk).

#### Procedure

To define a printer for a specific pay desk, see [Configure the printer client for POS](./03_ConfigurePrinter.md). You just have to select the desired pay desk from the *Event* drop-down list. 

> [Info] If you configure a new printer, bear in mind that it may take some time for the newly created pay desk to be displayed in the *Event* drop-down list.



## Define the store address

The store address is required as the delivery address, which has to be defined for tax purposes. In addition, a delivery address and an invoice address should be printed on every receipt created in the POS system.

#### Prerequisites

A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Tab Settings*

![Store Basic Data](../../Assets/Screenshots/POS/Management/Stores/Store/Settings/Settings.png "[Store Basic Data]")

1. Select the *Store address* entry in the list of settings in the left column.   
    The *Store address* view is displayed on the right side.

    ![Store Basic Data](../../Assets/Screenshots/POS/Management/Stores/Store/Settings/StoreAddress.png "[Store Basic Data]")

2. Enter the store address in the fields.

    > [Info] The store address corresponds to the delivery address. You must at least enter the country and the ZIP code.   

    For detailed information, see [Stores](../UserInterface/02b_Stores.md).

3. Click the [Save] button in the upper right corner.   
    A confirmation message is displayed. The store address is saved.


## Assign the POS warehouse

To connect the warehouse management and the stock management to your POS, you have to assign a warehouse from which to take the materials. The warehouse specifies where exactly the material is taken from when a product is sold.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- A warehouse for POS is configured, see [Configure the warehouse for POS](./01_ConfigureWarehouse.md).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings*

![Store Admin Settings](../../Assets/Screenshots/POS/Management/Stores/Store/AdminSettings/AdminSettings.png "[Store Admin Settings]")

1. Select the *Warehouse assignment orders* entry in the list of settings in the left column.   
    The *Warehouse assignment orders* section is displayed on the right side.

    ![Warehouse assignment orders](../../Assets/Screenshots/POS/Management/Stores/Store/AdminSettings/WarehouseAssignment.png "[Warehouse assignment orders]")

2. Select the warehouse you want to take the material from in the *Warehouse* drop-down list.

3. Activate the *Automatically assign product to warehouse when activated in store* toggle to automate the assignment process. It is recommended to activate this option.   
For detailed information, see [Stores](../UserInterface/02b_Stores.md).

   > [Info] A product must have stock allocation in a warehouse in order to be sold from that warehouse. Products only have a stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf. The products get a shelf the first time the corresponding channels offer is activated.    
   This automation only works if you have enabled the storage of multiple items per shelf when creating the warehouse. For detailed information, see [Configure the warehouse for POS](./01_ConfigureWarehouse.md).

4. Enter a shelf number for the products in the *Shelf* field. The shelf number can be any arbitrary number.

5. Click the [Save] button in the upper right corner.   
    A confirmation message is displayed. The warehouse assignment is saved.


## Configure the stock withdrawal matrix

Define in the stock withdrawal matrix from which warehouses defined in the system the stock level is taken from.  
For detailed information on the stock withdrawal matrix, see [Configure the stock withdrawal matrix](../../RetailSuiteWarehousing/Integration/05_ConfigureStockWithdrawalMatrix.md) in the *Warehousing* documentation.

#### Prerequisites

A warehouse for POS is configured, see [Configure the warehouse for POS](./01_ConfigureWarehouse.md).

#### Procedure

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Click the [ADD] button in the bottom left corner.   
    A new row is displayed in the list.

2. Configure the following settings:

    + Select the **--all--** option in the drop-down list in the *Product group* column.
    + Select the output channel via which you want to create offers in the drop-down list in the *Sales channel* column.
    + Select the created POS store in the drop-down list in the *Account* column.
    + Select the **--all--** option in the drop-down list in the *Sub-account* column.
    + Select the **--all--** option in the drop-down list in the *Shipping provider* column.
    + Select the warehouse from which you want to take the stock in the drop-down list in the *Warehouse* column.

3. Click the [SAVE ASSIGNMENTS] button in the bottom right corner.   
    The new assignment in the stock withdrawal matrix is saved.


## Assign the stock source

Assign a stock source to manage the store stock. The stock source specifies how the stock available in the POS system is calculated. In most cases, the stock source and the warehouse are identical, but they can also differ.   

### Create a stock attribute

#### Prerequisites

No prerequisites to fulfill.

[comment]: <> (Muss ein entsprechendes Attributset existieren?)

#### Procedure

*PIM > Settings > Tab ATTRIBUTES*

![PIM Attributes](../../Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[PIM Attributes]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create attribute* view is displayed.

    ![Create attribute](../../Assets/Screenshots/PIM/Settings/Attributes/CreateAttribute.png "[Create attribute]")

2. Enter an appropriate name for the attribute in the *Name* field, for instance **Stock test store**.

3. Enter an appropriate key in the *Key* field.

    > [Info] Only alphanumeric characters and _ are allowed. The key has to start with a letter. Blank spaces are not permitted in the *Key* field.

4. Select the **Stock value** option in the *Data type* drop-down list.

5. Click the ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add) button in the *Assigned sets* section.   
    A new drop-down list is displayed in the *Assigned sets* section.

6. Select the corresponding set in the *Assigned sets* drop-down list.

7. Click the [SAVE] button in the upper right corner.   
    The attribute is saved. The page *Create attribute* is closed.

8. Press the **F5** key to initialize the *Core1 Platform*.


### Configure the stock allocation

Configure the stock allocation. For detailed information, see also [Configure the stock allocation](../../RetailSuiteWarehousing/Integration
/04_ConfigureStockAllocation.md "[Configure the stock allocation]")

#### Prerequisites

- A warehouse for POS is configured, see [Configure the warehouse for POS](./01_ConfigureWarehouse.md).
- A stock attribute has been created, see [Create a stock attribute](#create-a-stock-attribute).

#### Procedure

*Warehousing > Settings > Tab WAREHOUSE > Tab Stock allocation*

![Stock allocation](../../Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockAllocation/StockAllocation.png "[Stock allocation]")

1. Select the row with the stock allocation attributes name.

2. Double-click the field with the **Default (Calculation, stock)** option in the *Stock calculation* column.   
    A drop-down list is displayed.

3. Select the **Calculation, stock** option in the drop-down list in the *Stock calculation* column.   
    The fields in the warehouse columns are unlocked.

4. Double-click the option in a warehouse column to display the drop-down list.

5. Select the **Yes** option in the drop-down list to include the corresponding warehouse in the stock allocation calculation or select the **No** option to exclude it.

    > [Info] Select for each warehouse whether it should be included or not.

6. Click the [Save] button in the bottom right corner.   
    The stock allocation is saved. When the stock in a warehouse that is included in the formula is changed, the stock will be entered automatically in the stock field.


### Map the attribute to the stock of the store

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- A stock attribute has been created, see [Create a stock attribute](#create-a-stock-attribute).

#### Procedure

*DataHub > ETL > Tab MAPPINGS*

![Mappings](../../Assets/Screenshots/DataHub/Settings/ETL/AttributeSetMappings.png "[Mappings]")

1. Select the checkbox of the mapping with the new store as a destination attribute set in the list of attribute set mappings and click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button in the editing toolbar in the upper right corner.   
    The *Mapping* view is displayed.

    ![Mapping](../../Assets/Screenshots/DataHub/Settings/ETL/Mapping.png "[Mapping]")

2. Click the row with the destination attribute **Stock** in the list of mappings.   
    The *Settings* section is displayed on the right side.

    ![Mapping Settings](../../Assets/Screenshots/DataHub/Settings/ETL/MappingSettings.png "[Mapping Settings]")

3. Select the **Basic Mapping** option in the *Extension* drop-down list in the *Settings* section.

4. Select the stock attribute in the *Source attribute* drop-down list.

5. Click the [SAVE] button in the upper right corner.   
    The mapping is saved.

6. Select the checkbox of the new mapping and click the [RERUN SELECTED MAPPING] button.   
    The mapping is executed again.

    > [Info] If necessary, repeat step **2** to **6** for all mappings with the store as a destination attribute.


## Assign the accounts

In this step you assign the accounts to which you want to post the payments.   
You may assign the same accounts to all stores, or you may assign different accounts per store or even per pay desk. Depending on your choice, you have to assign the accounts in different places:   
- To [assign the same accounts to all stores](#assign-the-accounts-in-the-global-settings), enter the accounts in the global settings.
- To [assign the accounts to a single store](#assign-the-accounts-in-the-store-settings), enter the accounts in the admin settings of the respective store.
- To [assign the accounts to a single pay desk](#assign-the-accounts-in-the-pay-desk-settings), enter the accounts in the admin settings of the respective pay desk.


    > [Info] Note that the more specific settings always override the more general settings.

    This means that the accounts specified in the pay desks admin settings are always used first. If none are specified there, the accounts from the store admin settings are used and only when nothing is specified there, the accounts from the global settings are used.

### Assign the accounts in the global settings

To assign the same accounts to all stores, you may enter the account numbers in the global settings.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- The global settings for POS are configured, see [Configure the global settings for POS](./05_ConfigureGlobalSettings.md).
- The accounts for POS are configured, see [Manage the accounts for POS](./02_ManageAccounts.md).

#### Procedure

*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Account allocation Accounting*

![Allocate accounts global settings](../../Assets/Screenshots/POS/Management/GlobalSettings/AccountAssignAccounting.png "[Allocate accounts global settings]")

1. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies.    
    For detailed information, see [Manage the accounts for POS](./02_ManageAccounts.md).

2. Click the [Save] button in the bottom right corner of the window.   
    A confirmation message is displayed. The account assignment is saved.



### Assign the accounts in the store settings

To assign the accounts to a single store, you may enter the account numbers in the store admin settings.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- The accounts for POS are configured, see [Manage the accounts for POS](./02_ManageAccounts.md).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings > Entry Account assignment*

![Assign accounts in store settings](../../Assets/Screenshots/POS/Management/Stores/Store/AdminSettings/AccountAssignment.png "[Assign accounts in store settings]")

> [Info] In the top right corner, the *Apply from global* toggle is displayed. Activate the toggle to apply the account assignment from the global settings. 

When the toggle is active, all fields in the detail view are locked. By default, this toggle is inactive.

1. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies.    
For detailed information, see [Manage the accounts for POS](./02_ManageAccounts.md).

2. Click the [Save] button in the bottom right corner of the window.   
    A confirmation message is displayed. The account assignment for the selected store is saved.



### Assign the accounts in the pay desk settings

To assign the accounts to a single pay desk, you may enter the account numbers in the pay desk admin settings.

#### Prerequisites

- A store has been created, see [Create a store manually](#create-a-store-manually) or [Create a store using the wizard](./06_CreateStore.md#create-a-store-using-the-wizard).
- At least one pay desk has been created, see [Create a pay desk](#create-a-pay-desk).
- The accounts for POS are configured, see [Manage the accounts for POS](./02_ManageAccounts.md).

#### Procedure

*Venduo POS > Management > Tab STORES > Select Store > Select Pay Desk > Tab Admin Settings > Entry Account assignment*

![Assign accounts pay desk settings](../../Assets/Screenshots/POS/Management/Stores/Store/AdminSettings/AccountAssignment.png "[Assign accounts pay desk settings]")

> [Info] In the top right corner, the *Apply from global* toggle is displayed. Activate the toggle to apply the account assignment from the global settings.   

When the toggle is active, all fields in the detail view are locked. By default, this toggle is inactive.

1. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies.    
    For detailed information, see [Manage the accounts for POS](./02_ManageAccounts.md).

2. Click the [Save] button in the bottom right corner of the window.   
    A confirmation message is displayed. The account assignment for the selected pay desk is saved.

