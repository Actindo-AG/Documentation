# Manage definition settings

The definition of the EDIFACT export messages specifies the definition settings with template engine and the connection to be used, contain the message structure with predefined data as well as the data mapping and the mapping settings.
Each EDIFACT export message requires two definitions in the *DataHub Exporter* module:
- Definition of the message header   
    Figuratively speaking, the message header is the envelope, with which the message is sent. It contains general data such as receiver &frasl; sender information and dates.
- Definition of the line items  
    The line items contain the single positions of the message, for example the single items on an invoice.

You can create a definition setting. After you have defined the file settings, the data sources, and the mapping settings, you can activate the definitions setting.


## Create definition settings 

Define basic data for the export definition. You must define a definition setting for the header as well as for the line items of a message.


#### Prerequisites

- - At least one connection has been created, see [Create connection](../Integration/01_ManageConnections.md#create-connection).

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create definition* view is displayed.

    ![Create definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionCreate.png "[Create definition]")

2. Enter a label for the definition. It might be useful, to choose a name that contains the following:
        - The message type (for example, INVOIC)  
        - The direction (Export)   
        - The business partner name  
        - The information, if these are the header or the line items of the message.    
    For example, INVOIC Export items "customer name".

3. Click the *Template engine* drop-down list and select the **XmlExportTemplateEngine**.

4. Click the *Default connection* drop-down list and the connection to the related business partner. 

5. Define the *Access key* and click the ![Add](../../Assets/Icons/Plus01.png "[Add]") button. 

6. Click the [SAVE] button.   
    The *Submitting data* screen is displayed. After that, the *Exporter definitions* view is displayed again, the newly created definition is added. 

7. Repeat the procedure to create a definition for the line item. 


## Edit definition settings 

Edit basic data for the export definition. You can edit a definition setting for the header as well as for the line items of a message.


#### Prerequisites

- At least one connection has been created, see [Create connection](../Integration/01_ManageConnections.md#create-connection).
- At least one definition setting has been created, see [Create definition settings](#create-definition-settings).

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the definition whose settings you want to edit in the list of export definitions.   
    The *Edit definition "definition name"* view is displayed. The *SETTINGS* tab is displayed by default.

    ![Edit definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionEdit.png "[Edit definition]")

2. Edit the data you want to change.

3. Click the [SAVE] button.   
    The *Submitting data* screen is displayed. After that, the *Exporter definitions* view is displayed again. 





## Preview definition

After you have configured the entire definition, you can preview the message that will be sent to the business partner. You can use this function to let the business partner check, whether the message is correct.

#### Prerequisites

- At least one definition setting has been created, see [Create definition settings](#create-definition-settings).
- You have defined the file settings for this definition, see
- You have defined the data sources for this definition, see
- You have defined the mapping settings for this definition, see


#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the checkbox of the definition(s) you want to preview.
    The toolbar is displayed.

    ![Toolbar](../../Assets/Screenshots/EDI/Operation/ExportDefinitionToolbar.png "[Toolbar]")

2. Click the [PREVIEW] button.   
    A new browser window is opened in which the definition is output.
    ![Preview settings](../../Assets/Screenshots/EDI/Operation/ExportDefinitionToolbar.png "[Preview settings]")





## Activate definition

#### Prerequisites

- At least one definition setting has been created, see [Create definition settings](#create-definition-settings).
- You have defined the file settings for this definition, see
- You have defined the data sources for this definition, see
- You have defined the mapping settings for this definition, see
- You have sent the preview to the customer to check whether the message is correct, see [Preview definition](#preview-definition).

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")







## Delete definition

Delete a definition if you no longer need it. You can delete several definitions at once.

> [CAUTION] Note that you will lose the whole definition with all EDIFACT message settings, data sources, and mapping settings when deleting a definition.


#### Prerequisites

- At least one connection has been created, see [Create connection](../Integration/01_ManageConnections.md#create-connection).
- At least one definition setting has been created, see [Create definition settings](#create-definition-settings).

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the checkbox of the definition(s) you want to delete.
    The toolbar is displayed.

    ![Delete definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionToolbar.png "[Delete definition]")

2. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") button.   
    The definition is deleted without preceding security query.
  
    



