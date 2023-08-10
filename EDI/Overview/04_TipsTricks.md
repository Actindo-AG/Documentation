# Tips and tricks for preparation

## Introduction

The EDIFACT standard defines the scheme according to which the messages should be structured. The EDIFACT standard is available in different versions, every year a new version with a and b is released. The users of the EDIFACT standard define their specification according to a specific version. Since Actindo provides the structure for the different versions, you can find the particular version that your business partner has specified in the Actindo standard.   
Note that the structure of the format is standardized, not the usage. As a result, each user defines the data to be provided for the message structure. This also applies to the classification of the segments and fields (mandatory, required, optional and others), which can sometimes differ from the EDIFACT standard.   
When we speak about a user or a business partner in the following, the company is meant, to which you must send the messages, for example your supplier, your customer, or your fulfiller.

## Tips for preparation in advance

- Ask your business partner for the EDIFACT message specification resp. the message implementation guide. Specifications of some big players are also available as download versions on the internet.

- Check this specification for the fields, that the user has defined as required and ensure that you have this data available.    
    Note, some segments are mandatory only in case if the overlying optional segment is to be filled. See the example:

    ![Mandatory segments](../../Assets/Screenshots/EDI/Overview/OptionalSegment.png "[Mandatory segments]")

- A lot of internet providers give information on EDIFACT. For a first impression we can recommend the https://www.truugo.com/edifact/ website that provides you with a very structured illustration of the EDIFACT messages in their different versions.

- Ask your business partner for the connection details that specify how the data are to be transferred.

- You can preview each message structure as a string. For example:
    UNB+UNOC:3+:14+:14+230810:1443+76817314338981'UNH+67850136066306+ORDERS:D:07A:UN:EAN008'BGM+220+202300001'DTM+8::102'UNS+S'UNT+5+67850136066306'UNZ+1+76817314338981'