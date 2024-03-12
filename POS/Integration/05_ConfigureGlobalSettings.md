[!!Create a store in POS](./06_CreateStore.md)
[!!User interface Global settings](../UserInterface/02a_GlobalSettings.md)
[!!User interface DataHub ETL](../../DataHub/UserInterface/02a_Mappings.md)

[comment]: <> (add link to Order management module if available)

# Configure the global settings for POS

POS offers many settings to customize the POS system to your specific needs. For detailed information about the specific settings, see [Global Settings](../UserInterface/02a_GlobalSettings.md).

Before creating a new store in the POS system, you should configure the following settings:

- [Configure a default customer](#configure-a-default-customer) whose billing address will be added to all future POS bills to establish a connection to the *Order management* module.
- [Configure the VAT-ID in POS](#configure-the-VAT-ID-in-POS) for the printing on receipts, which is mandatory in most countries.


## Configure a default customer

To connect the POS system with the *Order management* module, you must define an invoice address for all occasional customers.   
Further, a delivery address and an invoice address should be indicated on every receipt created in the POS system. To specify an invoice address for occasional customers, you must create a default customer. The data of this default customer is used for all occasional customers.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*POS > Management > Tab GLOBAL SETTINGS > Entry Default customer*

![Default customer](../../Assets/Screenshots/POS/Management/GlobalSettings/GS27.png "[Default customer]")

1. Click the *Default customer* entry in the list of settings in the left column.   
    The *Default customer* view is displayed on the right side.

2. Enter the fields for the default customer.

    > [Info] You must at least enter the country and an e-mail address for the default customer.

3. Click the [Save] button in the upper right corner.   
    A confirmation message is displayed. The default customer is saved for all stores.



## Configure the VAT-ID in POS

In most countries it is mandatory to indicate the VAT-ID on receipts. Therefore, it is recommended to define the VAT-ID prior to creating a store.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*POS > Management > Tab GLOBAL SETTINGS > Entry VAT-ID*

![VAT-ID](../../Assets/Screenshots/POS/Management/GlobalSettings/GS08.png "[VAT-ID]")

1. Click the *VAT-ID* entry in the list of settings in the left column.   
    The *VAT-ID* view is displayed on the right side.

2. Enter the VAT-ID in the *VAT-ID* field.

3. Click the [Save] button in the upper right corner.   
    A confirmation message is displayed. The VAT-ID is saved for all stores.




## Define a new payment method for POS

By default, the payment methods debit card, credit card, and Paypal are predefined for the POS system. You can add several other payment methods that are predefined in the system, or you define a custom payment method for the POS system.

### Create a payment method in Order management

If the existing payment methods in *POS* are not appropriate for your special needs, you can create a custom payment method. Therefore, you have to create a new payment method in the *Order management* module first.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Order management > Settings > Tab PAYMENT METHOD(S)*

![Payment method](../../Assets/Screenshots/RetailSuiteFaktBase/Settings/PaymentMethods/PaymentMethods.png "[Payment methods]")

1. Click the [NEW] button.   
    The *Edit payment method* window is displayed.

    ![Edit payment method](../../Assets/Screenshots/RetailSuiteFaktBase/Settings/PaymentMethods/EditPaymentMethod.png "[Edit payment method]")

2. Enter a name for the payment method in the *Title* field.   

3. Enter an ID for the payment method in the *ID* field.   

4. Click the [SAVE] button in the bottom right corner of the window.   
    The *Saving...* window is displayed.

    When the window is closed, the new payment method is saved in the *Order management* module. The new payment method is displayed in the list of payment methods in the *PAYMENT METHOD(S)* tab.


### Create a payment method in POS

If the existing payment methods in *POS* are not appropriate for your special needs, you can create a custom payment method. Therefore, you have to create a new payment method in the *POS* module based on the payment method created in the *Order management* module.

#### Prerequisites

- A payment method has been created in the *Order management* module, see [Create a payment method in Order management](#create-a-payment-method-in-order-management).


#### Procedure

*POS > Management > Tab GLOBAL SETTINGS*

![GlobalSettings](../../Assets/Screenshots/POS/Management/GlobalSettings/GlobalSettings.png "[GlobalSettings]")

1. Click the *Payment methods (manual terminal payment)* setting in the list of settings.   
    The *Payment methods (manual terminal payment)* view is displayed.

    ![Payment methods](../../Assets/Screenshots/POS/Management/GlobalSettings/GS04.png "[Payment methods]")

2. Click the ![Add](../../Assets/Icons/Plus04.png "[Add]") (Add) button.
    A new row for a payment method is displayed.

3. Enter the key of the new payment method in the *Key* field.

4. Enter a name for the payment method in POS in the *Name* field.   

    > [Info] The name of the payment method in POS can differ from the name of the payment method in the *Order management* module. It is only necessary that the ID (key) of the payment method in *POS* and *Order management* match.

5. Click the [Save] button in the upper right corner.   
    The new payment method is saved in POS.




### Map the payment methods

If you have created a new payment method in POS, you need to map the payment method in POS with the payment method in the *Order Management* module.

<!---TO BE ENHANCED-->

#### Prerequisites

- A payment method has been created in the *Order management* module, see [Create a payment method in Order management](#create-a-payment-method-in-order-management).
- A payment method has been created in the *POS* module, see [Create a payment method in POS](#create-a-payment-method-in-pos).
- At least, one store has been created so that the relevant attribute set is available in the *DataHub* module, see [Configure the store details](./06_CreateStore.md#configure-the-store-details).

#### Procedure

*DataHub > ETL > Tab Mappings*

![ETL](../../Assets/Screenshots/DataHub/Settings/ETL/ETL.png "[ETL]")

1. Click the **Order channels POS Store "Name of the store"** attribute set mapping of the corresponding store in the *Source attribute set* column.   
    The *Mapping* view of the selected attribute set is displayed.

2. Click the attribute mapping with the **Payment method** attribute in the *Destination attribute* column.   
    The *Settings* section is displayed in the right part of the tab.

    ![Mapping](../../Assets/Screenshots/DataHub/Settings/ETL/MappingSettings.png "[Mapping]")

3. Click the *Extension* drop-down list in the *Settings* section and select the **Mapping table** option.

4. Click the *Source attribute* drop-down list in the *Settings* section and select the **Payment methods** option.   
    The mapping table for the selected mapping is displayed in the *Configuration* section.

5. Search for the *Order management* name of the new payment method in the *Source value* column, click the drop-down list in the same row in the *Destination value* column and select the *POS* name of the new payment method.

6. Click the [SAVE] button in the upper right corner.   
    The *Submitting data...* message is displayed in the right part of the *Mapping* view. The mapping is saved, when nothing is displayed in the right part of the *Mapping* view.
