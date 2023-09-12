# Manage data sources
Define the data sources from which you want to retrieve the string attribute data that you have defined both in the header file settings and the line items file settings. For example, you have defined a string attribute to determine the invoice document number. By specifying a data source here, you determine the data source from which this information is to be retrieved. If desired, you can create multiple data sources from which you may retrieve data from different sources.   
In the next step, you can map the field with the relevant information with the EDIFACT field. The EDIFACT fields are automatically provided after you have saved a string attribute allocation in the file settings.
If you want to map the fields directly after you have specified them in the file settings, it is recommended to create the data source before specifying the header &frasl; line items file segments.

## Create data source
Define the data source from which you want to retrieve the data with which you want to fill the EDIFACT message.

#### Prerequisites

At least one definition setting has been created, see [Create basic definition settings](#create-basic-definition-settings).
>[INFO] The *Data source* tab is visible only if you have created a basic definition setting. 

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the exporter definition for which you want to define the data source.   
    The *Edit definition "Definition name"* view is displayed. The *Settings* tab is displayed by default.

2. Click the *Data sources* tab.   
    The *Data sources* tab is displayed. Since you have not yet created a data source, *No data source* is displayed in the list. 

    ![Data sources tab](../../Assets/Screenshots/EDI/Operation/DataSourcesList.png "[Data sources tab]")

3. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.     
    The *Select source* popup window is displayed.

    ![Select source](../../Assets/Screenshots/EDI/Operation/DataSourcesSelectSource.png "[Select source]")

4. Select the data source in the *Entity type* drop-down list.   
    - If desired, use the *RetailSuite Business document* entity type if you currently define the data source for a header file.    
    You typically use this entity type for the header data, if you want to transfer data with its origin from the *Actindo Core1 Platform*.
    - If desired, use the *RetailSuite Business document postition* entity type if you currently define the data source for a line item file.   
    You typically use this entity type for the line item data, if you want to transfer data with its origin from the *Actindo Core1 Platform*.  
    - If desired, use any other data source that provides you with data needed for the transfer.   
    For example, you want to send an EDIFACT message with invoice data from SAP. In this case select the SAP data source with which you can access the data needed for the header file or the line item file.   
    
    The *Attribute set* drop-down list is automatically filled with the data source defined in the *Entity type* field.
    
5. Click the *Continue* button at the bottom right corner.   
    The Map attributes popup window is displayed. If you have not yet defined string attributes in your file settings, the *There are no mappable fields in the destination* text is displayed.



## Map attributes



## Edit data source