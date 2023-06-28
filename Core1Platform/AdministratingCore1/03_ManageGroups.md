# Manage user groups

Create admin group ->  Genau überlegen, da Admins alle Rechte haben und daher Lizenzen verbrauchen

Note that user groups in opposite to the users are not global. Group rights are valid for the current instance only. This means that they are not shared between the main account and the sandboxes. 
If you add a user to a group, the user is automatically listed for this account. If you want to remove a user from an account, you need to remove the user from all groups.



# Manage the user rights

Manage the user rights to allow a user or a group of users to access specific data. User rights can be individually granted or denied pro query and pro query category to a user group based on their user role. 



[comment]: <> (Stimmt das so? Check andere Folders mit Julian: InfluxDB, Interactive MySQL console.)

The user rights are managed centrally for all modules and plugins installed in the Core1 in the *Settings* module. You can create, edit and delete user groups, add specific users to a group, remove users from the a group, and assign rights to a user group.


## Create a user group

Create a user group based on a user role in order to subsequently assign them a specific set of user rights.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/DatabaseAndReporting/GroupManagement.png "[Group management]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create group* window is displayed.

    ![Create group](../../Assets/Screenshots/DatabaseAndReporting/CreateGroup.png "[Create group]")

2. Enter a name for the group in the *Group name* field.

3. Click the [SAVE] button.   
    The *Group saved* pop-up window is displayed.
    
    ![Group saved](../../Assets/Screenshots/DatabaseAndReporting/GroupSaved.png "[Group saved]")

    The newly created group is displayed in the list of groups.

    ![Group created](../../Assets/Screenshots/DatabaseAndReporting/GroupCreated.png "[Group created]")
 

## Edit a user group

Edit a user group to add users to it, remove users from it and assign rights to the users included in it. 

### Add a user to a user group

Add any number of users to a user group ir order to assign them rights subsequently.

#### Prerequisites


- A user group has been created, see [Create a user group](#create-a-user-group).

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/DatabaseAndReporting/GroupCreated.png "[Group management]")

1. Select the checkbox of the user group to which you want to add users.   
    The editing toolbar is displayed.

2. Click the ![Edit](../../Assets/Icons/Edit01.png "[Edit]") (Edit) button in the editing toolbar.    
    The *Edit group* view is displayed. By default, the *Users* tab is preselected.

    > [Info] If no users have been added yet, the *No users added. Use + button to add one to group* notice is displayed. Otherwise, the details of the user(s) included in the group are displayed.

    ![Edit group no users](../../Assets/Screenshots/DatabaseAndReporting/EditGroupNoUsers.png "[Edit group no users]")

3. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Add user* view is displayed.

    ![Add user](../../Assets/Screenshots/DatabaseAndReporting/AddUser.png "[Add user]")

4. Click the *Add user* drop-down list and select the desired user.   
    The selected user has been added to the group.

5. If desired, click the ![Add](../../Assets/Icons/Plus05.png "[Add]") (Add) button below the *Add user* drop-down list to add an additional user.   
    An additional drop-down list is displayed. Repeat steps **4** and **5** to add as many users as necessary.

6. Click the ![Add](../../Assets/Icons/Plus05.png "[Add]")  (Calendar) button and select the validity start date in the *Valid from* field.  

7. Click the ![Add](../../Assets/Icons/Plus05.png "[Add]")  (Calendar) button and select the validity end date in the *End date* field.

8. Click the [SAVE] button in the upper right corner of the *Add user* window.  
    The user has been saved to the group and is displayed in the list of users.

9. Click the [SAVE] button in the upper right corner of the *Edit group* view.   
    The *Group saved* pop-up window is displayed. The changes to the group have been saved.

    ![Group saved](../../Assets/Screenshots/DatabaseAndReporting/GroupSaved.png "[Group saved]")


### Remove a user from a user group

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/DatabaseAndReporting/GroupCreated.png "[Group management]")

### Assign rights to a user group

- Execute query via API 
- Queries 
- Query categories 
- InfluxDB 
- Interactive MySQL console 

## Delete a user group

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Settings > Users and groups > Tab GROUP MANAGEMENT*

![Group management](../../Assets/Screenshots/DatabaseAndReporting/GroupManagement.png "[Group management]")
