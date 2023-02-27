[!!Manage the HTML templates](../Operation/03_ManageHTMLTemplates.md)

# HTML templates

*DataHub > Settings > Tab HTML TEMPLATES*

![HTML templates](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/HTMLTemplates.png "[HTML templates]")

**HTML templates list**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an HTML template.

[comment]: <> (Wonach kann ich suchen? Nur name und description?)

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of dimensions.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. You cannot select multiple checkboxes at once.

- ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit)   
    Click this button to edit the selected HTML template. This button is only displayed if the checkbox of an HTML template is selected. Alternatively, you can click directly a row in the list to edit an HTML template.   

The list displays all HTML templates. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *ID*   
    HTML template identification number. The ID number is automatically assigned by the system.

- *Name*   
    HTML template name.

- *Description*   
    Description to the HTML template.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to create an HTML template. The *Create HTML template* view is displayed.   


## Create HTML template

*DataHub > Settings > Tab HTML TEMPLATES > Button Add*

![Create HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/CreateHTMLTemplate.png "[Create HTML template]")

**Create HTML template**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Create HTML template* view and return to the HTML templates list. All changes are rejected.

- [CANCEL]   
    Click this button to cancel creating an HTML template. The *Create HTML template* view is closed.

- [SAVE]   
    Click this button to save the HTML template. The *Create HTML template* view is closed.

- *Name*   
    Enter an HTML template name.

- *Description*   
    Enter a description to the HTML template.

- *Key*   
    Enter an HTML template key. The key is required for API access and must be system wide unique.

- Textarea   
    Enter the content for the HTML template. Use the Smarty template engine to include variables and tags to the template, see [Smarty](https://www.smarty.net/) .    

**Preview**

- *Entity type*   
    Click the drop-down list and select the entity type which should be applied within the template. All entity types are displayed in the list.

    > [Info] Entity types are all classes interacting with the *DataHub* module.

- *Entity ID*   
    Enter the ID of the entity which should be applied within the template.

- [SHOW POSSIBLE VARIABLES]   
    Click this button to display all variables to the selected entity. The code containing all variables to the entity is displayed in a new window. The possible variables can only be displayed if both, an entity type and an entity ID have been selected.

- [SAVE AND PREVIEW TEMPLATE]   
    Click this button to save the HTML template and display a preview of the template with the selected entity. The preview is displayed in a new window. The preview can only be displayed if both, an entity type and an entity ID have been selected. In the *Create HTML template* view, the button is locked.

[comment]: <> (Ist das so gedacht, dass ich den Button nicht klicken kann?)



## Edit HTML template

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

**Edit HTML template**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Edit HTML template* view and return to the HTML templates list. All changes are rejected.

- [CANCEL]   
    Click this button to cancel editing an HTML template. The *Edit HTML template* view is closed.

- [SAVE]   
    Click this button to save all changes to the HTML template. The *Edit HTML template* view is closed.

- *Name*   
    Click the field to edit the HTML template name.

- *Description*   
    Click the field to edit the description to the HTML template.

- *Key*   
    HTML template key. In the *Edit HTML template* view, this field is locked.

- Textarea   
    Click the field to edit the content for the HTML template. Use the Smarty template engine to include variables and tags to the template, see [Smarty](https://www.smarty.net/) .   

**Preview**

- *Entity type*   
    Click the drop-down list and select the entity type which should be applied within the template. All entity types are displayed in the list.

    > [Info] Entity types are all classes interacting with the *DataHub* module.


- *Entity ID*   
    Enter the ID of the entity which should be applied within the template.

- [SHOW POSSIBLE VARIABLES]   
    Click this button to display all variables to the selected entity. The code containing all variables to the entity is displayed in a new window. The possible variables can only be displayed if both, an entity type and an entity ID have been selected.

- [SAVE AND PREVIEW TEMPLATE]   
    Click this button to save the HTML template and display a preview of the template with the selected entity. The preview is displayed in a new  window. The preview can only be displayed if both, an entity type and an entity ID have been selected.
