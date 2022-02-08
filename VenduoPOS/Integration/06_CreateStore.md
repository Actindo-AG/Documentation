[!!Venduo POS](Actindo/Venduo POS)
[!!Lager](Actindo/Lager)
[!!PIM](Actindo/PIM)
[!!DataHub](Actindo/DataHub)

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

![Stores](/Assets/Screenshots/VenduoPOS/Management/Stores/Stores.png "[Stores]")

1. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  The two buttons [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] and [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] are displayed.

2. Click the button [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] to start the store creation wizard.   
  The *Create Store* wizard window is displayed.

#### Configure the store details

In this step, you can add additional information for your store and assign a store manager.

![Wizard 01](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW01.png "[Store Wizard]")

1. Enter a store name in the field *Store Name* and add a short description if you like.

2. Select a store manager from the list by selecting the corresponding checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") .

  > [Info] The store managers list displays all the users who are assigned to the POS store manager group. You may select multiple users as store managers.
    For detailed information, see [Assign users to the POS groups](04_AssignUsers.md).

3. Click the button [CREATE STORE] in the bottom right corner of the window.   
  The message *Creating Store...* is displayed. It may take several minutes until the creation is completed.  

  ![Wizard 01](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW01a.png "[Store Wizard]")

  The *Pay desks* wizard window is displayed when the store is created.


#### Configure the pay desk

In this step, you create one or several pay desks and assign cashiers.

![Wizard 02](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW02.png "[Store Wizard]")

1. Enter a pay desk name in the field *PayDesk 1*.

  > [Info] Click the button ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) right next to the pay desk name to add another pay desk. You can add as many pay desks as you need.

2. Select a cashier from the list by selecting the corresponding checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") .

  > [Info] The cashiers list displays all the users who are assigned to the POS cashier group. You may select multiple users as cashiers. Only cashiers who are assigned to a certain pay desk can use the pay desk.
   For detailed information, see [Assign users to the POS groups](04_AssignUsers.md)

3. Click the button [CREATE PAYDESKS] in the bottom right corner of the window.   
    The *Printing* wizard window is displayed when the pay desk is created.


#### Select a printer

In this step you select a printer for the receipt printing.

![Wizard 03](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW03.png "[Store Wizard]")

> [Info] To select a printer, the printer client *APS (Actindo Print System)* must be installed and configured.   
For detailed information, see [Configure the printer client for POS](03_ConfigurePrinter.md).

1. Select a client for the pay desk in the drop-down list *Client*.

2. Select a printer for the pay desk in the drop-down list *Printer*.

3. Select a tray in the drop-down list *Tray*.

4. Select a format for printing. By default, portrait format is preselected for receipt printing.

5. Click the button [SAVE PAYDESK] in the bottom to save the printing settings for the selected pay desk.

  > [Info] If you created multiple pay desks, you can switch to another pay desk by clicking the tab with the name of the respective pay desk. You may configure different print settings for each pay desk.

6. Click the button [CONTINUE] in the bottom right corner of the window.   
  The *Store Address* wizard window is displayed when the printer is configured.


#### Enter the store address

In this step you define the store address. The store address is the delivery address, which has to be defined for tax purposes. Further, a delivery address and an invoice address should be indicated on every receipt created in the POS system.


![Wizard 04](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW04.png "[Store Wizard]")

1. Enter the store address in the fields.

  > [Info] The store address corresponds to the delivery address. You must at least enter the country and the ZIP code.   
   For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).

2. Click the button [CONTINUE] in the bottom right corner of the window.   
    The message *Saving successful* and the *Stock* wizard window are displayed when the store address is saved.

    ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")



#### Assign a POS warehouse

In this step you assign the warehouse from which you want to take the stock from, you assign the shelf and you configure the stock source matrix. The warehouse specifies where exactly the stock is booked out when a product is sold.

![Wizard 05](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW05.png "[Store Wizard]")

1. Select the warehouse you want to take the stock from in the drop-down list *Lager*.

2. Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically assign product to warehouse when activated in store* to automate the assignment process.    
  It is recommended to activate this option. For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).

  > [Info] A product must have inventory in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf. The products get a shelf the first time the corresponding channels offer is activated.    
  This automation only works if you have enabled the storage of multiple items per shelf when creating the warehouse. For detailed information, see [Configure the warehouse for POS](01_ConfigureWarehouse.md).

3. Enter a shelf number for the products in the field *Shelf*. The shelf number can be any arbitrary number.

  > [Info] A product must have inventory in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf.

4. Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Configure stock source matrix* to automate the configuration of the stock source matrix.      
  It is recommended to activate this option. For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).

5. Click the button [CONTINUE] in the bottom right corner of the window.   
  The *inventory assignment* wizard window is displayed when the warehouse assignment is saved.


#### Assign an inventory source

In this step you assign the inventory source to manage the store inventory. The inventory source specifies how the stock available in the POS system is calculated. In most cases, the inventory source and the warehouse are identical, but they can also differ.

![Wizard 06](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW06a.png "[Store Wizard]")

1. Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Create new inventory source* to add a new inventory source that only considers the stock of the warehouse selected in the previous step.   
  It is recommended to activate this option. For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).   
  The drop-down list *Select existing inventory Source* is hidden.

2. Click the button [CONTINUE] in the bottom right corner of the window.   
  The *Accounting* wizard window is displayed when the inventory source assignment is saved.     


#### Assign an account

In this step you assign the accounts to which you want to book the payments.   

![Wizard 07](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW07a.png "[Store Wizard]")

1. Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Account per pay desk* to assign the accounts to each pay desk individually.   

  > [Info] If you deactivate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Account per pay desk*, you may only assign the accounts per store.   
  For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).

2. Select the respective pay desk in the drop-down list *Select Pay Desk* .     
  A table to assign the accounts is displayed in the window.

  ![Wizard 07](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW07b.png "[Store Wizard]")


3. Select the respective account in the column *Account* and enter the corresponding account numbers for the different payment types and currencies.     
  For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

  > [Info] You only have to enter the account numbers for the accounts with the used currency. To delete the unused currencies from the list of available currencies, see [User Interface Venduo POS/Management/Global Settings/Verfügbare Währungen](VenduoPOS/UserInterface/02a_Management.md#available-currencies).

4. Click the button [CONTINUE] in the bottom right corner of the window.   
  The *Summary* wizard window is displayed when the account assignment is saved.


#### Finalize the wizard

In this step, you check if any necessary information is still missing and you complete the configuration of the store.

![Wizard 08](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW08.png "[Store Wizard]")

1. Check the summary.     

  > [Info] In the summary, missing data or problems that can lead to restrictions when using Venduo POS are indicated with a yellow warning triangle.    
    Remember these points and correct them manually afterwards if necessary.   
    The summary also indicates whether the POS can be used.  

2. . Click the button [FINALIZE] in the bottom right corner of the window.   
      The wizard window is closed and the store is configured.

### Next steps

- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Venduo POS](VenduoPOS/UserInterface/00_UserInterface.md)
- [Create a store manually](#create-a-store-manually)
- [Open a pay desk](VenduoPOS/Operation/01_OpenPayDesk.md)
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

![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/Stores.png "[Create Store]")

1. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  The two buttons [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] and [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] are displayed.

2. Click the button [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] to add a new store manually.   
  The *Create Store* window is displayed.

  ![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/CreateStore.png "[Create Store]")

3. Enter a store name in the field *Name*.

4. Click the button [CREATE]:   
  The message *Creating Store* is displayed. The new store is displayed in the tab *STORES*.

  ![Creating Store](/Assets/Screenshots/VenduoPOS/Management/Stores/CreatingStore.png "[Creating Store]")

> [Info] To use the store and its full functionality, it is necessary to configure the following settings manually:
  - [Configure the store details](#configure-the-store-details-2)
  - [Create a pay desk](#create-a-pay-desk)
  - [Configure the pay desk details](#configure-the-pay-desk-details)
  - [Select a printer](#select-a-printer-2)
  - [Enter the store address](#enter-the-store-address-2)
  - [Assign the POS warehouse](#assign-the-pos-warehouse)
  - [Configure the stock source matrix](#configure-the-stock-source-matrix)
  - [Assign the inventory source](#assign-the-inventory-source)
  - [Assign the accounts](#assign-the-accounts)

#### Configure the store details

In the store details, you give some detailed information about your store. Further, you assign a store manager.

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Store Details](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/BasicData.png "[Store Details]")

1. Enter a short description of the store in the field *Short description*.

2. Click the button [ADD] in the section *Store Manager*.   
   The window *Store Managers* is displayed.

3. Select a store manager from the list by selecting the corresponding checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]").

  > [Info] The store managers list displays all users who are assigned to the POS store manager group. You may select multiple users as store managers.    
    For detailed information, see [Assign users to the POS groups](04_AssignUsers.md).

4. Click the button [Add] in the upper right corner of the window.

5. Click the button [SAVE] left below the section *Store Manager* .   
  The store manager is saved. The tab *STORES* is displayed.

[comment]: <> (Is it a feature or is it a bug?)

#### Create a pay desk

Create at least one pay desk to be able to process any type of transaction via Venduo POS.

A pay desk can be used in different manners. You can consider a pay desk as a physical unit and consequently create one pay desk per physically existing pay desk.   
However, you can also create one pay desk per user, so that each pay desk is assigned to one specific cashier and can only be used by that cashier. In this way, you can also create several pay desks in the POS system for one physically existing pay desk.

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/BasicData.png "[Basic Data]")

1. Click the button [ADD] in the section *Pay desks* .    
   The window *Create pay desk* is displayed.

   ![Create Pay Desk](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/CreatePayDesk.png "[Create Pay Desk]")

2. Enter a pay desk name in the field *Name*.

3. Click the button [SAVE].   
  The new pay desk is displayed in the section *Pay desks*.

  > [Info] Repeat step 1 to 3 to add another pay desk. You can add as many pay desks as you need.

4. Click the button [SAVE] left below the section *Store Manager* .   
  The pay desk is saved. The tab *STORES* is displayed.

[comment]: <> (Is it a feature or is it a bug?)


#### Configure the pay desk details

In the pay desk details, you give some detailed information about the pay desk. Further, you assign one or several cashiers to prevent the pay desk from unauthorized access.

*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data > Select Pay Desk*

![Pay Desk Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/BasicData/BasicData.png "[Pay Desk Basic Data]")

1. If desired, enter a short description for the pay desk in the field *Short Description*.

2. Click the button [ADD] in the section *Cashiers* .    
   The window *Cashiers* is displayed.

   ![Pay Desk Cashiers](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/BasicData/Cashiers.png "[Pay Desk Cashiers]")

3. Select a cashier from the list by selecting the corresponding checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]").

  > [Info] The cashiers list displays all users who are assigned to the POS cashier group. You may select multiple users as cashiers. Only cashiers who are assigned to a certain pay desk can use the pay desk.  
   For detailed information, see [Assign users to the POS groups](04_AssignUsers.md)

4. Click the button [Add] in the upper right corner of the window.

5. Click the button [SAVE] left below the section *Store Manager*.

  The cashier is saved. The selected store is displayed in the tab *STORES*.

[comment]: <> (Is it a feature or is it a bug?)


#### Select a printer

You have to select a printer for the printing of receipts.

[comment]: <> (How does this work?)


#### Enter the store address

The store address is required as the delivery address, which has to be defined for tax purposes. Further, a delivery address and an invoice address should be indicated on every receipt created in the POS system.

*Venduo POS > Management > Tab STORES > Select Store > Tab Settings*

![Store Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings.png "[Store Basic Data]")

1. Select the entry *Store-Adresse* in the list of settings in the left column.   
  The section *Store-Adresse* is displayed on the right side.

  ![Store Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/StoreAddress.png "[Store Basic Data]")

2. Enter the store address in the fields.

  > [Info] The store address corresponds to the delivery address. You must at least enter the country and the ZIP code.   
   For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).

3. Click the button [Speichern] in the upper right corner.   
    The message *Saving successful* is displayed. The store address is saved.

    ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


#### Assign the POS warehouse

To connect the warehouse management and the inventory management to your POS, you have to assign a warehouse from which to take the stock. The warehouse specifies where exactly the stock is booked out when a product is sold.

*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings*

![Store Admin Settings](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings.png "[Store Admin Settings]")

1. Select the entry *Lagerzuordnung Bestellungen* in the list of settings in the left column.   
  The section *Lagerzuordnung Bestellungen* is displayed on the right side.

2. Select the warehouse you want to take the stock from in the drop-down list *Warehouse*.

3. Activate the toggle ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically assign product to warehouse when activated in store* to automate the assignment process.    
  It is recommended to activate this option. For detailed information, see [User Interface Venduo POS/Management/Stores](VenduoPOS/UserInterface/02b_Management.md).

  > [Info] A product must have inventory in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf. The products get a shelf the first time the corresponding channels offer is activated.    
  This automation only works if you have enabled the storage of multiple items per shelf when creating the warehouse. For detailed information, see [Configure the warehouse for POS](01_ConfigureWarehouse.md).

4. Enter a shelf number for the products in the field *Shelf*. The shelf number can be any arbitrary number.

  > [Info] A product must have inventory in a warehouse in order to be sold from that warehouse. Products only have stock in a warehouse if a shelf is defined for them. By default, a shelf is not defined for products. Therefore, each product that is to be sold in the POS system must first get a shelf.

5. Click the button [Speichern] in the upper right corner.   
  The message *Saving successful* is displayed. The warehouse assignment is saved.

    ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


#### Configure the stock source matrix

Define in the stock source matrix from which warehouses defined in the system the stock is booked out.

*Lager > Einstellungen > Tab LAGER > Tab Lagerentnahme-Matrix*

![Lagerentnahme-Matrix](/Assets/Screenshots/Lager/Einstellungen/Lager/LagerentnahmeMatrix/LagerentnahmeMatrix.png "[Lagerentnahme-Matrix]")

1. Click the button [HINZUFÜGEN] in the bottom left corner.   
  A new row is displayed in the list.

2. Configure the following settings:

  + Select the option **--alle--** in the drop-down list in the column *Produkt-Warengruppe*.

  + Select the output channel via which you want to create offers in the drop-down list in the column *Marktplatz*.

  + Select the created POS store in the drop-down list in the column *Account*.

  + Select the option **--alle--** in the drop-down list in the column *Sub-Account*.

  + Select the option **--alle--** in the drop-down list in the column *Versandanbieter*.

  + Select the warehouse from which you want to take the stock in the drop-down list in the column *Lager*.

3. Click the button [ZUORDNUNGEN SPEICHERN] in the bottom right corner.   
  The new assignment in the stock source matrix is saved.


#### Assign the inventory source

Assign an inventory source to manage the store inventory. The inventory source specifies how the stock available in the POS system is calculated. In most cases, the inventory source and the warehouse are identical, but they can also differ.   

##### Create an inventory attribute
*PIM > Settings > Tab ATTRIBUTES*

![PIM Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[PIM Attributes]")

1. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
  The *Create Attribute* view is displayed.

  ![Create Attribute](/Assets/Screenshots/PIM/Settings/Attributes/CreateAttribute.png "[Create Attribute]")

2. Enter an appropriate name for the attribute in the field *Name*, e.g. **inventory test store**.

3. Enter an appropriate key in the field *Key*.

  > [Info] Only alphanumeric characters and _ are allowed. The key has to start with a letter. Blank spaces are not permitted in the field *Key*.

4. Select the option **Stock Value** in the drop-down list *Data Type*.

5. Click the button ![Add](/Assets/Icons/Plus05.png "[Add]") (Add) in the section *Assigned Sets* .   
  A new drop-down list is displayed in the section *Assigned Sets*.

6. Select the corresponding set in the drop-down list *Assigned Sets*.

7. Click the button [SAVE] in the upper right corner.   
  The attribute is saved. The page *Create Attribute* is closed.

8. Press **F5** to initialize the Core1 Platform.


##### Configure the inventory assignment
*Lager > Einstellungen > Tab LAGER > Tab Bestandszuteilung*

![Bestandszuteilung](/Assets/Screenshots/Lager/Einstellungen/Lager/Bestandszuteilung/Bestandszuteilung.png "[Bestandszuteilung]")

1. Select the row with the inventory attributes name.

2. Double-click the field with the option **Voreinstellung (Berechnung, Lagerbestand)** in the column *Bestandsberechnung* .   
  A drop-down list is displayed.

3. Select the option **Berechnung, Lagerbestand** in the drop-down list in the column *Bestandsberechnung* .   
  The fields in the warehouse columns are unlocked.

4. Double-click the option in a warehouse column to display the drop-down list.

5. Select the option **Yes** in the drop-down list to include the corresponding warehouse in the inventory calculation or select the option **No** to exclude it.

  > [Info] Select for each warehouse whether it should be included or not.

6. Click the button [SPEICHERN] in the bottom right corner.   
  The inventory assignment is saved. When the stock in a warehouse that is included in the formula is changed, the stock will be entered automatically in the stock field.

##### Map the attribute to the inventory of the store
*DataHub > Settings > Tab ETL*

![ETL](/Assets/Screenshots/DataHub/Settings/ETL/ETL.png "[ETL]")

1. Select the checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the mapping with the new store as a destination attribute set in the list of attribute set mappings and click the button ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit) in the editing toolbar in the upper right corner.   
  The *Mapping* view is displayed.

  ![Mapping](/Assets/Screenshots/DataHub/Settings/ETL/Mapping.png "[Mapping]")

2. Click the row with the destination attribute **Bestand** in the list of mappings.   
  The section *Settings* is displayed on the right side.

  ![Mapping Settings](/Assets/Screenshots/DataHub/Settings/ETL/MappingSettings.png "[Mapping Settings]")

3. Select the option **Basic Mapping** in the drop-down list *Extension* in the section *Settings*.

4. Select the inventory attribute in the drop-down list *Source attribute*.

5. Click the button [SAVE] in the upper right corner.   
  The mapping is saved.

6. Select the checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the new mapping and click the button [RERUN SELECTED MAPPING].   
  The mapping is executed again.

  > [Info] If necessary, repeat step **2** to **6** for all mappings with the store as a destination attribute.


#### Assign the accounts

In this step you assign the accounts to which you want to book the payments.   
You may assign the same accounts to all stores or you may assign different accounts per store or even per pay desk. Depending on your choice, you have to assign the accounts in different places:   
- To [assign the same accounts to all stores](#assign-the-accounts-in-the-global-settings), enter the accounts in the global settings.
- To [assign the accounts to a single store](#assign-the-accounts), enter the accounts in the admin settings oft the respective store.
- To [assign the accounts to a single pay desk](#assign-the-accounts-in-the-pay-desk-settings), enter the accounts in the admin settings of the respective pay desk.


  > [Info] Remember that the more specific settings always override the more general settings.  
  This means that the accounts specified in the pay desks admin settings are always used first. If none are specified there, the accounts from the stores admin settings are used and only when nothing is specified there, the accounts from the global settings are used.

##### Assign the accounts in the global settings
To assign the same accounts to all stores, you may enter the account numbers in the global settings.

*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Kontenzuteilung Buchhaltung*

![Assign accounts Global Settings](/Assets/Screenshots/VenduoPOS/Management/GlobalSettings/GS24.png "[Assign accounts Global Settings]")

1. Select the respective account in the column *Account* and enter the corresponding account numbers for the different payment types and currencies.  
   For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

2. Click the button [Speichern] in the bottom right corner of the window.   
  The message *Saving successful* is displayed. The account assignment is saved.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


##### Assign the accounts in the store settings
To assign the accounts to a single store, you may enter the account numbers in the store admin settings.

*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings > Entry Kontenzuteilung Buchhaltung*

![Assign accounts Store Settings](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings07.png "[Assign accounts Store Settings]")

  > [Info] In the bottom right corner, the toggle *Von Global übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") is displayed. Activate the toggle to apply the account assignment from the global settings.   
  When the toggle is active, all fields in the detail view are locked. By default, this toggle is inactive.

1. Select the respective account in the column *Account* and enter the corresponding account numbers for the different payment types and currencies.  
   For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

2. Click the button [Speichern] in the bottom right corner of the window.   
  The message *Saving successful* is displayed. The account assignment for the selected store is saved.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")


##### Assign the accounts in the pay desk settings
To assign the accounts to a single pay desk, you may enter the account numbers in the pay desk admin settings.

*Venduo POS > Management > Tab STORES > Select Store > Select Pay Desk > Tab Admin Settings > Entry Kontenzuteilung Buchhaltung*

![Assign accounts Pay Desk Settings](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings07.png "[Assign accounts Pay Desk Settings]")

> [Info] In the bottom right corner, the toggle *Von Global übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") is displayed. Activate the toggle to apply the account assignment from the global settings.   
When the toggle is active, all fields in the detail view are locked. By default, this toggle is inactive.

1. Select the respective account in the column *Account* and enter the corresponding account numbers for the different payment types and currencies.  
   For detailed information, see [Manage the accounts for POS](02_ManageAccounts.md).

2. Click the button [Speichern] in the bottom right corner of the window.   
  The message *Saving successful* is displayed. The account assignment for the selected pay desk is saved.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")

### Next steps

- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)

### See also

- [User Interface Venduo POS](VenduoPOS/UserInterface/00_UserInterface.md)
- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create a store via wizard](06_CreateStore.md#create-a-store-via-wizard)
- [Open a pay desk](VenduoPOS/Operation/01_OpenPayDesk.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
