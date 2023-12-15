# Manage line item file settings

The following procedures show by using an example how to specify the line item section required by your business partner. As example the D07A INVOIC message is used.

For detailed information on examples how to define constant text values, string attributes, dates, and free texts, see [Specify header file settings](./02_ManageHeaderFileSett.md).



## Get line item segments

Get the line item segments of an EDIFACT message in order to be able to fill them. You can add constant values as well as strings that are to be determined via attribute mapping later. 


#### Prerequisites

- You have the message specification of your business partner at hand.
- You have created the basic definition settings for the line items for this type of message and business partner, see [Create basic definition settings](./01_ManageDefinitions.md#create-basic-definition-settings).
- You have prepared the line item export in the header file definition, see [Prepare line item export](./02_ManageHeaderFileSett.md#prepare-line-item-export).

#### Procedure

*DataHub Exporter > EXPORTS tab*

![Exporter definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Exporter definitions]")

1. Click the definition for which you want to specify the line item settings.   
    The *Edit definition "definition name"* view is displayed. The *Settings* tab is displayed by default.

    ![Edit definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionEditLineItems.png "[Edit definition]")

2. Click the *File settings* tab.   
    The *File settings* tab is displayed.

     ![File settings tab](../../Assets/Screenshots/EDI/Operation/ExportDefEmptyfileSettings.png "[File settings tab]")

3. Click the *Release* dropdown list and select the required EDIFACT release. In our example, it is **D07a**.

4. Click the *Message type* dropdown list and select the required EDIFACT message type. In our example, it is **INVOIC**. You can use the search function on top of the dropdown list.

5. Enter the *Reference node path*. Use the following syntax:    
    /M_[Message type, for example INVOIC]\_[EDIFACT version number (last three digits)]/ G\_[Message type, for example INVOIC]\_[EDIFACT version number (last three digits)]\_SG[Group number].     
    For example: /M_INVOIC_07A/G_INVOIC_07A_SG26*   
    Alternatively, you can copy the two parts from the header file message structure.  

    >[INOF] Note that depending on the EDIFACT version, the line items (LIN segment) are included in different groups, such as the SG26 or SG27 group.

    ![File settings tab](../../Assets/Screenshots/EDI/Operation/ExportDefMessagData.png)

 
6. Click the ![Get](../../Assets/Icons/Download.png "[Get]") [GET] button.   
    The message structure of the SG26/SG27 group is displayed. The segment is highlighted in red because it is still empty.    
    It starts with the SG26/SG27 element. Note that in the header definition file settings, after saving, you are no longer able to expand the *G_INVOIC_07A_SG26* or *G_INVOIC_07A_SG27* group.

    ![Message](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructureLineItems.png "[Message]")

7. If desired, expand the message structure by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button.   
    The message structure with its single segments is displayed, it starts with the S_LIN segment. The ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button has changed to an ![Expanded](../../Assets/Icons/NodeExpanded.png "[Expanded]") (Expanded) button.

    ![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructureSG26.png "[Message structure]")

8. Click the [SAVE] button.   
     - The *Exporter definitions* view is displayed.   
     - If you now open the definition again for editing, both the *Data Sources* tab and the *Mapping settings* tab is additionally displayed. 



## Specify line item identifier

Start specifying the line item segments by filling out the single elements of the S_LIN (Line item) segment. This procedure shows how to edit the position number on the invoice.

#### Prerequisites

- You have expanded the message structure, see [Get line item segments](#get-line-item-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

 ![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructureSG26.png "[Message structure]")

1. Expand the S_LIN segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_LIN* segment.   
    The S_LIN segment in turn consists of subordinate segments and fields.

    ![S_LIN segment](../../Assets/Screenshots/EDI/Operation/ExportDefLIN.png "[S_LIN segment]")

2. Check the specification for the fields that are required to be filled. In most cases, you must fill the line item identifier in the *D_1082* row (to identify a line item). This is a numerical value that must be unique. For this reason, it is to be determined dynamically by a data source mapping. 

3. Click the ![Add string attribute](../../Assets/Icons/Plus03.png "[Add string attribute]") (Add string attribute) button to the right of the *D_1082* row.   
     - To the right of the *D_1082* row only the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is available now, with which you can remove the data, if required. The field name and description are no longer displayed in italics.  
    - The *S_LIN* segment is now highlighted in red. This indicates that the segment contains data, but not all required data for the EDIFACT message structure are filled.   
    - The string attribute has been marked for a later data mapping.

    ![D_1082 row](../../Assets/Screenshots/EDI/Operation/ExportDefLIN1082.png "[D_1082 row]")

 4. Click the [SAVE] button to save the message structure.   
    The *Exporter definitions* list is displayed. The defined string attribute is mow added to the attribute mapping function in the *Data source* tab.

5. If desired, check whether the string attribute has been really marked for a later data mapping. For detailed information, see [Map attributes](./04_ManageDataSources.md#map-attributes).   
    The EDI Export LIN/1082 *Destination attribute* has been added to the attributes to be mapped later or directly afterwards, if desired.

    ![Map attributes](../../Assets/Screenshots/EDI/Operation/ExportDefLIN1082Mapping.png "[Map Attributes]")

