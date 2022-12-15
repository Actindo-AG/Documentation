[!!Tag](../Integration/tobecompleted.md)
[!!Tag](../Integration/tobecompleted.md)

# Offers

*Omni-Channel > Offers > Tab OFFERS*

[comment]: <> (Datei 02a_List.md aus PIM/UserInterface als Referenz verwendet. Ggf. Änderungen hier auch übernehmen)

![Offers](../../Assets/Screenshots/Channels/Offers/Offers/Offers.png "[Offers]")

**Offers**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for an offer.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of offers.

- *View*   
  Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu and create or edit a view.    
  For detailed information, see [Create a view](#create-a-view).

  - View context menu   
    Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![Create](../../Assets/Icons/Plus06.png "[Create]") create   
      Click this entry to create a view. The *Create view* window is displayed.

    - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename    
      Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed if a view has been selected.

    - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset    
      Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

    - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish    
      Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

    - ![Private view](../../Assets/Icons/Unpublish.png "[Unpublish]") private view    
      Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

    [comment]: <> (Private view oder unpublish? Cf. default sentences)

    - ![Save](../../Assets/Icons/Save.png "[Save]") save    
      Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

      > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete    
      Click this entry to delete the selected view. A confirmation window is displayed to confirm the deletion. This menu entry is only displayed if a view has been selected.

- *All Connections*    
  Click the drop-down list to select a connection. All supported connections are displayed in the list.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all offers in the list are selected.

- *Change status to*  
    Click this drop-down list to change the offer status. This drop-down list is displayed when the checkbox of one or more offers is selected. The following options are available:   
    - **Active**  
        Select this option to change the offer status to active.
    - **Inactive**  
        Select this option to change the offer status to inactive. 	
    - **Not available**  
        Select this option to change the offer status to not available.  	

- ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit)           
  Click this button to edit an offer. This button is only displayed when the checkbox of one offer is selected.  Alternatively, you can click the offer to be edited.  
  The *Edit offer "SKU"* view is displayed, see [Edit offer](#edit-offer).


The list displays all offers available. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *SKU*   
  Stock Keeping Unit. Identification number for the offer. 
 
- *Variant status*  
  Indication whether the the offer is based on a master product or a variant of it. The following options are available:  
    - **Master offer**  
    - **Variant offer**  

[comment]: <> (Bessere Erklärung?)

- *Status*  
  Offer status. The following options are available:  
    - **Active**  
      The offer is uploaded and available to be sold in the marketplace.
    - **Inactive**  
      The offer is uploaded but not available to be sold in the marketplace.
    - **Not available**  
      The offer is offline, that is, neither uploaded nor available to be sold in the marketplace.

- *Pending status/Errors*  
    - **Active**	  
    - **Inactive**   	 
    - **Not available**  

[comment]: <> (Info fehlt)

- *Last upload*  
  Date and time of last offer upload.

- *Connection*  
  Connection via which the upload has been performed.

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
  Offer identification number. The ID number is automatically assigned by the system.


- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)           
  Click this button to add an offer. The [Manual offer ![Document](../../Assets/Icons/Document.png "[Document]") ] button and the [Create from PIM product ![Documents](../../Assets/Icons/Documents.png "[Documents]") ] button are displayed. For detailed information, see [Add offer](#add-offer).


## Add offer

*Omni-Channel > Offers > Tab OFFERS > Button Add*

![Add offer](../../Assets/Screenshots/Channels/Offers/Offers/AddOffer.png "[Add offer]")

- [Manual offer ![Documents](../../Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to create a manual offer. The *Create offer* window is displayed, see [Create manual offer](#create-manual-offer).

- [Create from PIM product ![Documents](../../Assets/Icons/Documents.png "[Documents]") ]    
  Click this button to create an offer from a PIM product. The *Create from PIM product* wizard window is displayed, see [Create from PIM product](#create-from-PIM-product).

- ![Cancel](../../Assets/Icons/Cross01.png "[Cancel]") (Cancel)   
  Click this button to hide the buttons and return to the *OFFERS* tab.


### Create manual offer

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Manual offer*

![Create manual offer](../../Assets/Screenshots/Channels/Offers/Offers/CreateManualOffer.png "[Create manual offer]")


- *SKU*  
    Enter an individual SKU for the offer. The SKU (Stock Keeping Unit) is an identification number and should be assigned only once. 

- *Selection connection*  
    Click the drop-down list to select a connection for the offer. All available connections are displayed in the list. Once a connection has been selected, the *Select attribute set* drop-down list is unlocked.

- *Select attribute set*  
    Click the drop-down list to select an attribute set for the offer. All active attribute sets are displayed in the drop-down list. The drop-down list is locked if no connection is selected.

- [CANCEL]   
    Click this button to cancel adding an offer. The *Create manual offer* window is closed.

- [SAVE]  
    Click this button to save the offer. The *Create manual offer* window is closed and the *Create offer* view is displayed, see [Create offer](#create-offer).

[comment]: <> (Hier wird es verwirrend mit der Benennung von Fenster Create offer und von darauffolgendem View Create offer. Evtl. Fenster als Create manual offer oder nur Manual offer umbenennen?)


#### Create offer

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Manual offer > Button SAVE*

![Create offer](../../Assets/Screenshots/Channels/Offers/Offers/CreateOffer.png "[Create offer]")

 ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create offer* view and return to the offer list. All changes are rejected.

- [CANCEL]   
  Click this button to cancel creating an offer. The *Create offer* view is closed.

- [SAVE]   
  Click this button to save the new product. The *Create offer* view is closed. The new offer is added to the offer list.

[comment]: <> (Keine Image box hier?)

- *SKU*   
  Stock Keeping Unit. Identification number for the product. The SKU (Stock Keeping Unit) is an identification number for the product. Therefore, it should be uniquely assigned to a single product.   
  Click the button ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit) to the right of the SKU to edit it.

- ![Edit](../../Assets/Icons/Edit02.png "[Edit]") (Edit)   
  Click this button to edit the SKU.

- ![Apply](../../Assets/Icons/Check.png "[Apply]") (Apply)   
  Click this button to apply the changes to the SKU. This button is only displayed if you are editing the SKU.

- *Language*   
  Click the drop-down list to select a language for the offer. All active languages are displayed in the drop-down list. The default language is preselected.

- [Completeness: Not available]     
  Completeness of the offer. In the *Create offer* view, the completeness cannot be indicated. The completeness is indicated once the offer have been saved.

#### Create offer &ndash; Attributes

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Manual offer > Button SAVE > Tab Attributes*

![Attributes](../../Assets/Screenshots/Channels/Offers/Offers/CreateOffer.png "[Attributes]")

In the left margin column, all available attribute groups are displayed. Click an attribute group to display the attributes that are assigned to this group on the right side of the *Attributes* tab. If the offer contains attributes that are unassigned, the *Unassigned group* attribute group is automatically displayed in the left margin column.

The right side of the *Attributes* tab displays all attributes that are assigned to the selected group in the left margin column.

- ![Fade in/out](../../Assets/Icons/FadeInOut01.png "[Fade in/out]") (Fade in/out)    
  Click this button to hide or display the left margin column with the attribute groups. When the left margin is displayed and you click this button, the column is hidden. When the column is hidden and you click this button, the column is displayed again.


#### Create offer &ndash; Variants

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Manual offer > Button SAVE > Tab Variants*

[comment]: <> (s. PIM)

#### Create offer &ndash; Dependencies

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Manual offer > Button SAVE > Tab Dependencies*

[comment]: <> (s. PIM)


### Create from PIM product

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Create from PIM product*

#### Select marketplace

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Create from PIM product > Wizard window Select marketplace*

![Select marketplace](../../Assets/Screenshots/Channels/Offers/Offers/PIMOffer01.png "[Select marketplace]")


**Select marketplace**

- *Which products do you wish to create offers from?*	
    - ![Radionbutton](../../Assets/Icons/Radiobutton.png "[Radiobutton]") **All products**
    - ![Radionbutton](../../Assets/Icons/Radiobutton.png "[Radiobutton]") **Select products**

- *Which connection do you want to create offers on?*	

- *Connection*	

- *Do you wish to only create offers for products that do not yet have an offer on this connection?*

Do not create duplicates	

STEP 1: Select marketplace

- [CANCEL] 	
- [CONTINUE]


#### Select products

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Create from PIM product > Wizard window Select products*

![Select products](../../Assets/Screenshots/Channels/Offers/Offers/PIMOffer02.png "[Select products]")


Select products  
View  
Language  
Channel  
Catalog

Products	
SELECT ALL X PRODUCTS	
ADD TO SELECTION	
Add to selection x products
SKU	
Images	
No data	

- [BACK]	

STEP 2: Select products

- [CANCEL] 	
- [CONTINUE]


#### Review and finalize

*Omni-Channel > Offers > Tab OFFERS > Button Add > Button Create from PIM product > Wizard window Review and finalize*

![Review and finalize](../../Assets/Screenshots/Channels/Offers/Offers/PIMOffer03.png "[Review and finalize]")


After confirming the following details this dialog will close and the creation of the channel offers will take place in a background job.	

- **Matched**	
- **Not matched (unclear)**	
- **Not matched (not possible)**	

Already have offers on this connection and would create duplicates.

- *Change tracking mode*
    - **manual**	
    - **semi-automatic**	
    - **semi-automatic, changes must be confirmed by another user**	
    - **automatic**	

[comment]: <> (aus PIM genommen, dementsprechend anpassen bzw. aktualisieren)

- *Change tracking mode*   
  Click the drop-down list to change the change tracking mode (ETL mode) of the offer. The currently selected change tracking mode is displayed in the *Change tracking mode* column. This drop-down list is only displayed if the checkbox of one offer is selected. The following options are available:    
  - **Manual**   
    Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.
  - **Semi-automatic**   
    Changes in a PIM product are automatically applied to the offer after confirmation. The initial offer is automatically applied without confirmation.   
  - **Semi-automatic, changes must be confirmed by another user**   
    Changes in a PIM product are automatically applied to the offer after confirmation by another user. The initial offer is only applied after confirmation by another user.       
  - **Automatic**   
    Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

- *Initial offer status*	
    - **Active**	
    - **Inactive**	
    - **Offline**	

Map attribute sets	
Source attribute set	
Destination attribute set	

- [BACK]	

STEP 3: Review and finalize	

- [CANCEL]	
- [CREATE OFFERS]  



## Edit offer

*Omni-Channel > Offers > Tab OFFERS > Select offer*

![Edit offer](../../Assets/Screenshots/Channels/Offers/Offers/EditOffer.png "[Edit offer]")

### Edit offer &ndash; Attributes

**Edit offer "SKU"**	

- [CANCEL]  	
- [SAVE]  

- SKU	
- Language	
- COMPLETE:	
Completeness	
- Channels (All)
- Not multi-channel
- Languages (All)	
- Not multi-language
x total missing required attributes	
show empty required attributes only	Show empty required attributes only
- *Status:*	
    - **Active**	
    - **Inactive**	
    - **Offline**
- *Pending status:*
    - **Active**	
    - **Inactive**	
    - **Offline**

- *Pending status/Errors*   
  Indication of the pending status or an error for this offer. The selected status is displayed if you have changed the offer status via the editing toolbar. The following options are available:
  - **Active**   
  - **Inactive**   
  - **Offline**

Attributes	

### Edit offer &ndash; Variants


Variants	
Variant set	
Status	
SKU	
ID	
Add single variant	
Add single variant	
Additional fields	
sku	SKU
Use formula	
Defined values	

- [CANCEL]	
- [SAVE]  

Add multiple variants	
Select values    
ADD ALL VALUES	   
ADD VALUE	  
Value	  

STEP 1: Select values  

- [CANCEL]
- [NEXT]

Summary	
Variants that will be created (ignoring duplicated)	

GO BACK	

STAGE 2: Summary	STEP 2: Summary

CANCEL
FINISH	


### Edit offer &ndash; Dependencies

Dependencies	
Dependent entity id	
Dependent entity type	
Change tracking	Change tracking mode
Dependent entity friendly identifier	
No other entities depend on this entity	


## Create view

*Omni-Channel > Offers > Tab OFFERS > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Channels/CreateView.png "[Create view]")

- *Name*   
  Enter a name for the view.

- [CANCEL]   
  Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]   
  Click this button to save the new view and display it in the *VIEW* drop-down list. The *Create view* window is closed.

This window can also be accessed from the following tabs in the user interface:

- [Orders](05a_Orders.md#create-view)
- [Log](06a_Log.md#create-view)
- [Connections](08a_Connections.md#create-view)


## Rename view

*Omni-Channel > Offers > Tab OFFERS > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Channels/RenameView.png "[Rename view]")


- *Name*   
  Click this field to edit the view name.

- [CANCEL]   
  Click this button to cancel renaming the view. The *Rename view* window is closed.

- [SAVE]   
  Click this button to save the changes and display it in the *VIEW* drop-down list. The *Rename view* window is closed.

This window can also be accessed from the following tabs in the user interface:

- [Orders](05a_Orders.md#rename-view)
- [Log](06a_Log.md#rename-view)
- [Connections](08a_Connections.md#rename-view)
