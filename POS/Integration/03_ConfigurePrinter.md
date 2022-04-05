[!!Printing](Printing)

# Configure the printer client for POS

[comment]: <> (Need more information about the APS)

To print receipts, invoices, shift summaries etc., a printer must be configured for POS.

## Prerequisites

The current APS is installed and has been started including a successful login.

> [Info] Note that you have to use a separate user for the APS client as parallel logins are forbidden.

## Procedure

*Printing > Settings > Tab ASSIGN PRINTERS*

  ![Printing Settings](/Assets/Screenshots/Printing/Settings/AssignPrinters.png "[Printing Settings]")

1. Click the *Global (for all groups)* printer in the list of printers.   
  The *Settings for group Global* view is displayed.

  ![Settings Group](/Assets/Screenshots/Printing/Settings/SettingsGroup.png "[Settings Group]")

2. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Print Settings* window is displayed.

  ![Add Print Settings](/Assets/Screenshots/Printing/Settings/PrintSettings.png "[Add Print Settings]")

3. Click the *Client* drop-down list and select the appropriate client.

4. Click the *Printer* drop-down list and select the appropriate printer, for instance for receipts.

5. If necessary, click the *Tray* drop-down list and select the appropriate tray. By default, the tray is automatically selected.

6. Select the portrait or the landscape format in the *LAYOUT* section.

> [Info] For receipt printers always select portrait format.

7. Click the *Format* drop-down list and select the appropriate width of the receipt.

8. Click the *Module* drop-down list and select **POS** in the list of modules.

9. Click the *Event* drop-down list and select the appropriate pay desk and store in the list of pay desks.

10. Click the [SAVE] button in the bottom right corner of the window.   
  The printer is configured for the selected pay desk. The *Print Settings* window is closed. The *Settings for group Global* view is displayed again. The new setting is displayed in the list of settings.

[comment]: <> (Is that right? Check it, when APS is installed)

## Next steps

- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

## See also

- [User Interface Printing](/POS/UserInterface/00_UserInterface.md)
- [Install the APS](to_be_completed)
- [Select a printer](06_CreateStore.md)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
