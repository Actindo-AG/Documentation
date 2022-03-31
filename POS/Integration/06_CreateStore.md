[!!Venduo POS](POS)
[!!Warehouse](RetailSuiteWarehousing)
[!!PIM](PIM)
[!!DataHub](DataHub)

# Create a store in POS

There are two ways to create a store in POS:  
Either you use the [wizard to create a store](#create-a-store-via-wizard) or you [create the store manually](#create-a-store-manually).   


## Create a store via wizard

The Store Wizard guides you through all steps to create a store and its full functionality. Therefore, it is highly recommended to use the wizard instead of creating a store manually.

### Prerequisites

- A warehouse for POS is configured, see [Configure the warehouse for POS](01_ConfigureWarehouse.md).
- The accounts for POS are configured, see [Manage the accounts for POS](02_ManageAccounts.md).
- The printer for POS is configured, see [Configure the printer for POS](03_ConfigurePrinter.md).
- The users are asigned to the POS groups, see [Assign users to the POS groups](04_AssignUsers.md).
- The global settings for POS are configured, see [Configure the global settings for POS](05_ConfigureGlobalSettings.md).

### Procedure

#### Start the store wizard

*Venduo POS > Management > Tab STORES*

![Stores](/Assets/Screenshots/POS/Management/Stores/Stores.png "[Stores]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] button and the [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] button are displayed.

2. Click the [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] button to start the store creation wizard.   
  The *Create Store* wizard window is displayed.

#### Configure the store details

In this step, you can add additional information for your store and assign a store manager.

![Wizard 01](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW01.png "[Store Wizard]")

1. Enter a store name in the *Store Name* field and add a short description if you like.

2. Select a store manager from the list by selecting the corresponding checkbox.

  > [Info] The store managers list displays all the users who are assigned to the POS store manager group. You may select multiple users as store managers.
    For detailed information, see [Assign users to the POS groups](04_AssignUsers.md).

3. Click the [CREATE STORE] button in the bottom right corner of the window.   
  The *Creating Store...* message is displayed. It may take several minutes until the creation is completed.  

  ![Wizard 01](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW01a.png "[Store Wizard]")

  The *Pay desks* wizard window is displayed when the store is created.


#### Configure the pay desk

In this step, you create one or several pay desks and assign cashiers.

![Wizard 02](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW02.png "[Store Wizard]")

1. Enter a pay desk name in the *PayDesk 1* field.

  > [Info] Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button right next to the pay desk name to add another pay desk. You can add as many pay desks as you need.

2. Select a cashier from the list by selecting the corresponding checkbox.

  > [Info] The cashiers list displays all the users who are assigned to the POS cashier group. You may select multiple users as cashiers. Only cashiers who are assigned to a certain pay desk can use the pay desk.
   For detailed information, see [Assign users to the POS groups](04_AssignUsers.md)

3. Click the [CREATE PAYDESKS] button in the bottom right corner of the window.   
    The *Printing* wizard window is displayed when the pay desk is created.


#### Select a printer

In this step you select a printer for the receipt printing.

![Wizard 03](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW03.png "[Store Wizard]")

> [Info] To select a printer, the printer client *APS (Actindo Print System)* must be installd and configured.   
For detailed information, see [Configure the printer client for POS](03_ConfigurePrinter.md).

1. Select a client for the pay desk in the *Client* drop-down list.

2. Select a printer for the pay desk in the *Printer* drop-down list.

3. Select a tray in the *Tray* drop-down list.

4. Select a format for printing. By default, portrait format is preselected for receipt printing.

5. Click the [SAVE PAYDESK] button in the bottom to save the printing settings for the selected pay desk.

  > [Info] If you created multiple pay desks, you can switch to another pay desk by clicking the tab with the name of the respective pay desk. You may configure different print settings for each pay desk.

6. Click the [CONTINUE] button in the bottom right corner of the window.   
  The *Store Address* wizard window is displayed when the printer is configured.


#### Enter the store address

In this step you define the store address. The store address is the delivery address, which has to be defined for tax purposes. Further, a delivery address and an invoice address should be indicated on every receipt created in the POS system.


![Wizard 04](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW04.png "[Store Wizard]")

1. Enter the store address in the fields.

  > [Info] The store address corresponds to the delivery address. You must at least enter the country and the ZIP code. For detailed information, see [Store Address](/POS/UserInterface/02b_Management.md#step-4-store-address).

2. Click the [CONTINUE] button in the bottom right corner of the window.   
    The *Saving successful* message and the *Stock* wizard window are displayed when the store address is saved.

    ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")



#### Assign a POS warehouse

In this step you assign the warehouse from which you want to take the stock from, you assign the shelf and you configure the stock withdrawal matrix. The warehouse specifies where exactly the stock is booked out when a product is sold.

![Wizard 05](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW05.png "[Store Wizard]")

1. Select the warehouse you want to take the stock from in the *Warehouse* drop-down list.

2. Activate the *Automatically assign product to warehouse when activated in store* toggle to automate the assignment process. It is recommended to activate this option.

  > [Info] A product must have stock in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf. The products get a shelf the first time the corresponding channels offer is activated.    
  This automation only works if you have enabled the storage of multiple items per shelf when creating the warehouse. For detailed information, see [Configure the warehouse for POS](01_ConfigureWarehouse.md).

3. Enter a shelf number for the products in the *Shelf* field. The shelf number can be any arbitrary number.

  > [Info] A product must have stock in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf.

4. Activate the *Configure stock withdrawal matrix* toggle to automate the configuration of the stock withdrawal matrix. It is recommended to activate this option.

5. Click the [CONTINUE] button in the bottom right corner of the window.   
  The *Stock allocation* wizard window is displayed when the warehouse assignment is saved.


#### Assign a stock source

In this step you assign the stock source to manage the store stock. The stock source specifies how the stock available in the POS system is calculated. In most cases, the stock source and the warehouse are identical, but they can also differ.

![Wizard 06](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW06a.png "[Store Wizard]")

1. Activate the *Create new stock source* toggle to add a new stock source that only considers the stock of the warehouse selected in the previous step. It is recommended to activate this option.     
  The *Select existing stock Source* drop-down list is hidden.

2. Click the [CONTINUE] button in the bottom right corner of the window.   
  The *Accounting* wizard window is displayed when the stock source assignment is saved.     


#### Assign an account

In this step you assign the accounts to which you want to book the payments.   

![Wizard 07](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW07a.png "[Store Wizard]")

1. Activate the *Account per pay desk* toggle to assign the accounts to each pay desk individually.   

  > [Info] If you deactivate the *Account per pay desk* toggle, you may only assign the accounts per store.   

2. Select the respective pay desk in the *Select Pay Desk* drop-down list.     
  A table to assign the accounts is displayed in the window.

  ![Wizard 07](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW07b.png "[Store Wizard]")


3. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies. For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

  > [Info] You only have to enter the account numbers for the accounts with the used currency. To delete the unused currencies from the list of available currencies, see [Available Currencies](/POS/UserInterface/02a_Management.md#available-currencies).

4. Click the [CONTINUE] button in the bottom right corner of the window.   
  The *Summary* wizard window is displayed when the account assignment is saved.


#### Finalize the wizard

In this step, you check if any necessary information is still missing and you complete the configuration of the store.

![Wizard 08](/Assets/Screenshots/POS/Management/Stores/StoreWizard/SW08.png "[Store Wizard]")

1. Check the summary.     

  > [Info] In the summary, missing data or problems that can lead to restrictions when using Venduo POS are indicated with a yellow warning triangle.    
    Remember these points and correct them manually afterwards if necessary.   
    The summary also indicates whether the POS can be used.  

2. . Click the [FINALIZE] button in the bottom right corner of the window.   
      The wizard window is closed and the store is configured.

### Next steps

- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [Create a store manually](#create-a-store-manually)
- [Open a pay desk](/POS/Operation/01_OpenPayDesk.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)



## Create a store manually

Alternatively to using the [store wizard](#create-a-store-via-wizard), you can create the store and all connections to the warehouse, accounting and invoicing manually.

### Prerequisites

- A warehouse for POS is configured, see [Configure the warehouse for POS](01_ConfigureWarehouse.md).
- The accounts for POS are configured, see [Manage the accounts for POS](02_ManageAccounts.md).
- The printer for POS is configured, see [Configure the printer for POS](03_ConfigurePrinter.md).
- The users are asigned to the POS groups, see [Assign users to the POS groups](04_AssignUsers.md).
- The global settings for POS are configured, see [Configure the global settings for POS](05_ConfigureGlobalSettings.md).

### Procedure

#### Start the store creation manually

*Venduo POS > Management > Tab STORES*

![Create Store](/Assets/Screenshots/POS/Management/Stores/Stores.png "[Create Store]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] button and the [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] button are displayed.

2. Click the [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] button to add a new store manually.   
  The *Create Store* window is displayed.

  ![Create Store](/Assets/Screenshots/POS/Management/Stores/CreateStore.png "[Create Store]")

3. Enter a store name in the *Name* field.

4. Click the [CREATE] button.   
  The *Creating Store* message is displayed. The new store is displayed in the *STORES* tab.

  ![Creating Store](/Assets/Screenshots/POS/Management/Stores/CreatingStore.png "[Creating Store]")

> [Info] To use the store and its full functionality, it is necessary to configure the following settings manually:
  - [Configure the store details](#configure-the-store-details-2)
  - [Create a pay desk](#create-a-pay-desk)
  - [Configure the pay desk details](#configure-the-pay-desk-details)
  - [Select a printer](#select-a-printer-2)
  - [Enter the store address](#enter-the-store-address-2)
  - [Assign the POS warehouse](#assign-the-pos-warehouse)
  - [Configure the stock withdrawal matrix](#configure-the-stock-withdrawal-matrix)
  - [Assign the stock source](#assign-the-stock-source)
  - [Assign the accounts](#assign-the-accounts)

#### Configure the store details

In the store details, you give some detailed information about your store. Further, you assign a store manager.

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Store Details](/Assets/Screenshots/POS/Management/Stores/Store/BasicData/BasicData.png "[Store Details]")

1. Enter a short description of the store in the *Short description* field.

2. Click the [ADD] button in the *Store Manager* box.   
   The window *Store Managers* is displayed.

3. Select a store manager from the list by selecting the corresponding checkbox.

  > [Info] The store managers list displays all users who are assigned to the POS store manager group. You may select multiple users as store managers.    
    For detailed information, see [Assign users to the POS groups](04_AssignUsers.md).

4. Click the [Add] button in the upper right corner of the window.

5. Click the [SAVE] button left below the *Store Manager* box.   
  The store manager is saved. The *STORES* tab is displayed.

[comment]: <> (Is it a feature or is it a bug?)

#### Create a pay desk

Create at least one pay desk to be able to process any type of transaction via Venduo POS.

A pay desk can be used in different manners. You can consider a pay desk as a physical unit and consequently create one pay desk per physically existing pay desk.   
However, you can also create one pay desk per user, so that each pay desk is assigned to one specific cashier and can only be used by that cashier. In this way, you can also create several pay desks in the POS system for one physically existing pay desk.

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Basic Data](/Assets/Screenshots/POS/Management/Stores/Store/BasicData/BasicData.png "[Basic Data]")

1. Click the [ADD] button in the *Pay desks* box.    
   The window *Create pay desk* is displayed.

   ![Create Pay Desk](/Assets/Screenshots/POS/Management/Stores/Store/BasicData/CreatePayDesk.png "[Create Pay Desk]")

2. Enter a pay desk name in the *Name* field.

3. Click the [SAVE] button.   
  The new pay desk is displayed in the *Pay desks* box.

  > [Info] Repeat step 1 to 3 to add another pay desk. You can add as many pay desks as you need.

4. Click the [SAVE] button left below the *Store Manager* section.   
  The pay desk is saved. The *STORES* tab is displayed.

[comment]: <> (Is it a feature or is it a bug?)


#### Configure the pay desk details

In the pay desk details, you give some detailed information about the pay desk. Further, you assign one or several cashiers to prevent the pay desk from unauthorized access.

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data > Select Pay Desk*

![Pay Desk Basic Data](/Assets/Screenshots/POS/Management/Stores/PayDesk/BasicData/BasicData.png "[Pay Desk Basic Data]")

1. If desired, enter a short description for the pay desk in the *Short Description* field.

2. Click the [ADD] button in the *Cashiers* box.    
   The window *Cashiers* is displayed.

   ![Pay Desk Cashiers](/Assets/Screenshots/POS/Management/Stores/PayDesk/BasicData/Cashiers.png "[Pay Desk Cashiers]")

3. Select a cashier from the list by selecting the corresponding checkbox.

  > [Info] The cashiers list displays all users who are assigned to the POS cashier group. You may select multiple users as cashiers. Only cashiers who are assigned to a certain pay desk can use the pay desk.  
   For detailed information, see [Assign users to the POS groups](04_AssignUsers.md)

4. Click the [Add] button in the upper right corner of the window.   
  The selected cashier is added to the box.

5. Click the [SAVE] button left below the *Store Manager* box.   
  The *Submitting data...* message is displayed. The cashier is saved when the *Store* view is displayed.

[comment]: <> (Is it a feature or is it a bug?)


#### Select a printer

You have to select a printer for the printing of receipts.

[comment]: <> (How does this work?)


#### Enter the store address

The store address is required as the delivery address, which has to be defined for tax purposes. Further, a delivery address and an invoice address should be indicated on every receipt created in the POS system.

*Venduo POS > Management > Tab STORES > Select Store > Tab Settings*

![Store Basic Data](/Assets/Screenshots/POS/Management/Stores/Store/Settings/Settings.png "[Store Basic Data]")

1. Select the *Store Address* entry in the list of settings in the left column.   
  The *Store Address* view is displayed on the right side.

  ![Store Basic Data](/Assets/Screenshots/POS/Management/Stores/Store/Settings/StoreAddress.png "[Store Basic Data]")

2. Enter the store address in the fields.

  > [Info] The store address corresponds to the delivery address. You must at least enter the country and the ZIP code.   
   For detailed information, see [User Interface Venduo POS/Management/Stores](/POS/UserInterface/02b_Management.md).

3. Click the [Save] button in the upper right corner.   
    The *Saving successful* message is displayed. The store address is saved.

    ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


#### Assign the POS warehouse

To connect the warehouse management and the stock management to your POS, you have to assign a warehouse from which to take the stock. The warehouse specifies where exactly the stock is booked out when a product is sold.

*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings*

![Store Admin Settings](/Assets/Screenshots/POS/Management/Stores/Store/AdminSettings/AdminSettings.png "[Store Admin Settings]")

1. Select the *Warehouse assignment orders* entry in the list of settings in the left column.   
  The *Warehouse assignment orders* section is displayed on the right side.

2. Select the warehouse you want to take the stock from in the *Warehouse* drop-down list.

3. Activate the *Automatically assign product to warehouse when activated in store* toggle to automate the assignment process.    
  It is recommended to activate this option. For detailed information, see [User Interface Venduo POS/Management/Stores](/POS/UserInterface/02b_Management.md).

  > [Info] A product must have stock allocation in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf. The products get a shelf the first time the corresponding channels offer is activated.    
  This automation only works if you have enabled the storage of multiple items per shelf when creating the warehouse. For detailed information, see [Configure the warehouse for POS](01_ConfigureWarehouse.md).

4. Enter a shelf number for the products in the *Shelf* field. The shelf number can be any arbitrary number.

  > [Info] A product must have stock allocation in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf.

5. Click the [Save] button in the upper right corner.   
  The *Saving successful* message is displayed. The warehouse assignment is saved.

    ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


#### Configure the stock withdrawal matrix

Define in the stock withdrawal matrix from which warehouses defined in the system the stock is booked out.

*Warehouse > Settings > Tab WAREHOUSE > Tab Stock withdrawal matrix*

![Stock withdrawal matrix](/Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockWithdrawalMatrix/StockWithdrawalMatrix.png "[Stock withdrawal matrix]")

1. Click the [ADD] button in the bottom left corner.   
  A new row is displayed in the list.

2. Configure the following settings:

  + Select the **--all--** option in the drop-down list in the *Product group* column.

  + Select the output channel via which you want to create offers in the drop-down list in the *Marketplace* column.

  + Select the created POS store in the drop-down list in the *Account* column.

  + Select the **--all--** option in the drop-down list in the *Sub-account* column.

  + Select the **--all--** option in the drop-down list in the *Shipping provider* column.

  + Select the warehouse from which you want to take the stock in the drop-down list in the *Warehouse* column.

3. Click the [SAVE ASSIGNMENTS] button in the bottom right corner.   
  The new assignment in the stock withdrawal matrix is saved.


#### Assign the stock source

Assign a stock source to manage the store stock. The stock source specifies how the stock available in the POS system is calculated. In most cases, the stock source and the warehouse are identical, but they can also differ.   

##### Create a stock attribute
*PIM > Settings > Tab ATTRIBUTES*

![PIM Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[PIM Attributes]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create Attribute* view is displayed.

  ![Create Attribute](/Assets/Screenshots/PIM/Settings/Attributes/CreateAttribute.png "[Create Attribute]")

2. Enter an appropriate name for the attribute in the *Name* field, for instance **stock test store**.

3. Enter an appropriate key in the *Key* field.

  > [Info] Only alphanumeric characters and _ are allowed. The key has to start with a letter. Blank spaces are not permitted in the *Key* field.

4. Select the **Stock Value** option in the *Data Type* drop-down list.

5. Click the ![Add](/Assets/Icons/Plus05.png "[Add]") (Add) button in the *Assigned Sets* section.   
  A new drop-down list is displayed in the *Assigned Sets* section.

6. Select the corresponding set in the *Assigned Sets* drop-down list.

7. Click the [SAVE] button in the upper right corner.   
  The attribute is saved. The page *Create Attribute* is closed.

8. Press **F5** to initialize the Core1 Platform.


##### Configure the stock allocation
*Warehouse > Settings > Tab WAREHOUSE > Tab Stock allocation*

![Stock allocation](/Assets/Screenshots/RetailSuiteWarehousing/Settings/Warehouse/StockAllocation/StockAllocation.png "[Stock allocation]")

1. Select the row with the stock allocation attributes name.

2. Double-click the field with the **Default (Calculation, Stock)** option in the *Stock calculation* column.   
  A drop-down list is displayed.

3. Select the **Calculation, Stock** option in the drop-down list in the *Stock calculation* column.   
  The fields in the warehouse columns are unlocked.

4. Double-click the option in a warehouse column to display the drop-down list.

5. Select the **Yes** option in the drop-down list to include the corresponding warehouse in the stock allocation calculation or select the **No** option to exclude it.

  > [Info] Select for each warehouse whether it should be included or not.

6. Click the [Save] button in the bottom right corner.   
  The stock allocation is saved. When the stock in a warehouse that is included in the formula is changed, the stock will be entered automatically in the stock field.

##### Map the attribute to the stock of the store
*DataHub > Settings > Tab ETL*

![ETL](/Assets/Screenshots/DataHub/Settings/ETL/ETL.png "[ETL]")

1. Select the checkbox of the mapping with the new store as a destination attribute set in the list of attribute set mappings and click the ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit) button in the editing toolbar in the upper right corner.   
  The *Mapping* view is displayed.

  ![Mapping](/Assets/Screenshots/DataHub/Settings/ETL/Mapping.png "[Mapping]")

2. Click the row with the destination attribute **Stock** in the list of mappings.   
  The *Settings* section is displayed on the right side.

  ![Mapping Settings](/Assets/Screenshots/DataHub/Settings/ETL/MappingSettings.png "[Mapping Settings]")

3. Select the **Basic Mapping** option in the *Extension* drop-down list in the *Settings* section.

4. Select the stock attribute in the *Source attribute* drop-down list.

5. Click the [SAVE] button in the upper right corner.   
  The mapping is saved.

6. Select the checkbox of the new mapping and click the [RERUN SELECTED MAPPING] button.   
  The mapping is executed again.

  > [Info] If necessary, repeat step **2** to **6** for all mappings with the store as a destination attribute.


#### Assign the accounts

In this step you assign the accounts to which you want to book the payments.   
You may assign the same accounts to all stores or you may assign different accounts per store or even per pay desk. Depending on your choice, you have to assign the accounts in different places:   
- To [assign the same accounts to all stores](#assign-the-accounts-in-the-global-settings), enter the accounts in the global settings.
- To [assign the accounts to a single store](#assign-the-accounts), enter the accounts in the admin settings of the respective store.
- To [assign the accounts to a single pay desk](#assign-the-accounts-in-the-pay-desk-settings), enter the accounts in the admin settings of the respective pay desk.


  > [Info] Remember that the more specific settings always override the more general settings.  
  This means that the accounts specified in the pay desks admin settings are always used first. If none are specified there, the accounts from the stores admin settings are used and only when nothing is specified there, the accounts from the global settings are used.

##### Assign the accounts in the global settings
To assign the same accounts to all stores, you may enter the account numbers in the global settings.

*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Account assignment*

![Assign accounts Global Settings](/Assets/Screenshots/POS/Management/GlobalSettings/GS24.png "[Assign accounts Global Settings]")

1. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies.  
   For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

2. Click the [Save] button in the bottom right corner of the window.   
  The *Saving successful* message is displayed. The account assignment is saved.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


##### Assign the accounts in the store settings
To assign the accounts to a single store, you may enter the account numbers in the store admin settings.

*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings > Entry Account assignment*

![Assign accounts Store Settings](/Assets/Screenshots/POS/Management/Stores/Store/AdminSettings/AdminSettings07.png "[Assign accounts Store Settings]")

  > [Info] In the bottom right corner, the *Apply from global* toggle is displayed. Activate the toggle to apply the account assignment from the global settings.   
  When the toggle is active, all fields in the detail view are locked. By default, this toggle is inactive.

1. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies.  
   For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

2. Click the [Save] button in the bottom right corner of the window.   
  The *Saving successful* message is displayed. The account assignment for the selected store is saved.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


##### Assign the accounts in the pay desk settings
To assign the accounts to a single pay desk, you may enter the account numbers in the pay desk admin settings.

*Venduo POS > Management > Tab STORES > Select Store > Select Pay Desk > Tab Admin Settings > Entry Account assignment*

![Assign accounts Pay Desk Settings](/Assets/Screenshots/POS/Management/Stores/PayDesk/AdminSettings/AdminSettings07.png "[Assign accounts Pay Desk Settings]")

> [Info] In the bottom right corner, the *Apply from global* toggle is displayed. Activate the toggle to apply the account assignment from the global settings.   
When the toggle is active, all fields in the detail view are locked. By default, this toggle is inactive.

1. Select the respective account in the *Account* column and enter the corresponding account numbers for the different payment types and currencies.  
   For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

2. Click the [Save] button in the bottom right corner of the window.   
  The *Saving successful* message is displayed. The account assignment for the selected pay desk is saved.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")

### Next steps

- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface Venduo POS](/POS/UserInterface/00_UserInterface.md)
- [User Interface Warehouse](/RetailSuiteWarehousing/UserInterface/00_UserInterface.md)
- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create a store via wizard](06_CreateStore.md#create-a-store-via-wizard)
- [Open a pay desk](/POS/Operation/01_OpenPayDesk.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
