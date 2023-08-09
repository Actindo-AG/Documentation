# Manage definition settings

The definition of the EDIFACT export messages specifies the definition settings with template engine and the connection to be used, contain the message structure with predefined data as well as the data mapping and the mapping settings.
Each EDIFACT export message requires two definitions in the *DataHub Exporter* module:
- Definition of the message header   
    Figuratively speaking, the message header is the envelope, with which the message is sent. It contains general data such as receiver &frasl; sender information and dates
- Definition of the line items  
    The line items contain the single positions of the message, for example the single items on an invoice.


## Create definition settings



#### Prerequisites


#### Procedure