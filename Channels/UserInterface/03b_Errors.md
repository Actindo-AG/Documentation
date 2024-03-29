[!!Check the failed offer uploads](../Operation/03_CheckOfferUpload.md#check-the-failed-offer-uploads)
[!!Retry a faulty offer upload](../Troubleshooting/01_RetryFaultyUpload.md)

# Errors

*Omni-Channel > Offer upload > Tab ERRORS*

![Errors](../../Assets/Screenshots/Channels/OfferUpload/Errors/ExportErrors.png "[Errors]")

**Export errors**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an offer export error.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of offer export errors.

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


- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

The list displays all offer export errors. Depending on the settings, the displayed columns may vary. All fields are read-only. If no errors exist currently, the *There are no export errors for this offer* notice is displayed.

- *SKU*   
    Stock Keeping Unit. Identification number for the offer.

- *Connection*   
    Assigned connection of the offer.

- *Fast/Default Queue*    
    Indication via which queue the offer was uploaded. The queue is automatically selected by the system depending on the changes to the offer. For instance, stock changes are prioritized and therefore uploaded via the fast queue. The following options are available:
    - **Default queue**   
        The offer was uploaded via the default queue.
    - **Fast queue**   
        The offer was prioritized and therefore uploaded via the fast queue.

- *Log Message Title*    
    Title of the error log message.

- *Log Message*   
    Complete log message to the error. Click the corresponding row of the error to display the *Detail of log message "Log message title"* view and check further details of the error.

- *Finally Failed*   
    Indication whether the offer upload finally failed or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The offer upload finally failed.
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The offer upload can be retried.

- *ID*  
    Error identification number. The ID number is automatically assigned by the system.

- *Created on*  
    Date and time when the error occurred.

- *Created by*  
    Name and username of the user who triggered the offer upload in which the error occurred. By default, the field is blank as the upload job is triggered by the system.

- *Modified on*  
    Date and time of the last modification.

- *Modified by*  
    Name and username of the user who modified the offer upload in which the error occurred. By default, the field is blank as the upload job is modified by the system.



## Detail of log message

*Omni-Channel > Offer upload > Tab ERRORS > Select export error*

![Detail of log message](../../Assets/Screenshots/Channels/OfferUpload/Errors/DetailLogMessage.png "[Detail of log message]")

For a detailed description of this view and the corresponding functions, see [LOG](./06a_Log.md#detail-of-log-message).