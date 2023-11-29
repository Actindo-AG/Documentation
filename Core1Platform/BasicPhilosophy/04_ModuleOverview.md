# Module overview

In this part of the *Actindo Core1 Platform* documentation, you will find a brief overview on the most important *Actindo Core1 Platform* modules and technical components as well as a description of the data streams between these components.   
<!---For a detailed illustration of the interactions between modules, see also the overview graphic [Module overview &ndash; Diagram](./04a_GraphicModuleOverview.md).-->


## Basic plugins and modules

The following modules and plugins are the basis for the *Actindo Core1 Platform*. Their features control and process the data flow, the data processing, the data mapping as well as the communication with third party applications. In addition, it provides master data needed for many modules.

**Core1 Platform**   
The *Core1 Platform* is the foundation of every module/plugin. It offers basic functions such as the following:
- Request handling
- User management
- Asynchronous jobs 
- License handling
- Event system
- Database connection
- Sandbox system   
- and much more...

**Process orchestration**    
The *Workflows* module is a tool that allows you to shape, control, map, and monitor your business processes. Based on your special and individual business rules, you can map and made available your company's processes &ndash; from simple processes to complex workflows. You can build your own custom workflows to automate the processing of entities such as products and orders.

**Currency**   
The *Currency* plug-in provides a list of currencies with their ISO codes as well as daily exchange rates provided by the European Central Bank (ECB).

**Taxes**   
The *Taxes* module allows you to configure the automatic tax feature of the system to match your specific business requirements. You can define specific tax classes applicable to your products and determine different tax zones where you operate. Additionally, you can set up an unlimited number of tax rates, which you can also specify according to their validity period.   
For each tax zone &frasl; tax class combination you can define tax rates. You can determine relevant tax zones based on country, ZIP-code, B2B/B2C, and much more.

**Countries and languages**   
The *Countries and languages* plugin provides any country with their ISO code and supports country classifications such as European Union (EU).


**Data hub**   
The *DataHub* module offers you the possibility to extend any data model with user-defined custom fields. The integrated ETL function allows to control the data flow between the different data models. Most *Actindo* modules and plugins are based on the *DataHub* module.  
This enables you to customize your individual data fields and sources for each process. The *DataHub* module is the system’s central data hub and is extended by the following modules:   
- DataHub Importer  
Allows the import of any data from various data sources into DataHub-based entities by uploading CSV, JSON, XML, and EDI file types via the network protocols HTTP and SFTP.

- DataHub Exporter  
Allows the export of any data to various data sources by exporting CSV, JSON, XML, and EDI file types via the network protocols HTTP and SFTP.



## Product data

**Cloudinary**  
The *Cloudinary* module is an integration of Cloudinary&trade; to Actindo. It allows to output the Cloudinary&trade; images by their URLs in web shops or sales channels by the ETL mapping in Actindo. It is integrated via the *DataHub* module.  
 You can use the integration to upload images to Cloudinary&trade; via Actindo, to import images from Cloudinary&trade; to Actindo, and to delete images in Cloudinary&trade; via Actindo.

**PIM**  
The *Product Information Management* (PIM) module is the master data store for collecting, managing, and enriching product data and thus the heart of all your sales channels. You can integrate the *PIM* module quickly into your existing system landscapes. It serves as the basis for efficient unified commerce across all channels.
The PIM master data is used to provide material master data as well as data needed for the communication with web shops and sales channels.

**Material**   
Material master data from the *PIM* module such as SKU (stock keeping unit), weight, and length is used as basis for warehousing. This master data does not contain metadata such as shop descriptions or keywords. The *Warehousing* enriches this data with information on stock levels and other warehousing relevant data.

**Omni-Channel**  
The *Omni-Channel* module uses the product metadata to control the communication of your web store with all relevant sales channels. Additionally, it controls the communication with POS systems with multi-location and multi-cash register handling. It is used to upload offers and to import orders from the sales channels. It allows exporting and importing of returns. 
With the *Omni-Channel* module, you can connect your web store and all relevant sales channels directly to the platform and manage them centrally from it. You can integrate various store systems such as Shopware 6&trade;, Shopify&trade; or Amazon&trade;.
It provides orders for the *Order Management System* (OMS) and authorizations for the *Payments* module.

**Venduo POS**  
With the cloud-based POS system of the *Actindo Core1 Platform*, you not only control your online channels via Actindo, but can also easily integrate your offline stores. The *POS* module enables digital and centralized management of your physical stores directly through the platform, dissolving obstructive boundaries between digital and classic commerce.
You can integrate POS-Systems with multi-location and multi-cash register handling. It provides payment data to be posted in the *Accounting* module. 



## Order Management


**Warehousing**   
The *Warehouse Management* is the central point on *Actindo's Core1 platform* for organizing and monitoring warehouse processes. It stores basic data needed for order management as well as for warehouse handling. You can use it to manage stock levels per material. It allows several kinds of postings from the *Order Management System* (OMS) such as inventory, reservation, pickings, sells, and much more. 
The module provides a complete inventory overview of all your products and warehouses, as well as inventory tracking in real time. You can plan warehouse locations according to different metrics such as building shapes and sizes, shelves or compartments, as well as manage individual storage bins. The module receives the material master data and provides stock levels for them. It receives stock updates from the *Fulfillment* module.  

**Customers and Suppliers**    
After orders are imported from any connected stores and sales channels, customer master data is automatically created, or existing master data records are recognized and updated as needed. It provides customer data for the POS systems and receives updates from it.


**Accounting**    
The *Actindo Core1 Platform* is the only digital operations platform worldwide with a complete accounting module integrated. This means that all postings for all orders of the connected channels and accounts are automatically generated and optionally transferred live to a group accounting system.   
The module stores any information on financial transactions. POS systems post payments directly to the *Accounting* module. It receives transactions from the *Payment Processing* module. 
The *Accounting* module gets postings from the *Order Management System* and sends back updates on the payment status to ensure that no unpaid orders are delivered.


**Payment Processing**   
The *Payment Processing* module receives external payments and tries to match them with open positions. It is connected to the EBIC (European Banking Industry Committee) interface for importing transactions on bank accounts. The *Payment Processing* module receives transactions from the *Payments* module.

**Payments**   
The *Payments* module gives you the possibility to exchange data with various payment service providers such as Adyen&trade;, Paypal&trade;, or Stripe&trade;. The module allows fully automated processing of incoming payments and refunds. It provides transactions for the *Payment Processing* module and thus acts as a link between payment service providers and the *Accounting* module.


**Order Management**   
The *Order Management* (OMS) module collects and orchestrates customer orders from all connected B2C and B2B sales channels in one place. It enables fast, seamless, and highly accurate processing of your orders by automating processes.  
The module manages documents such as order confirmations, invoices, delivery notes, and returns. It books materials in the *Warehousing* module. It receives return documents from the return management and provides orders for it. The OMS sends delivery notes to the *Fulfillment* module and ensures through updates from the *Accounting* module that the orders are paid.

**Return Management**   
The *Returns* module of the *Actindo Core1 Platform* offers the necessary basis for intelligent processing of returns with practical customization and automation options. It manages returns and follow-up actions via defined workflows. It gets orders from the *Order Management* (OMS) and creates return documents for it. 

**Fulfillment**   
Whether you work with external fulfillment providers or handle shipping yourself, the *Fulfillment* module allows you to seamlessly integrate external service providers for fast shipping processing and clear monitoring.  
The module gets delivery notes from *Order Management System* (OMS) and provides stock updates for the *Warehouse Management* module. 


<!--- rauslassen?
**Reporting**    
The *Reporting* module is a powerful tool to quickly access, retrieve and manage all data contained in your system. SQL, which stands for Structured Query Language, is used to communicate with your databases. Its applications range from selecting and retrieving data to altering table structures and updating contents, to name just a few. The *Reporting* module also allows you to create predefined queries to determine who can access your data and how. -->




[^1]: **Disclaimer:** InfluxDB&trade; is a trademark owned by InfluxData, which is not affiliated with, and does not endorse, this site.  
