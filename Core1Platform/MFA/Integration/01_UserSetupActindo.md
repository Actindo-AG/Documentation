[!!Core1 Platform](Core1Platform)

# User-side setup for U2F

For the U2F setup of an Actindo account, a user-side setup as well as an administrator-side setup is necessary. The user needs to define several settings within its Actindo account to add *U2F* with the *YubiKey* as an authorization method.

#### Prerequisites

- You possess an *YubiKey*.
- You have an active Actindo account.

#### Procedure

*Login Actindo*

![Login user name](/Assets/Screenshots/Core1Platform/LoginUserName.png "[Login user name]")

> [Info] For the user-side setup, you can log in to both, a live account or a sandbox of the Core1 PLattform.

1. Enter your user name in the *User name* field and click the [LOGIN] button.   
  The *Password* field is displayed.

  ![Login password](/Assets/Screenshots/Core1Platform/LoginPassword.png "[Login password]")

2. Enter your password in the *Password* field and click the [LOGIN] button.   
  You are logged in. The *Actindo Dashboard* is displayed.

  ![Actindo dashboard](/Assets/Screenshots/ActindoDashboard/ActindoDashboard.png "[Actindo dashboard]")

3. Click your avatar icon in the upper right corner.   
  The profile menu is displayed.

  ![Profile menu](/Assets/Screenshots/Core1Platform/ProfileMenu.png "[Profile menu]")

4. Click the *Settings* entry in the profile menu.   
  The *Profile* tab is displayed.

  ![Profile](/Assets/Screenshots/Core1Platform/ProfileSettings/Profile/Profile.png "[Profile]")

5. Click to the *U2F* tab.   
  The *U2F* tab is displayed.

  ![U2F](/Assets/Screenshots/Core1Platform/ProfileSettings/U2F/U2F.png "[U2F]")

6. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Add new U2F device* window is displayed.

  ![Add new U2F device](/Assets/Screenshots/Core1Platform/ProfileSettings/U2F/AddNewU2FDevice.png "[Add new U2F device]")

7. Click the [OK] button to continue the device registration for U2F.   
  A browser window is displayed to select the device type for U2F.

  ![USB security key](/Assets/Screenshots/Core1Platform/ProfileSettings/U2F/USBSecurityKey.png "[USB security key]")

8. Select the *USB security key* option in the browser window.   
  The browser window prompts to insert the key and touch it.

  ![Use security key](/Assets/Screenshots/Core1Platform/ProfileSettings/U2F/UseSecurityKey.png "[Use security key]")

9. Insert the *YubiKey* into your device.   
  The *YubiKey* starts to flash.

  > [Info] Note that problems with the connection to the *YubiKey* may occur if you use an adapter or an additional cable to connect the *YubiKey*.

8. Touch the flashing area on your *YubiKey*.    

   > [Info] Depending on the browser configuration, a confirmation message is displayed in the browser window. Click the [Accept] button in the browser window to authorize the website to read the key and close the browser window.    

   The U2F key is added to the list of keys and displayed in the *U2F* tab. The user side setup for U2F is completed.

> [Info] Note that the U2F login needs also to be activated by an administrator to be used for the Actindo U2F login.



## Related content

- [Administrator-side setup for U2F](02_AdminSetupActindo.md)
- [User Interface Profile settings](/Core1Platform/UserInterface/01d_U2F.md)
