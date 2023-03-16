[!!User interface Query categories](../UserInterface/03b_QueryCategories.md)
[!!Manage the categories](./01_ManageCategories.md)
[!!Manage the query categories](./02_ManageQueryCategories.md)

#  Queries

*Database and reporting > Managed queries > Tab QUERIES*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")

**Query categories tree**

 - ![Folders](../../Assets/Icons/Folders01.png "[Folders]") (Folders)  
    Query category that contains query sub-categories. Click the arrow *>* left to the query category to unfold it and display the query sub-categories. 

- ![Folder](../../Assets/Icons/Folder01.png "[Folder]") (Folder)  
    Query category. Click the query category to display all queries that are assigned to the selected query category in the *Queries* list.

**Queries**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a query. 

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of queries. 

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all queries in the list are selected.

- [CSV/XML]   
    Click this drop-down list to selected the desired format to visualize or download the query results. This button is only displayed if a single checkbox in the list of queries is selected. 

- ![Download](../../Assets/Icons/Download.png "[Download]") (Download)   
    Click this button to download the query results. This button is only displayed if a single checkbox in the list of queries is selected.   
    The *Execute saved query* window is displayed, see [Execute saved query](#execute-saved-query).

- ![View](../../Assets/Icons/Eye02.png "[View]") (View)   
      Click this button to visualize the query results onscreen. This button is only displayed if a single checkbox in the list of queries is selected.  
      The *Execute saved query* window is displayed, see [Execute saved query](#execute-saved-query).

- [COPY DOWNLOAD LINK]  
    Click this button to copy the download link to your clipboard. This button is only displayed if a single checkbox in the list of queries is selected and if public download has been enabled for the selected query.  

- ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit)   
    Click this button to edit a query. This button is only displayed if a single checkbox in the list of queries is selected. Alternatively, you can click directly a query in the list to edit it.
    The *Edit MySQL query* window is displayed, see [Edit MySQL query](#edit-mysql-query).

- ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete)   
    Click this button to delete a query. It is possible to delete several queries at once. This button is displayed if at least one checkbox in the list of queries is selected.       

The list displays all predefined queries. Depending on the settings, the displayed columns may vary. All fields are read-only. If no query has been created yet, the notice *No queries created. Use + button to create one* is displayed.

- *ID*  
    Query identification number. The ID number is automatically assigned by the system. 

- *Name*   
    Attribute name.

- *Query*   
    Predefined query expressed in SQL.

- *ETL use enabled*   
    Indication whether the ETS use is enabled or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The ETL use is enabled.  
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The ETL use is not enabled.
    
    > [Info] This function is not available in the current version.

[comment]: <> (Check!)

- *API and download enabled*   
    Indication whether the public download is enabled or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The API access and download is enabled.  
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The API access and download is not enabled.

- *Public download enabled*   
    Indication whether the public download is enabled or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): The public download is enabled.  
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): The public download is not enabled.

- *Write access enabled*   
    Indication whether the write operations are enabled or not:
    - ![Check](../../Assets/Icons/Check.png "[Check]") (Checkmark): Write operations are enabled.  
    - ![Cross](../../Assets/Icons/Cross02.png "[Cross]") (Cross): Write operations are not enabled.

- *UUID*   
    Universally Unique Identifier. This code is required to execute a query via web browser. 

- ![Copy](../../Assets/Icons/Copy01.png "[Copy]") (Copy)  
    Click this button to copy the UUID (Universally Unique Identifier) to your clipboard.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to create a query. The *Create MySQL query* view is displayed.   


 ## Create MySQL query

*Database and reporting > Managed queries > Tab QUERIES > Button Add*

![Create query](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/CreateQuery.png "[Create query]")

- *Name*  
    Enter a description for the query.

- *Category*  
    Click the drop-down list to assign the query to a category. All available categories are displayed in the list. 

- *Query*  
    Enter the SQL query.

- *IP whitelist (only public download)*  
    Enter the IP address(es) you want to limit access to in case of public download. It is possible to enter one or several IP addresses or an IP range (subnet mask). When entering more than one IP address, each IP address must be entered on a separate line.  

- [x] ETL use enabled
    Click the checkbox to enable ETL use. 
    > [Info] This function is not available in the current version.
    
- [x] API and download enabled
    Click the checkbox to enable API access and download.

- [x] Public download enabled
    Click the checkbox to enable public download.
   
- [x] Write access enabled
    Click the checkbox to enable write operations.
   
- [TRY QUERY] (READ ONLY)   
    Click this button to try the defined query. The *Try query result* box is displayed.

- [CANCEL]  
    Click this button to cancel creating the query. The *Create MySQL query* view is closed.

- [SAVE]  
    Click this button to save the query. The *Create MySQL query* view is closed.


## Edit MySQL query

*Database and reporting > Managed queries > Tab QUERIES > Select query*
*Database and reporting > Managed queries > Tab QUERIES > Select query checkbox > Button Edit*

![Edit query](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/EditQuery.png "[Edit query]")


- *ID*  
    Query identification number. The identification number is automatically assigned by the system when the query is created and cannot be edited.

- *UUID*
    Universally Unique Identifier. The UUID is automatically assigned by the system when the query is created and cannot be edited.

- *Name*  
    Edit the description for the query.

- *Category*  
    Click the drop-down list to assign the query to a category. All available categories are displayed in the list. 

- *Query*  
    Edit the SQL query.

- *IP whitelist (only public download)*  
    Enter the IP address(es) you want to limit access to in case of public download. It is possible to enter one or several IP addresses or an IP range (subnet mask). When entering more than one IP address, each IP address must be entered on a separate line.  

- [x] ETL use enabled
    Click the checkbox to enable/disable ETL use. 
    > [Info] This function is not available in the current version.
    
- [x] API and download enabled
    Click the checkbox to enable/disable API access and download.

- [x] Public download enabled
    Click the checkbox to enable/disable public download.
   
- [x] Write access enabled
    Click the checkbox to enable/disable write operations.
   
- [TRY QUERY] (READ ONLY)   
    Click this button to try the edited query. The *Try query result* box is displayed.

- [CANCEL]  
    Click this button to cancel editing the query. The *Edit MySQL query* view is closed.

- [SAVE]  
    Click this button to save any changes made. The *Edit MySQL query* view is closed.


## Execute saved query

*Database and reporting > Managed queries > Tab QUERIES > Select query checkbox > Button View*
*Database and reporting > Managed queries > Tab QUERIES > Select query checkbox > Button Download*

![Edit query](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/EditQuery.png "[Edit query]")




## Bind query parameters placeholders

*Database and reporting > Managed queries > Tab QUERIES > Select query checkbox > Button View*
*Database and reporting > Managed queries > Tab QUERIES > Select query checkbox > Button Download*

![Bind query parameters placeholders](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/BindQueryParamsPlaceholdersFreetext.png "[Bind query parameters placeholders]")

> [Info] This window is only displayed when the query selected contains placeholders to be bound before executing it. 
