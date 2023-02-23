[!! Import an offer](../Operation/02_ImportOffers.md)

# PIM->CHANNELS

*Omni-Channel > Offer import > Tab PIM->CHANNELS*

![PIM->CHANNELS](../../Assets/Screenshots/Channels/OfferImport/PIMChannels/PIMChannels.png "[PIM->CHANNELS]")

**Channels offers to be created from PIM products**	

- [CLEAR ALL]  
    Click this button to clear all scheduled offer imports.

[comment]: <> (Bedeutung von CLEAR hier? Delete? Auf DE = ALLE LEEREN)

[comment]: <> (Scheduled offer imports? Channels offers to be created from PIM products)

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of scheduled offer imports.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.


The list displays all scheduled offer imports. Depending on the settings, the displayed columns may vary. All fields are read-only. If no offer imports are scheduled, the *No imports are currently scheduled* notice is displayed. 


- *SKU*  
   Stock Keeping Unit. Identification number for the offer.

- *Change tracking mode*  
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:  
    - **manual**   
        Changes in a PIM product must be triggered manually to be applied to the offer. The initial offer is automatically applied.
    - **semiautomatic**   
        Changes in a PIM product are automatically applied to the offer after confirmation. The initial offer is automatically applied without confirmation.   
    - **semiautomatic, changes must be confirmed by another user**   
        Changes in a PIM product are automatically applied to the offer after confirmation by another user. The initial offer is only applied after confirmation by another user.       
    - **automatic**    
        Changes in a PIM product are automatically applied to the offer. The initial offer is also automatically applied.

- *Created*  
    Date and time of the offer import creation.

- *Author*  
    Name and username of the user who changed the offer and triggered the import.

[comment]: <> (oder eher: user who triggered the import)

- *ID*  
    Offer identification number. The ID number is automatically assigned by the system after creation.

[comment]: <> (offer oder offer import identification number? Vgl. Offer ID / ID + comment in 03a_ScheduledUploads.md)

