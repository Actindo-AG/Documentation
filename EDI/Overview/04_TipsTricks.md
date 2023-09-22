# Tips and tricks for preparation



## Introduction

The EDIFACT standard defines the scheme according to which the messages should be structured. The EDIFACT standard is available in different versions, every year a new version is released (often also an a or b version). Your business partners, the receivers of the EDIFACT messages define their specifications according to a specific version. Since Actindo provides the structure for the different versions, you can find the particular version that your business partner has specified in the Actindo standard.   
Note that the structure of the format is standardized, not the usage. As a result, each user/business partner defines the data to be provided for the message structure. This also applies to the classification of the segments and fields (mandatory, required, optional and others), which can sometimes differ from the EDIFACT standard.   
>[INFO] When we speak about a user or a business partner in the following, the company is meant, to which you must send the messages, for example your supplier, your customer, or your fulfiller.



## Tips for preparation in advance

- A lot of internet providers give information on EDIFACT. For a first impression we can recommend the https://www.truugo.com/edifact/ website that provides you with a very structured illustration of the EDIFACT messages in their different versions.  

- Ask your business partner for the EDIFACT message specification resp. the message implementation guide. Specifications of some big players are also available as download versions on the internet.

- Ask your business partner for the connection details that specify to which address and with which credentials the data are to be transferred.

- Check this specification for the segments, that your business partner has defined as required and ensure that you have this data available.   

- Note the following: 
    - Some segments are mandatory (M) only in case if the overlying optional segment is to be filled. See the example:

    ![Mandatory segments the Edifact standard](../../Assets/Screenshots/EDI/Overview/OptionalSegment.png "[Mandatory segments]")

    - Depending on the business partner, there are deviations from the standard.    
        - Some segments are required (R), even if it is not mandatory in the EDIFACT message definition.  These are then usually indicated with **R** (required) in contrast to **M** (mandatory) in the EDIFACT standard. 
        - The reverse situation is also possible. Sometimes the business partners do not want to have mandatory segments of the EDIFACT message filled.
        Actindo highlights a segment in red, if mandatory parts are not filled according to EDIFACT. But nevertheless, Actindo sends the message anyway, even if parts defined as mandatory by EDIFACT are missing.  

- Actindo enables you to preview each message structure as a string. For example:
    UNB+UNOC:3+:14+:14+230810:1443+76817314338981'UNH+67850136066306+ORDERS:D:07A:UN:EAN008'BGM+220+202300001'DTM+8::102'UNS+S'UNT+5+67850136066306'UNZ+1+76817314338981'   
    The specifications of the big players often also shows parts of this string as examples, so that you can use the preview for checking the message output. Check the specification of your business partner for these examples. Then join the required parts together or copy the individual parts so that they are output in a single string. This way you can always check in between whether you are on the right track. 