# Module overview

In this part of the *Actindo Core1 Platform* documentation, you will find a brief overview on the most important *Actindo Core1 Platform* modules and technical components as well as a description of the data streams between these components.



## Basic plugins and modules

The following modules and plugins are the basis for the *Actindo Core1 Platform*. Their features control and process the data flow, the data processing, the data mapping as well as the communication with third party applications. In addition, it provides master data needed for a lot of modules.

**Core1 Platform**   
The *Core1 Platform* is underlying any plugin. It offers basic functions such as the following:
- Request handling
- User management
- Asynchronous jobs 
- License handling
- Event system
- Database connection
- Sandbox system   
- and much more...

**Process orchestration**    
The *Actindo Work Flow Engine* module is a tool that allows you to shape, control, map, and monitor your business processes. Based on your special and individual business rules, you can map and made available your company's processes &ndash; from simple processes to complex workflows. You can build your own custom workflows to automate the processing of entities such as products and orders.

**Currency**   
The *Currency* module (?) <!---ist das ein Modul?--> provides a list of currencies with their ISO codes as well as daily exchange rates provided by the European Central Bank (ECB).

**Taxes**   
The *Taxes* module allows you to configure the system automatic tax feature to match your specific business requirements. You can define specific tax classes applicable to your products and determine different tax zones where you operate. Additionally, you can set up an unlimited number of tax rates, which you can also specify according to their validity period.   
For each tax zone &frasl; tax class combination you can define tax rates. You can determine relevant tax zones based on country, ZIP-code, B2B/B2C, and much more.

**Countries and languages**   
Provides any country with their ISO code and supports country classifications such as European Union (EU).


**Data hub**   
The *DataHub* module offers you the possibility to extend any data model with user-defined custom fields. The ETL-Functionality allows to control the data flow between the different data models. The most Actindo modules and plugins are based on the *DataHub* module.  
This enables you to customize your individual data fields and sources for each process. The *Actindo DataHub* module is the system’s central data hub and is extended by the following modules:   
- DataHub Importer  
Allows the import of any data from various data sources into DataHub-based entities by uploading the file types csv, json, xml, and edi via the network protocols HTTP and SFTP.

- DataHub Exporter  
Allows the export of any data from various data sources into DataHub-based entities by uploading the file types csv, json, xml, and edi via the network protocols HTTP and SFTP.



## Product data

**Cloudinary**  
The *Actindo Cloudinary* module is an integration of Cloudinary&trade; to Actindo. It allows to output the Cloudinary&trade; images via their URLs in web shops or marketplaces via the ETL mapping in Actindo. It is integrated via the *Actindo DataHub* module.  
 You can use the integration to upload images to Cloudinary&trade; via Actindo, to import images from Cloudinary&trade; to Actindo, and to delete images in Cloudinary&trade; via Actindo.


**PIM**  
The *Actindo Product Information Management* (PIM) module is the master data store for collecting, managing, and enriching product data and thus the heart of all your sales channels. You can integrate the *PIM* module quickly and into your existing system landscapes and serves as the basis for efficient unified commerce across all channels.
The PIM master data are used to provide material master data as well as data needed for the communication with webshops and marketplaces.

**Material**   
Material master data from the *PIM* module such as SKU (stock keeping unit), weight, and length is used as basis for warehousing. These master data does not contain metadata such as shop descriptions or keywords. The warehousing enriches these data with information on stock levels etc.

**Omni-channel**  
The *Actindo Omni-Channel* module uses the product metadata to control the communication of your web store with all relevant marketplaces. Additionally, it controls the communication with POS systems with multi location and multi cash register handling. It is used to upload offers and to import orders from the marketplaces. It allows exporting and importing of returns. 
With the *Actindo Omni-Channel* module, you can connect your web store and all relevant marketplaces directly to the platform and manage them centrally from it. You can integrate various store systems such as Shopware 6&trade;, Shopify&trade; or Amazon&trade;.

## Order management

**Warehousing**   
The *Actindo Warehouse Management* stores basic data needed for order management as well as for warehouse handling. You can use it to manage stock levels per material. It allows several kinds of postings such as inventory, reservation, pickings, sells and much more. 

The *Actindo Warehouse Management* module is the central place on *Actindo's Core1 platform* for organizing and monitoring warehouse processes. It provides a complete inventory overview of all your products and warehouses, as well as inventory tracking in real time. It stores basic data needed for order management as well as warehouse handling, such as SKU (stock keeping unit), weight, length. You can plan warehouse locations according to different metrics such as building shapes and sizes, shelves or compartments, as well as manage individual storage bins. 

**Omni-channel**  
With *Actindos Omni-Channel* module, you can connect your web store and all relevant marketplaces directly to the platform and manage them centrally from it. You can integrate various store systems such as Shopware 6&trade;, Shopify&trade; or Amazon&trade;. You can use it to upload offers and to import orders. It allows exporting and importing returns.   
It provides orders for the *Actindo Order Management System* (OMS) and authorizations for the *Actindo Payments* module.

**POS**  
With the cloud-based POS system of the *Actindo Core1 Platform*, you not only control your online channels via Actindo, but can also easily integrate your offline stores. The *Venduo POS* module enables digital and centralized management of your physical stores directly through the platform, dissolving obstructive boundaries between digital and classic commerce.
You can integrate POS-Systems with multi location and multi cash register handling. It provides payment data to be posted for the *Actindo Accounting* module. 


## Order Management

**Fulfillment**   
Whether you work with external fulfillment providers or handle shipping yourself, the *Actindo Fulfillment* module allows you to seamlessly integrate external service providers for fast shipping processing and clear monitoring.  
It provides stock updates for the warehousing. 

**Warehousing**   
The *Warehouse Management* module is the central place on the *Actindo Core1 Platform* for organizing and monitoring warehouse processes. You can manage of stock levels per material. It allows several kinds of postings such as inventory, reservations, pickings, and sells.

**Order Management System**   
Manages documents such as order confirmations, invoices, delivery notes, and returns. It receives return documents from the return management and provides orders for it. It sends delivery notes to the *Actindo Fulfillment* module

**Customers and Suppliers**    
After orders are imported from any connected stores and marketplaces, customer master data is automatically created, or existing master data records are recognized and updated as needed.

**Return Management**   
The *Return management* module of the *Actindo Core1 Platform* offers the necessary basis for the intelligent processing of returns with practical customization and automation options. For example, you can define follow-up actions via customer-specific workflows.

**Accounting**    
The *Actindo Core1 Platform* is the only digital operations platform worldwide with a complete accounting module integrated. This means that all postings for all orders of the connected channels and accounts are automatically generated and optionally transferred live to a group accounting system. As a result, your data integration is extremely simplified and easy to manage.

**Payment Processing**   
The *Payment processing* module receives external payments and tries to match them with open positions. It contains the EBIC (European Banking Industry Committee) interface for importing transactions on bank accounts.

**Payments**   
The *Payments* module gives you the possibility to exchange data with various payment service providers such as Adyen&trade;, Paypal&trade;, or Stripe&trade;. The module allows fully automated processing of incoming payments and refunds. It acts as a link between payment service providers and an accounting solution.

**Business Intelligence**    
The *Database and reporting* module is a powerful tool to quickly access, retrieve and manage all data contained in your system. SQL, which stands for Structured Query Language, is used to communicate with your databases. Its applications range from selecting and retrieving data to altering table structures and updating contents, to name just a few. The *Actindo Database and reporting* module also allows you to create predefined queries to determine who can access your data and how. 




[^1]: **Disclaimer:** InfluxDB&trade; is a trademark owned by InfluxData, which is not affiliated with, and does not endorse, this site.  
