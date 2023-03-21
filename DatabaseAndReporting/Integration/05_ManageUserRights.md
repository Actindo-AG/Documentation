[!!Manage the queries](./01_ManageQueries.md)
[!!Manage the query categories](./02_ManageQueryCategories.md)

# Manage the user rights

The user rights for all modules and plugins installed in the Core1 are managed centrally in the *Settings* module. For detailed information on managing the user rights, see the *Settings* module documentation.

[comment]: <> (Link hinzufügen, wenn verfügbar)

## Grant access rights to a user group

Assign user access rights to control access to specific data. The following access rights must be individually granted to a user group based on their user role:

- **Execute query via API**  
    The user can execute a managed query via API if this option has been enabled in the query.
- **Queries**   
    Depending on the access permission type granted, the user can read, create, update, delete, and execute queries. Besides, queries must be individually selected to be executed.   
- **Query categories**  
    Depending on the access permission type granted, the user can read and save query categories.
- **InfluxDB**  
    Depending on the access permission type granted, the user can create, edit, list, delete, and execute InfluxDB time series.
- **Interactive MySQL console**  
    The user can execute any query in MySQL interactive console. Bear in mind that this gives the user access, and even write access, to all available data. 

    Additionally, access rights must be granted for the individual queries. By default, all access rights are denied to users with no administrator rights.

    [comment]: <> (Stimmt das so? Check mit Julian: InfluxDB, Interactive MySQL console, Execute individual queries.)


#### Prerequisites

- A user group has been created.
- The users to be granted access have been added to the applicable user group.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/DatabaseAndReporting/GroupManagement.png "[Group management]")

1. Select the checkbox of the user group to be granted access.   
    The editing toolbar is displayed.

2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button in the editing toolbar.    
    The *Edit group "Group name"* view is displayed. By default, the *Users* tab is preselected.

    ![Edit group users](../../Assets/Screenshots/DatabaseAndReporting/EditGroupUsers.png "[Edit group users]")

3. Click the *Rights* tab.  
    All modules and plugins installed are displayed.

    > [Info] It may take some time for the system to display all installed modules and plugins.

    ![Edit group rights](../../Assets/Screenshots/DatabaseAndReporting/EditGroupRights.png "[Edit group rights]")

4. Navigate the folder tree structure on the left side until you locate the *Modules.Actindo.Database and Reporting* folder.
    
5. If necessary, click the rightwards arrow to the left of the *Modules.Actindo.Database and Reporting* folder to display all contained sub-folders.  
    All contained sub-folders are displayed.

    ![Rights DB and reporting](../../Assets/Screenshots/DatabaseAndReporting/EditGroupRightsDatabaseAndReporting.png "[Rights DB and reporting]")

6. Locate the functions you want to grant access to.

7. Click the rightwards arrow to the left of the corresponding folder (function) to display all contained sub-folders (access permission types).  
    All contained sub-folders (access permission types) are displayed.

    ![Access permission types](../../Assets/Screenshots/DatabaseAndReporting/AccessPermissionTypes.png "[Access permission types]")

8. Select the checkbox of the applicable folder(s) and/or sub-folders.  
    The user group, and all users included in it, have been granted access rights to the selected functions.
