[!!Einstellungen](Actindo/Einstellungen)

# Establish the RetailSuite Connection

## Error Description
The RetailSuite is not connected to Venduo POS. The section *DATENÜBERTRAGUNG RETAILSUITE FAKTURA* is not displayed in the global settings.

Follow the instructions below to establish the connection to the RetailSuite.

## Prerequisites

You have the rights to install a plugin in the *Platform Manager*.

## Procedure

*Einstellungen > Platform Manager > Tab PLUGIN-ÜBERSICHT*

![Plugin Übersicht](/Assets/Screenshots/Einstellungen/PlatformManager/PluginUebersicht.png "[Plugin Übersicht]")

1. Check, if the plugin *UCS Sync for POS* is already installed.   

- If the plugin *UCS Sync for POS* is not yet installed, do the following:

  2. In the left section *Verfügbare Module* click the three points right to *Plugin* .   
    A context menu is displayed.

    ![Context Menu](/Assets/Screenshots/Einstellungen/PlatformManager/ContextMenu.png "[Context Menu]")

  3. Click the menu entry *Filters* .   
    The checkbox of the menu entry *Filters* is selected. A search bar is displayed right to the menu entry *Filters* .   

  4. Enter **UCS Sync for POS** in the search bar and click the **Enter** button on your keyboard to start the search.
    The plugin *UCS Sync for POS* is displayed in the section *Verfügbare Module*.

    > [Info] If the plugin *UCS Sync for POS* is not displayed, check the spelling of the entered search keyword. If you did no spelling mistake, check again, if the plugin is not already installed by searching it in the right section *installierte Module* .

  5. Click the plugin *UCS Sync for POS* in the left section *Verfügbare Module* and, using drag and drop, pull it in the right column *installierte Module* .   
  The plugin is displayed in the section *installierte Module*. The column *Status* indicates, if all dependencies for installing the plugin are fulfilled.

    ![Install Plugin](/Assets/Screenshots/Einstellungen/PlatformManager/InstallPlugin.png "[Install Plugin]")

    > [Info] Make sure that all dependencies are fulfilled before installing the plugin to guarantee the whole functuality.

  6. Click the button [ANWENDEN] in the upper right corner of the section *installierte Module* .   
    The *Änderungen anwenden* window is displayed. The tab *Reihenfolge festlegen* is preselected. The plugin *UCS Sync for POS* is displayed in the list.

    ![Reihenfolge Festlegen](/Assets/Screenshots/Einstellungen/PlatformManager/ReihenfolgeFestlegen1.png "[Reihenfolge Festlegen]")

  7. Click the button [AUSFÜHREN] in the bottom right corner of the window.   
    The tab *Änderungen ausführen* is displayed.

    ![Änderungen ausführen](/Assets/Screenshots/Einstellungen/PlatformManager/AenderungenAusfuehren1.png "[Änderungen ausführen]")

    The plugin is installed when the progress bar displays **100%**.

  8. Press **F5** to initialize the Core1 Platform.


  - If the plugin *UCS Sync for POS* is already installed, do the following:

    2. Double-click the row of the plugin *UCS Sync for POS* in the section *installierte Module* .  
      The fields of the plugin are unlocked.

      ![Installer ausführen](/Assets/Screenshots/Einstellungen/PlatformManager/InstallerAusfuehren.png "[Installer ausführen]")

    3. Select the option **Installer erneut ausführen** in the drop-down list of the column *Aktion*.

    4. Click the button [UPDATE] above the row.

    5. Click the button [ANWENDEN] in the upper right corner of the section *installierte Module* .   
      The *Änderungen anwenden* window is displayed. The tab *Reihenfolge festlegen* is preselected. The plugin *UCS Sync for POS* is displayed in the list.

      ![Reihenfolge Festlegen](/Assets/Screenshots/Einstellungen/PlatformManager/ReihenfolgeFestlegen2.png "[Reihenfolge Festlegen]")

    6. Click the button [AUSFÜHREN] in the bottom right corner of the window.   
      The tab *Änderungen ausführen* is displayed. The plugin is updated when the progress bar displays **100%**.

      ![Änderungen ausführen](/Assets/Screenshots/Einstellungen/PlatformManager/AenderungenAusfuehren2.png "[Änderungen ausführen]")

    7. Press **F5** to initialize the Core1 Platform.



## See also

- [User Interface Einstellungen](/Einstellungen/UserInterface/00_UserInterface.md)


## Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
