[!!Venduo POS](Actindo/Venduo POS)
[!!Fakturierung](Actindo/Fakturierung)
[!!DataHub](Actindo/DataHub)

# Configure the global settings for POS

Venduo POS provides many settings to  configure the POS system individually.

For detailed information about the specific settings, see [User Interface Venduo POS/Management](VenduoPOS/UserInterface/02a_Management.md#global-settings).

Before creating a new store in the POS system, you should configure the following settings:

- [Configure a default customer](#configure-a-default-customer) to establish a connection to invoicing which will be added as billing address to all future POS bills.
- [Configure the VAT-ID in POS](#configure-the-VAT-ID-in-POS) for the printing on receipts, which is mandatory in most countries.


## Configure a default customer

To connect the POS system with the invoicing, an invoice address has to be defined for all occasion customers.   
Further, a delivery address and an invoice address should be indicated on every receipt created in the POS system. To specify a invoice address for occasion customers, a default customer must be created. The data of this default customer is used for all occasion customers.

### Prerequisites

No prerequisites to fulfill.

### Procedure

*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Default Customer*

  ![Default Customer](/Assets/Screenshots/VenduoPOS/Management/GlobalSettings/GS27.png "[Default Customer]")

1. Select the entry *Standard-Kunde* in the list of settings in the left column.

  The section *Standard-Kunde* is displayed on the right side.

2. Enter the fields for the default customer.

  > [Info] You must at least enter the country and an e-mail address for the default customer.

3. Click the button [Speichern] in the upper right corner.   
  The message *Saving successful* is displayed. The default customer is saved for all stores.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")

### Next Steps

- [Configure the VAT-ID in POS](#configure-the-VAT-ID-in-POS)
- [Define a new payment method for POS](#define-a-new-payment-method-for-POS)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Venduo POS](VenduoPOS/UserInterface/00_UserInterface.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)


## Configure the VAT-ID in POS

In most countries it is mandatory to indicate the VAT-ID on receipts. Therefore, it is recommended to define the VAT-ID prior to creating a store.

### Prerequisites

No prerequisites to fulfill.

### Procedure

*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry VAT-ID*

  ![VAT-ID](/Assets/Screenshots/VenduoPOS/Management/GlobalSettings/GS08.png "[VAT-ID]")

1. Select the entry *USt-ID* in the list of settings in the left column.   
  The section *USt-ID* is displayed on the right side.

2. Enter the VAT-ID in the field *USt-ID*.

3. Click the button [Speichern] in the upper right corner.   
  The message *Saving successful* is displayed. The VAT-ID is saved for all stores.

  ![Saving successful](/Assets/Screenshots/SavingSuccessful.png "[Saving successful]")

### Next Steps

- [Define a new payment method for POS](#define-a-new-payment-method-for-POS)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Venduo POS](VenduoPOS/UserInterface/00_UserInterface.md)
- [Configure a default customer](#configure-a-default-customer)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)


## Define a new payment method for POS

By default, the payment methods debit card, credit card and paypal are predefined for the POS system. You can add several other payment methods that are predefined in the system, see [Payment methods](to_be_completed) or you define a custom payment method for the POS system.

### Prerequisites

No prerequisites to fulfill.

### Procedure

#### Create a payment method in Invoicing
*Fakturierung > Einstellungen > Tab ZAHLARTEN*

![Zahlarten](/Assets/Screenshots/Fakturierung/Einstellungen/Zahlarten/Zahlarten01.png "[Zahlarten]")

1. Click the button [NEU].   
  The *Zahlart bearbeiten* window is displayed.

  ![Zahlart bearbeiten](/Assets/Screenshots/Fakturierung/Einstellungen/Zahlarten/ZahlartBearbeiten.png "[Zahlart bearbeiten]")

2. Enter a name for the payment method in the field *Titel*.   

3. Enter an ID for the payment method in the field *ID*.   

4. Click the button [SPEICHERN] in the bottom right corner of the window.   
  The *Speichere...* window is displayed.

  ![Speichere](/Assets/Screenshots/Fakturierung/Einstellungen/Zahlarten/Speichere.png "[Speichere]")

  When the window is closed, the new payment method is saved in Invoicing. The new payment method is displayed in the list of payment methods in the tab *ZAHLARTEN*.


#### Create a payment method in POS
*Venduo POS > Management > Tab GLOBAL SETTINGS*

![GlobalSettings](/Assets/Screenshots/VenduoPOS/Management/GlobalSettings/GlobalSettings.png "[GlobalSettings]")

1. Click the setting *Zahlungsweisen (manuelle Zahlung Terminal)* in the list of settings.   
  The *Zahlungsweisen (manuelle Zahlung Terminal)* view is displayed.

  ![Zahlungsweisen](/Assets/Screenshots/VenduoPOS/Management/GlobalSettings/GS04.png "[Zahlungsweisen]")

2. Click the button ![Add](/Assets/Icons/Plus04.png "[Add]") (Add).
  A new row for a payment method is displayed.

3. Enter the key of the new payment method in the field *Key*.

4. Enter a name for the payment method in POS in the field *Name*.   

    > [Info] The name of the payment method in POS can differ from the name of the payment method in the *Invoicing* module. It is only necessary that the ID of the payment method in *Venduo POS* and *Invoicing* match.

5. Click the button [Speichern] in the upper right corner.   
    The new payment method is saved in POS.


#### Map the payment methods
*DataHub > Settings > Tab ETL*

![ETL](/Assets/Screenshots/DataHub/Settings/ETL/ETL.png "[ETL]")

1. Click the attribute set mapping **Orders POS Store** of the corresponding store in the column *Source Attribute Set* .   
  The *Mapping* view of the selected attribute set is displayed.

2. Click the attribute mapping with the attribute **Zahlungsweise** in the column *Destination Attribute* .   
  The section *Settings* is displayed in the right part of the tab.

  ![Mapping](/Assets/Screenshots/DataHub/Settings/ETL/MappingSettings.png "[Mapping]")

3. Click the drop-down list *Extension* in the section *Settings* and select the option **Mapping table**.

4. Click the drop-down list *Source attribute* in the section *Settings* and select the option **Zahlungsweisen** .   
    The mapping table for the selected mapping is displayed in the section *Configuration*.

5. Search for the invoicing name of the new payment method in the column *Source Value*, click the drop-down list in the same row in the column *Destination Value* and select the Venduo POS name of the new payment method.

6. Click the button [SAVE] in the upper right corner.   
    *Submitting data...* is displayed in the right part of the *Mapping* view. The mapping is saved, when nothing is displayed in the right part of the *Mapping* view.


### Next Steps

- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

### See also

- [User Interface Venduo POS](VenduoPOS/UserInterface/00_UserInterface.md)
- [Configure a default customer](#configure-a-default-customer)
- [Configure the VAT-ID in POS](#configure-the-VAT-ID-in-POS)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
