# Upload of product failed

An offer upload failed. The offer has been moved to the list of export errors.  
It is possible to enter a product URL to an *Omni-Channel* offer. If the product URL is not unique, the driver will stop the upload of this offer to a *BigCommerce* product.  

#### Error Message

"Upload of the product partially failed. Product is uploaded to the shop, some entries might be missing. HTTP Status: 207, Title: The product was saved with some issues, Errors: The URL is a duplicate."

Follow the instructions below to check your offer URLs for duplicates.

#### Prerequisites

- No prerequisites to fulfill

#### Procedure

*Omni-Channel > Offers* 

![Offers](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleOffers.png "[Offers]")

1. Click the offer that caused the error.
   The *Edit offer "offer name"* window is displayed. The *Attributes* tab is displayed by default. 

   ![Edit offer](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleEditOffer.png "[Edit offer]")

2. Click the *Search engine optimization* entry in the attribute group tree on the left.
  The assigned attributes are displayed.

   ![Edit offer](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleSearchEngineOp.png "[Edit offer]")

3. Check the entry in the *Custom URL* field. Change it if it is not correct and repeat the steps above for this entry.

4. Click the [SAVE] button.  
    The *Edit offer* view is automatically closed when the changes have been saved. The *Offers* view is displayed again.

5. Click the checkbox at the offer you have changed.
   The editing toolbar is displayed.

6. Click the [RETRY UPLOAD] button.   
    *Omni-Channel* starts the export for the offer. If the offer was exported successfully, the error message is no longer displayed.
    <!---Hallo Janik, stimmt das so? ich wollte es im System nicht machen, um die Beispieldaten nicht zu löschen--> 

    ![Edit offer](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleSearchEngineFinished.png "[Edit offer]")



