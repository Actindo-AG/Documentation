[!!User Interface Dispatch notes](../UserInterface/01a_List.md)


# Check a shipment

Once a dispatch note has been received, the fulfiller sends back a notification at every stage of the fulfillment process. The shipment status is then updated accordingly in the *Actindo Core1 Platform*. All shipment-related details provided by the fulfiller, such as tracking number or tracking link, can be checked in the *Actindo Core1 Platform*.  

## Check the shipment status

The shipment status can be checked in the list of dispatch notes. Even though dispatch note status and shipment status are related, they are updated independently from each other.

[comment]: <> (Stimmt das so?)

#### Prerequisites

A dispatch note has been generated. 

#### Procedure

*Fulfillment > Dispatch notes > Tab LIST*

![Dispatch notes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Dispatch notes]")

Check the shipment status in the *Shipment status* column. The following options are available:
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross)   
    No shipment has been arranged yet.  

  - ![Circular arrows](../../Assets/Icons/CircularArrows.png "[Circular arrows]") (Circular arrows)   
    The shipment is in progress.  

  - ![Double check](../../Assets/Icons/DoubleCheck.png "[Double check]") (Double check)    
  	The shipment has been delivered.

  - ![Error](../../Assets/Icons/Warning02.png "[Error]") (Error)    
    The shipment has given an error.

  - Empty  
    The shipment status is void.

[comment]: <> (Kann man sonst was tun? Evtl. alle Unterkapitel als Schritte in einem Procedure)


## Check the shipment details

The shipment details provided by the fulfiller can be accessed from the list of dispatch notes. 

#### Prerequisites

The shipment status is at least ![Circular arrows](../../Assets/Icons/CircularArrows.png "[Circular arrows]") (In progress), see [Check the shipment status](#check-the-shipment-status).

#### Procedure

*Fulfillment > Dispatch notes > Tab LIST*

![Dispatch notes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Dispatch notes]")

1. Click the dispatch note related to the shipment you want to check. Alternatively, you can click the checkbox of a dispatch note and the [VIEW] button in the editing toolbar.  
  The *Dispatch note ID* view is displayed. The *Attributes* tab is preselected by default.

    ![Dispatch note ID](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteAttributes.png "[Dispatch note ID]")

2. Select the *Shipments* tab.  
  All shipments belonging to the dispatch note are displayed.

    ![Shipments](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteShipments.png "[Shipments]")

3. Click the shipment to be checked.  
   The *Shipment ID* view is displayed. The *ATTRIBUTES* sub-tab is preselected by default.

    ![Shipment ID](../../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsAttributesAttributes.png "[Shipment ID]")

4. Select the *PACKAGES* sub-tab.  
  The package(s) included in the shipment are displayed. 

    ![Shipment packages](../../Assets/Screenshots/Fulfillment/DispatchNotes/ShipmentsPackages.png "[Shipment packages]")

5. The following shipment-related details, among others, are available:   
    - If desired, check the shipment tracking number in the *Tracking number* column.
    - If desired, check the URL for tracking in the *Tracking link* column.  
    
6. Click a package to display the individual items contained.  
The *Items* window is displayed listing all items contained in the selected package.  
  
   ![Package items](../../Assets/Screenshots/Fulfillment/DispatchNotes/Items.png "[Package items]")

7. The following item-related details, among others, are available: 
    - If desired, check an item SKU number in the *SKU* column. The SKU can be useful to locate a product in the *PIM* module and check its inventory in the *Warehouse* module.
    - If desired, check the amount of an item contained in the package in the *Amount* column.
    - If available, you can also check an item serial number in the *Serial number* column.

8. Press *Esc* to close the *Item* window.  
  The *PACKAGES* tab is displayed again.

    If needed, repeat the steps **6** to **7** to check other packages contained in the shipment. 

[comment]: <> (Kein CLOSE oder CANCEL button in Items Fenster. Bug?)

9. Click the [CLOSE] button on the right upper corner.  
  The *Dispatch note ID* view is closed. The list of dispatch notes is displayed again.
