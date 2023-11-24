[!!Set up U2F from the administrator side](../AdministratingCore1/03_AdminSetupActindo.md)
[!!User interface Profile settings](../UserInterface/01d_U2F.md)

# Set up U2F from the user side

The secure access to Actindo can be granted by using the *Multi-Factor Authentication (MFA)*. This method requires two or more verification factors to log in to an application or website.    
Actindo uses the *YubiKey* as a second factor for the two-factor authentication, using the *Universal Second Factor (U2F)* standard.
The *Multi-Factor Authentication (MFA)* offers the following benefits:
- Increased security in the login process and with third parties
- Increased security of the user's identity
- Better access control
- Reduction of password risks

For the U2F setup of an Actindo account, you need to set up *U2F* as a user. Additionally, your administrator must activate your user for *U2F*. As a user, you need to define several settings within your Actindo account to add *U2F* with the *YubiKey* as a login method.    
After the registration, the *YubiKey* as a login method is valid for all Actindo accounts, which means for the main account as well as for the sandboxes.

#### Prerequisites

- You possess an *YubiKey*.
- You have an active Actindo account.

#### Procedure

*Login Actindo*

![Login username](../../Assets/Screenshots/Core1Platform/UsingCore1/LoginUserName.png "[Login username]")

> [Info] For the user-side setup, you can log in to both a main account and a sandbox of the *Core1 Platform*.

1. Log in to the main account or sandbox, see [Login to the Actindo Core1 Platform](./01_Login.md#login-to-the-actindo-core1-platform).   
    The *Actindo Dashboard* is displayed.

    ![Actindo dashboard](../../Assets/Screenshots/Core1Platform/Core1.png "[Actindo dashboard]")

2. Click your avatar icon in the upper right corner.   
    The profile menu is displayed.

    ![Profile menu](../../Assets/Screenshots/Core1Platform/UsingCore1/ProfileMenu.png "[Profile menu]")

3. Click the *Settings* entry in the profile menu.   
    The *PROFILE* tab is displayed.

    ![Profile](../../Assets/Screenshots/Core1Platform/ProfileSettings/Profile/Profile.png "[Profile]")

4. Click the *U2F* tab.   
    The *U2F* tab is displayed.

    ![U2F](../../Assets/Screenshots/Core1Platform/ProfileSettings/U2F/U2F.png "[U2F]")

5. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Add new U2F device* window is displayed.

    ![Add new U2F device](../../Assets/Screenshots/Core1Platform/ProfileSettings/U2F/AddNewU2FDevice.png "[Add new U2F device]")

    > [Info] The following steps may vary depending on the key used. Some keys also require a Windows pin that you can choose by yourself.


6. Click the [OK] button to continue the device registration for U2F. Note that after clicking the [OK] button you only have time for about 15 seconds for finishing the registration. After that, the process will be timed out. Restart the registration if a time-out occurs.   
    The browser window *Verify your identity* is displayed to select the device type for the identity verification.

    ![Verify your identity](../../Assets/Screenshots/Core1Platform/ProfileSettings/U2F/VerifyIdentity.png "[Verify your identity]")


8. Select the *USB security key* option in the browser window.   
    The browser window changes to the *Use your security key* window and prompts you to insert the key and touch it.

    ![Use security key](../../Assets/Screenshots/Core1Platform/ProfileSettings/U2F/UseSecurityKey.png "[Use security key]")

9. Insert the *YubiKey* into your device.   
    The *YubiKey* starts to flash.

    > [Info] Note that problems with the connection to the *YubiKey* may occur if you use an adapter or an additional cable to connect the *YubiKey*.

8. Touch the flashing area on your *YubiKey*.    
    Depending on the browser configuration, a confirmation message is displayed in the browser window. Click the [Accept] button in the browser window to authorize the website to read the key and close the browser window.    
    The U2F key is added to the list of keys and displayed in the *U2F* tab.  The user side setup for U2F is completed. It is now shared with all Actindo instances (main account and sandboxes).
    Note that the U2F login must additionally be enabled by an administrator to be used for the Actindo U2F login.
