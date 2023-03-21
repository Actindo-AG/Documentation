[!!User interface Interactive console](../UserInterface/04a_InteractiveConsole.md)
[!!Manage user rights](../Integration/05_ManageUserRights.md)

# Execute queries in MySQL console

MySQL console allows the user to query any data contained in your *Actindo Core1 Platform*. The queries must be performed using SQL commands, and therefore SQL knowledge is required. 

All data available in the system can be accessed, retrieved and modified using MySQL interactive console. For this reason, MySQL interactive console must be handle with extreme caution, and access rights should only be granted to personnel with the appropriate role and skills. For detailed information about managing user rights, see [Manage user rights](../Integration/05_ManageUserRights.md).


## Access and retrieve data

Access and retrieve any data contained in your system's databases using the interactive console. The data displayed in the console is read-only.

#### Prerequisites

The user has been granted the applicable access rights, see [Grant access rights to a user group](../Integration/05_ManageUserRights.md#grant-access-rights-to-a-user-group).

#### Procedure

*Database and reporting > MySQL console > Tab INTERACTIVE CONSOLE*

![Interactive console](../../Assets/Screenshots/DatabaseAndReporting/MySQLConsole/InteractiveConsole.png "[Interactive console]")

1. Enter a valid SQL statement, for example **SELECT name FROM datahub_attributes;** to retrieve all attribute names contained in the *datahub_attributes* table. 
    > [Info] SQL knowledge is required to perform the queries. For detailed informationL, see [SQL Tutorial](https://www.w3schools.com/sql/default.asp).
    
2. Press the **ENTER** key.  
    The query results are displayed in the interactive console.    

    ![Query results](../../Assets/Screenshots/DatabaseAndReporting/MySQLConsole/QueryResultsReadOnly.png "[Query results]")


## Edit data

Data contained in your system's database can also be modified using the interactive console, for instance, a record can be inserted, updated or even deleted.

> [Caution] **Potential loss of data**   
  Editing has the potential to cause loss of data due to overwrite or deletion. The overwrite or deletion cannot be undone and the overwritten or deleted data cannot be restored.    
  Check all your entries before proceeding. 

#### Prerequisites

The user has been granted the applicable access rights, see [Grant access rights to a user group](../Integration/05_ManageUserRights.md#grant-access-rights-to-a-user-group).

#### Procedure

*Database and reporting > MySQL console > Tab INTERACTIVE CONSOLE*

![Interactive console](../../Assets/Screenshots/DatabaseAndReporting/MySQLConsole/InteractiveConsole.png "[Interactive console]")

1. Enable the *Write access* toggle in the upper left corner.  
    A warning message with the following notice is displayed:   
    *Write access is now enabled. All queries are logged, and Actindo is not liable for any loss of data or impairment of the account's functionality resulting from use of this module*. 

    ![Warning write access](../../Assets/Screenshots/DatabaseAndReporting/MySQLConsole/Warning.png "[Warning write access]")

2. Click the [OK] button to proceed.   
    The text in the interactive console turns red. Write access is enabled. 

    ![Interactive console with write access](../../Assets/Screenshots/DatabaseAndReporting/MySQLConsole/InteractiveConsoleWriteAccess.png "[Interactive console with write access]")

3. Enter a valid SQL statement, for example **INSERT INTO table_name (column1, column2) VALUES (value1, value2)** to edit the selected data accordingly. 

    > [Caution] **Potential loss of data**   
  Editing has the potential to cause loss of data due to overwrite or deletion. The overwrite or deletion cannot be undone and the overwritten or deleted data cannot be restored.    
  Check all your entries before proceeding. 

4. Press the **ENTER** key.  
    The data has been modified.   

    ![Query results](../../Assets/Screenshots/DatabaseAndReporting/MySQLConsole/QueryResults.png "[Query results]")

[comment]: <> (Screenshots with write access ziehen lassen?)

