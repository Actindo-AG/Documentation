[!!Set up U2F from the user side](../UsingCore1/01a_UserSetupActindo.md)
[!!User interface Profile](../UserInterface/01a_Profile.md)

# Set up U2F from the administrator side

For the U2F setup of an Actindo account, a user-side setup as well as an administrator-side setup is necessary. As an administrator, you must activate U2F as an authorization method for the corresponding user to complete the *U2F* setup.

- Strong protection     
    The user credentials are protected with strong public key cryptography and bound to the service. Since only the real site can authenticate with a key, this provides a high level of protection against account takeover.  

- No additional apps or software required  
    The *YubiKey* protects access to computers, networks and online services with a single touch.

- Convenient authentication with just a few steps     
    The authentication code is created via USB between the *YubiKey* and your device without further manual input steps.

#### Prerequisites

- You have the required admin rights in the *Actindo Core1 Platform*.
- You are logged in a live account of the *Core1 Platform* with a user assigned to the admin group.

#### Procedure

*Settings > Users and groups > Tab User management*

![User management](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/UserManagement.png "[User management]")

> [Info] For the admin-side setup, you must log in to an Actindo live account with the corresponding user.

1. Click the user for whom you want to activate U2F in the users list.     
    The *Edit user* view is displayed. By default, the *Profile* tab is displayed.

    ![Edit user profile](../../Assets/Screenshots/Settings/UsersGroups/UserManagement/EditUserProfile.png "[Edit user profile]")

2. Enable the *Universal Second Factor (U2F)* toggle.

3. Click the [SAVE] button in the upper right corner.     
    U2F is activated as authorization method for the selected user.

   > [Info] You can repeat this procedure for all users for whom you want to activate U2F. Note that the U2F login needs also to be set up by the corresponding user to be used for the Actindo U2F login.
