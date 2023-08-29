# Specify header file settings


The following procedures show by using an example how to specify the fields required by your business partner. As example the D07A INVOIC message is used.

## Get header file segments

Get the header file segments of an EDIFACT message in order to be able to fill them.  
  
> [INFO] The UNA, UNB and UNH segments are generated automatically, for this reason, the definition starts with the S_BGM segment

You can add constant values as well as strings that are to be determined via attribute mapping. Example: The document number is a variable value that differs for each message. 


#### Prerequisites

- You have the message specification of your business partner at hand.
- You have created the basic definition settings for this type of message and business partner, see [Create basic definition settings](./01_ManageDefinitions.md#create-basic-definition-settings).

#### Procedure

*DataHub Exporter > EXPORTS tab*

![Exporter definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Exporter definitions]")

1. Click the definition for which you want to specify the header file settings.   
    The *Edit definition "definition name"* view is displayed. The *Settings* tab is displayed by default.

    ![Edit definition](../../Assets/Screenshots/EDI/Operation/ExportDefinitionEdit.png "[Edit definition]")

2. Click the *File settings* tab.   
    The *File settings* tab is displayed.

     ![File settings tab](../../Assets/Screenshots/EDI/Operation/ExportDefDefineFileSettings.png "[File settings tab]")


3. Click the ![Get](../../Assets/Icons/Download.png "[Get]") [GET] button.   
    The message structure is displayed. The message name is highlighted in red because it is still empty.

    ![Message](../../Assets/Screenshots/EDI/Operation/ExportDefMessNew.png "[Message]")

4. Expand the message structure by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button.   
    The message structure with its single segments is displayed. The ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button has changed to an ![Expanded](../../Assets/Icons/NodeExpanded.png "[Expanded]") (Expanded) button.

    ![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")

5. Click the [SAVE] button.




## Specify message name &frasl; constant text value

Start specifying the header file segments by filling out the single elements of the BGM (Beginning of message) segment. This procedure shows how to edit a constant text value, for example the transaction type *Commercial invoice* that specifies the type of the INVOIC message.

>[INFO] The following procedures show by using examples how to specify specific header segments of the EDIFACT message. Follow the guidelines of your business partner when specifying the EDIFACT message! 


#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")

1. Expand the S_BGM segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM* segment.   
    The S_BGM segment in turn consists of subordinate segments and fields.

    ![S_BGM segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM.png "[S_BGM segment]")

2. Expand the *S_BGM C002* (Document/message name) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM C_C002* segment. In most cases it is mandatory to specify this segment.   
    The *S_BGM C_C002* segment has been expanded. The individual fields of this segment are displayed.

    ![S_BGM C_C002 segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C002.png "[S_BGM  C_C002 segment]")

3. Check the specification for the fields that are required to be filled. In most cases, you must fill the *1001* field (Document name code). This is a constant value for which your business partner may have specified predefined codes for the document type.

4. Click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") buttonto the right of the *D_1001* row.  
    The *Edit text value* window is displayed.

    ![Edit text value](../../Assets/Screenshots/EDI/Operation/ExportDefEditTextValue.png "[Edit text value]")


5. Enter the required document name code in the *Text value* field.

6. Click the [SAVE] button.   
    The *Edit definition "Definition name"* view is displayed again. To the right of the *D_1001* row the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is available only, with which you can remove your new entry.   
    The *S_BGM C_C002* segment is now highlighted with a small black border. This indicates that the segment contains data.

    ![Highlighted segment](../../Assets/Screenshots/EDI/Operation/ExportDefHighlightSegment.png "[Highlighted segment]")



## Specify document number &frasl; string attribute

Specify the header file segments by filling out the single elements of the BGM (Beginning of message) segment. This procedure shows how to edit a string attribute which must be automatically determined by a data source mapping later, because you need to specify a document number of the INVOIC message that must be unique. 

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")

1. Expand the S_BGM segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM* segment.   
    The S_BGM segment in turn consists of subordinate segments and fields.

    ![S_BGM segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM.png "[S_BGM segment]")

2. Expand the *S_BGM C_C106* (Document/message identification) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_BGM C_C106* segment. In most cases it is required to specify this segment.   
    The *S_BGM C_C106* segment has been expanded. The individual fields of this segment are displayed.

    ![S_BGM C_C106 segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C106.png "[S_BGM  C_C106 segment]")

3. Check the specification for the fields that are required to be filled. In most cases, you must fill the document number in the *1004* field (Document identifier). This is a numerical value that must be unique. For this reason, it is to be determined dynamically by a data source mapping. 

4. Click the ![Add string attribute](../../Assets/Icons/Plus03.png "[Add string attribute]") button to the right of the *D_1004* row.   
     - To the right of the *D_1004* row only the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is available now, with which you can remove the data, if required.   
    - The *S_BGM C_C106* segment is now highlighted with a small black border. This indicates that the segment contains data.   
    - The string attribute has been marked for a later data mapping.

6. Click the [SAVE] button to save the message structure.   
    The *Exporter definitions* list is displayed.

5. If desired, check whether the string attribute has been really marked for a later data mapping. For detailed information, see [Map attributes](./04_ManageDataSources.md#map-attributes).   
    The EDI Export BGM/C106/1004 *Destination attribute* has been added to the attributes to be mapped later or directly afterwards, if desired.

    ![Map attributes](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C106Mapping.png "[Map Attributes]")



## Specify message dates

Each invoice can have a lot of different dates, for example the invoice date, the expected delivery date, the tax point date, and much more. The Actindo EDIFACT message structure contains only one BTM segment in the raw state. However, for many business partners, multiple BTM segments must be completed. As soon as you have specified one value in a BTM segment, a further BTM segment is added automatically so that you can specify as much BTM segments as your business partner require.

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDates.png "[Message structure]")

1. Expand the *S_DTM* (DATE &frasl; TIME &frasl; PERIOD) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_DTM* segment.   
    The *S_DTM* segment in turn consists of the subordinate *C_C507* segment.

2. Expand the *C_C507* (Date and &frasl; or time, or period relevant to the) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *C_C507* segment. In most cases it is required to specify this segment.   
    The *C_C507* segment has been expanded. The individual fields of this segment are displayed.

    ![C_C507 segment](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDTMSegment.png "[C_C507 segment]")

3. Specify the *D_2005 (Date or time or period function code qualifier)* field. In most cases, a constant value is required here. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") (Set constant value) button to the right of the *D_2005* row.  
    The *Edit text value* window is displayed.

    ![Edit text value](../../Assets/Screenshots/EDI/Operation/ExportDefEditTextValue.png "[Edit text value]")
 
4. Enter the text value and click the [SAVE] button.   
    A new *S_DTM* segment has been added below the *S_DTM* segment you are currently working on.

5. Specify the *D_2380 (Date or time or period text)* field. In most cases, a string attribute is required here. To do this, click the ![Add string attribute](../../Assets/Icons/Plus03.png "[Add string attribute]") (Add string attribute) button to the right of the *D_2380* row.    
    The *D_2380* field is marked for a later data mapping. 

6. Specify the *D_2379 (Date or time or period format code)* field. In most cases, a constant value is required here. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") (Set constant value) button to the right of the *2005* row.  
    The *Edit text value* window is displayed. 

7. Enter the text value and click the [SAVE] button.   
    This *S_DTM* segment has been finished. 

8. Click the [SAVE] button to save the message structure.   
    The *Exporter definitions* list is displayed.

9. If desired, check whether the string attribute has been really marked for a later data mapping. For detailed information, see [Map attributes](./04_ManageDataSources.md#map-attributes).   
    The EDI Export DTM/C507/2380 *Destination attribute* has been added to the attributes to be mapped later or directly afterwards, if desired.

     ![Map attributes](../../Assets/Screenshots/EDI/Operation/ExportDefDTM_C507Mapping.png "[Map Attributes]")
 
10. Now continue specifying the required DTM file segments.



## Specify message free texts

Specify message free text, with which you can inform your business partner on individual subjects.  This procedure shows how to add individual textual information as well as to add additionally required segments.

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDates.png "[Message structure]")


1. Expand the *S_FTX* (FREE TEXT) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *S_FTX* segment.   
    The *S_FTX* segment in turn consists of the subordinate *C_C107* and *C_C108* segments.

    ![S_FTX segment](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefFTXSegment.png "[S_FTX segment]")

2.  Specify the *D_4451 (Code qualifying the subject of the text)* field. In most cases, a constant value is required here. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") (Set constant value) button to the right of the *D_4451* row.  
    The *Edit text value* window is displayed. 

    ![Edit text value](../../Assets/Screenshots/EDI/Operation/ExportDefEditTextValue.png "[Edit text value]")
 
3. Enter the text code and click the [SAVE] button. 

4. Expand the *C_C108 (Free text; one to five lines)* segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the *C_C108* segment.

5. Enter a free text in the *C_4440* line. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") (Set constant value) button to the right of the *C_4440* row.  
    The *Edit text value* window is displayed.

6. Enter the free text, for example "Please note our changed bank details" and click the [SAVE] button. You can write up to five lines.

7. Specify the language used in the *D_3453 (Code specifying the language name)* line. To do this, click the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") (Set constant value) button to the right of the *D_3453* row and specify the language code in the *Edit text value* window.  
    
8. Collapse the *S_FTX* segment by clicking the ![Expanded ](../../Assets/Icons/NodeExpanded.png "[Expanded]") (Expanded) button to the right of the *S_FTX* segment row.   
    The segment is collapsed.

9. If desired, add further *S_FTX* segments by clicking the ![Add XML attribute](../../Assets/Icons/Plus08.png "[Add XML attribute]") (Add XML attribute) button.   
    An additional *S_FTX* segment is added below the currently processed segment.

    ![Additional S_FTX segment](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefFTXAdditionalSegment.png "[Additional S_FTX segment]")

10. Now continue specifying the header file segments until you have specified all fields that your business partner require.



## Prepare line item export

In order to be able to export the single positions of an invoice, for example, 
the relevant group for the line items of an EDIFACT message must be indicated to be exported as a whole. You have to do this here in the header definition file settings. 

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDates.png "[Message structure]")


1. Check the EDIFACT message structure, in which group the LIN segment is available. In newer versions, the LIN segment is included in group 27, in older versions, it is in group 26.

2. Scroll down in the message structure until you have found the relevant group, *G_INVOIC_07A_SG26* resp. *G_INVOIC_07A_SG27*.

3. Click the ![Add XML attribute](../../Assets/Icons/Plus08.png "[Add XML attribute]") (Add XML attribute) button to the right of the *G_INVOIC_07A_SG26* resp. *G_INVOIC_07A_SG27* row. 
    The segment is now highlighted with a small black border. You cannot expand it.   
    Another *G_INVOIC_07A_SG26* resp. *G_INVOIC_07A_SG27* row has been added. You can ignore it.   
    The EDI Export BGM/C106/1004 *Destination attribute* has been added to the attributes to be mapped later.

4. Click the [SAVE] button.

5. If desired, check whether the group has been really marked for a later data mapping. For detailed information, see [Map attributes](./04_ManageDataSources.md#map-attributes).   
    The EDI Export SG[Group name] *Destination attribute* has been added to the attributes to be mapped later or directly afterwards, if desired.

     ![Map attributes](../../Assets/Screenshots/EDI/Operation/ExportDefSG26Mapping.png "[Map Attributes]")
     BILD NEU MACHEN

5. Continue processing the EDIFACT message by specifying the line item segment. For detailed information, see [Specify line item file settings](./03_ManageLineItemsFileStt.md).   




## Edit header file settings

To edit the header file settings, you must remove the data you have provided for a segment resp. a segment row before.

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > EXPORTS tab > Select message definition > File settings tab > Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessDefDates.png "[Message structure]")

**Remove data from the whole segment**

1. If you want to remove the data from a whole segment, click the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button to the right of the corresponding segment.   
    The ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is replaced by the ![Add XML attribute](../../Assets/Icons/Plus08.png "[Add XML attribute]") (Add XML attribute) button.   
    The segment is no longer highlighted with a small black border, the data are removed from the segment.

2. Start specifying again the segment with new data.

**Remove data from a segment row**

1. If you want to remove data from a segment row, expand the corresponding  segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the segment.   

2. Click the ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button to the right of the row, from which you want to remove the data.   
    The ![Delete attribute](../../Assets/Icons/Trash10.png "[Delete attribute]")(Delete attribute) button is replaced both by the ![Add string attribute](../../Assets/Icons/Plus03.png "[Add string attribute]") (Add string attribute) button and the ![Set constant value](../../Assets/Icons/Edit04.png "[Set constant value]") (Set constant value) button.

3. Start specifying again the row with new data.
    