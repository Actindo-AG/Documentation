# Dependencies tab

*Any module that processes DataHub entities > Select entity > Click the Dependencies tab*

![Dependencies](../../Assets/Screenshots/DataHub/Others/Dependencies.png)

This tab is not part of the *DataHub* module, but it is used in many other *Core1 Platform* modules that refer to information coming from the *DataHub* module.  

**Dependencies**

The list displays all dependencies of the selected entity. Dependencies exist when individual attributes of an entity or the entire entity are linked to another entity, such as through inheritance or automatic mapping. This is the case, for example, of an offer in the *Omni-Channel* module that has been created by an automatic mapping from a product of the *PIM* module.    

Depending on the settings, the displayed columns may vary.

- *Dependent entity ID*   
    Identification number of the dependent entity.

- *Dependent entity type*   
    Type of the dependent entity. The available types depend on the installed plugins.

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Another more descriptive identifier of the dependent entity such as the SKU number or an invoice number.


The following functions are available for the editing toolbar:

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependent entities in the list are selected.

- [RERUN MAPPING]   
    Click this button to rerun the ETL mapping of the selected entity or entities. This button is only displayed if the checkbox of at least one dependency is selected.
    
    >  [Caution] When rerunning an ETL mapping, it is possible to overwrite the data in the dependent entity. This is especially relevant for manual change tracking mode, since . This function should therefore be used with extreme caution and being fully aware of the consequences.

[comment]: <> (Reformulate!)

- [DELETE DEPENDENCY]  
    Click this button to delete the dependency of the selected entity. This button is only displayed if the checkbox of one dependency is selected. 

    > [Caution] This function allows you to break the link established between two interdependent entities. As a result, automatic updates in the dependent entity will no longer work. This function should therefore be used with extreme caution and being fully aware of the consequences. 
    
- *Change tracking mode*   
    Select the *Change tracking mode (ETL mode)* drop-down list of the dependent entity. This drop-down list is only displayed if the checkbox of one dependency is selected. The following options are available:
    - **Manual**
    - **Semiautomatic**
    - **Semiautomatic, changes must be confirmed by another user**   
    - **Automatic**





    

