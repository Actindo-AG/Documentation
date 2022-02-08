[!!Lager](Actindo/Lager)

# Manage the POS warehouse

Manage the warehouse settings to assign one or more specific warehouses to the POS from which the stock is taken and booked. The warehouse specifies where exactly the stock is booked out when a product is sold.

## Check the inventory assignment

Check if the inventory assignment is correctly configured so that the store inventory is correctly assigned to the warehouse. The inventory source specifies how the inventory available in the POS system is calculated. In most cases, the inventory source and the warehouse are identical, but they can also differ.   

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- The inventory assignment is configured, see [Configure the inventory assignment](06_CreateStore.md#configure-the-inventory-assignment).

### Procedure

*Lager > Einstellungen > Tab LAGER > Tab Bestandszuteilung*

![Bestandszuteilung](/Assets/Screenshots/Lager/Einstellungen/Lager/Bestandszuteilung/Bestandszuteilung.png "[Bestandszuteilung]")

1.  Search for the target channel of the appropriate POS store in the column *Zielkanal*  and check the settings in the corresponding row.

2. If necessary, edit the settings as described in the following:
  - Select the option **Berechnung, Lagerbestand** in the drop-down list in the column *Bestandsberechnung* .   
    The fields in the warehouse columns are unlocked.

  - Double-click the option in a warehouse column to display the drop-down list.

  - Select the option **Yes** in the drop-down list to include the corresponding warehouse in the inventory calculation or select the option **No** to exclude it.

  > [Info] Select for each warehouse whether it should be included or not.

3. Click the button [SPEICHERN] in the bottom right corner.   
  The inventory assignment is saved. The stock is calculated from all selected warehouses.

### Next steps

- [Check the stock source matrix](#check-the-stock-source-matrix)
- [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products)
- [Manage the stock for POS products](#manage-the-stock-for-pos-products)

### See also

- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)


## Check the stock source matrix

Check if the stock source matrix is correctly configured so that a specific warehouse is assigned to a specific store in POS.

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- The stock source matrix is configured, see [Configure the stock source matrix](06_CreateStore.md#configure-the-stock-source-matrix).

### Procedure

*Lager > Einstellungen > Tab LAGER > Tab Lagerentnahme-Matrix*

![Lagerentnahme-Matrix](/Assets/Screenshots/Lager/Einstellungen/Lager/LagerentnahmeMatrix/LagerentnahmeMatrix.png "[Lagerentnahme-Matrix]")

1. Search for the appropriate POS store in the column *Account* and check the settings in the corresponding row.   

2. If necessary, edit the settings as described in the following:

  + Select the option **--alle--** in the drop-down list in the column *Produkt-Warengruppe*.

  + Select the output channel via which you want to create offers in the drop-down list in the column *Marktplatz*.

  + Select the option **--alle--** in the drop-down list in the column *Sub-Account*.

  + Select the option **--alle--** in the drop-down list in the column *Versandanbieter*.

  + Select the warehouse from which you want to take the stock in the drop-down list in the column *Lager*.

3. Click the button [ZUORDNUNGEN SPEICHERN] in the bottom right corner.   
  The new assignment in the stock source matrix is saved.

### Next steps

- [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products)
- [Manage the stock for POS products](#manage-the-stock-for-pos-products)

### See also

- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Check the inventory assignment](#check-the-inventory-assignment)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)


## Manage the warehouse logistics for POS products

Manage the warehouse logistics for POS product to ensure that products are active for warehousing.

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- A POS offer is created, see [Create an offer for POS](07_ManageOffers.md#create-an-offer-for-pos).

### Procedure

*Lager > Schnellbuchen > Tab SCHNELLBUCHEN > Tab Artikelliste*

![Artikelliste](/Assets/Screenshots/Lager/Schnellbuchen/Artikelliste.png "[Artikelliste]")

1.  Double click the article in the article list that you want to check. Alternatively, first right click the article and click then the entry **Öffnen** in the displayed context menu.    
  The article details are displayed on several tabs below the article list. The tab *Basisdaten* is preselected.

  ![Artikel Basisdaten](/Assets/Screenshots/Lager/Schnellbuchen/Basisdaten/Basisdaten.png "[Artikel Basisdaten]")

2. Click the drop-down list *Lageristik für diesen Artikel aktiv* on the right side of the tab *Basisdaten* and select the option **JA**.


3. Click the button [SPEICHERN] in the bottom right corner of the tab *Basisdaten* .   
  The message *Erfolgreich gespeichert* is displayed at the top. The active warehouse logistics for this article is saved.

  ![Erfolgreich gespeichert](/Assets/Screenshots/Lager/Schnellbuchen/ErfolgreichGespeichert.png "[Erfolgreich gespeichert]")

### Next steps

- [Manage the stock for POS products](#manage-the-stock-for-pos-products)

### See also

- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Check the inventory assignment](#check-the-inventory-assignment)
- [Check the stock source matrix](#check-the-stock-source-matrix)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)


## Manage the stock for POS products

You can adjust the stock quantity of your POS products, e. g. because of an inventory, a purchasing or an ordering.

### Prerequisites

- A POS store is created, see [Create a store](06_CreateStore.md).
- A POS offer is created, see [Create an offer for POS](07_ManageOffers.md#create-an-offer-for-pos).
- The warehouse logistics for the POS article is active, see [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products).
- A warehouse with a defined shelf is assigned to the POS product.

### Procedure

*Lager > Schnellbuchen > Tab SCHNELLBUCHEN > Tab Artikelliste*

![Artikelliste](/Assets/Screenshots/Lager/Schnellbuchen/Artikelliste.png "[Artikelliste]")

1.  Double click the article in the article list that you want to check. Alternatively, first right click the article and click then the entry **Öffnen** in the displayed context menu.    

  ![Kontextmenu](/Assets/Screenshots/Lager/Schnellbuchen/Kontextmenu.png "[Kontextmenu]")   

  The article details are displayed on several tabs below the article list. The tab *Basisdaten* is preselected.

  ![Artikel Basisdaten](/Assets/Screenshots/Lager/Schnellbuchen/Basisdaten/Basisdaten.png "[Artikel Basisdaten]")

2. Click the tab *Lager/Lieferanten* .   
  The tab *Lager/Lieferanten* is displayed. The sub tab *Lagerverwaltung* is preselected.

  ![Artikel Lager](/Assets/Screenshots/Lager/Schnellbuchen/LagerLieferanten/Lagerverwaltung/Lagerverwaltung.png "[Artikel Lager]")

  > [Info] Check if a warehouse is displayed in the section *Lagerorte*. You can only change the stock for the POS article, if a warehouse is assigned.

3. Click the button [BUCHUNG HINZUFÜGEN] at the bottom of the section *Bestände* .   
  A window to enter the booking is displayed.

  ![Buchung hinzufügen](/Assets/Screenshots/Lager/Schnellbuchen/LagerLieferanten/Lagerverwaltung/BuchungHinzufuegen.png "[Buchung hinzufügen]")

4. Configure the following settings:

  + Click the drop-down list *Lager* and select the appropriate warehouse from which you want to adjust the stock.

  + Click the drop-down list *Buchungsart* and select the appropriate reason for the booking. The following options are available:
      - **Reservierung**
      - **Verkauf**
      - **Bestellung**
      - **Einkauf**
      - **Inventurbuchung**
      - **Lagerumbuchung**
      - **Retoure**
      - **Problem**

      > [Info] For detailed information, see [User Interface Lager](/Lager/UserInterface/00_UserInterface.md).

  + Enter the number by which the stock should be changed in the field *Änderung*.

    > [Info] For a stock increase, enter a positive number. For a stock decrease, enter a negative number with a minus sign as a prefix. In the right column of the window, the old stock and a preview of the new stock are displayed.  

  + If desired, select the date on which the stock change will be booked in the field *Buchungsdatum*. By default, the current date is preselected.

  + If desired, enter a comment in the text field *Bemerkung*.

5. Click the button [SPEICHERN & NEU] in the bottom right corner of the window.   
    The window is closed. The new stock is displayed in the section *Bestände*.

### Next Steps

- [Open a pay desk](VenduoPOS/Operation/01_OpenPayDesk.md)

### See also

- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [Create a warehouse](to_be_completed)
- [Check the inventory assignment](#check-the-inventory-assignment)
- [Check the stock source matrix](#check-the-stock-source-matrix)
- [Manage the warehouse logistics for POS products](#manage-the-warehouse-logistics-for-pos-products)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
- [Assign users to the POS groups](04_AssignUsers.md)
- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
