[!!User interface Queries](../UserInterface/01a_Queries.md)
[!!Execute the managed queries](../Operation/01_ExecuteManagedQueries.md)
[!!Manage the query categories](./02_ManageQueryCategories.md)
[!!Manage the user rights](./05_ManageUserRights.md)

# Manage the queries

Queries can be predefined to determine the data that may be accessed by specific user groups. Instead of entering and executing a query directly in MySQL console, the user can simply select the query to be executed from the list of queries. 

Data can be accessed via API and download, that is, users must be logged in the Core1, or via public download in a web browser. In the case of public download, a download link and a UUID (Universally Unique Identifier) are required. Queries can be read-only, that is, the mere access and retrieval of available data, or write access can be enabled, which additionally allows to modify the data contained in the database. 

Managed queries can be created, edited, and deleted, as well as organized in categories, see [Manage the query categories](./02_ManageQueryCategories.md). Query access can also be restricted or granted pro query based on the user group, see 
[Grant access rights to a user group](./05_ManageUserRights.md#grant-access-rights-to-a-user-group).

## Create a query

Define a query, determine how the data may be accessed and by whom, allow write operations, and, if necessary, insert placeholders to represent any desired variables. The queries must be written in SQL syntax, and therefore SQL knowledge is required. 

#### Prerequisites 

No prerequisites to fulfill.

#### Procedure

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")


1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.  
    The *Create MySQL query* is displayed.

    ![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/CreateQuery.png "[Queries]")

2. Enter a name in the *Name* field.

3. If desired, click the *Category* drop-down list and select the applicable category. All available query categories are displayed in the list. 
    > [Info] The query category can be assigned while creating the query or later on, after the query has been created. To create a query category, see [Create a query category](./02_ManageQueryCategories.md#create-a-query-category).  

4. Enter a valid MySQL query.  
    
5. If desired, insert a placeholder to your query to represent any variables to be specified when executing a query.  
    Placeholders are most often used in the SET, VALUES, and WHERE clauses, as in the example provided below where a time condition is defined: 
      
    - Enter a condition (WHERE clause) in the query followed by a placeholder, for example **WHERE created > \~creationDate|datetime\~**.
        > [Info] Placeholders can be named freely. It is recommended to use a descriptive name, as this description is displayed later on as a field name.
        
    - If desired, click the [TRY QUERY (READ ONLY)] button to test it.   
        The *Bind query parameters placeholders* window is displayed.
        > [Info] There are two possible placeholders to define time conditions: **|datetime** and **|string**. The **|datetime** placeholder generates a calendar button in the *Bind query parameters placeholders* window, whereas the **|string** placeholder creates a free text field.

        ![Bind query parameters placeholders](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/BindQueryParamsPlaceholders.png "[Bind query parameters placeholders]")

    - Define the desired time criteria in the *creationDate* field, either by entering the date with the keyboard or by clicking the calendar button to select the desired date and time. 

    - Click the [EXECUTE] button.   
        The query results are displayed in table format at the bottom of the workspace. 

[comment]: <> (ETL use enabled muss noch ausgeblendet werden, laut JS)

6. If desired, enter one or several IP addresses or an IP range (subnet mask) in the *IP whitelist (only public download)* field to allow access only to those IP addresses entered in case of public download.  
    > [Info] When entering more than one IP address, each IP address must be entered on a separate line. Bear in mind that if no IP address is whitelisted, any person with the link, from any IP address, can access the query results via public download. If at least one IP address is whitelisted, all other IP addresses are blacklisted. 

7. Select the *API and download enabled* checkbox to allow logged in users with the appropriate rights to execute the query and download the retrieved data.
    > [Info] Additionally, user access rights must be granted for every single predefined query, see [Grant access rights to a user group](./05_ManageUserRights.md#grant-access-rights-to-a-user-group).

8. Select the *Public download enabled* checkbox to allow any user, also non-logged in users, with the applicable link to execute the query and download the retrieved data via web browser. 
    > [Info] A specific download link, containing a UUID (Universally Unique Identifier), is required to execute the query in a web browser.

9. Select the *Write access enabled* checkbox to allow write operations when executing the query. Otherwise, a query with write operations, such as INSERT or DELETE, will not be executed and an error message will be displayed.

10. If desired, click the [TRY QUERY (READ ONLY)] button to test the query.  
    The query results are displayed in table format at the bottom of the workspace.

11. Click the [SAVE] button.  
   The query has been saved. The *Create MySQL query* is closed. The new query is displayed in the list of queries.


## Edit a query

After you have a created a query, it can be edited to change any previously set values. The fields *ID* and *UUID*, however, are automatically assigned by the system and cannot be modified.

#### Prerequisites 

A query has been created, see [Create a query](#create-a-query).

#### Procedure

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")


1. Click the query to be edited in the list of queries. Alternatively, select the checkbox of the query to be edited and click the ![Edit](../../Assets/Icons/Edit01.png) (Edit) button in the editing toolbar.  
    The *Edit MySQL query* view is displayed.

    ![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/EditQuery.png "[Queries]")

2. Edit the query set values as necessary in the corresponding fields and checkboxes.
    
3. If desired, click the [TRY QUERY (READ ONLY)] button to test the query.  
  The query results are displayed in table format at the bottom of the workspace.

4. Click the [SAVE] button.  
  The changes have been saved. The *Edit MySQL query* is closed. 


## Delete a query

Delete a query that is no longer needed. It is possible to delete several queries at once.  

#### Prerequisites 

At last a query has been created, see [Create a query](#create-a-query).

#### Procedure

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")


1. Select the checkbox of the query to be deleted.   
    The editing toolbar is displayed.

2. Click the ![Delete](../../Assets/Icons/Trash03.png) (Delete) button in the editing toolbar.  
    The *Deleted queries xxxx* window is displayed. The number indicates the identifier of the deleted query as displayed in the *ID* column. The deleted query is removed from the list of queries. 

    ![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/DeletedQueries.png "[Queries]")


