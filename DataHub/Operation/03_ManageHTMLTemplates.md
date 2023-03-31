[!!User interface HTML templates](../UserInterface/02j_HTMLTemplates.md)

# Manage the HTML templates

HTML templates are mainly used for email messages such as confirmations or shipping messages. Further, they can be used to write detailed product descriptions that are uploaded to a shop or marketplace, for example to ebay.
HTML templates allow you to generate HTML content from data based on templates using the *Smarty template engine*.
Further, you are able to include data from all available source entities in HTML as well as all sub-entities if they are present in the JSON representation of the source entity using the HTML templates.

## Create an HTML template

Create an HTML template so that it is available for the ETL mapping.

#### Prerequisites

The *HTML Templates for ETL* plugin has been installed.

#### Procedure

*DataHub > Settings > Tab HTML TEMPLATES*

![HTML templates](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/HTMLTemplates.png "[HTML templates]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create HTML template* window is displayed.

    ![Create HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/CreateHTMLTemplate.png "[Create HTML template]")

2. Enter an expressive name for the HTML template in the *Name* field and, if desired, add a description to the HTML template in the *Description* field.

3. Enter a key for the HTML template in the *Key* field. The key is required for API access and must be system wide unique.

4. Click the textarea and enter the appropriate content for the HTML template. You can either include HTML text and/or Smarty templates:
    - [Include HTML text](#include-html-text)
    - [Include Smarty templates](#include-smarty-templates)

5. Click the [SAVE] button in the upper right corner.   
    The new HTML template has been saved. The *Create HTML template* view is closed.  



## Include HTML text

You can include HTML text in the HTML template.

#### Prerequisites

The *HTML Templates for ETL* plugin has been installed.

#### Procedure

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

> [Info] If you want to include HTML text into a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

1. Click the textarea and enter the desired HTML text.

    > [Info] For detailed information about the HTML structure and elements, see https://html.spec.whatwg.org/.

2. If desired, include Smarty templates, see [Include Smarty templates](#include-smarty-templates) or display a preview of the HTML template, see [Preview an HTML template](#preview-an-html-template).

3. Click the [SAVE] button in the upper right corner.   
    The HTML template has been saved. The *HTML template* view is closed.  



## Include Smarty templates

The *Smarty template engine* allows you to include Smarty templates into your HTML template.    
For detailed information about Smarty templates, see [Smarty](https://www.smarty.net/).    
Always use the delimiters *{}* as separator for the Smarty templates.  

#### Prerequisites

The *HTML Templates for ETL* plugin has been installed.

#### Procedure

> [Info] If you want to include Smarty templates into a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

1. Click the textarea and enter the desired Smarty template(s).

    > [Info] For detailed information about the Smarty template structure and elements, see [Smarty](https://www.smarty.net/).

2. If desired, include HTML text, see [Include HTML text](#include-html-text) or display a preview of the HTML template, see [Preview an HTML template](#preview-an-html-template).

3. Click the [SAVE] button in the upper right corner.   
    The HTML template has been saved. The *HTML template* view is closed.  



### Include attribute variables

You can include variables for attributes via Smarty templates into your HTML template.   
Always use the *$* sign to introduce an attribute variable.

#### Prerequisites

The *HTML Templates for ETL* plugin has been installed.

#### Procedure

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

> [Info] If you want to include an attribute variable into a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

1. Click the textarea and, if desired, edit or add the Smarty template(s) and/or HTML text for the template.

2. Include a variable in the textarea by entering the corresponding variable inside the delimiters *{}* and starting with the *$* sign. You can include one of the following variables:
    - **entity**   
        Use the entity variable to include a variable referring to an attribute of a certain entity within the system, for instance *{$entity.id}*.
    - **tenant**   
        Use the tenant variable to include a variable referring to an attribute of the platform tenant, for instance *{$tenant.shortName}*.  

    > [Info] The data fields of an entity you can refer to are described in the API documentation. To include a deeper level of the data field, enter a point *.* at a time, for instance *{$entity._pim_tax_zone.id}*.    

3. If desired, include the destination language and/or the destination channel to the attribute variable value by adding the following suffixes at the end of the variable name:
    - *destination language*   
        Add **__LanguageKey** to include the destination language to the variable. Replace **LanguageKey** by the corresponding language key and note, that all signs must be replaced by a **_**, for instance, add **__de_DE** for the language key *de-DE*. Pay attention to upper and lower case as the variables are case sensitive.
    - *destination channel*   
        Add **__ChannelKey** to include the destination channel to the variable. Replace **ChannelKey** by the corresponding channel key and note, that all signs must be replaced by a **_**, for instance, add **__actindo_basic** for the channel key *actindo_basic*. Pay attention to upper and lower case as the variables are case sensitive.

    > [Info] You can display all possible variables of a certain entity.    
    For detailed information, see [Display the possible variables](#display-the-possible-variables).

4. If desired, display a preview of the HTML template, see [Preview an HTML template](#preview-an-html-template).

5. Click the [SAVE] button in the upper right corner.   
    The HTML template has been saved. The *HTML template* view is closed.  



### Include a tree node variable

A tree node variable is a special type of variables that can be included via Smarty templates into your HTML template.   
The special rules to be followed to correctly include a tree node variable are described below.

#### Prerequisites

- The *HTML Templates for ETL* plugin has been installed.
- At least one tree node variable is available.

#### Procedure

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

> [Info] If you want to include a tree node variable into a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

1. Click the textarea and, if desired, edit or add the Smarty template(s) and/or HTML text for the template.

2. Include a tree node variable by doing the following:
    + Add **{datahub_translatable_value entity=$entity property="PropertyKey" languageKey=$languageKey entityTypeClassName="Actindo\Modules\Actindo\DataHub\Models\Tenant\TreeNode"}** to the textarea.
    + Define the tree node attribute you want to include a variable for by adding the corresponding attribute key as a suffix to the entity variable.
    + Replace **"PropertyKey"** between the quotes by the desired property key of the corresponding tree node variable.

[comment]: <> (stimmt das so? Muss der namespace immer der angegebene sein, oder variiert der auch?)

3. If desired, display a [preview of the HTML template](#preview-an-html-template).

4. Click the [SAVE] button in the upper right corner.   
    The HTML template has been saved. The *HTML template* view is closed.  



### Include language independent variables

It is possible to define a variable in such a way, that it is language independent.   
The special rules to be followed to correctly include a language independent variable via Smarty templates into your HTML template are described below.

#### Prerequisites

The *HTML Templates for ETL* plugin has been installed.

#### Procedure

> [Info] If you want to include a language independent variable into a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

1. Click the textarea and, if desired, edit or add the Smarty template(s) and/or HTML text for the template.

2. Include a language independent variable by doing the following:
    + Add **{datahub_attribute_value entity=$entity attributeKey="attributeKey" scopeKey="scopeKey" languageKey=$languageKey}** to the textarea.
    + Replace **"attributeKey"** between the quotes by the desired attribute key, for instance use **"pim_art_name"** for the PIM product name.
    + Replace **"scopeKey"** between the quotes by the desired channel key, for instance use **"actindo_basic** for the *Actindo Basic* channel.

[comment]: <> (stimmt das so? geht das auch mit dem Channel so?)

3. If desired, display a preview of the HTML template, see [Preview an HTML template](#preview-an-html-template).

4. Click the [SAVE] button in the upper right corner.   
    The HTML template has been saved. The *HTML template* view is closed.  



## Edit an HTML template

After you have created an HTML template, you can edit it.
You can edit the name, the description of the template or the template content.

#### Prerequisites

At least one HTML template has been created, see [Create an HTML template](#create-an-html-template).

#### Procedure
*DataHub > Settings > Tab HTML TEMPLATES*

![HTML templates](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/HTMLTemplates.png "[HTML templates]")

1. Click the HTML template you want to edit in the list of HTML templates.   
    The *Edit HTML template* window is displayed.

    ![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

2. Edit the desired data of the HTML template in the corresponding fields. The HTML template key is locked in the *Edit HTML template* view.

3. If desired, use the preview functionality in the *Preview* section to display the possible variables or a template preview for the selected entity. For detailed information, see [Preview an HTML template](#preview-an-html-template).

4. Click the [SAVE] button in the upper right corner.   
    The changes have been saved. The *Edit HTML template* view is closed.  



## Display the possible variables

It is possible to display all available variables of a certain entity so that you can select the variables you want to use in the HTML template.

#### Prerequisites

The *HTML Templates for ETL* plugin has been installed.

#### Procedure

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

> [Info] If you want to display the possible variables within a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

1. In the *Preview* section at the bottom of the *HTML template* view, select an entity type in the drop-down list *Entity type*. All available entities are displayed in the list.

    > [Info] The available entities depend on the plugins installed in your *Core1 Platform*.

2. Enter the corresponding entity identification number of the entity in the field *Entity ID*.

3. Click the [SHOW POSSIBLE VARIABLES] button.  
    A new browser window is displayed with all possible variables for the selected entity.

    ![Show possible variables](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/ShowPossibleVariables.png "[Show possible variables]")

4. Close the browser window and click the ![Back](../../Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the HTML templates list or proceed to edit the HTML template, see [Edit an HTML template](#edit-an-html-template).



## Preview an HTML template

It is possible to display a preview of the HTML template to check its functionality.

#### Prerequisites

At least one HTML template has been created, see [Create an HTML template](#create-an-html-template).

#### Procedure

*DataHub > Settings > Tab HTML TEMPLATES > Select HTML template*   

![Edit HTML template](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/EditHTMLTemplate.png "[Edit HTML template]")

> [Info] If you want to preview a new HTML template, follow the steps described in the [Create an HTML template](#create-an-html-template) procedure before proceeding to the steps below.

1. In the *Preview* section at the bottom of the *Edit HTML template* view, select an entity type in the drop-down list *Entity type*. All available entities are displayed in the list.

    > [Info] The available entities depend on the plugins installed in your *Core1 Platform*.

2. Enter the corresponding entity identification number of the entity for which you want to preview the template in the field *Entity ID*.

3. Click the [SAVE AND PREVIEW TEMPLATE] button.  
    The template has been saved and a new browser window is displayed with a preview of the template for the selected entity.

    ![Preview](../../Assets/Screenshots/DataHub/Settings/HTMLTemplates/Preview.png "[Preview]")

4. Close the browser window and click the ![Back](../../Assets/Icons/Back02.png "[Back]") (Back) button in the upper left corner to return to the HTML templates list or proceed to edit the HTML template, see [Edit an HTML template](#edit-an-html-template).
