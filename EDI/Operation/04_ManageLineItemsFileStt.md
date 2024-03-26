[!!Exports](../UserInterface/01_Exports.md)
[!!Manage header file settings](02_ManageHeaderFileSett.md)

# Manage line item file settings

The following procedures show by using an example how to specify the line item section required by your business partner. As example, the D07A INVOIC message is used.

For detailed information on examples how to define constant text values, string attributes, dates, and free texts, see [Manage header file settings](./02_ManageHeaderFileSett.md#).


## Prepare data mapping for the line items

Prepare the data mapping for the line items so that the relevant data for the mapping is available to retrieve the line items.

#### Prerequisites

- You have defined both the definitions for the header and the line items, see [Create basic definition settings](./01_ManageDefinitions.md#create-basic-definition-settings).
- You have prepared the line item export, see [Prepare line item export](./02_ManageHeaderFileSett.md#prepare-line-item-export).


#### Procedure

*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the header export definition for which you want to prepare the data mapping for the line items. 
    The *Edit definition "Definition name"* view is displayed. The *Settings* tab is displayed by default.

2. Click the *Data sources* tab.   
    The *Data sources* tab is displayed.  

    ![Data sources tab](../../Assets/Screenshots/EDI/Operation/DataSourcesListWithEntries.png "[Data sources tab]")

3. Click the data source for which you want to map the segment for the line items.   
    - The *Map attributes* wizard window is displayed.     
    - In the *Destination attribute* column, a list of all EDI segment rows for which you have defined a string attribute is displayed.    
    - The *EDI export SG26* entry is available.

        ![SG26 Mapping](../../Assets/Screenshots/EDI/Operation/ExportDefMapSG26Segment.png "[SG26 Mapping]")

6. Click the *EDI Export SG26* destination attribute and define the mapping.    
   The *Settings* section is displayed on the right.

    ![SG26 Mapping settings](../../Assets/Screenshots/EDI/Operation/ExportDefSG26MappingKonfig.png "[SG26 mapping settings]")
   
     -  Click the *Extension* drop-down list and select the **XML SubExport extension**.   
        The left part of the *Settings* section displays both the *Source attribute* drop-down list and the *Configuration* section.

     - Click the *Override change tracking mode* drop-down list and select the desired one.

     -  On the left part of the *Settings* section, click the *Source attribute* drop-down list and select **Positions** or another attribute that represents a line item. 

     -  In the *Configuration* section, click the *Subexport definition* drop-down list and select the required line item definition, for example **EDIFACT INVOIC export items Customer 4.**
     
        ![SG26 Mapping settings](../../Assets/Screenshots/EDI/Operation/ExportDefSG26MappingDone.png "[SG26 mapping settings]")  

7. Click the [SAVE] button in the top right corner of the wizard.   

8. Finalize the *Map attributes* wizard by clicking the [CONTINUE] button until you can click the [FINALIZE] button.
  
9. Click the [SAVE] button in the top right corner to save the header definition.   
   The *Exporter definitions* view is displayed.


## Get line item segments

Get the line item segments of an EDIFACT message in order to be able to fill them. You can add constant values as well as strings and conditions that are to be determined via attribute mapping later. 
By getting the line item segments of an EDIFACT message, you need to specify the EDIFACT group segment that contains the LIN segment used to transfer of the message line items. For the D07A INVOIC, it is the SG26 group.


#### Prerequisites

- You have the message specification of your business partner at hand.
- You are currently creating the line item definition and have entered the necessary data in the *Settings* tab, see [Create basic definition settings](./01_ManageDefinitions.md#create-basic-definition-settings).

    > [Info] You cannot save the definition until you have entered the settings in the file settings tab.

- You have prepared the line item export in the header file definition, see [Prepare line item export](./02_ManageHeaderFileSett.md#prepare-line-item-export).
- You have prepared the data mapping for the line items, [Prepare data mapping for the line items](#prepare-data-mapping-for-the-line-items).

#### Procedure

*DataHub Exporter > Tab EXPORTS > Settings tab*

![Edit definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionEditLineItems.png "[Edit definition]")

1. Click the *File settings* tab.   
    The *File settings* tab is displayed.

     ![File settings tab](../../Assets/Screenshots/EDI/Operation/ExportDefinitionEmptFileSettings.png "[File settings tab]")

2. Click the *Release* drop-down list and select the required EDIFACT release. In our example, it is **D07a**.

3. Click the *Message type* drop-down list and select the required EDIFACT message type. In our example, it is **INVOIC**. You can use the search function on top of the drop-down list.

4. Enter the *Reference node path*. Use the following syntax:    
    /M_[Message type, for example INVOIC]\_[EDIFACT version number (last three digits)]/ G\_[Message type, for example INVOIC]\_[EDIFACT version number (last three digits)]\_SG[Group number].     
    For example: /M_INVOIC_07A/G_INVOIC_07A_SG26   
    Alternatively, you can copy the two parts from the header file message structure.  

    

    ![File settings tab](../../Assets/Screenshots/EDI/Operation/ExportDefMessagData.png)

 
5. Click the ![Get](../../Assets/Icons/Download.png "[Get]") [GET] button.   
    The message structure of the SG26 group is displayed. The segment is highlighted in red because it is still empty.    
    It starts with the SG26 element. 

    ![Message](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructureLineItems.png "[Message]")


6. If desired, expand the message structure by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button.   
    The message structure with its single segments is displayed. It starts with the *S_LIN* segment. The ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button has changed to an ![Expanded](../../Assets/Icons/NodeExpanded.png "[Expanded]") (Expanded) button.

    ![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructureSG26.png "[Message structure]")

7. Click the [SAVE] button in the top right corner.   
     - The *Exporter definitions* view is displayed.   
     - If you now open the definition again for editing, both the *Data Sources* tab and the *Mapping settings* tab are additionally displayed. 
     - In the header definition file settings, you are no longer able to expand the *G_INVOIC_07A_SG26* group.

8. If desired, create the data source and define the mapping setting. For detailed information, see [Prepare definition of file settings](./01_ManageDefinitions.md#prepare-definition-of-file-settings).



## Specify line item number

Start specifying the line item segments by filling out the single elements of the *S_LIN* (line item) segment. This procedure shows how to edit the line item number on the invoice, so that each invoice line item gets a unique and ascending number.

#### Prerequisites

You have expanded the message structure of the line item definition, see [Get line item segments](#get-line-item-segments).

#### Procedure

*DataHub Exporter > Tab EXPORTS > Select message definition > Tab File settings > Expand message structure*

 ![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructureSG26.png "[Message structure]")

1. Expand the *S_LIN* segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_LIN* segment.   
    The *S_LIN* segment in turn consists of subordinate segments and fields.

    ![S_LIN segment](../../Assets/Screenshots/EDI/Operation/ExportDefLIN.png "[S_LIN segment]")

2. Check the specification for the fields that are required to be filled. In most cases, you must fill the line item identifier in the *D_1082* row (to identify a line item). This is an ascending numeric value that must be unique for each invoice. For this reason, it is to be determined dynamically by a data source mapping. 

3. Click the ![Add string attribute](../../Assets/Icons/Plus03.png "[Add string attribute]") (Add string attribute) button to the right of the *D_1082* row.   
     - To the right of the *D_1082* row only the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is available now, with which you can remove the data, if required. The field name and description are no longer displayed in italics.  
    - The *S_LIN* segment is now highlighted in red. This indicates that the segment contains data, but not all required data for the EDIFACT message structure is filled.   
    - The string attribute has been marked for a later data mapping.

    ![D_1082 row](../../Assets/Screenshots/EDI/Operation/ExportDefLIN1082.png "[D_1082 row]")

4. Click the [SAVE] button in the top right corner to save the message structure.   
    The *Exporter definitions* list is displayed. The defined string attribute is now added to the attribute mapping function in the *Data sources* tab.

5. Open the line item definition again and click the *Data sources* tab.   
    The *EDI Export LIN/1082* destination attribute has been added to the attributes to be mapped.

    ![Map attributes](../../Assets/Screenshots/EDI/Operation/ExportDefLIN1082Mapping.png "[Map Attributes]")

 
6. Click the *EDI Export LIN/1082* destination attribute.    
   In the *Settings* section on the right, the configuration options are displayed.

     - Click the *Extension* drop-down list and select the **Mathematical expression** (also called arithmetic extension, depending on your version) entry.  
         The section for selecting a source attribute is displayed.

     - Click the *Override change tracking* mode and select the desired mode.

     - On the left side of the *Settings* section, click the drop-down list to select a source attribute that specifies the line item number, for example **positionNumber**.

     - In the *Configuration* section, enter **x1+1** in the *Equitation 1* field.

      ![Specify line item number](../../Assets/Screenshots/EDI/Operation/ExportDefLIN1082MappingDone.png "[Specify line item number]")

7. Click the [SAVE] button in the top right corner of the wizard and finalize the *Map attributes* wizard by clicking the [CONTINUE] button until you can click the [FINALIZE] button.

8. Click the [SAVE] button in the top right corner to save the line item definition.   
   The *Exporter definition sources* view is displayed.

9. Continue with specifying the line items file settings. For detailed information on examples how to define constant text values, string attributes, dates, conditions, and free texts, see [Manage header file settings](./02_ManageHeaderFileSett.md#).




