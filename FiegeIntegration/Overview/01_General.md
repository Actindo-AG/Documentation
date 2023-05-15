# General information

The *Fiege* driver seamlessly connects the *Actindo Core1 Platform* and the Fiege fulfillment system. 

Actindo sends automatically a dispatch note containing all relevant order and product data to Fiege when a delivery note has been issued by the *Order management* module. In turn, all shipment data provided by Fiege can be checked and monitored centrally in the *Fulfillment* module. 

The creation of dispatch notes and the triggering of the export need to be configured through the relevant workflow in the *Workflows* module. For detailed information, see [Workflows](../../ActindoWorkFlow/Overview/01_General.md). The export will then instruct the *Fiege* driver to send all necessary data over to them.

This documentation refers to *Fiege Integration* plugin version 1.0.0. There may be differences in the UI, features and operation if your *Fiege Integration* plugin is installed in a different version.


## Benefits

The Actindo *Fiege Integration* plugin offers the following benefits:

- export of orders, SKUs and basic product data to Fiege
- automatic status updates 
- handling of returns
- provision of documents, such as delivery notes or pro-forma invoices, via SFTP upload

[comment]: <> (Info aus Confluence space Product, Status Mai 2023)

## Prerequisites

- The *Configuration Driver Fulfillment Abstract* plugin version 1.0.0 or higher is installed.
- The *Configuration Driver GDM Abstract* plugin version 1.0.0 or higher is installed.
- The *Fulfillment* module version 1.2.0 or higher is installed.


 