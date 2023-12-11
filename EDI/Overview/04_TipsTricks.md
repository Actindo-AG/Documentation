# Tips and tricks for preparation



## Introduction

The EDIFACT standard defines the scheme according to which the messages should be structured. The EDIFACT standard is available in different versions, every year a new version is released (often also an a or b version). Your business partners, the receivers of the EDIFACT messages define their specifications according to a specific version. Since Actindo provides the structure for the different versions, you can find the particular version that your business partner has specified in the Actindo standard.   
Note that the structure of the format is standardized, not the usage. As a result, each user/business partner defines the data to be provided for the message structure. This also applies to the classification of the segments and fields (mandatory, required, optional and others), which may sometimes differ from the EDIFACT standard.   
>[INFO] When we refer to a user or a business partner in the following, we mean the company you need to send the messages to, such as your supplier, your customer, or your fulfillment partner.



## Tips for preparation in advance

- Many internet providers offer EDIFACT information. For a first impression, we can recommend the https://www.truugo.com/edifact/ website which provides a very structured presentation of the EDIFACT messages in their different versions.  

- Ask your business partner for the EDIFACT message specification resp. the message implementation guide. Specifications of some big players are also available as download versions on the internet.

- Ask your business partner for the connection details that specify to which address and with which credentials the data are to be transferred.

- Review this specification for the segments your business partner has defined as required and ensure that you have this data available.   

- Note the following: 
    - Some segments are mandatory (M) only in case if the optional segment above is to be filled. See the example:

      ![Mandatory segments of the EDIFACT standard](../../Assets/Screenshots/EDI/Overview/OptionalSegment.png "[Mandatory segments of the EDIFACT standard]")

    - Depending on the business partner, there are deviations from the standard:    
        - Some segments are required (R), even if it is not mandatory in the EDIFACT standard message definition.  These are then usually indicated with **R** (required) in contrast to **M** (mandatory) in the EDIFACT standard. 
        - The reverse situation is also possible. Sometimes the business partners do not want to have mandatory segments of the EDIFACT message filled.
        *Actindo* highlights a segment in red, if mandatory parts are not filled according to the EDIFACT standard. But nevertheless, *Actindo* sends the message anyway, even if parts defined as mandatory by EDIFACT are missing.  

- *Actindo* enables you to preview each message structure as a string. For example:
    UNB+UNOC:3+:14+:14+230810:1443+76817314338981'UNH+67850136066306+ORDERS:D:07A:UN:EAN008'BGM+220+202300001'DTM+8::102'UNS+S'UNT+5+67850136066306'UNZ+1+76817314338981'   
    The specifications of the big players often also shows parts of this string as examples, so that you can use the preview for checking the message output. Check the specification of your business partner for these examples. Then join the required parts together or copy the individual parts so that they are output in a single string. This way, you can verify from time to time if you are on the right track. 


## Tips for managing the definitions

Use the following checklist to organize your work. Managing of definitions follows the following sequence:  

|To do                                   | Done   
|-----|------- 
|1. Create the connection to your business partner, see [Manage connections](../Integration/01_ManageConnections.md).|   |     
|2. Create a basic definition setting for the header, see [Create basic header definition settings](../Operation/01_ManageHeaderDefinition.md#create-basic-definition-setting-for-the-header).|   |   
|3. Prepare the definition of file settings to make this task easier, see [Prepare definition of file settings](../Operation/01_ManageHeaderDefinition.md#prepare-definition-of-file-settings).|   |   
|4. Define the file settings for the header, see [Manage header file settings](../Operation/02_ManageHeaderFileSett.md)|   |   
|5. If desired, you can add an attribute mapping after finishing one file setting section, or you do it after finishing the whole EDIFACT message definition. |   |   
|6. Create a basic definition setting for the line item, see [Manage basis line item definition](../Operation/03_ManageLineItemDefinition.md). |   |   
|7. After you have added the file settings, you can preview a message, see [Preview definition](#preview-definition).|   |   
|8. Create basic definition settings for the line items, see [Create basic definition settings](#create-basic-definition-settings).|  |   
|9. If desired, you activate the definition, see.[Activate definition](#activate-definition).|   |    
|10. If desired, you can deactivate or delete a definition, see [Deactivate definition](#deactivate-definition) and [Delete definition](#delete-definition).|   |  