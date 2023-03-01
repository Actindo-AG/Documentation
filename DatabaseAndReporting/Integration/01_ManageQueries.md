[!!User interface Queries](../UserInterface/01a_Queries.md)
[!!Manage the query categories](./02_ManageQueryCategories.md)
[!!Manage the user rights](./05_ManageUserRights.md)

# Manage the queries

Queries can be predefined to determine the queries that user can execute and the data that be can accessed. Instead of entering and executing a query directly in MySQL console, the user can simply select the query to be executed from the list of queries. 

Access to data can be defined via API and download or via public download. In this case, a download link and a UUID (Universally Unique Identifier) are needed. Queries can be read-only, that is, the mere access the available data, or write access can be enabled, which additionally allows to modify the data contained in the database. 

Managed queries can be created, edited, and deleted, as well as organized in categories, see [Manage the query categories](./02_ManageQueryCategories.md). Query access can also be restricted pro query and query category depending on the user role, see [Manage the user rights](./05_ManageUserRights.md).


## Create a query

Define a query, determine how the data are accessed and, if necessary, restrict access to data.

#### Prerequisites 

No prerequisites to fulfill.

#### Procedure

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")


1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.  
    The *Create MySQL query* is displayed.

2. Enter a name in the *Name* field.

3. If desired, click the *Category* drop-down list and select teh applicable category. All available query categories are displayed in the list. 
    > [Info] The query category can be assigned when creating the query or afterwards. To create a query category, see [Create a query category](01_ManageQueries.md#create-a-query-category).  

4. Enter the MySQL query.

5. If desired, enter one or several IP addresses or an IP range (subnet mask) in the *IP whitelist (only public download)* field to restrict access to those IP addresses entered in case of public download.  
    > [Info] When entering more than one IP address, each IP address must be entered on a separate line. 

[comment]: <> (ETL use enabled vorest ignorieren, laut JS)

6. Select the *API and download enabled* checkbox to allow logged in users with the appropriate rights to execute the query and export the extracted data.
    > [Info] The user rights must be granted for every single query, see [Manage the user rights](./05_ManageUserRights.md).

[comment]: <> (Evtl. Link updaten, wenn relevanter Unterkapitel definiert wird)

7. Select the *Public download enabled* checkbox to allow any user, also non-logged in users, with the appropriate link to execute the query and export the extracted data in a browser. 
    > [Info] To be able to execute the query in the browser, the corresponding download link and UUID (Universally Unique Identifier) must be known.

8. Select the *Write access enabled* checkbox to allow write operations when executing the query. Otherwise, the query is not executed and an error message is displayed.

9. If desired, click the [TRY QUERY (READ ONLY)] button to test the query.  
  The query results are displayed in table format at the bottom of the workspace.

10. Click the [SAVE] button.  
  The query has been saved. The *Create MySQL query* is closed.


## Edit a query

Edit a query to change any previously set values or add an operation.

#### Prerequisites 

A query has been created, see [Create a query](#create-a-query).

#### Procedure

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")


1. Click the query to be edited in the list of queries. Alternatively, select the checkbox of the query to be edited and click the ![Edit](../../Assets/Icons/Edit01.png) (Edit) button in the editing toolbar.  
    The *Edit MySQL query* is displayed.

2. Modify the query set values as necessary.
    > [Info] The fields *ID* and *UUID* are automatically assigned by the system and cannot be modified.

3. If desired, click the [TRY QUERY (READ ONLY)] button to test the query.  
  The query results are displayed in table format at the bottom of the workspace.

4. Click the [SAVE] button.  
  The changes have been saved. The *Create MySQL query* is closed. 


## Delete a query

Delete a query that is no longer needed. It is possible to several queries at once.  

#### Prerequisites 

A query has been created, see [Create a query](#create-a-query).

#### Procedure

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")


1. Click the query to be deleted in the list of queries. Alternatively, select the checkbox of the query to be deleted and click the ![Delete](../../Assets/Icons/Trash03.png) (Delete) button in the editing toolbar.  
    The *Deleted queries xxxx* window is displayed. The number indicates the identifier of the deleted query as displayed in the *ID* column. The deleted query is removed from the list of queries. 



## Restrict access to a query (public download)

[comment]: <> (Vielleicht nicht nötig, s. Create a query. Evtl. löschen)

#### Prerequisites 

#### Procedure

