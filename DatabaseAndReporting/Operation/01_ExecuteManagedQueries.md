[!!User interface Managed queries](../UserInterface/01_ManagedQueries.md)
[!!Manage the queries](../Integration/01_ManageQueries.md)
[!!Manage the user rights](../Integration/05_ManageUserRights.md)


# Execute the managed queries

Once the queries have been predefined, they can be executed. When executing a query, the query results can be provided in CSV or XML format, either as a download file or as a preview.

Depending on the options that have been enabled in the query, a query can be executed via API or via download link. Besides, the managed queries may only be executed by users who have been granted the applicable access rights. For detailed information, see [Manage the user rights](../Integration/05_ManageUserRights.md). 


## Execute a query via API 

Execute a predefined query to access the available data in your Core1 account. To execute a query via API, the user must be logged in. The query results may be previewed in your browser in XML format or may be downloaded in a CSV or a XML file. 

### Preview the query results

Execute the query and preview the results in your browser in XML format.

#### Prerequisites

- A predefined query has been created, see [Create a query](../Integration/01_ManageQueries.md#create-a-query).
- The API and download option has been enabled. 
- The user has been granted the applicable access rights, see [Manage the user rights](../Integration/05_ManageUserRights.md).

#### Procedure

*Database and reporting > Managed queries > Queries*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")

1. Select the checkbox of the query you want to execute.  
    The editing toolbar is displayed.

2. If necessary, click the file format drop-down list in the editing toolbar and select the **XML** option. 

3. Click the ![Preview](../../Assets/Icons/Eye02.png "[Preview]") (Preview) button in the editing toolbar.  
    The *Execute saved query* is displayed.  

    ![Execute saved query](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/ExecuteSavedQuery.png "[Execute saved query]")

4. Click the [EXECUTE] button.   
    The query is executed. The query results are displayed in the new browser window.

    ![Query results](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/QueryResultsPreview.png "[Query results]")

[comment]: <> (Screenshot mit Query results?)

[comment]: <> (Preview as CSV: By default, a file containing the query results is downloaded and saved in the downloads folder of your device. Oder gibt es preview as CSV? Bei mir klappt es nicht.)


### Download the query results

Execute the query and download the results in an XML or CSV format file.

[comment]: <> (Download nur möglich als CSV?)

#### Prerequisites

- A predefined query has been created, see [Create a query](../Integration/01_ManageQueries.md#create-a-query).
- The API and download option has been enabled. 
- The user has been granted the applicable access rights, see [Manage the user rights](../Integration/05_ManageUserRights.md).

#### Procedure

*Database and reporting > Managed queries > Queries*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")

1. Select the checkbox of the query you want to execute.  
    The editing toolbar is displayed.

2. Click the file format drop-down list in the editing toolbar and select the desired option. The following options are available:
    - **CSV**  
        The query results are downloaded as a CSV (comma-separated values) file. CSV files can be visualized with most spreadsheet programs and text editors.   
    - **XML**  
        The query results are downloaded as an XML file. XML files can be visualized using most web browsers and text editors.

3. Click the ![Download](../../Assets/Icons/Download.png "[Download]") (Download) button in the editing toolbar.  
    The *Execute saved query* is displayed.  

    ![Execute saved query](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/ExecuteSavedQuery.png "[Execute saved query]")

4. Click the [EXECUTE] button.   
    The query is executed. The query results are downloaded in an XML or CSV format file. By default, the file is saved in the downloads folder of your device. 


## Execute a query via download link 

Execute a query in a web browser using the download link provided in the Core1. To execute the query via public download, the query download link and the UUID (Universally Unique Identifier) are required.

#### Prerequisites

- A predefined query has been created, see [Create a query](../Integration/01_ManageQueries.md#create-a-query).
- The public download option has been enabled. 
- The user has been granted the applicable access rights, see [Manage the user rights](../Integration/05_ManageUserRights.md).

#### Procedure

*Database and reporting > Managed queries > Queries*

![Queries](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/Queries/Queries.png "[Queries]")

1. Select the checkbox of the query you want to execute.  
    The editing toolbar is displayed.

2. Click the [COPY DOWNLOAD LINK] button in the editing toolbar.  
    The query download link is copied to your clipboard.

    > [Info] The download link contains the query URL and the required UUID (Universally Unique Identifier), which is automatically assigned when creating a query.

3. Click the [ENTER] key to execute the query via public download.  
    The query is executed. The query results are downloaded in a CSV format file. By default, the file is saved in the downloads folder of your device.  

[comment]: <> (Ist es möglich, als XML zu herunterladen via download link?)