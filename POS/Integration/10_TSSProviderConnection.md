# Create connection to TSS Provider

In Germany, the Kassensicherungsverordnung (KassenSichV) is an ordinance that define the technical requirements for electronic recording and security systems in business transactions. It enforces that the merchant records all transactions in a non-manipulable manner.   
The TSS (Technical security system) must fulfill certain requirements and needs certification. It must generate certain data like a sequence number, digital signing, and much more. This information must be either printed on the receipt in human-readable form or encoded in a QR code that can be scanned to reveal the information.   
Actindo currently works with fiskaly&trade;, which is a cloud provider for TSS. It allows to register the transactions via API calls after everything is set up.   
Actindo has the license to fiskaly&trade; and a master account. Each Actindo customer receives a sub-account of it. Each sub-account can have multiple TSS', for example, for each location one TSS. In turn, each TSS can have multiple clients that correspond to the paydesks.

You use this procedure to create a connection to your sub account of the 
fiskaly&trade; Actindo master account. Usually you have only one TSS connection.

https://actindo.atlassian.net/wiki/spaces/DEVELOPMEN/pages/374505795/TSE 

#### Prerequisites

The Fiskaly Cloud plugin as of version xxx is installed.

#### Procedure

*POS > Management > Tab TSS PROVIDERS*

![TSS Providers](../../Assets/Screenshots/POS/Management/TSSProviders/TSSProviders.png "[TSS Providers]")

1.  Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create Connection* view is displayed.  

    ![Create connection](../../Assets/Screenshots/POS/Management/TSSProviders/CreateConnection.png "[Create connection]")