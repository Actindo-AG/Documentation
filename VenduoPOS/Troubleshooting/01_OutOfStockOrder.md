[!!Lager](Actindo/Lager)
[!!Omni-Channel](Actindo/Omni-Channel)

# Handle an out-of-stock order

## Error Message

Error booking bill: [stage: lager_book] Fehler beim Erzeugen der Lagerbuchungen: Der Bestand für Artikel *x* im Lager *x* ist nur 0.00, benötigt würden *x*.

Follow the instructions below if this error message is displayed.

## Procedure
*Lager > Schnellbuchen > Tab SCHNELLBUCHEN > Tab Artikelliste*

![Artikelliste](/Assets/Screenshots/Lager/Schnellbuchen/Artikelliste.png "[Artikelliste]")

1.  Double click the article in the article list that you want to check. Alternatively, first right click the article and click then the entry **Öffnen** in the displayed context menu.    
    The article details are displayed on several tabs below the article list. The tab *Basisdaten* is preselected.

  ![Artikel Basisdaten](/Assets/Screenshots/Lager/Schnellbuchen/Basisdaten/Basisdaten.png "[Artikel Basisdaten]")

2. Click the tab *Lager/Lieferanten* .   
  The tab *Lager/Lieferanten* is displayed. The sub tab *Lagerverwaltung* is preselected.

  ![Lagerverwaltung](/Assets/Screenshots/Lager/Schnellbuchen/LagerLieferanten/Lagerverwaltung/Lagerverwaltung.png "[Lagerverwaltung]")

  > [Info] Check if a warehouse is displayed in the section *Lagerorte*. You can only change the stock for the POS article, if a warehouse is assigned.

3. Click the button [BUCHUNG HINZUFÜGEN] at the bottom of the section *Bestände* .   
  A window to enter the booking is displayed.

  ![Buchung hinzufügen](/Assets/Screenshots/Lager/Schnellbuchen/Lagerlieferanten/Lagerverwaltung/BuchungHinzufuegen.png "[Buchung hinzufügen]")

4. Configure the following settings:

  + Click the drop-down list *Lager* and select the appropriate warehouse from which you want to adjust the stock.

  + Click the drop-down list *Buchungsart* and select the appropriate reason for the booking. The following options are available:
      - Reservierung
      - Verkauf
      - Bestellung
      - Einkauf
      - Inventurbuchung
      - Lagerumbuchung
      - Retoure
      - Problem

      > [Info] For detailed information, see [User Interface Lager](/Lager/UserInterface/00_UserInterface.md).

  + Enter the number by which the stock should be changed in the field *Änderung*.

    > [Info] For a stock increase, enter a positive number. For a stock decrease, enter a negative number with a minus sign as a prefix. In the right column of the window, the old stock and a preview of the new stock are displayed.  

  + If desired, select the date on which the stock change will be booked in the field *Buchungsdatum*. By default, the current date is preselected.

  + If desired, enter a comment in the field *Bemerkung*.

5. Click the button [SPEICHERN & NEU] in the bottom right corner of the window.   
    The window is closed. The new stock is displayed in the section *Bestände*.

6. Switch to the *Omni-Channel* module: *Omni-Channel > Orders and Returns > Tab ORDERS* .    
  The tab *ORDERS* is displayed.

  ![Orders](/Assets/Screenshots/OmniChannel/OrdersReturns/Orders/Orders.png "[Orders]")

7. Select the checkbox ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the order that was out-of-order and click the button [EXPORT TO OMS] in the editing toolbar at the top.     
  The order export is restarted. During the export, the status **Being exported** is displayed in the column *Status of Export to OMS*.

  > [Info] The export can take several minutes. Click the button ![Process](/Assets/Icons/Process.png "[Process]") (Process) in the upper right corner to display the process window with the current state of export.

8. Click the button ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) in the upper right corner to update the order list.   
  The order status in the column *Status of Export to OMS* changed to **Exported**. The order is correctly exported.

## See also

- [User Interface Lager](/Lager/UserInterface/00_UserInterface.md)
- [User Interface Omni-Channel](/OmniChannel/UserInterface/00_UserInterface.md)

## Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
