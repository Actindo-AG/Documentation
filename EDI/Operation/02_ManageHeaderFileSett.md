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



## Specify message name

Specify the header file segments by filling out the single elements of the BGM (Beginning of message) segment. This procedure shows how to edit a constant text value.

#### Prerequisites

- You have expanded the message structure, see [Get header file segments](#get-header-file-segments).

#### Procedure

*DataHub Exporter > Exports > Select message definition > File settings tab >Expand message structure*

![Message structure](../../Assets/Screenshots/EDI/Operation/ExportDefMessageStructure.png "[Message structure]")

1. Expand the S_BGM segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the **S_BGM** segment.   
    The S_BGM segment in turn consists of subordinate segments and fields.

    ![S_BGM segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM.png "[S_BGM segment]")

2. Expand the **S_BGM C002** (Document/message name) segment by clicking the ![Collapsed](../../Assets/Icons/NodeCollapsed.png "[Collapsed]") (Collapsed) button at the **S_BGM** segment. In most cases it is mandatory to specify this segment.   
    The **S_BGM C002** segment has been expanded. The individual fields of this segment are displayed.

    ![S_BGM C_C002 segment](../../Assets/Screenshots/EDI/Operation/ExportDefBGM_C002.png "[S_BGM  C_C002 segment]")

3. Check the specification for the fields that are required to be filled. In most cases, you must fill the 1001 field (Document name code). This is a constant value with predefined codes for the document name.

4. Click the ![Constant value](../../Assets/Icons/Edit04.png "[Constant value]") button at the end of the 1001 field line.
    The *Edit text value* window is displayed.

    ![Edit text value](../../Assets/Screenshots/EDI/Operation/ExportDefEditTextValue.png "[Edit text value]")


5. Enter the required text value in field *Text value*.

6. Click the [SAVE] button.



 

