[!!User Interface Dispatch notes](../UserInterface/01a_List.md)


# Check a shipment

Once a dispatch note has been received, the fulfiller sends back a notification at every stage of the fulfillment process. The shipment status is then updated accordingly in the *Actindo Core1 Platform*. All shipment-related details provided by the fulfiller, such as tracking number or tracking link, can be checked in the *Actindo Core1 Platform*.  


## Check the shipment status

The shipment status can be checked in the list of dispatch notes. Even though dispatch note status and shipment status are related, they are updated independently from each other.

#### Prerequisites

A dispatch note has been generated. 

#### Procedure

*Fulfillment > Dispatch notes > Tab LIST*

![Dispatch notes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Dispatch notes]")

Check the shipment status in the *Shipment status* column. The following options are available:
  - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross)   
    No shipment has been arranged yet.  

  - ![Circular arrows](../../Assets/Icons/CircularArrows.png "[Circular arrows]") (Circular arrows)   
    The shipment is in progress. For more information on the specific stage of the shipment process, see [Check the shipment details](#check-the-shipment-details). 

  - ![Double check](../../Assets/Icons/DoubleCheck.png "[Double check]") (Double check)    
  	The shipment has been delivered.

  - ![Error](../../Assets/Icons/Warning02.png "[Error]") (Error)    
    The shipment has given an error. A shipment is set to error only when the fulfiller reports an error due to a number of reasons. For detailed information, see [Handle an error status](../Troubleshooting/01_HandleErrorStatus.md). 

  - Empty  
    No information on the shipment status has been received from the fulfiller.


## Check the shipment details

The shipment details provided by the fulfiller can be accessed from the list of dispatch notes. 

#### Prerequisites

The shipment status is at least ![Circular arrows](../../Assets/Icons/CircularArrows.png "[Circular arrows]") (Circular arrows), that is, in progress, in the list of dispatch notes, see [Check the shipment status](#check-the-shipment-status).

#### Procedure

*Fulfillment > Dispatch notes > Tab LIST*

![Dispatch notes](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Dispatch notes]")

1. Click the dispatch note related to the shipment you want to check. Alternatively, you can click the checkbox of a dispatch note and the [VIEW] button in the editing toolbar.  
    The *Dispatch note "Dispatch note ID"* view is displayed. The *Attributes* tab is preselected by default.

    ![Dispatch note ID](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteAttributes.png "[Dispatch note ID]")

2. Select the *Shipments* tab.  
    All shipments included in the dispatch note are displayed.

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

    > [Info] The fields (attributes) displayed vary depending on the fulfiller's driver.  
    
6. Click a package to display the individual items contained.  
    The *Items* window is displayed listing all items contained in the selected package.  
  
   ![Package items](../../Assets/Screenshots/Fulfillment/DispatchNotes/Items.png "[Package items]")

7. The following item-related details, among others, are available: 
    - If desired, check an item SKU number in the *SKU* column.  
      The SKU can be useful to locate a product in the *PIM* module and check its inventory in the *Warehouse* module.
    - If desired, check the amount of an item contained in the package in the *Amount* column.
    - If available, you can also check an item serial number in the *Serial number* column.

    > [Info] The fields (attributes) displayed vary depending on the fulfiller's driver.  

8. Press *Esc* to close the *Item* window.  
  The *PACKAGES* tab is displayed again.

[comment]: <> (Kein CLOSE oder CANCEL button in Items Fenster. Bug gemeldet am 15.02.23. Evtl. nicht gefixed bis neuer UI. Alternativ außerhalb des Fensters klicken, dann verschwindet/schließt es auch.)

9. Click the [BACK] button on the upper right corner of the *PACKAGES* sub-tab to go back to the *PACKAGES* view.

    If needed, repeat the steps **6** and **7** to check other packages contained in the shipment. 

10. Click the [CLOSE] button on the right upper corner of the *Dispatch note "Dispatch note ID"* view.  
    The *Dispatch note ID* view is closed. The list of dispatch notes is displayed again.
