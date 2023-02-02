# CHANNELS->PIM

*Omni-Channel > Offer import > Tab CHANNELS->PIM*

![CHANNELS->PIM](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/ChannelsPIM.png "[CHANNELS->PIM]")

**Please select a connection to proceed to the import wizard**

- *Select connection*   
  Click the drop-down list to select the connection from which you want to import the Omni-Channel offers to PIM. All available

- [SELECT]   
  Click this button to confirm the selected connection in the *Select connection* drop-down list and proceed to the import wizard. The *Map attribute sets* wizard window is displayed.


## Map attribute sets

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Wizard window Map attribute sets*

![Map attribute sets](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/MapAttributeSets.png "[Map attribute sets]")

**Scope and language**

- *Language in PIM*   
  Click the drop-down list to select the language in PIM to which the value of a destination multi-language attribute will be written.

- *Channel in PIM*   
  Click the drop-down list to select the channel in PIM to which the value of a destination multi-channel attribute will be written.

**Source attribute set: "Source attribute set name"**

A single box is displayed for each attribute set in the selected connection. 

- *Assigned PIM attribute set*   
  Click the drop-down list to select the attribute set in PIM which will be assigned to the corresponding Omni-Channel attribute set. All PIM attribute sets that are mapped to the corresponding Omni-Channel attribute sets are displayed in the list. You can assign multiple PIM attribute sets to a single Omni-Channel attribute set.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)   
  Click this button to delete the corresponding mapping. You can only delete a mapping, if at least one more mapping is assigned to the attribute set.

- ![Add](../../Assets/Icons/Plus04.png "[Add]") (Add)   
  Click this button to add a further attribute set to the mapping. You can add an unlimited number of attribute sets to a mapping.


- [CANCEL]   
  Click this button to cancel the import wizard. The *Map attribute sets* wizard window is closed.

- [CONTINUE]   
  Click this button to proceed to the next step. The *Adjust mappings* wizard window is displayed.


## Adjust mappings

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Wizard window Adjust mappings*

![Adjust mappings](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/AdjustMappings.png "[Adjust mappings]")

**Select channels set and PIM product type**

- *Channels attribute set*   
  Click the drop-down list to select the Omni-Channel attribute set for mapping. All Omni-Channel attribute sets are displayed in the list.

- *PIM attribute set*   
  Click the drop-down list to select the PIM attribute set for mapping. All PIM attribute sets are displayed in the list. The *Mapping from "Omni-Channel attribute set name" to "PIM attribute set name"* section with the corresponding mapping is displayed.


**Mapping from "Omni-Channel attribute set name" to "PIM attribute set name"**

This view equals the attribute mapping in the *DataHub* module: *DataHub > Settings > Tab ETL > Select attribute set mapping*   

For a detailed description of this window and the corresponding functions, see [ETL](../../DataHub/UserInterface/02d_ETL.md#mapping).

- [BACK]   
  Click this button to go back to the previous step of the import wizard. The *Map attribute sets* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel the import wizard. The *Adjust mappings* wizard window is closed.

- [CONTINUE]   
  Click this button to proceed to the next step. The *Matching and behavior after import* wizard window is displayed.


## Matching and behavior after import

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Wizard window Matching and behavior after import*

![Matching and behavior after import](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/MatchingBehaviorAfterImport.png "[Matching and behavior after import]")

**Behaviour if a matched PIM product has been found**

- *Mode*   
  Click the *Mode* drop-down list to select the behaviour if a matched PIM product has been found. The following options are available:
    - **Link only**   
    - **Link and transfer data**       


**Behaviour on change of the PIM product**

- *Mode*   
  Click the *Mode* drop-down list to select the behaviour on change of the PIM product. The following options are available:   
  - **manual**   
    Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.
  - **semi-automatic**   
    Changes in a PIM product are automatically applied to the offer after confirmation. The initial offer is automatically applied without confirmation.   
  - **semi-automatic, changes must be confirmed by another user**   
    Changes in a PIM product are automatically applied to the offer after confirmation by another user. The initial offer is only applied after confirmation by another user.       
  - **automatic**    
    Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

- [BACK]   
  Click this button to go back to the previous step of the import wizard. The *Adjust mappings* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel the import wizard. The *Matching and behavior after import* wizard window is closed.

- [CONTINUE]   
  Click this button to proceed to the next step. The *Summary* wizard window is displayed. The *Wizard finalized* pop-up window is displayed.


## Summary

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Wizard window Summary*

![Summary](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/Summary.png "[Summary]")

The *Mapped AttributeSets* box displays the selected mapping. The *Matching and behavior after import* box displays the selected behavior after import.

- [BACK]   
  Click this button to go back to the previous step of the import wizard. The *Matching and behavior after import* wizard window is displayed.

- [CANCEL]   
  Click this button to cancel the import wizard. The *Summary* wizard window is closed.

- [FINALIZE]   
  Click this button to save the import settings. The *Summary* wizard window is closed. The *Offers* view is displayed.


## Offers   

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Finalize wizard*

![Offers](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/Offers.png "[Offers]")

**Offers**

- [CHANGE IMPORT SETTINGS]   
  Click this button to restart the import wizard. The *CHANNELS->PIM* tab is displayed, see [CHANNELS->PIM](#channels-pim).

- [IMPORT/MAP ALL OFFERS TO PIM PRODUCTS]    
  Click this button to import all offers in the list. The *Summary* window is displayed, see [Summary](#summary-1).

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an offer.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of offers.

- *VIEW*   
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *VIEW* drop-down list to display the context menu. The following menu entries are available:

        - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
            Click this entry to create a view. The *Create view* window is displayed, see [Create view](#create-view).

        - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
            Click this entry to rename the selected view. The *Rename view* window is displayed, see [Rename view](#rename-view). This menu entry is only displayed if a view has been selected.

        - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset  
            Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

        - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish  
            Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

        - ![Unpublish](../../Assets/Icons/Unpublish.png "[Unpublish]") unpublish  
            Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

        - ![Save](../../Assets/Icons/Save.png "[Save]") save  
            Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

            > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

        - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete  
            Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed if a view has been selected.


- Selected connection    
  The selected connection is displayed in the drop-down list. The drop-down list is locked.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all offers in the list are selected.

- [CREATE PIM PRODUCTS/MAP OFFERS TO EXISTING PIM PRODUCTS]            
  Click this button to import the selected offers in the list. The *Summary* window is displayed, see [Summary](#summary-1).


The list displays all offers to be imported. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *SKU*   
  Stock Keeping Unit. Identification number of the product to the offer. 
 
- *Variant status*  
  Variant type of the offer. The following options are available:  
  - **Master offer**   
    This offer refers to a master product.
  - **Variant offer**   
    This offer refers to a variant.
  - **Standalone Offer**  
    This offer refers to a single product.

- *Status*  
  Status of the offer. The following options are available:  
  - **Active**   
    The offer is active. It is displayed in the marketplace, where it can be sold.   
  - **Inactive**   
    The offer is inactive. It is not longer displayed in the marketplace and thus cannot be sold anymore.   
  - **Not available**   
    The offer is deleted from the marketplace.   
    The *Change offer status* confirmation window is displayed. If the variant status of the selected offer equals **Master offer**, an additional toggle is displayed within the confirmation window.   

  ![Change offer status](../../Assets/Screenshots/Channels/Offers/Offers/ChangeOfferStatus.png "[Change offer status]")

- *Pending status/Errors*  
  Indication of the pending status or an error for this offer. The selected status is displayed if you have changed the offer status via the editing toolbar. The following options are available:
  - **Active**	  
  - **Inactive**   	 
  - **Not available**  

[comment]: <> (when is an error displayed here? what is displayed? The Error code or message?)

- *Last upload*  
  Date and time of the last offer upload.

- *Connection*  
  Selected connection for the offer.

- *Attribute set*  
  Attribute set assigned to the offer.  

- *Created on*  
  Date and time of the creation.

- *Created by*  
  Name and username of the user who created the offer.

- *Modified on*  
  Date and time of the last modification.

- *Modified by*  
  Name and username of the user who modified the offer.

- *ID*  
  Offer identification number. The ID number is automatically assigned by the system after creation.

- Attribute    
  You can add a column for each attribute that is assigned to the offer. The column displays the attribute name, the row displays the corresponding attribute value of the offer.


**Processes**

[comment]: <> (was wird hier angezeigt?)


### Summary

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Finalize wizard > Tab Offers > Button IMPORT/MAP ALL OFFERS TO PIM PRODUCTS*   

*Omni-Channel > Offer import > Tab CHANNELS->PIM > Select connection > Button SELECT > Finalize wizard > Tab Offers > Select offer(s) > Button CREATE PIM PRODUCTS/MAP OFFERS TO EXISTING PIM PRODUCTS*

![Summary import](../../Assets/Screenshots/Channels/OfferImport/ChannelsPIM/SummaryImport.png "[Summary import]")

- *Affected offers*   
  Number of offers that are affected by this import.

- *Found PIM products*   
  Number of PIM products that match the offer.

[comment]: <> (stimmt das?)

- *Import name*   
  Enter a PIM product name for the offer to be imported.

[comment]: <> (stimmt das?)

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Start Import automatically without manual checking of assignment to PIM products*   
  Enable this toggle to automatically start the import without checking the assignments to the PIM product. Disable the toggle to ?. By default, this toggle is disabled.

[comment]: <> (was ist hier anders, wenn der toggle deaktiviert ist?)

- *Select a destination set for each source set*   
  
[comment]: <> (was kann ich hier machen?)

- [CANCEL]   
  Click this button to cancel the import to PIM. The *Summary* window is closed.

- [PREPARE IMPORT]    
  Click this button to cancel the import to PIM. The *Summary* window is closed.

[comment]: <> (was passiert hier sonst noch, wenn ich das abschließe?)
