# Manage header file settings


The following procedures show you by using an example how to specify the fields required by your business partner. As example the D07A INVOIC message is used.

## Get header file segments

/M_INVOIC_07A/G_INVOIC_07A_SG26  
> [INFO] The UNA, UNB and UNH segments are generated automatically, for this reason, the definition starts with the S_BGM segment

You can add constant values as well as strings that are to be determined via attribute mapping. Example: The document number is a variable value that differs for each message. 


#### Prerequisites

- You have the message specification resp. implementation guide of your business partner at hand.
- You have created the basic definition settings for this type of message and business partner, see [Create basic definition settings](./01_ManageDefinitions.md#create-basic-definition-settings).

#### Procedure

*DataHub Exporter > Exports*

![Exporter definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Exporter definitions]")

1. Click the definition for which you want to specify the header file settings.
    The *Edit definition "definition name"* view is displayed. The *SETTINGS* tab is displayed by default.

    ![Edit definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionEdit.png "[Edit definition]")

2. Click the *File settings* tab.

    BILD ERGÄNZEN MIT OHNE MESSAGE

3. Click the *Release* drop-down list and select the EDIFACT version to which you want to refer. Information on the relevant version is specified in the specification resp. implementation guide of your business partner.

4. Click the *Message type* drop-down list and select the message type which you want to set up, for example INVOIC.

5. Click the ![Get](../../Assets/Icons/Download.png "[Get]")[GET] button.   
    The *Reference node path* as well as the message is displayed. The message name is highlighted in red, because it is still empty.

    ![Message](../../Assets/Screenshots/EDI/Operation/ExportDefMessNew.png "[Message]")

6. Expand the message by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button.   
    The message structure with its single segments is displayed. The ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button has changed to an ![Expanded](../../Assets/Icons/NodeExpanded.png "[Expanded]") (Expanded) button.

    ![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")
BILD NEU MACHEN OHNE MARKIERUNGEN



## Specify message name &frasl; constant text value

Specify the header file segments by filling out the single elements of the BGM (Beginning of message) segment. This procedure shows how to edit a constant text value, for example the transaction type *Commercial invoice* that specifies the type of the INVOIC message.

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > Exports > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")

1. Expand the S_BGM segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM* segment.   
    The S_BGM segment in turn consists of subordinate segments and fields.

    ![S_BGM segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM.png "[S_BGM segment]")

2. Expand the *S_BGM C002* (Document/message name) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM C_C002* segment. In most cases it is mandatory to specify this segment.   
    The *S_BGM C_C002* segment has been expanded. The individual fields of this segment are displayed.

    ![S_BGM C_C002 segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C002.png "[S_BGM  C_C002 segment]")

3. Check the specification for the fields that are required to be filled. In most cases, you must fill the 1001 field (Document name code). This is a constant value with predefined codes for the document type.

4. Click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") button at the end of the 1001 row.  
    The *Edit text value* window is displayed.

    ![Edit text value](../../Assets/Screenshots/EDI/Operation/ExportDefEditTextValue.png "[Edit text value]")


5. Enter the required text value in the *Text value* field.

6. Click the [SAVE] button.   
    The *Edit definition "Definition name"* view is displayed again. At the end of the *1001* row the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is available only, with which you can remove your new entry.   
    The *S_BGM C_C002* segment is now highlighted with a small black border. This indicates that the segment contains data.

    ![Highlighted segment](../../Assets/Screenshots/EDI/Operation/ExportDefHighlightSegment.png "[Highlighted segment]")



## Specify document number &frasl; string attribute

Specify the header file segments by filling out the single elements of the BGM (Beginning of message) segment. This procedure shows how to edit a string attribute which is automatically determined by a data source mapping. For example the document number of the INVOIC message that must be unique. fortlaufend?

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > Exports > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")

1. Expand the S_BGM segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM* segment.   
    The S_BGM segment in turn consists of subordinate segments and fields.

    ![S_BGM segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM.png "[S_BGM segment]")

2. Expand the *S_BGM C_C106* (Document/message identification) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM C_C106* segment. In most cases it is required to specify this segment.   
    The *S_BGM C_C106* segment has been expanded. The individual fields of this segment are displayed.

    ![S_BGM C_C106 segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C106.png "[S_BGM  C_C106 segment]")

3. Check the specification for the fields that are required to be filled. In most cases, you must fill the *1004* field (Document identifier). This is a dynamic value with predefined codes for the document type.

4. Click the ![Add string attribute](../../Assets/Icons/Plus08.png "[Add string attribute]") button at the end of the *D_1004* row.   
     - At the end of the *D_1004* row the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is available only, with which you can remove your new entry.   
    - The *S_BGM C_C106* segment is now highlighted with a small black border. This indicates that the segment contains data.   
    - The string attribute has been marked for a later data mapping.


5. If desired, check whether the string attribute has been really marked for a later data mapping. For detailed information, see [Map attributes](./04_ManageDataSources.md#map-attributes).   
    The EDI Export BGM/C106/1004 *Destination attribute* has been added to the attributes to be mapped later.

    ![Map attributes](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C106Mapping.png "[Map Attributes]")


6. Click the [SAVE] button. 



## Specify message dates

Each invoice can have a lot of different dates, for example the invoice date, the expected delivery date, the tax point date, and much more. The Actindo EDIFACT message structure contains only one BTM segment in the raw state. However, for many business partners, multiple BTM segments must be completed. As soon as you have specified one value in a BTM segment, a further BTM segment is added automatically. 

#### Prerequisites

- - You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > Exports > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDates.png "[Message structure]")

1. Expand the *S_DTM* (DATE &frasl; TIME &frasl; PERIOD) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_DTM* segment.   
    The *S_DTM* segment in turn consists of the subordinate *C_C507* segment.

2. Expand the *C_C507* (Date and&frasl;or time, or period relevant to the) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *C_C507* segment. In most cases it is required to specify this segment.   
    The *C_C507* segment has been expanded. The individual fields of this segment are displayed.

    ![C_C507 segment](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDTMSegment.png "[C_C507 segment]")

3. Specify the *2005 (Date or time or period function code qualifier)* field. In most cases, a constant value is required here. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") button at the end of the *2005* row.  
    The *Edit text value* window is displayed.

    ![Edit text value](../../Assets/Screenshots/EDI/Operation/ExportDefEditTextValue.png "[Edit text value]")
 
4. Enter the text value and click the [SAVE] button.
    A new *S_DTM* segment has been added below the *S_DTM* segment you are currently working on.

5. Specify *2380 (Date or time or period text)* field. In most cases, a string attribute is required here. To do this, click the ![Add string attribute](../../Assets/Icons/Plus08.png "[Add string attribute]") button at the end of the *2380* row.  

6. Specify *2379 (Date or time or period format code)* field. In most cases, a constant value is required here. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") button at the end of the *2005* row.  
    The *Edit text value* window is displayed. 

7. Enter the text value and click the [SAVE] button.   
    The *S_DTM* segment has been finished. 

8. Click the [SAVE] button to save the message structure.   
    The *Exporter definitions* list is displayed.
 

