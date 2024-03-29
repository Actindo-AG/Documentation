[!! Check the failed offer upload](../../Channels/Operation/03_CheckOfferUpload.md#check-the-failed-offer-uploads)


# Export of offer failed

Initial situation: An offer export failed. The offer export has been moved to the list of export errors.  

#### Error Description

Error message: Upload of the product partially failed. Product is uploaded to the store, some entries might be missing. HTTP Status: 207, Title: The product was saved with some issues, Errors: The URL is a duplicate.

Cause: It is possible to enter a product URL to an *Omni-Channel* offer. If the product URL is not unique or invalid, the driver will stop the import of this offer to a *BigCommerce* product.  

Follow the instructions below to check your offer URLs for duplicates.

#### Prerequisites

You are both permitted to start offer exports in the *Omni-Channel* module and to change offer data there.

#### Procedure

*Omni-Channel > Offers > Tab OFFERS* 

![Offers](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleOffers.png "[Offers]")

1. Click the offer that caused the error.   
   The *Edit offer "offer name"* window is displayed. The *Attributes* tab is displayed by default. 

   ![Edit offer](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleEditOffer.png "[Edit offer]")

2. Click the *Search engine optimization* entry in the attribute group tree on the left.   
  The assigned attributes are displayed.

   ![Edit offer](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleSearchEngineOp.png "[Edit offer]")

3. Check the entry in the *Custom URL* field. Change it if it is not unique or invalid. A valid URL both must not contain any special characters such as (, - ; - % - & - § - $ - etc.) and must start with a slash. For example, /custom/url.   
    
4. If the URL is correct, check similar offers to see if the duplicate is recorded there.

5. Click the [SAVE] button.  
    The *Edit offer* view is automatically closed when the changes have been saved. The *Offers* view is displayed again.

6. Click the checkbox of the offer you have changed.   
   The editing toolbar is displayed.

7. Click the [RETRY UPLOAD] button.   
    *Omni-Channel* starts the export for the offer. 
      The *Export triggered* pop-up window is displayed. The error message is no longer displayed if you have successfully corrected the issue.  

     ![Edit offer](../../Assets/Screenshots/Channels/Settings/Connections/BigCommerce/TroubleSearchEngineFinished.png "[Edit offer]")


#### Was this chapter helpful?
If you need further assistance, please contact your MPS consultant.
   
   


