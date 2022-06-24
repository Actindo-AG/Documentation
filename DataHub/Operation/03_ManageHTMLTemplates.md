[!!DataHub](DataHub)

# Manage the HTML templates


## Create an HTML template

### Prerequisites

The *HTML Templates for ETL* plugin is installed.

### Procedure
*DataHub > Settings > Tab HTML TEMPLATES*

![HTML templates](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/HTMLTemplates.png "[HTML templates]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create HTML template* window is displayed.

  ![Create HTML template](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/CreateHTMLTemplate.png "[Create HTML template]")

2. Enter an expressive name for the HTML template in the *Name* field and, if desired, add a description to the HTML template in the *Description* field.

3. Enter a key for the HTML template in the *Key* field. The key is required for API access and must be system wide unique.

4. Click the textarea and enter the appropriate content for the HTML template. To include variables, use Smarty templates, see [Include Smarty Templates](#include-smarty-templates).

5. Click the [SAVE] button in the upper right corner.   
  The new attribute is saved. The *Create HTML template* view is closed.  

### Next steps

- [Edit an HTML template](#edit-an-html-template)
- [Include Smarty templates](#include-smarty-templates)
- [Include entity variables](#include-entity-variables)
- [Include a tree node variable](#include-a-tree-node-variable)
- [Include language independent variables](#include-language-independent-variables)
- [Preview an HTML template](#preview-an-html-template)
- [Manage the dashboards](04_ManageDashboards.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage the ETL mappings](01_ManageETLMappings.md)
- [Manage the ETL processes](02_ManageETLProcesses.md)



## Include Smarty templates


## Display the possible variables


### Include entity variables


### Include a tree node variable


### Include language independent variables






## Edit an HTML template


### Prerequisites

- The *HTML Templates for ETL* plugin is installed.
- At least one HTML template is created, see [Create an HTML template](#create-an-html-template).

### Procedure
*DataHub > Settings > Tab HTML TEMPLATES*

![HTML templates](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/HTMLTemplates.png "[HTML templates]")

1. Click the HTML template you want to edit in the list of HTML templates.   
  The *Edit HTML template* window is displayed.

  ![Edit HTML template](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

2. Edit the desired data of the HTML template in the corresponding. The HTML template key is locked in the *Edit HTML template* view.

3. If desired, use the preview functionality in the *Preview* section to display the possible variables or a template preview for the selected entity. For detailed information, see [Preview an HTML template](#preview-an-html-template).

4. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Edit HTML template* view is closed.  

### Next steps

- [Preview an HTML template](#preview-an-html-template)
- [Manage the dashboards](04_ManageDashboards.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage the ETL mappings](01_ManageETLMappings.md)
- [Manage the ETL processes](02_ManageETLProcesses.md)
- [Create an HTML template](#create-an-html-template)
- [Include Smarty templates](#include-smarty-templates)
- [Include entity variables](#include-entity-variables)
- [Include a tree node variable](#include-a-tree-node-variable)
- [Include language independent variables](#include-language-independent-variables)


## Preview an HTML template

### Prerequisites

- The *HTML Templates for ETL* plugin is installed.
- At least one HTML template is created, see [Create an HTML template](#create-an-html-template).

### Procedure
*DataHub > Settings > Tab HTML TEMPLATES*

![HTML templates](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/HTMLTemplates.png "[HTML templates]")

1. Click the HTML template you want to preview in the list of HTML templates.   
  The *Edit HTML template* window is displayed.

  ![Edit HTML template](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

2. In the *Preview* section at the bottom of the *Edit HTML template* view, select an entity type in the drop-down list *Entity type*. All available entities are displayed in the list.

  > [Info] The available entities depend on the modules installed in you Core1 Platform.

3. Enter the corresponding entity identification number of the entity for which you want to preview the template in the field *Entity ID*.

4. Click the [SAVE AND PREVIEW TEMPLATE] button.  
  The template is saved and a new browser window opens displaying a preview of the template for the selected entity.

  ![Preview](/Assets/Screenshots/DataHub/Settings/HTMLTemplates/Preview.png "[Preview]")

5. Close the browser window and click the ![Back](/Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the HTML templates list or proceed to [edit the HTML template](#edit-an-html-template).


### Next steps

- [Manage the dashboards](04_ManageDashboards.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage the ETL mappings](01_ManageETLMappings.md)
- [Manage the ETL processes](02_ManageETLProcesses.md)
- [Create an HTML template](#create-an-html-template)
- [Edit an HTML template](#edit-an-html-template)
- [Include Smarty templates](#include-smarty-templates)
- [Include entity variables](#include-entity-variables)
- [Include a tree node variable](#include-a-tree-node-variable)
- [Include language independent variables](#include-language-independent-variables)
