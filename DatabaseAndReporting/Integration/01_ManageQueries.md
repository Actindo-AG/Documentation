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

3. If desired, click the *Category* drop-down list and select a category.   
    > [Info] The query categories must be previously created, see [Create a query category](01_ManageQueries.md#create-a-query-category).  

4. Enter the MySQL query.

5. If desired, enter a single or several IP addresses or an IP range (subnet) to limit access to data in case of public download in the *IP whitelist (only public download)* field.  
    > [Info] When entering more than one IP address, each IP address must be entered on separate lines. For an IP range configuration, see ...  

[comment]: <> (ETL use enabled vorest ignorieren, laut JS)

6. Select the *API and download enabled* checkbox to enable access via API and download.

7. Select the *Public download enabled* checkbox to enable access via public download.

8. Select the *Write access enabled* checkbox to enable write access...

[comment]: <> (Mehr info)

9. If desired, click the [TRY QUERY (READ ONLY)] button to execute the query.  
  The query result is displayed in a table.

10. Click the [SAVE] button.  
  The query has been saved. The *Create MySQL query* is closed.


## Edit a query

#### Prerequisites 

#### Procedure


## Delete a query

#### Prerequisites 

#### Procedure



## Restrict access to a query (public download)

#### Prerequisites 

#### Procedure

