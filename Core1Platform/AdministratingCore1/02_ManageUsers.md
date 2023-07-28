# Manage users

A user is a global *Actindo* entity that is shared between the main account and the sandboxes. If you create a user in the main account, and you invite this user to a sandbox, the user dates are automatically available in this sandbox. If you change user data, the data are synchronized with the sandboxes in which the user is assigned a user group.   
You must create users in the main account. It is not possible to create users in a sandbox.   
> [INFO] As a user without admin rights, you can change some data too. For detailed information, see [Edit profile settings](../UsingCore1/02_EditProfileSettings.md "Edit profile settings"). 



## Create user
Users are created in the main account only.

#### Prerequisites

- You are logged in to a main account
- You are granted to create users.

#### Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The screen is grayed out. A small menu is opened in the bottom right corner.

   ![User management menu](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserAdd.png "[User management menu]")

2. Click the ![Create user](../../Assets/Icons/Edit02.png "[Create user]") (Create user) button.   
  The *Create user* window is opened.    
    
    ![Create user](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserCreate.png "[Create user]")

3. Click the *Select active option* drop-down list to select whether the new user will be able to log in or not. The following options are available: 
    - **Active, can log in**
    - **Inactive, user is locked**

4. Click the *Password type* drop-down list to select how the password is to be created and submitted to the user. The following options are available:
    - **Generate password and send via email**  
      A password is generated automatically, and it is sent by Actindo to the email address specified below. 
    - **Enter password and send by email**    
      You define an individual password, and it is sent by Actindo to the email address specified below. 
    - **Specify and save password**   
      You define an individual password and save it. It is not sent via email. 
    -**Do not send password**   
      Use this option if you want to change the user's data but you do not want to edit the password to be sent. 

5. If you have not selected the *Generate password and send via email* option in the *Password type option* drop-down list, define the password in the *Set password* field.

6. Enter the username in the *Login* field. This is the name with which the user must log in.  

7. Enter the name and address of the user. Use the *Address* field to enter street and house number.

8. Enter the email address of the new user.   
  After you have saved the new user, it will be used to send the password to the user.

9. If desired, click the *Role in company* drop-down list. The following options are available:
    - Entwicklung (Development)
    - Buchhaltung (Accounting)
    - Logistik (Logistics)
    - Artikelanlage (Creating products)
    - Einkauf (Procurement)
    - Marktplätze (Market places)
    - Anderes (Others)

10. Click the [SAVE] button.   
  The new user is created and, if applicable, informed about username and password by email. 
  


## Assign user to user group

Assigning users to a user group is necessary to activate a user on a current instance. A user that is not assigned any group, is not active in the instance. This means in reverse, you must remove a user from all groups on an instance to deactivate him or her.

## Prerequisite

- You are granted to assign users to groups.
- The user groups are already created. For detailed information, see [Create user group](../AdministratingCore1/03_ManageGroups.md#create-user-group "Create user group").

## Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

1. Click the user you want to assign a group.   
  The *Edit user "username"* view is displayed. By default, the *Profile* tab is preselected. 

2. Click the *Groups* tab.   
  The groups the user is assigned are listed.

   ![Groups](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserGroups.png "[Groups]")  

3. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Add Group* window is displayed.

    ![Add group](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserAddGroup.png "[Add user]")   

4. Click the *Select group* drop-down list and select the desired group.

5. Click the ![Calendar](../../Assets/Icons/Calendar.png "[Add]") (Calendar) button and select the validity start date in the *Valid from* field.  

6. Click the ![Calendar](../../Assets/Icons/Calendar.png "[Calendar]") (Calendar) button and select the validity end date in the *End date* field.   
   > [INFO] It is not possible to change the validity period later. If you want to delimit the validity period, you must remove the group assignment and assign the user again with a different validity period.

7. Click the [SAVE] button.   
  The *Profile* tab is displayed. The new assigned group is added to the list of groups.



## Edit user

Users are edited in the main account only. There is one exception: Users are able to change their personal data on a sandbox (see [Edit profile settings](../UsingCore1/02_EditProfileSettings.md "Edit profile settings")).

#### Prerequisites

- You are logged in to a main account
- You are granted to edit users.


#### Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

1. Select the user whose data you want to edit.   
  The *Edit user "username"* view is opened. By default, the *Profile* tab is preselected. 

   ![User management](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserEdit.png "[User management]")

2. If desired. Click the *Select active option* drop-down list to select whether the user can log in or not. The following options are available: 
    - **Active, can log in**
    - **Inactive, user is locked**

3. If desired, click the *Password type* drop-down list to select how the password is to be created and submitted to the user. This password is valid for the main account and is sandboxes. The following options are available:
    - **Generate password and send via email**  
      A password is generated automatically, and it is sent by Actindo to the email address specified below. 
    - **Enter password and send by email**    
      You define an individual password, and it is sent by Actindo to the email address specified below. 
    - **Specify and save password**   
      You define an individual password and save it. It is not sent via email.   
    - **Do not send password**   
      Use this option if you want to change the user's data, but you do not want to change the password resp. the password to be sent. 

4. If desired, disable the *Universal Second Factor (U2F)* toggle.
  If the *Universal Second Factor (U2F)* is disabled, the user will no longer need to use the *Yubikey* to log in. 

5. If desired, edit the user's personal data.

6. Click the [SAVE] button.   

7. If desired, change the group assignment of the user. For detailed information, see [Assign user to user group](#assign-user-to-user-group "Assign user to user group").



## Remove user from a group

When editing a user, you can remove a user from a group to which he or she is assigned.  
Alternatively, you can remove a user from a group during editing the groups, see [Remove users from a group via the group management](../AdministratingCore1/03_ManageGroups.md#remove-users-from-a-group-via-the-group-management "Remove users from a group via the group management").

#### Prerequisites

- You are logged in to a main account or a sandbox
- You are granted to remover users from groups.

#### Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

1. Click the user you want to remove from a group.   
  The *Edit user "username"* view is displayed. By default, the *Profile* tab is preselected. 

2. Click the *Groups* tab.   
  The groups the user is assigned are listed.

   ![Groups](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserGroups.png "[Groups]")  

3. Select the group from which you want to remove the user.   
  The toolbar is displayed.

   ![Select group](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserSelectGroup.png "[Select group]")

4. Click the ![Delete](../../Assets/Icons/Trash03.png  "[Delete]") (Delete) button.   
  The user is removed from the selected group.<!--Julian, gibt es da noch einen Bestätigungsscreen?-->



## Invite user to sandbox

It is necessary to invite a user to a sandbox because users cannot be created there.
When inviting a user to a sandbox, it is necessary to assign the user to a user group. Only then the user is listed in this instance and can access the sandbox. <!---Julian, ist das richtig oder habe ich etwas falsch verstanden? Ist User denn schon in Sandbox, ober prüft system in main account auf Plausibility?-->

#### Prerequisites

- You are logged in to a sandbox.
- You are granted to invite users.
- The user is assigned a group. Only then the user is listed in this account and can access the sandbox.

#### Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    

    The *Workspace* is grayed out. You can cancel the action by clicking the ![Cancel ](../../Assets/Icons/Cross01.png  "[Invite user]") (Cancel) button.   

    ![Invite user](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserInvite.png "[Invite user]")


2. Click the ![Invite user](../../Assets/Icons/UserInvite02.png  "[Invite user]") (Invite user) button in the bottom right corner.   
 The *Invite user* window is opened.

    ![Invite user](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserInviteWindow.png  "[Invite user]") 

3. Enter the "Login name" of the user.

4. In the "Assigned groups" section, select a group from the "Select group" drop-down list to which you want to assign the user.   

5. If necessary, click the ![Add another group](../../Assets/Icons/Plus05.png  "[Add another group]") (Add another group) button to assign further groups.

6. Click the [SAVE] button.   
  Depending on the settings, the user gets an email that informs him or her about the invitation. The email contains a button, with which the user can open the sandbox.
 


## Remove user in sandbox

If you want to remove a user from a sandbox, you need to remove the user from all groups. For detailed information, see [Remove user from a group](#remove-user-from-a-group "Remove user from a group ").  
There is the following limitation: You cannot remove a user from the *ActindoAdmingroup* in a sandbox of which he&frasl;she is the owner. <!--- Kann man den owner ändern? -->
 


## Delete user 

Delete a user, if he&frasl;she works no longer in your company, for example. You can delete a user in the main account only.

#### Prerequisites

- You are logged in to the main account
- You are granted to delete users.

#### Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

1. Select the user you want to delete.   
  The *Edit user "username"* view is opened. By default, the *Profile* tab is preselected. 

   ![Edit user](../../Assets/Screenshots/Core1Platform/AdministratingCore1/UserEdit.png "[Edit user]")

2. Click the [DELETE] button down right and confirm the confirmation pop-up window.  
  The user is deleted.





