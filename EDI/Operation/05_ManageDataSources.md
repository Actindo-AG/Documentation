[!!Exports](../UserInterface/01_Exports.md)

# Manage data sources
Specify the data sources from which you want to retrieve the string attribute data that you have defined both in the header file settings and the line items file settings.   
For example, you have defined a string attribute to determine the invoice document number. By specifying a data source here, you determine the data source from which the invoice document number is to be retrieved.    
If required, you can specify here multiple data sources from which you can retrieve data from different sources, such as invoice data, customer data, and product data. In the next step, you can map a data source field containing the related data (source attribute) with the EDIFACT field (destination attribute). The EDIFACT fields are automatically provided after you have saved a string attribute allocation in the file settings.   
Tip: If you want to map the fields directly after you have specified an EDIFACT field in the file settings, it is recommended to create the data source before specifying the header &frasl; line item file segments.



## Assign data source

Assign the data source from which you want to retrieve the data with which you want to fill the EDIFACT message fields.

#### Prerequisites

At least one definition setting has been created, see [Create basic definition settings](./01_ManageDefinitions.md#create-basic-definition-settings).
> [Info] The *Data sources* tab is visible only if you have created and saved a basic definition setting. 

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the exporter definition for which you want to define the data source.   
    The *Edit definition "Definition name"* view is displayed. The *Settings* tab or the last opened tab is displayed by default.

2. Click the *Data sources* tab.   
    The *Data sources* tab is displayed. Because you have not yet created a data source, *No data source* is displayed in the list. 

    ![Data sources tab](../../Assets/Screenshots/EDI/Operation/DataSourcesList.png "[Data sources tab]")

3. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.     
    The *Select source* wizard window is displayed.

    ![Select source](../../Assets/Screenshots/EDI/Operation/DataSourcesSelectSource.png "[Select source]")

4. Select the data source in the *Entity type* drop-down list.   
    - If desired, use the *RetailSuite Business document* entity type when you are currently defining the data source for a header file.    
    You typically use this entity type for the header data when you want to transfer data with its origin from the *Actindo Core1 Platform*.
    - If desired, use the *Business document position* entity type when you are currently defining the data source for a line item definition.   
    You typically use this entity type for the line item data when you want to transfer line item data with its origin from the *Actindo Core1 Platform*.  
    - If desired, use any other data source that provides you with data needed for the transfer.   
    For example, you want to send an EDIFACT message with invoice data from SAP. In this case, select the related SAP data sources with which you can access the data needed for the header&frasl;line item files.   
    
    The *Attribute set* drop-down list is automatically filled with the data source defined in the *Entity type* field.
    
5. Click the [CONTINUE] button in the bottom right corner.   
    The *Map attributes* wizard window is displayed. If you have not yet defined string attributes in your file settings, the *There are no mappable fields in the destination* message is displayed. You can ignore this step for now.

    ![Map attributes](../../Assets/Screenshots/EDI/Operation/DataSourcesMapAttributes.png "[Map attributes]")

6. Click the [CONTINUE] button in the bottom right corner.  
    The *Optional: Filter items* wizard window is displayed. You can ignore it. It is only relevant for mass transports.

     ![Optional: Filter items](../../Assets/Screenshots/EDI/Operation/DataSourcesOptionalFilterItems.png "[Optional:Filter items]")

7. Click the [CONTINUE] button in the bottom right corner, until the [FINALIZED] button is displayed.   
    
9. Click the [FINALIZE] button in the bottom right corner to save the data source.   
   The *Exporter definition sources* view is displayed.

10. Click the [SAVE] button in the top right corner.    
   The *Submitting data* screen is displayed. After that, the *Exporter definitions* view is displayed again. 



## Map data source

Map the data sources by specifying the attributes that are to be mapped on EDIFACT message fields.

#### Prerequisites

- At least one data source has been assigned, see [Assign data source](#assign-data-source).
- In the file settings, you have added at least one string attribute. See an example under [Specify document number &frasl; string attribute](./02_ManageHeaderFileSett.md#specify-document-number-⁄-string-attribute).

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the exporter definition for which you want to define the data source.   
    The *Edit definition "Definition name"* view is displayed. The *Settings* tab is displayed by default.

2. Click the *Data sources* tab.   
    The *Data sources* tab is displayed.  

    ![Data sources tab](../../Assets/Screenshots/EDI/Operation/DataSourcesListWithEntries.png "[Data sources tab]")

3. Click the data source for which you want to map the attributes.   
    The *Map attributes* wizard window is displayed. In the *Destination attribute* column, a list of all EDI segment rows is displayed for which you have defined a string attribute or a condition.

    ![Data sources destination attributes](../../Assets/Screenshots/EDI/Operation/DataSourcesDestinationAttributes.png "[Data sources destination attributes]")

4. Map the source attributes and the destination attributes. For detailed information, see [Edit the ETL attribute mappings](../../DataHub/Operation/01_ManageETLMappings.md#edit-an-etl-attribute-set-mapping) in the *DataHub* documentation.

5. Click the [CONTINUE] button in the bottom right corner, until the [FINALIZED] button is displayed.   

8. Click the [FINALIZE] button in the bottom right corner to save the mappings.   
  You have saved the data source mappings. The *Exporter definitions* view is displayed. 




## Remove data source assignment

 Remove an exporter definition data source if you no longer need it. Note that you will lose all related attribute mappings by removing a data source.

 #### Prerequisites

At least one data source has been assigned, see [Assign data source](#assign-data-source).

#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the exporter definition from which you want to remove the assigned data source.    
  The *Edit definition "Definition name"* view is displayed. The *Settings* tab is displayed by default.

2. Click the *Data sources* tab.   
    The *Data sources* tab is displayed.  
    
    ![Data sources tab](../../Assets/Screenshots/EDI/Operation/DataSourcesListWithEntries.png "[Data sources tab]")

3. Select the checkbox of the data source you want to remove.    
   The editing toolbar is displayed.

4. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button.   
   The data source has been removed.

5. Click the [SAVE] button in the top right corner.    
    You have saved the definition settings. The *Exporter definitions* view is displayed. 
     




