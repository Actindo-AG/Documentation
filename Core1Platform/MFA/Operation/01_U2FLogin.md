[!!Core1 Platform](Core1Platform)

# Log in via U2F

After U2F has been configured for your Actindo account, you will use U2F from your next login to your Actindo account on.

#### Prerequisites

- U2F has been configured for your account, see [Set up U2F from the user side](/Core1Platform/MFA/Integration/01_UserSetupActindo.md) and [Set up U2F from the administrator side](/Core1Platform/MFA/Integration/02_AdminSetupActindo.md).
- You possess a *YubiKey*.

#### Procedure

*Login Actindo*

![Login user name](/Assets/Screenshots/Core1Platform/LoginUsername.png "[Login user name]")

1. Enter your user name in the *User name* field and click the [LOGIN] button.   

  > [Info] If SSO is configured for Actindo and you are not yet logged in to another application via SSO, you must follow the login via SSO before continuing with step **3** of this procedure. For detailed information about the login via SSO, see [Log in via SSO](/Core1Platform/SSO/Operation/01_SSOLogin.md).

  The *Password* field is displayed.

  ![Login password](/Assets/Screenshots/Core1Platform/LoginPassword.png "[Login password]")

2. Enter your password in the *Password* field and click the [LOGIN] button.   
  The *Click here to start the second factor authentication* button is displayed.

  ![Login U2F](/Assets/Screenshots/Core1Platform/LoginU2F.png "[Login U2F]")

3. Click the *Click here to start the second factor authentication* button.    
  A browser window is displayed to select the device type for U2F.

  ![USB security key](/Assets/Screenshots/Core1Platform/ProfileSettings/U2F/USBSecurityKey.png "[USB security key]")

4. Select the *USB security key* option in the browser window.   
  The browser window prompts to insert the key and touch it.

  ![Use security key](/Assets/Screenshots/Core1Platform/ProfileSettings/U2F/UseSecurityKey.png "[Use security key]")

5. Insert the *YubiKey* into your device.   
  The *YubiKey* starts to flash.

  > [Info] Note that problems with the connection to the *YubiKey* may occur if you use an adapter or an additional cable to connect the *YubiKey*.

6. Touch the flashing area on your *YubiKey* .   
  The browser window is closed. You are logged in to your account after a few moments.  



## Related content

- [Set up U2F from the user side](/Core1Platform/MFA/Integration/01_UserSetupActindo.md)
- [Set up U2F from the administrator side](/Core1Platform/MFA/Integration/02_AdminSetupActindo.md)
