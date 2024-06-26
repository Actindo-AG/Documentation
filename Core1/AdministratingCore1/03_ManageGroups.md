# Manage user groups

User groups define the individual permissions that a user assigned to this group has in the *Actindo Core1 Platform*. 
In contrast to the users, user groups are not global. Group rights are valid for the current instance only. This means that they are not shared between the main account and the sandboxes.   

**Manage user rights** 

User rights are defined by assigning the user to a (user) group. Groups define specific roles that a user has when working on the *Actindo Core1 Platform*.   
For example, a bookkeeper needs access to specific functions of the *Accounting* module in addition to general rights for accessing the *Actindo Core1 Platform*. Additionally, rights to access other modules might be required. For this reason, you can create a specific group for the bookkeeper's role in which you can collect all rights the bookkeepers need. 

> [Info] The standard role "ActindoUsersGroup" is available to grant general access rights for the *Actindo Core1 Platform* needed by all users.

The user rights are individually managed for the main account and each sandbox, in which the users do their daily work. In the *Settings* module, you assign the user rights for all modules and plugins installed on the *Actindo Core1 Platform*. You can create, edit, and delete user groups, add specific users to a group, remove users from a group, and assign rights.    

> [Info] When assigning the rights, it is very important to know that sandboxes share the licenses with the main account. This means, that if you have five licenses for the *Accounting* module, and two bookkeepers who work in the main account, you have three licenses left for the sandboxes. This is especially relevant when using the *Actindo* admin group, see below.

**Actindo admin group**   

A special group is the "ActindoAdminGroup". This group has automatically all rights for everything, and you cannot maintain specific rights for it.   
Regarding the licenses, keep in mind, that each Administrator has automatically access to all modules, which means that a license for each module and admin user is counted.

**Users from Actindo AG**   

*Actindo AG* employees such as developers or consultants do not consume licenses, they are not counted.

## Create user group

Create a user group based on a user role to subsequently assign them a specific set of user rights.

#### Prerequisites

You have permission to edit, save, and list groups.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupCreated.png "[Group management]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create group* window is displayed.

    ![Create group](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupCreate.png "[Create group]")

2. Enter a name for the group in the *Group name* field.

3. Click the [SAVE] button.   
    A confirmation message is displayed. The newly created group is displayed in the list of groups.

    ![Group created](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupCreated.png "[Group created]")
 


## Add user to user group

Add any number of users to a user group to assign them rights subsequently.

#### Prerequisites

A user group has been created, see [Create user group](#create-user-group).

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupCreated.png "[Group management]")

1. Select the checkbox of the user group for which you want to add a user.   
    The editing toolbar is displayed.

2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button in the editing toolbar.       
    The *Edit group "Group name"* view is displayed. By default, the *Users* tab is preselected.

    > [Info] If no users have been added yet, the *No users added. Use + button to add one to group* notice is displayed. Otherwise, the details of the user(s) included in the group are displayed.   
    
     ![Edit group no users](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupEditNoUsers.png "[Edit group no users]")


3. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Add user* window is displayed.

    ![Add user](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupAddUser.png "[Add user]")

4. Click the *Add user* drop-down list and select the desired user.   
    The selected user has been added to the group. Per default, the validity period is set from today to the system end date. 

    ![Add user](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupAddUserValidity.png "[Add user]")

     1. Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button and select the validity start date in the *Valid from* field.  

     2. Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button and select the validity end date in the *End date* field.    
        > [Info] It is not possible to change the validity period later. If you want to delimit the validity period, you must remove the group assignment and assign the user again with a different validity period.

5. To add further users, click the ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add) button below the *Add user* drop-down list.   
    A further drop-down list is displayed. Repeat steps **4** and **5** to add as many users as necessary.

6. Click the [SAVE] button in the upper right corner of the *Add user* window.  
    The users have been saved to the group and are displayed in the list of users.

7. Click the [SAVE] button in the upper right corner of the *Edit group* window.   
    A confirmation message is displayed. The changes to the group have been saved.



## Remove user from a group via the group management

A user is active in an account as long as s/he is assigned to a user group.    
If you want to remove a user from a sandbox, you must remove the user from all groups to which s/he is assigned. There are the following limitations:
- You cannot remove a user from the *ActindoAdminGroup* in a sandbox of which s/he is the owner. 
- You cannot remove a user from all groups in an account in which the user has been created. In this case, you have to inactivate him/her, see [Edit user](./02_ManageUsers.md#edit-user).   

Note that it is not possible to remove a group assignment by delimiting the validity end date to a specific date. If you want to change the validity period, you must remove the group assignment and create a new one with a limited validity end date.

#### Prerequisites

You have permission to remove the user assignment from a group.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupManagment.png "[Group management]")

1. Select the group from which you want to remove a user.   
    The editing toolbar is displayed.

   ![Group selected](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupSelected.png "[Group selected]")

2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button.
    The *Edit group "Group name"* view is opened. By default, the *Users* tab is displayed. 

   ![Group users](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupManagementUsers.png "[Group users]")

3. Select a user.   
    The editing toolbar is displayed.

   ![User selected](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupUserSelected.png "[User selected]")

4. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button.   
    The selected user is removed from the list.

5. Click the [SAVE] button.   
    The changes have been saved. The *GROUP MANAGEMENT* view is displayed again.


## Delete user group

If a user group is no longer needed, you can delete it. Note that it is possible to delete groups regardless of whether users are still assigned.

#### Prerequisites

You have permission to delete groups.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupManagment.png "[Group management]")

1. Check whether users are assigned to the group. To do this, select the checkbox of the user group you want to delete.   
    The editing toolbar is displayed.

    ![Group selected](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupSelected.png "[Group selected]")

2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button.
    The *Edit group "Group name"* view is displayed.  

    ![Edit group](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupEditNoUsers.png "[Edit group]")

3. Check whether users are assigned to the group. If necessary, remove the assignment, see [Remove user from a group via the group management](#remove-user-from-a-group-via-the-group-management) and assign the user a different group that may be equivalent. 

4. Return to the *GROUP MANAGEMENT* tab by clicking the ![BACK](../../Assets/Icons/Back02.png "[BACK]")(Back) button.

5. Select the checkbox of the user group you want to remove.   
    The editing toolbar is displayed.

   ![Group selected](../../Assets/Screenshots/Core1Platform/AdministratingCore1/GroupSelected.png "[Group selected]")

2. Click the ![Delete](../../Assets/Icons/Trash03.png "[Delete]") (Delete) button.  
    The *Group was deleted* pop-up window is displayed. 


