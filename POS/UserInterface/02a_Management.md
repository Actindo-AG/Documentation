# Global Settings
*Venduo POS > Management > Tab GLOBAL SETTINGS*

In the tab *GLOBAL SETTINGS*, you define basic settings for all your stores.

  > [Info] Global settings are valid for all stores as long as no different settings are defined for the respective stores or pay desks.
  In principle, the more specific setting always overrides the more general setting.

![Global Settings](/Assets/Screenshots/POS/Management/GlobalSettings/GlobalSettings.png "[Global Settings]")

| (1) | **Selection list *Settings**|
|-----|---------------------|
|**(2)**|**View of the selected setting**|

In the left part of the page, the selection list *Settings* is displayed. The list is divided in the following sections:
 - [UNKNOWN SECTION](0#unknown-section)
 - [WÄHRUNGEN](#währungen)
 - [RETOUREN](#retouren)
 - [BELEGDRUCK](#belegdruck)
 - [DATENÜBERTRAGUNG RETAILSUITE FAKTURA](#datenübertragung-retailsuite-faktura)

In the right part of the page, a view of the selected setting is displayed when clicking on it.

In the following, each setting and its view is explained.

[comment]: <> (no section name for the first section -> Pay Desk and Payments?)

## UNKNOWN SECTION

In this section, you define all pay desk and payment settings.

## Format laufende Nummer
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Format laufende Nummer*

Configure the details of the POS specific cash receipt number. The cash receipt number is independent of the receipt number in invoicing and is therefore selected from a different number range to be defined here.

![Format laufende Nummer](/Assets/Screenshots/POS/Management/GlobalSettings/GS01.png "[Format laufende Nummer]")

- *Format*   
  Define the format of the sequential number. It is mandatory to include the store identifier (S) and the sequential number (L). The place holders are indicated on the right side.

- *Length of the sequential number*   
  Define the length of the sequential number.
  [comment]: <> (Is it the maximum length of the number or the exact length?)

- [x] *Reset after time interval*   
  Choose whether or not to reset the sequential number after the time interval.
  [comment]: <> (What does it mean?)

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")   
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Bon immer ausdrucken
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Bon immer ausdrucken*

Activate or deactivate the option to print the cash receipt.

 ![Bon immer ausdrucken](/Assets/Screenshots/POS/Management/GlobalSettings/GS02.png "[Bon immer ausdrucken]")

 - [x] *Bon immer ausrdrucken*   
   Choose whether or not to print the cash receipt for each transaction. If the receipt printing is deactivated, you can still initiate the receipt printing manually via the order history.

     > [Info] Remember that receipt printing is mandatory in several countries. Please inform yourself about the country-specific regulations before you deactivate this option.

 - *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
   Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


## Anzahl Gutscheine pro Bestellung
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Anzahl Gutscheine pro Bestellung*

Define how many vouchers may be redeemed per order.

![Anzahl Gutscheine pro Bestellung](/Assets/Screenshots/POS/Management/GlobalSettings/GS03.png "[Anzahl Gutscheine pro Bestellung]")

- *Anzahl Gutscheine pro Bestellung*   
  Enter the number of vouchers that can be redeemed per order. By default, one voucher per order is set.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Zahlungsweisen (manuelle Zahlung Terminal)

*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Zahlungsweisen (manuelle Zahlung Terminal)*

If you use an external terminal that is not connected to Venduo POS, cashless payment is completed manually through that terminal.
In Venduo POS, you can specify for statistical purposes which payment method was used for the cashless payment. You define the different payment methods in this setting.

![Zahlungsweisen](/Assets/Screenshots/POS/Management/GlobalSettings/GS04.png "[Zahlungsweisen]")

> [Info] By default, the payments methods *debit card*, *credit card* and *PayPal* are preset.

- *Key*   
  Enter the key of the payment method. The following keys are available:
  [comment]: <> (list of keys is needed)

- *Name*   
  Enter the name of the payment method.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)    
  Click this button to delete the payment method left to the button.

- ![Add](/Assets/Icons/Plus04.png "[Add]") (Add)    
  Click this button to add a new payment method. A new line for a payment method is displayed.

- [Speichern]   
  Click this button to save any changes.


## Automatischer Discount
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Automatischer Discount*

Define a discount that is automatically applied above a certain amount.

![automatischer Discount](/Assets/Screenshots/POS/Management/GlobalSettings/GS05.png "[automatischer Discount]")

- *ab Betrag*   
  Enter the amount from which the discount is granted.

- *Discount in %*   
  Enter the amount of the discount in percent.

  > [Info] If you leave the fields blank, no automatic discount will be granted.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the discount left to the button.

- ![Add](/Assets/Icons/Plus04.png "[Add]") (Add)  
  Click this button to add a new discount. A new line for a discount is displayed.

- [Speichern]    
  Click this button to save any changes.


## Kasse öffnen bei Barzahlung
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Kasse öffnen bei Barzahlung*

Activate or deactivate the option to open the cash drawer for cash payment.

![Kasse öffnen bei Barzahlung](/Assets/Screenshots/POS/Management/GlobalSettings/GS06.png "[Kasse öffnen bei Barzahlung]")

- [x] *Kassenschublade öffnen bei Barzahlung*   
  Choose whether or not to open the cash drawer for cash payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


## Kasse öffnen nach bargeldlosem Zahlen
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Kasse öffnen nach bargeldlosem Zahlen*

Activate or deactivate the option to open the cash drawer for cashless payment.

![Kasse öffnen nach bargeldlosem Zahlen](/Assets/Screenshots/POS/Management/GlobalSettings/GS07.png "[Kasse öffnen nach bargeldlosem Zahlen]")

- [x] *Kasse öffnen*    
  Choose whether or not to open the cash drawer for cashless payment. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


## USt-ID
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry USt-ID*

Define the VAT ID, which is mandatory to be indicated on receipts in some countries.

![USt-ID](/Assets/Screenshots/POS/Management/GlobalSettings/GS08.png "[USt-ID]")

- *USt-ID*   
  Enter your VAT ID. By default, The VAT-ID is printed on your receipts.

- [Speichern]    
  Click this button to save any changes.


## Bargeldloses Zahlen
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Bargeldloses Zahlen*

Activate or deactivate the options for cashless payment.

![Bargeldloses Zahlen](/Assets/Screenshots/POS/Management/GlobalSettings/GS09.png "[Bargeldloses Zahlen]")

- [x] ![Voucher](/Assets/Icons/Voucher.png "Voucher") *Refund auf Gutschein (refund only)*   
  Choose whether or not to refund cashless payments only on vouchers. By default, this option is inactive.

- [x] ![Terminal](/Assets/Icons/Terminal.png "Terminal") *Manuelles Zahlen am Terminal*   
  Choose whether or not to allow cashless payments via manual payment at the terminal. If you use an external terminal that is not connected to Venduo POS, you need to enable that option. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


## Kassenjournal auf User binden
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Kassenjournal auf User binden*

When a pay desk is opened, it is linked to a specific user. This user is the only one who can use the pay desk until he closes it again. To allow that several users can access the same pay desk without closing it, you can deactivate the option to link the cash register to a specific user.

![Kassenjournal auf User binden](/Assets/Screenshots/POS/Management/GlobalSettings/GS10.png "[Kassenjournal auf User binden]")

- [x] *Kassenbuch auf User gebunden*   
  Choose whether or not to link the cash register to a special user. By default, this option is active.

  > [Info] Remember that even if you deactivate this option, a user must log out to allow another user to access the pay desk.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Abschöpfen bis Betrag
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Abschöpfen bis Betrag*

Define an amount up to which the pay desk is skimmed after the pay desk closes. The amount is automatically entered in the cash register and taken as the opening float.

![Abschöpfen bis Betrag](/Assets/Screenshots/POS/Management/GlobalSettings/GS11.png "[Abschöpfen bis Betrag]")

- *Abschöpfen bis Betrag*    
  Enter the amount up to which the pay desk is skimmed after the pay desk closing.

- [Speichern]  
  Click this button to save any changes.


## Erwarteten Betrag verbergen
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Erwarteten Betrag verbergen*

By default, the expected amount in the pay desk is indicated. deactivate this option to hide the expected amount from the cashier in order to prevent the concealment of shortfalls.

![Erwarteten Betrag verbergen](/Assets/Screenshots/POS/Management/GlobalSettings/GS12.png "[Erwarteten Betrag verbergen]")

- [x] *Erwarteten Betrag verbergen*   
  Choose whether or not to hide the expected amount in the pay desk from the cashier. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## WÄHRUNGEN

In this section, you define all settings concerning the currencies in your POS system.

## Available Currencies
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Available Currencies*

Define the currencies that are available in your POS system as well as the coins and bills that exist in each currency. By default, the four currencies Euro, Swiss Franc, US Dollar and British Pound are predefined.

[comment]: <> (is that right?)

![Verfügbare Währungen](/Assets/Screenshots/POS/Management/GlobalSettings/GS13.png "[Verfügbare Währungen]")

**AvailableCurrencies**

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the column editing bar and customize the displayed columns and the order of columns in the table. The *x* indicates the number of columns that are currently displayed in the table.

- [x]     
  Select the checkbox to display the editing toolbar and to edit or delete the selected currency.

- [EDIT]   
  Click this button to edit the selected currency. The [*Edit currency*](#edit-currency) view is displayed. This button is displayed only if a currency checkbox is selected.

- [DELETE]   
  Click this button to delete the selected currency. This button is displayed only if a currency checkbox is selected.

The table displays all available currencies. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *Name*  
  Name or abbreviation of the currency.

- *Abkürzung*    
  Symbol of the currency.

- *Münzen*   
  Available coins (values) of the currency.

- *Scheine*   
  Available bills (values) of the currency.

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a new currency to the list of currencies. The [*Create currency*](#create-currency) view is displayed where you have to define the currency settings.

- [SAVE]  
  Click this button to save any changes.



### Create currency
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Available Currencies > Button Add*

Add a new currency to the list of available currencies and define the coins and notes of the new currency.

![Währung anlegen](/Assets/Screenshots/POS/Management/GlobalSettings/GS13b.png "[Währung anlegen]")

**DESCRIPTION**
- *Name*   
  Enter the name of the new currency.

- *Symbol*   
  Enter the symbol of the new currency.

**COINS AND NOTES**

- ![Banknote](/Assets/Icons/Banknote01.png "[Banknote]") (Banknote)   
  The banknote icon indicates which banknotes are defined for the respective currency. The number in the middle indicates the amount of the banknote.  
  When you hover over a banknote icon, the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) is displayed in the upper right corner of the banknote. Click the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) to delete the banknote.
  The banknote icon is displayed only if a banknote is defined for the currency.

- ![Coin](/Assets/Icons/Coin.png "[Coin]") (Coin)   
  The coin icon indicates which coins are defined for the respective currency. The number in the middle indicates the amount of the coin.   
  When you hover over a coin icon, the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) is displayed in the upper right corner of the coin. Click the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) to delete the coin.
  The coin icon is displayed only if a coin is defined for the currency.

- *Betrag*   
  Enter the amount of the banknote or the coin.

- *Note*   
  Click the drop-down list to select if the entered amount refers to a banknote or a coin.

- ![Add](/Assets/Icons/Plus04.png "[Add]") (Add)    
  Click this button to add the specified banknote or coin to the currency.

- [CANCEL]   
  Click this button to cancel the creation of a new currency. The view *Available Currencies* is displayed again.

- [SAVE]   
  Click this button to save the new currency and add it to the list of currencies. The view *Available Currencies* is displayed again.


### Edit currency
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Available Currencies > Button Edit*

Edit the settings of an existing currency.

![Währung bearbeiten](/Assets/Screenshots/POS/Management/GlobalSettings/GS13c.png "[Währung bearbeiten]")

**DESCRIPTION**
- *Name*   
  Enter the name of the currency.

- *Symbol*   
  Enter the symbol of the currency.

**COINS AND NOTES**

- ![Banknote](/Assets/Icons/Banknote01.png "[Banknote]") (Banknote)   
  The banknote icon indicates which banknotes are defined for the respective currency. The number in the middle indicates the amount of the banknote.   
  When you hover over a banknote icon, the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) is displayed in the upper right corner of the banknote. Click the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) to delete the banknote.
  The banknote icon is displayed only if a banknote is defined for the currency.

- ![Coin](/Assets/Icons/Coin.png "[Coin]") (Coin)   
  The coin icon indicates which coins are defined for the respective currency. The number in the middle indicates the amount of the coin.   
  When you hover over a coin icon, the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) is displayed in the upper right corner of the coin. Click the button ![Delete Currency](/Assets/Icons/Cross05.png "[Delete Currency]") (Delete) to delete the coin.
  The coin icon is displayed only if a coin is defined for the currency.

- *Betrag*   
  Enter the amount of the banknote or the coin.

- *Note*   
  Click the drop-down list to select if the entered amount refers to a banknote or a coin.

- ![Add](/Assets/Icons/Plus04.png "[Add]") (Add)   
  Click this button to add the specified banknote or coin to the currency.

- [CANCEL]   
  Click this button to discard the changes to the currency. The view *Available Currencies* is displayed again.

- [SAVE]   
  Click this button to save all changes. The view *Available Currencies* is displayed again.


## Verwendete Währungen
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Verwendete Währungen*

Select all currencies that are used in your POS system and define a default currency.

![Verwendete Währungen](/Assets/Screenshots/POS/Management/GlobalSettings/GS14.png "[Verwendete Währungen]")

- [x] *Currency Name*   
  Choose whether or not to use this currency in your POS system.

- *Standard*   
  Click the drop-down list to select the currency that is used as default currency. All available currencies are displayed in the drop-down list. When you select a default currency that is not yet selected as used currency, that currency is automatically selected as used currency.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## RETOUREN

In this section, you define all settings concerning returns.

## Retouren-Gründe
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Retouren-Gründe*

Define the return reasons that are available in the POS system.

![Retouren-Gründe](/Assets/Screenshots/POS/Management/GlobalSettings/GS15.png "[Retouren-Gründe]")

- *Schlüssel*   
  Enter the return reason key. The following keys are available:
  [comment]: <> (insert list of return reason keys)

- *Wert*   
  Enter a value for the return reason. The value is displayed when returning an order.

- ![Delete](/Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the return reason left to the button.

- ![Add](/Assets/Icons/Plus04.png "[Add]") (Add)   
  Click this button to add a return reason. A new line for a return reason is displayed.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Refund nur auf gleiches Zahlungsmittel
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Refund nur auf gleiches Zahlungsmittel*

Activate or deactivate the refund to the same payment method for returns.

![Refund Zahlungsmittel](/Assets/Screenshots/POS/Management/GlobalSettings/GS16.png "[Refund Zahlungsmittel]")

- [x] *nur auf gleiches Zahlungsmittel*   
  Choose whether or not a refund for a return can only be made to the same payment method. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Retoure nur in gleichem Store
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Retoure nur in gleichem Store*

Activate or deactivate the return to the same store.

![Retoure Store](/Assets/Screenshots/POS/Management/GlobalSettings/GS17.png "[Retoure Store]")

- [x] *Retoure nur in gleichem Store*   
  Choose whether or not a return can only be made in the same store. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## BELEGDRUCK

In this section, you define all settings concerning the receipt printing.

## Händler-Beleg drucken
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Händler-Beleg drucken*

Activate or deactivate the printing of a merchant receipt for cashless payment.

![Händler-Beleg drucken](/Assets/Screenshots/POS/Management/GlobalSettings/GS18.png "[Händler-Beleg drucken]")

- [x] *Händler-Beleg drucken*   
  Choose whether or not to print a merchant receipt in addition to the customer receipt for cashless payments. By default, this option is active.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")      
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Nativer Bon-Druck
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Nativer Bon-Druck*

Activate or deactivate the native receipt printing.

![Nativer Bon-Druck](/Assets/Screenshots/POS/Management/GlobalSettings/GS19.png "[Nativer Bon-Druck]")

- [x] *Nativer Bon-Druck*   
  Choose whether or not to use the native receipt print. By default, this option is active.

  [comment]: <> ("Setting will be deleted, should always be active")

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Logo-Druck Kompatibilitätsmodus
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Logo-Druck Kompatibilitätsmodus*

Activate or deactivate the compatibility mode for logo printing. As some receipt printer have issues with printing logos, it may help to activate this option.

![Logo-Druck](/Assets/Screenshots/POS/Management/GlobalSettings/GS20.png "[Logo-Druck]")

- [x] *Logo-Druck Kompatibilitätsmodus*   
  Choose whether or not to use the compatibility mode for logo printing. By default, this option is inactive.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


## Bon-Format
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Bon-Format*

Define the width of the receipt, as it may vary depending on the printer.

![Logo-Druck](/Assets/Screenshots/POS/Management/GlobalSettings/GS21.png "[Logo-Druck]")

- *Breite in Zeichen*   
  Define the width of the receipt in characters. This size is needed to calculate the width for the text.

  > [Info] So-called monospaced fonts are used For receipt printing. This means that each character has the same width.

- *Breite in Pixel*   
  Define the width of the receipt in pixels. This size is needed to calculate the width for images, for instance logos.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Zahlenformat
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Zahlenformat*

Define the number format on the receipt.

![Zahlenformat](/Assets/Screenshots/POS/Management/GlobalSettings/GS22.png "[Zahlenformat]")

- *Decimal separator*   
  Enter the decimal separator for the numbers on your receipt. You can use any separator including a blank space. This field is mandatory.

- *Thousand separator*   
  Enter the thousand separator for the numbers on your receipt. You can use any separator including a blank space.

- *Precision*   
  Enter the number of decimal places for the numbers on your receipt or use the arrow buttons in the field to increase or decrease the number of decimal places. You can select a number between 0 and 4. This field is mandatory.

  > [Info] The sample view below the input fields displays a live preview of the number with the selected separators and decimal places.

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]    
  Click this button to save any changes.


## Logo
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Logo*

Upload a logo for your receipts.

![Logo](/Assets/Screenshots/POS/Management/GlobalSettings/GS23.png "[Logo]")

  >  [Info] The png format is the only image format supported for logo images. So make sure that your image logo is also saved in the png format before uploading it.

- [SELECT FILE]   
  Click this button to select a logo image for your receipts. The explorer is displayed for image selection. The selected logo image is displayed in the preview box right from the button. Alternatively, you can select an image using drag & drop.

- ![Upload](/Assets/Icons/Upload.png "[Upload]") *Drop file here...*   
  Drag the logo image from your local folder and drop it in this dashed box to upload it. The background color of the box turns to blue when you can drop the image.  The selected logo image is displayed in the preview box right from the button. Alternatively, you can select an image using the button [SELECT FILE].

- Preview box   
  The preview box displays the uploaded logo image. If a logo image is already displayed and you upload a new one, the current logo image will be overwritten by the new logo image.
  Remove a displayed logo by clicking the button ![Remove](/Assets/Icons/Cross03.png "[Remove]") (Remove) in the upper right corner of the logo.

- [Speichern]   
  Click this button to save any changes.


## DATENÜBERTRAGUNG RETAILSUITE FAKTURA

In this section, you define all settings concerning the connection to invoicing. The settings are only displayed if the accounting is correctly configured.

## Kontenzuteilung Buchhaltung
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Kontenzuteilung Buchhaltung*

Assign the accounts to which you want to book the payments. The accounts are assigned for all stores, unless they are overwritten in the store or pay desk admin settings.
For more information, see [Admin Settings - Store](02b_Management.md#admin-settings-store) or [Admin Settings - Pay Desk](02b_Management.md#admin-settings-pay-desk).

The number of accounts to be assigned depends on the number of available currencies.

![Zahlenformat](/Assets/Screenshots/POS/Management/GlobalSettings/GS24.png "[Zahlenformat]")

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


## Korrekturbuchung auf Ursprungslager
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Korrekturbuchung auf Ursprungslager*

Activate or deactivate the reverse booking to the original warehouse. Any discrepancies in store deliveries are automatically booked back to the original warehouse.   

![Korrekturbuchung](/Assets/Screenshots/POS/Management/GlobalSettings/GS25.png "[Korrekturbuchung]")

- [x] *Korrekturbuchung auf Ursprungslager*    
  Choose whether or not to book discrepancies between the delivery receipt and the delivery are automatically booked back to the original warehouse. By default, this option is active.

    >  [Info] This option is only applicable if store deliveries are activated.    
    For detailed information, see [Shop-Lieferungen aktiv](POS_UserInterface_02_Management.md####Shop-Lieferungen-aktiv).

- *Von Default übernehmen* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]")     
  Activate this toggle to apply the default settings or deactivate this toggle to specify custom settings. When the toggle is active, all fields in the view are locked. By default, this toggle is active.

- [Speichern]   
  Click this button to save any changes.


## Retourenlager (Sperrlager)
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Retourenlager (Sperrlager)*

[comment]: <> (need information; Is that right?)

Define a shelf in the quarantine warehouse for returns with defects.

![Retourenlager](/Assets/Screenshots/POS/Management/GlobalSettings/GS26.png "[Retourenlager]")

- *Lager ID*   
  Enter the number of the quarantine warehouse.

[comment]: <> (Is shelf name right? Not number of the shelf?)

- *Fachname*   
  Enter the name of the shelf for the defect returns.

- [Speichern]   
  Click this button to save any changes.


## Standard-Kunde
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Standard-Kunde*

Define an invoice address for a default customer to connect the POS system with the invoicing. The invoice address of this default customer is used for all occasion customers.

![Standard-Kunde](/Assets/Screenshots/POS/Management/GlobalSettings/GS27.png "[Standard-Kunde]")

- *Title*   
  Enter the customer title.

- *First Name*   
  Enter the customer first name.

- *Last Name*   
  Enter the customer last name.

- *Company*   
  Enter the customer company name.

- *Email Name*   
  Enter the customer e-mail address.

- *Street*   
  Enter the street name of the customer address.

- *HouseNumber*   
  Enter the house number of the customer address.

- *ZIP*   
  Enter the ZIP code of the customer address.

- *City*   
  Enter the city name of the customer address.

  [comment]: <> (Should the country field be mandatory and a drop-down list?)

- *Country*   
  Enter the country name of the customer address.

  >  [Info] It is recommended to define at least the country of the customer address as it is needed for tax purposes.

- [Speichern]    
  Click this button to save any changes.


## Shop-Lieferungen aktiv
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Shop-Lieferungen aktiv*

Activate or deactivate the store deliveries. If the store deliveries are active, deliveries to the store can be entered and the POS inventory is automatically increased by the delivered products.

>  [Info] Deliveries to the store can only be added if a delivery receipt for this delivery exists in invoicing.

![Shop-Lieferungen aktiv](/Assets/Screenshots/POS/Management/GlobalSettings/GS28.png "[Shop-Lieferungen aktiv]")

- [x] *Shop-Lieferung aktiv*   
  Choose whether or not to activate deliveries from the store. By default, this option is inactive.   
  When the store deliveries are active, the three new tabs [*ABGESCHLOSSENE LIEFERSCHEINE*](02e_Management.md), [*OFFENE LIEFERSCHEINE*](02f_Management.md) and  [*WARENEINGANGS-SYNC*](02g_Management.md) are displayed in the menu entry *Management* and the new tab [*WARENEINGANG*](01g_Sales.md) is displayed in the menu entry *Sales*.

  >  [Info] You have to save the changes and press **F5** to initialize the Core1 Platform and display the new tabs.


- [Speichern]    
  Click this button to save any changes.


## Kundendaten aus RetailSuite übernehmen
*Venduo POS > Management > Tab GLOBAL SETTINGS > Entry Kundendaten aus RetailSuite übernehmen*

Activate or deactivate the application of customer data from RetailSuite.

![Kundendaten RetailSuite](/Assets/Screenshots/POS/Management/GlobalSettings/GS29.png "[Kundendaten RetailSuite]")

- [x] *Kundendaten aus RetailSuite uebernehmen*   
  Choose whether or not to apply customer data from RetailSuite when receipts are linked to a customer. By default, this option is active.

- [Speichern]    
  Click this button to save any changes.
