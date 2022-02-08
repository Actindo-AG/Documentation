# Stores
*Venduo POS > Management > Tab STORES*

In the tab *STORES*, you select a store and define the settings of the selected store and its pay desks.
To define the settings of a store and its pay desk, you have to select the corresponding store first.

![Select Store](/Assets/Screenshots/VenduoPOS/Management/Stores/Stores.png "[Select Store]")

**Stores**

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a store.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of stores.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]   
  Select the checkbox to display the editing toolbar.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)   
  Click this button to edit the selected store. This button is only displayed, when the checkbox of a store is selected. Alternatively, you can click directly a row in the table to edit a store.

The table displays all created stores. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*  
  Name of the store.  

- *Short Description*  
  Short description of the store.  

- *Store Managers*   
  Managers that are assigned to the store.

- *Revenue (Today/Month/Year)*   
  Store revenue of the current day/the current month/the current year.

- *Cash Balance*   
  Current cash balance in the pay desk.

- *ID*   
  Store identification number.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a new store. The two buttons [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ] and [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ] are displayed.



## Create Store
*Venduo POS > Management > Tab STORES > Button Add*

![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/Add.png "[Create Store]")

- [Create store via wizard (recommended) ![Store Wizard](/Assets/Icons/Tool.png "[Store Wizard]") ]   
  Click this button to create a store via wizard.

- [Create Store ![Store Manual](/Assets/Icons/Plus02.png "[Store Manual]") ]   
  Click this button to create a store manually.

- ![Cancel](/Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to cancel the store creation and exit the current view.


### Create store via wizard
*Venduo POS > Management > Tab STORES > Button Add > Button Create store via wizard*


#### Step 1 - Create Store
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW01.png "[Create Store]")

- *Store-Name*   
  Enter the store name.

- *Short description*   
  Enter a short description to the store.

**Select Store Managers**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)    
  Click this button to update the list of store managers.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to select the user as store manager. If you click the checkbox in the header, all users are selected.

The table displays all available users. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Login*   
  User name.

- *First Name*   
  First name of the user.

- *Name*   
  Last name of the user.

- *ID*   
  Identification number of the user.

- [CANCEL]   
  Click this button to cancel the store creation and close the wizard window.

- [CREATE STORE]   
  Click this button to create the store and proceed to the next step in the store wizard. The *Creating Store* window is displayed. When the store is created, the *Pay desks* wizard window is displayed.

#### Step 2 - Pay desks
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW02.png "[Create Store]")

- *PayDesk1*   
  Enter the pay desk name.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)    
  Click this button to delete the pay desk left to the button. The first pay desk cannot be deleted.

- ![Add](/Assets/Icons/Plus04.png "[Add]") (Add)    
  Click this button to add a new pay desk. A new line for a pay desk is displayed below.

**Select Cashiers**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)    
  Click this button to update the list of store managers.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to select the user as cashier. If you click the checkbox in the header, all users are selected.

The table displays all available users. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Login*   
  User name.

- *First Name*   
  First name of the user.

- *Name*   
  Last name of the user.

- *ID*   
  Identification number of the user.

- [< BACK]   
  Click this button to go back to the previous step. The *Create Store* wizard window is displayed.
[comment]: <> (not working)

- [CANCEL]   
  Click this button to cancel the pay desk creation and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [CREATE PAYDESKS]   
  Click this button to create the pay desks and proceed to the next step in the store wizard. The *Printing* wizard window is displayed.

#### Step 3 - Printing
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW03.png "[Create Store]")

For each pay desk, a tab with the printer settings below is displayed.

**PRINTER**

- *Client*   
  Click the drop-down list to select a default client. All available clients are displayed in the list.

- *Printer*   
  Click the drop-down list to select a default printer. All available printers are displayed in the list.

- *Tray*   
  Click the drop-down list to select a default tray. All available trays are displayed in the list.

**LAYOUT**

- Landscape rectangle   
  Click the landscape rectangle to define landscape as the default paper size.

- Portrait rectangle   
  Click the portrait rectangle to define portrait as the default paper size.

- *Format*   
  Click the drop-down list to select a default format. The formats below are available.
  [comment]: <> (which formats? doesn't work)

- [SAVE FOR PAYDESK]   
  Click this button to save the printer configuration for the selected pay desk.

  > [Info] If you switch the pay desk tab without saving, all changes are rejected.  

- [CANCEL]   
  Click this button to cancel configuring the printer settings and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [CONTINUE]   
  Click this button to save the printer settings for the pay desks and proceed to the next step in the store wizard.  The *Store Address* wizard window is displayed. The *Saving successful* message is displayed in the upper right corner of the wizard window.

#### Step 4 - Store Address
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW04.png "[Create Store]")

- *Owner*   
  Enter the name of the store owner.

- *Street*   
  Enter the street name of the store.

- *Email*   
  Enter the e-mail address of the store.

- *Phone*   
  Enter the phone number of the store.

- *ZIP*   
  Enter the ZIP code of the store address.

- *City*   
  Enter the city name of the store address.

- *Country*   
  Enter the country name of the store address.
  [comment]: <> (Should the country field be mandatory and a drop-down list?)

- [< BACK]   
  Click this button to go back to the previous step. The *Printing* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel defining the store address and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [CONTINUE]   
  Click this button to save the store address and proceed to the next step in the store wizard. The *Stock* wizard window is displayed. The *Saving successful* message is displayed in the upper right corner of the wizard window.


#### Step 5 - Stock
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW05.png "[Create Store]")

- *Warehouse*   
  Click the drop-down list and select the warehouse you want to take the stock from. By default, you can select the warehouses **Verkaufslager**, **Eigenlager** and **Außenlager**. Further, you can create your own warehouses, that are displayed in this drop-down list.   
  For detailed information, see [Configure the warehouse for POS](VenduoPOS/Integration/01_ConfigureWarehouse.md).

- [REFRESH LIST]   
  Click this button to update the drop-down list *Warehouse*.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically assign product to warehouse when activated in store*   
  Activate this toggle to automate the assignment process of products to a shelf in a warehouse. It is recommended to activate this option.

- *Shelf*   
  Enter a shelf number in the warehouse to which the stock is to be assigned.

- [< BACK]   
  Click this button to go back to the previous step. The *Store Address* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel defining the stock settings and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [CONTINUE]   
  Click this button to save the stock settings and proceed to the next step in the store wizard. The *Saving...* window is displayed. When the saving is completed, the *Inventory assignment* wizard window is displayed.


#### Step 6 - Inventory assignment
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW06a.png "[Create Store]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Create new inventory source*   
  Activate this toggle to add a new inventory source that only considers the stock of the warehouse selected in the previous step for calculating the warehouse stock. Deactivate this toggle to select an existing inventory source in the drop-down list *Select existing inventory Source* or to add no inventory source. When you activate this toggle, the drop-down list *Select existing inventory Source* is hidden.

- *Select existing inventory Source*   
  Click the drop-down list and select an inventory source for the POS store. The inventory source specifies how the inventory available in the POS system is calculated. All available inventory sources are displayed in the list. This drop-down list is only displayed when the toggle *Create new inventory source* is active.  

- [< BACK]   
  Click this button to go back to the previous step. The *Stock* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel defining the inventory assignment and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [CONTINUE]   
  Click this button to assign the inventory source and proceed to the next step in the store wizard. The *Saving...* window is displayed. When the saving is completed, the *Accounting* wizard window is displayed.

[comment]: <> (when I proceed with the active toggle, go back and try to continue the wizard again, an error message is displayed: Saving failed ETLAttributeMap for destinationAttribute with name Bestand does already exist for ETLAttributeSetMap with id 672. -> Bug?)  


#### Step 7 - Accounting
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW07b.png "[Create Store]")

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Account per pay desk*   
  Activate this toggle to assign the accounts to each pay desk individually. Deactivate the toggle to assign the accounts for the entire store. When you activate this toggle, the drop-down list *Select Pay Desk* is hidden. By default, this toggle is active.

- *Select Pay Desk*   
  Click the drop-down list and select the pay desk for which you want to assign the accounts. All accounts are displayed below the drop-down list for each available currency. This drop-down list is only displayed when the toggle *Account per pay desk* is active.

  > [Info] If you have multiple pay desks, switch the pay desk in the drop-down list after defining the accounts to define also the accounts for this pay desk. Repeat this procedure for all created pay desks.

The list of accounts is displayed either when you deactivate the toggle *Account per pay desk* or when you select a pay desk in the drop-down list *Select Pay Desk*.

- *Type*   
  In this column, the account type is indicated. Six accounts are displayed per currency. The currency of the account is indicated in brackets after the account type name. The fields are display fields only. They cannot be changed.

  - *Bar*   
    This type of account serves as a cash account for cash payments.

  - *Redeem Voucher*    
    This type of account serves as --- add information ---

  - *Gegenkonto Cash-In*   
    This type of account serves as a clearing account against which cash deposits without customers are booked.

  - *Gegenkonto Cash-Out*   
    This type of account serves as a clearing account against which cash withdrawals without customers are booked.

  - *Refund auf Gutschein (refund only)*   
    This type of account serves as a refund account for refunds of cashless payments.

  - *Manuelles Zahlen am Terminal*   
    This type of account serves as a cash account for cashless payments.

- *Account*   
  Enter the account number for the corresponding account types. You can assign another account number for each account type.

- [< BACK]   
  Click this button to go back to the previous step. The *Inventory assignment* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel defining the inventory assignment and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [CONTINUE]   
  Click this button to assign the accounts and proceed to the next step in the store wizard. The *Loading...* window is displayed. When the saving is completed, the *Summary* wizard window is displayed.


#### Step 8 - Summary
![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/StoreWizard/SW08.png "[Create Store]")

The wizard window displays a summary of the store configuration. Missing data or problems that can lead to restrictions when using the POS store are indicated with a yellow warning triangle.    

- [< BACK]   
  Click this button to go back to the previous step. The *Accounting* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel the store finalization and close the wizard window.

  > [Info] If you cancel the wizard now, the store is nevertheless created but you have to configure the further store settings manually.

- [FINALIZE]   
  Click this button to complete the store configuration and close the wizard window. The configured store is displayed in the list of stores.  

### Create store manually
*Venduo POS > Management > Tab STORES > Button Add > Button Create Store*

![Create Store](/Assets/Screenshots/VenduoPOS/Management/Stores/CreateStore.png "[Create Store]")

- *Name*   
  Enter the store name.

- [CANCEL]   
  Click this button to cancel the store creation and close the window.

- [CREATE]   
  Click this button to create the store. The *Creating Store* window is displayed. When the store is created, the window is closed and the *Store* view of the new store is displayed.  


## Store
*Venduo POS > Management > Tab STORES > Select Store*

![Store Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/BasicData.png "[Store Basic Data]")

- *Name*   
  Name of the store.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the store name.

- ![Apply](/Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the store name. This button is only displayed when you are editing the store name.

- ![Pay Desk](/Assets/Icons/PayDesk.png "[Pay Desk]") (Pay desk)   
  Number of pay desks in the selected store. The number of pay desks currently in use is displayed in the brackets. This field is read-only.

- ![Banknote](/Assets/Icons/Banknote02.png "[Banknote]") (Banknote)   
  Current amount of revenue from all pay desks. This field is read-only.

- *Created MM/DD/YYYY*   
  Date of store creation. This field is read-only.

- [SAVE]   
  Click this button to save any changes.


### Basic Data - Store
*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data*

![Store Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/BasicData.png "[Store Basic Data]")

- *Short Description*   
  Enter a short description to the store.

- [SAVE]   
  Click this button to save any changes.

**Store Manager**

- [Add]      
  Click this button to add a store manager to the store. The *Store Managers* window is displayed.

- *First Name*   
  First name of the store manager.

- *Last Name*   
  Last name of the store manager.

- *Login*   
  User name of the store manager.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the store manager. This button is only displayed when you hover over the store manager. Click the [SAVE] button to save the changes.


**Pay desks**

  Click this button to add a pay desk to the store. The *Create pay desk* window is displayed.

- *Name*   
  Name of the pay desk.

- *Used by*   
  Full name and user name of the current pay desk user. If the pay desk is currently not in use, a dash (*-*) is displayed.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the pay desk. This button is only displayed when you hover over the pay desk. Click the [SAVE] button to save the the changes.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the pay desk. This button is only displayed when you hover over the pay desk. Click the [SAVE] button to save the the changes.


#### Store Managers
*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data > Add Store Manager*

![Store Managers](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/StoreManagers.png "[Store Managers]")

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)    
  Click this button to update the list of store managers.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]       
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all users are selected.

- [Add]   
  Click this button to add the selected user to the list of store managers. This button is only displayed, when the checkbox of a user is selected.

The table displays all available store managers. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *First Name*   
  First name of the user.

- *Last Name*   
  Last name of the user.

- *Login*   
  Login name of the user.

- *ID*   
  Identification number of the user.


#### Create Pay Desk
*Venduo POS > Management > Tab STORES > Select Store > Tab Basic Data > Add Pay Desk*

![Create pay desk](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/BasicData/CreatePayDesk.png "[Create pay desk]")

- *Name*   
  Enter the name of the new pay desk.

- [CANCEL]   
  Click this button to cancel the creation of a pay desk.

- [SAVE]   
  Click this button to add the pay desk to the list of pay desks.



### Settings
*Venduo POS > Management > Tab STORES > Select Store > Tab Settings*

![Settings Store](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings.png "[Settings Store]")

#### UNKNOWN SECTION

In this section, you define all pay desk and payment settings.

#### Bon immer ausdrucken

Activate or deactivate the option to print the cash receipt.

![Bon immer ausdrucken](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings01.png "[Bon immer ausdrucken]")

 - [x] *Bon immer ausdrucken*   
   Choose whether or not to print the cash receipt for each transaction. If the receipt printing is deactivated, you can still initiate the receipt printing manually via the order history.

     > [Info] Remember that receipt printing is mandatory in several countries. Please inform yourself about the country-specific regulations before you deactivate this option.

 - *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
   Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Kasse öffnen bei Barzahlung

Activate or deactivate the option to open the cash drawer for cash payment.

![Kasse öffnen bei Barzahlung](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings02.png "[Kasse öffnen bei Barzahlung]")

- [x] *Kassenschublade öffnen bei Barzahlung*   
  Choose whether or not to open the cash drawer for cash payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Kasse öffnen nach bargeldlosem Zahlen

Activate or deactivate the option to open the cash drawer for cashless payment.

![Kasse öffnen bei Barzahlung](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings03.png "[Kasse öffnen bei Barzahlung]")

- [x] *Kasse öffnen*    
  Choose whether or not to open the cash drawer for cashless payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### USt-ID

Define the VAT ID, which is mandatory to be indicated on receipts in some countries.

![USt-ID](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings04.png "[USt-ID]")

- *USt-ID*   
  Enter your VAT ID. By default, The VAT-ID is printed on your receipts.

- [Speichern]    
  Click this button to save any changes.


#### Store-Adresse

Define the store address which is used as invoice address.

![Store Address](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings05.png "[Store Address]")

- *Owner*   
  Enter the name of the store owner.

- *Street*   
  Enter the street name of the store.

- *Email*   
  Enter the e-mail address of the store.

- *Phone*   
  Enter the phone number of the store.

- *ZIP*   
  Enter the ZIP code of the store address.

- *City*   
  Enter the city name of the store address.

  [comment]: <> (Should the country field be mandatory and a drop-down list?)

- *Country*   
  Enter the country name of the store address.


#### Abschöpfen bis Betrag

Define an amount up to which the pay desk is skimmed after the pay desk closes. The amount is automatically entered in the cash register and taken as the opening float.

![Abschöpfen bis Betrag](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings06.png "[Abschöpfen bis Betrag]")

- *Abschöpfen bis Betrag*    
  Enter the amount up to which the pay desk is skimmed after the pay desk closing.

- [Speichern]  
  Click this button to save any changes.


#### Erwarteten Betrag verbergen

By default, the expected amount in the pay desk is indicated. deactivate this option to hide the expected amount from the cashier in order to prevent the concealment of shortfalls.

![Erwarteten Betrag verbergen](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings07.png "[Erwarteten Betrag verbergen]")

- [x] *Erwarteten Betrag verbergen*   
  Choose whether or not to hide the expected amount in the pay desk from the cashier. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### BELEGDRUCK

#### Händler-Beleg drucken

Activate or deactivate the printing of a merchant receipt for cashless payment.

![Händler-Beleg drucken](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings08.png "[Händler-Beleg drucken]")

- [x] *Händler-Beleg drucken*   
  Choose whether or not to print a merchant receipt in addition to the customer receipt for cashless payments. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")    
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### Nativer Bon-Druck

Activate or deactivate the native receipt printing.

![Nativer Bon-Druck](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings09.png "[Nativer Bon-Druck]")

- [x] *Nativer Bon-Druck*   
  Choose whether or not to use the native receipt print. By default, this option is active.

  [comment]: <> ("Setting will be deleted, should always be active")

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### Logo-Druck Kompatibilitätsmodus

Activate or deactivate the compatibility mode for logo printing. As some receipt printer have issues with printing logos, it may help to activate this option.

![Logo-Druck](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings10.png "[Logo-Druck]")

- [x] *Logo-Druck Kompatibilitätsmodus*   
  Choose whether or not to use the compatibility mode for logo printing. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Bon-Format

Define the width of the receipt, as it may vary depending on the printer.

![Logo-Druck](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/Settings/Settings11.png "[Logo-Druck]")

- *Breite in Zeichen*   
  Define the width of the receipt in characters. This size is needed to calculate the width for the text.

  > [Info] So-called monospaced fonts are used For receipt printing. This means that each character has the same width.

- *Breite in Pixel*   
  Define the width of the receipt in pixels. This size is needed to calculate the width for images, e. g. logos.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.




### Admin Settings - Store
*Venduo POS > Management > Tab STORES > Select Store > Tab Admin Settings*

![Admin Settings Store](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings.png "[Admin Settings Store]")

#### UNKNOWN SECTION

In this section, you define all pay desk and payment settings.

#### Kasse öffnen bei Barzahlung

Activate or deactivate the option to open the cash drawer for cash payment.

![Kasse öffnen bei Barzahlung](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings01.png "[Kasse öffnen bei Barzahlung]")

- [x] *Kassenschublade öffnen bei Barzahlung*   
  Choose whether or not to open the cash drawer for cash payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Kasse öffnen nach bargeldlosem Zahlen

Activate or deactivate the option to open the cash drawer for cashless payment.

![Kasse öffnen nach bargeldlosem Zahlen](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings02.png "[Kasse öffnen nach bargeldlosem Zahlen]")

- [x] *Kasse öffnen*    
  Choose whether or not to open the cash drawer for cashless payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Kassenjournal auf User binden

When a pay desk is opened, it is linked to a specific user. This user is the only one who can use the pay desk until he closes it again. To allow that several users can access the same pay desk without closing it, you can deactivate the option to link the cash register to a specific user.

![Kassenjournal auf User binden](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings03.png "[Kassenjournal auf User binden]")

- [x] *Kassenbuch auf User gebunden*   
  Choose whether or not to link the cash register to a special user. By default, this option is active.

  > [Info] Remember that even if you deactivate this option, a user must log out to allow another user to access the pay desk.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### WÄHRUNGEN

#### Verwendete Währungen

Select all currencies that are used in your POS system and define a default currency.

![Verwendete Währungen](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings04.png "[Verwendete Währungen]")

- [x] *Currency Name*   
  Choose whether or not to use this currency in your POS system.

- *Standard*   
  Click the drop-down list to select the currency that is used as default currency. All available currencies are displayed in the drop-down list. When you select a default currency that is not yet selected as used currency, that currency is automatically selected as used currency.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### BELEGDRUCK

#### Zahlenformat

Define the number format on the receipt.

![Zahlenformat](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings05.png "[Zahlenformat]")

- *Decimal separator*   
  Enter the decimal separator for the numbers on your receipt. You can use any separator including a blank space. This field is mandatory.

- *Thousand separator*   
  Enter the thousand separator for the numbers on your receipt. You can use any separator including a blank space.

- *Precision*   
  Enter the number of decimal places for the numbers on your receipt or use the arrow buttons in the field to increase or decrease the number of decimal places. You can select a number between 0 and 4. This field is mandatory.

  > [Info] The sample view below the input fields displays a live preview of the number with the selected separators and decimal places.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### Logo

Upload a logo for your receipts.

![Logo](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings06.png "[Logo]")

  >  [Info] The png format is the only image format supported for logo images. So make sure that your image logo is also saved in the png format before uploading it.

- [SELECT FILE]   
  Click this button to select a logo image for your receipts. The explorer is displayed for image selection. The selected logo image is displayed in the preview box right from the button. Alternatively, you can select an image using drag & drop.

- ![Upload](/Assets/Icons/Upload.png "[Upload]") *Drop file here...*   
  Drag the logo image from your local folder and drop it in this dashed box to upload it. The background color of the box turns to blue when you can drop the image.  The selected logo image is displayed in the preview box right from the button. Alternatively, you can select an image using the button [SELECT FILE].

- Preview box   
  The preview box displays the uploaded logo image. If a logo image is already displayed and you upload a new one, the current logo image will be overwritten by the new logo image.
  Delete a displayed logo by clicking the button ![Remove](/Assets/Icons/Cross03.png "[Remove]") (Remove) in the upper right corner of the logo.

- [Speichern]   
  Click this button to save any changes.


#### DATENÜBERTRAGUNG RETAILSUITE FAKTURA

#### Kontenzuteilung Buchhaltung

Assign the accounts to which you want to book the payments. The accounts are assigned for all stores, unless they are overwritten in the store or pay desk admin settings.
For detailed information, see [Admin Settings - Store](#admin-settings-store) or [Admin Settings - Pay Desk](#admin-settings-pay-desk).

The number of accounts to be assigned depends on the number of available currencies.

![Zahlenformat](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings07.png "[Zahlenformat]")

- *Type*   
  In this column, the account type is indicated. Six accounts are displayed per currency. The currency of the account is indicated in brackets after the account type name. The fields are display fields only. They cannot be changed.

  - *Bar*   
    This type of account serves as a cash account for cash payments.

  - *Redeem Voucher*    
    This type of account serves as --- add information ---

  - *Gegenkonto Cash-In*   
    This type of account serves as a clearing account against which cash deposits without customers are booked.

  - *Gegenkonto Cash-Out*   
    This type of account serves as a clearing account against which cash withdrawals without customers are booked.

  - *Refund auf Gutschein (refund only)*   
    This type of account serves as a refund account for refunds of cashless payments.

  - *Manuelles Zahlen am Terminal*   
    This type of account serves as a cash account for cashless payments.

- *Account*   
  Enter the account number for the corresponding account types. You can assign another account number for each account type.

- [Speichern]   
  Click this button to save any changes.


#### Shop-Kundennummer für Nachbestellung

Define a customer ID for the store to restrict the reorder query to the selected store.

![Shop-Kundennummer](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings08.png "[Shop-Kundennummer]")

- *Kundennummer*   
  Enter a customer ID for the store. Only orders assigned to this ID can be queried. If you leave the field blank, all orders can be queried.

- [Speichern]   
  Click this button to save any changes.

#### Retourenlager (Sperrlager)

[comment]: <> (need information; Is that right?)

Define a shelf in the quarantine warehouse for returns with defects.

![Retourenlager](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings09.png "[Retourenlager]")

- *Lager ID*   
  Enter an identification number for the quarantine warehouse.

[comment]: <> (Is shelf name right? Not number of the shelf???)
- *Fachname*   
  Enter the name of the shelf for the defect returns.

- [Speichern]   
  Click this button to save any changes.


#### Lagerzuordnung Bestellungen

Change or define the warehouse from which to take the stock.

![Lagerzuordnung](/Assets/Screenshots/VenduoPOS/Management/Stores/Store/AdminSettings/AdminSettings10.png "[Lagerzuordnung]")

- *Warehouse*   
  Click the drop-down list and select the warehouse you want to take the stock from. By default, you can select the warehouses **Verkaufslager**, **Eigenlager** and **Außenlager**. Further, you can create your own warehouses, that are displayed in this drop-down list.   
  For detailed information, see [Configure the warehouse for POS](VenduoPOS/Integration/01_ConfigureWarehouse.md).

- [REFRESH LIST]   
  Click this button to update the drop-down list *Warehouse*.

- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Automatically assign product to warehouse when activated in store*   
  Activate this toggle to automate the assignment process of products to a shelf in a warehouse. It is recommended to activate this option.

- *Shelf*   
  Enter a shelf number in the warehouse to which the stock is to be assigned.

- [Speichern]   
  Click this button to save any changes.


## Pay Desk
*Venduo POS > Management > Tab STORES > Select Store > Edit Pay Desk*

![Pay Desk Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/BasicData/BasicData.png "[Pay Desk Basic Data]")

- *Name*   
  Name of the pay desk.

- ![Edit](/Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the pay desk name.

- ![Apply](/Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the store name. This button is only displayed when you are editing the store name.

- *Unassigned/user name*   
  Indication whether the pay desk is currently in use. If the pay desk is not in use, *Unassigned* is displayed. If the pay desk is in use, the user name of the cashier is displayed.

- ![Remove](/Assets/Icons/Cross03.png "[Remove]") (Remove)   
  Click this button to remove the cashier from the pay desk. This button is only displayed when the pay desk is in use.

- ![Location](/Assets/Icons/Location.png "[Store Location]") (Store)   
  Name of the store where the pay desk is located. This field is read-only.

- *x Users*   
  Number of cashiers assigned to the selected pay desk.

- ![Banknote](/Assets/Icons/Banknote02.png "[Banknote]") (Banknote)   
  Current amount of cash in the selected pay desks. This field is read-only.

- *Created MM/DD/YYYY*   
  Date of pay desk creation. This field is read-only.
  [comment]: <> (Why is the format another one than for the store?)

- [SAVE]   
  Click this button to save any changes.

### Basic Data - Pay Desk
*Venduo POS > Management > Tab STORES > Select Store > Edit Pay Desk > Tab Basic Data*

![Pay Desk Basic Data](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/BasicData/BasicData.png "[Pay Desk Basic Data]")

- *Short Description*   
  Enter a short description to the pay desk.

- [SAVE]   
  Click this button to save any changes.

**Cashiers**

- [Add]      
  Click this button to add a cashier to the pay desk. The *Cashiers* window is displayed.

- *First Name*   
  First name of the cashier.

- *Last Name*   
  Last name of the cashier.

- *Login*   
  User name of the cashier.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the cashier. This button is only displayed when you hover over the cashier. Click the [SAVE] button to save the changes.

#### Cashiers
*Venduo POS > Management > Tab STORES > Select Store > Edit Pay Desk > Tab Basic Data > Add Cashier*

![Cashiers](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/BasicData/Cashiers.png "[Cashiers]")

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of cashiers.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all users are selected.

- [Add]   
  Click this button to add the selected user to the list of cashiers. This button is only displayed, when the checkbox of a user is selected.

The table displays all available cashiers. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *First Name*   
  First name of the user.

- *Last Name*   
  Last name of the user.

- *Login*   
  Login name of the user.

- *ID*   
  Identification number of the user.


### Admin Settings - Pay Desk
*Venduo POS > Management > Tab STORES > Select Store > Edit Pay Desk > Tab Admin Settings*

![Admin Settings Pay Desk](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings.png "[Admin Settings Pay Desk]")

#### UNKNOWN SECTION

In this section, you define all pay desk and payment settings.

#### Kasse öffnen bei Barzahlung

Activate or deactivate the option to open the cash drawer for cash payment.

![Kasse öffnen bei Barzahlung](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings01.png "[Kasse öffnen bei Barzahlung]")

- [x] *Kassenschublade öffnen bei Barzahlung*   
  Choose whether or not to open the cash drawer for cash payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Kasse öffnen nach bargeldlosem Zahlen

Activate or deactivate the option to open the cash drawer for cashless payment.

![Kasse öffnen nach bargeldlosem Zahlen](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings02.png "[Kasse öffnen nach bargeldlosem Zahlen]")

- [x] *Kasse öffnen*    
  Choose whether or not to open the cash drawer for cashless payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### BELEGDRUCK

#### Händler-Beleg drucken

Activate or deactivate the printing of a merchant receipt for cashless payment.

![Händler-Beleg drucken](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings03.png "[Händler-Beleg drucken]")

- [x] *Händler-Beleg drucken*   
  Choose whether or not to print a merchant receipt in addition to the customer receipt for cashless payments. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")    
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### Nativer Bon-Druck

Activate or deactivate the native receipt printing.

![Nativer Bon-Druck](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings04.png "[Nativer Bon-Druck]")

- [x] *Nativer Bon-Druck*   
  Choose whether or not to use the native receipt print. By default, this option is active.

  [comment]: <> ("Setting will be deleted, should always be active")

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### Logo-Druck Kompatibilitätsmodus

Activate or deactivate the compatibility mode for logo printing. As some receipt printer have issues with printing logos, it may help to activate this option.

![Logo-Druck](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings05.png "[Logo-Druck]")

- [x] *Logo-Druck Kompatibilitätsmodus*   
  Choose whether or not to use the compatibility mode for logo printing. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


#### Bon-Format

Define the width of the receipt, as it may vary depending on the printer.

![Logo-Druck](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings06.png "[Logo-Druck]")

- *Breite in Zeichen*   
  Define the width of the receipt in characters. This size is needed to calculate the width for the text.

  > [Info] So-called monospaced fonts are used For receipt printing. This means that each character has the same width.

- *Breite in Pixel*   
  Define the width of the receipt in pixels. This size is needed to calculate the width for images, e. g. logos.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the detail view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


#### DATENÜBERTRAGUNG RETAILSUITE FAKTURA

#### Kontenzuteilung Buchhaltung

Assign the accounts to which you want to book the payments. The accounts are assigned for all stores, unless they are overwritten in the store or pay desk admin settings.
For detailed information, see [Admin Settings - Store](#admin-settings-store) or [Admin Settings - Pay Desk](#admin-settings-pay-desk).

The number of accounts to be assigned depends on the number of available currencies.

![Zahlenformat](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/AdminSettings/AdminSettings07.png "[Zahlenformat]")

- *Type*   
  In this column, the account type is indicated. Six accounts are displayed per currency. The currency of the account is indicated in brackets after the account type name. The fields are display fields only. They cannot be changed.

  - *Bar*   
    This type of account serves as a cash account for cash payments.

  - *Redeem Voucher*    
    This type of account serves as --- add information ---

  - *Gegenkonto Cash-In*   
    This type of account serves as a clearing account against which cash deposits without customers are booked.

  - *Gegenkonto Cash-Out*   
    This type of account serves as a clearing account against which cash withdrawals without customers are booked.

  - *Refund auf Gutschein (refund only)*   
    This type of account serves as a refund account for refunds of cashless payments.

  - *Manuelles Zahlen am Terminal*   
    This type of account serves as a cash account for cashless payments.

- *Account*   
  Enter the account number for the corresponding account types. You can assign another account number for each account type.

- [Speichern]   
  Click this button to save any changes.



### Transactions
*Venduo POS > Management > Tab STORES > Select Store > Edit Pay Desk > Tab Transactions*

![Transactions](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/Transactions/Transactions.png "[Transactions]")

**Shifts**

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of shifts.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

The table displays the shift summaries of all shifts on the selected pay desk. Depending on the settings, the displayed columns may vary.

  > [Info] A shift starts, when a pay desk is opened and ends, when the pay desk is closed.

- *Print Shift Summary*    
  Click the link to print the selected shift summary. The shift summary is displayed in a new browser tab.   
  If you want to display the detailed transactions within a shift instead of print the shift summary, click the row with the shift (except the field *Print Shift Summary* to display the window *Transactions*).

[comments]: <> (For me, a new tab in the browser is displayed with the shift summary. Is it like that by default or do I have to configure it somewhere in the printing settings?)

- *Cashiers*   
  Full name and user name of the cashier within the shift. This field is read-only.

- *# Transactions*   
  Number of transactions made within the shift. This field is read-only.

- *Start*  
  Date and time of the shift start. This field is read-only.

- *Opening floats*   
  Cash balance at the shift start. This field is read-only.

- *Opening diffs*   
  Cash difference at the shift start. This field is read-only.

- *Revenue*
  Cash revenue of the shift. This field is read-only.

- *End*   
  Date and time of the shift end. This field is read-only.

- *Closing/current float*
  Cash balance at the shift end/Current cash balance. This field is read-only.

- *Closing diffs*   
  Cash difference at the shift end. This field is read-only.

- *ID*   
  Shift identification number. This field is read-only.


#### Transactions Details
*Venduo POS > Management > Tab STORES > Select Store > Edit Pay Desk > Tab Transactions > Select Shift*

![Transactions](/Assets/Screenshots/VenduoPOS/Management/Stores/PayDesk/Transactions/Details.png "[Transactions]")

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of transactions.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

The table displays the detailed transactions of the selected shift. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Cashier*   
  Full name and user name of the cashier who made the transaction.

- *Created*   
  Date and time of the transaction.

- *Type*  
   Type of transaction. The following types are available:
   - Cash payment
   - Cashless payment
   - Cash in
   - Cash out
   - Opening diff
   - Closing diff


- *Amount*   
  Amount of transaction.

- *Bill number*   
  Bill number of the transaction.

- *Comment*
  Comment to the transaction.

- *ID*   
  Identification number of the user.
