# Set up SSO in Azure AD

For the SSO setup in Azure AD, it is required to configure several settings in Azure AD on the organization side for SSO and to provide the required data for the Actindo side configuration. The Azure AD configurations to be set are described below.


## Register a new application

#### Prerequisites

- You are logged in to the organization account in the Azure Portal.
- You have the required rights of an organization administrator in Azure AD.

#### Procedure

*Azure Portal > Login to Account*

![Azure portal](/Assets/Screenshots/Core1Platform/Azure/AzurePortal.png "[Azure portal]")

1. Search for the *Azure Active Directory* in the top search bar.    
  The search results are displayed below the search bar while typing.

2. Click on the *Azure Active Directory* entry in the *Services* section of the search results.    
  The *Azure Active Directory* is opened. By default, the *Overview* page is displayed.

  ![Azure AD overview](/Assets/Screenshots/Core1Platform/Azure/AzureADOverview.png "[Azure AD overview]")

3. Click the *App registrations* entry in the side menu on the left.     
  The *App registrations* page is displayed.

  ![App registrations](/Assets/Screenshots/Core1Platform/Azure/AppRegistrations.png "[App registrations]")

4. Click the [+ New registration] button in the top bar.   
  The *Register an application* page is displayed.

  ![Register an application](/Assets/Screenshots/Core1Platform/Azure/RegisterApplication.png "[Register an application]")

5. Enter a name for the application in the *Name* field, for instance **Actindo Core1**.
  - Select the radio button *Accounts in this organizational directory only (Organization only – Single tenant)* in the *Supported account types* section.
  - Select the option **Web** in the drop-down list in the *Redirect URI (optional)* section.
  - Enter the following URL in the field in the *Redirect URI (optional)* section:    
    https://login.actindo.com/Actindo.CoreModules.Auth.AuthForm.finishOAuth2   


6. Click the [Register] button in the bottom.    
  Actindo is registered as an application for SSO. The *Register an application* page is closed. You are automatically redirected to the page of your registered application.

7. Click the *Overview* menu entry in the left side menu.   
  The *Overview* page is displayed.

  ![Application overview](/Assets/Screenshots/Core1Platform/Azure/ApplicationOverview.png "[Application overview]")

8. Copy the *Application (client) ID* in the *Essentials* section and save this ID in a secure location.   

  > [Info] The *Application (client) ID* is needed by Actindo for the SSO configuration.



## Add a client secret

#### Prerequisites

- You are logged in to the organization account in the Azure Portal.
- You have the required rights of an organization administrator in Azure AD.
- You have registered an application for Actindo, see [Register a new application](#register-a-new-application).

#### Procedure

*Azure Portal > Login to Account > Overview page of your application*

![Application overview](/Assets/Screenshots/Core1Platform/Azure/ApplicationOverview.png "[Application overview]")

1. Click the *Certificates & secrets* entry in the side menu on the left.   
  The *Certificates & secrets* page is displayed.

  ![Certificates and secrets](/Assets/Screenshots/Core1Platform/Azure/CertificatesSecrets.png "[Certificates and secrets]")

2. Click the [+ New client secret] button in the *Client secrets* tab.    
  The *Add a client secret* window is displayed.   

  ![Add a client secret](/Assets/Screenshots/Core1Platform/Azure/AddClientSecret.png "[Add a client secret]")

3. Configure the settings below in the *Add a client secret* window:   
  - Enter a description for the client secret in the *Description* field, for instance **Actindo Core1**.
  - Select an expiration period in the *Expires* drop-down list.

  > [Info] Note to recreate the client secrets before expiration. It is recommended to select a long expiration period.


4. Click the [Add] button in the bottom of the window.   
   The client secret is saved and added to the application. The *Add a client secret* window is closed. The new client secret is displayed in the *Client secrets* tab.

   ![Client secrets](/Assets/Screenshots/Core1Platform/Azure/ClientSecrets.png "[Client secrets]")

5. Copy the content of the secret client in the *Value* column by clicking the ![Copy](/Assets/Icons/Copy01.png "[Copy]") (Copy) button in this column and save this value in a secure location.      

  > [Info] The *Client secret value* is needed by Actindo for the SSO configuration.



## Add API permissions

#### Prerequisites

- You are logged in to the organization account in the Azure Portal.
- You have the required rights of an organization administrator in Azure AD.
- You have registered an application for Actindo, see [Register a new application](#register-a-new-application).

#### Procedure

*Azure Portal > Login to Account > Overview page of your application*

![Application overview](/Assets/Screenshots/Core1Platform/Azure/ApplicationOverview.png "[Application overview]")

1. Click the *API permissions* entry in the side menu on the left.   
  The *API permissions* page is displayed.

  ![API permissions](/Assets/Screenshots/Core1Platform/Azure/APIPermissions.png "[API permissions]")

  > [Info] By default, the **User.Read** permission is listed in the *Configured permissions* section.   

2. Click the [+ Add a permission] button in the *Configured permissions* section.   
  The *Request API permissions* window is displayed. By default, the *Microsoft APIs* tab is preselected.

  ![Request API permissions](/Assets/Screenshots/Core1Platform/Azure/RequestAPIPermissions.png "[Request API permissions]")

3. Click the *Microsoft Graph* box in the *Microsoft APIs* tab.   
  The *Microsoft Graph* page is displayed.

  ![Microsoft graph](/Assets/Screenshots/Core1Platform/Azure/MicrosoftGraph.png "[Microsoft graph]")

4. Click the *Delegated permissions* box on the *Microsoft Graph* page.   
  The *Select permissions* view is displayed.

  ![Select permissions](/Assets/Screenshots/Core1Platform/Azure/SelectPermissions.png "[Select permissions]")

5. Click the *OpenId* permissions drop-down list and activate the following checkboxes:
  - email
  - openid
  - profile


6. Click the [Add permissions] button at the bottom of the window.   
  The selected permissions are saved. The *Request API permissions* window is closed. The selected permissions are listed in the *Configured permissions* section of the *API permissions* page.

  ![Configured permissions](/Assets/Screenshots/Core1Platform/Azure/ConfiguredPermissions.png "[Configured permissions]")



## Configure the application settings

#### Prerequisites

- You are logged in to the organization account in the Azure Portal.
- You have the required rights of an organization administrator in Azure AD.
- You have registered an application for Actindo, see [Register a new application](#register-a-new-application).

#### Procedure

*Azure Portal > Login to Account > Overview page of your application*

![Application overview](/Assets/Screenshots/Core1Platform/Azure/ApplicationOverview.png "[Application overview]")

1. Scroll down to the bottom of the *Overview* page.   
  The *Configure for your organization* section is displayed.

  ![Application overview enterprise](/Assets/Screenshots/Core1Platform/Azure/ApplicationOverviewEnterprise.png "[Application overview enterprise]")

2. Click the [Go to Enterprise applications] button in the *Configure for your organization* section.        
  You are redirected to the *Enterprise Application* page of your application.

3. Click the *Properties* entry in the side menu on the left.   
  The *Properties* page is displayed.

  ![Properties](/Assets/Screenshots/Core1Platform/Azure/Properties.png "[Properties]")

4. Set the *Assignment required?* option to **YES**.

5. Click the *Users and group* entry in the side menu on the left and configure the corresponding application settings in your organization as required.   

6. Close the *Enterprise Application* page, return to you application page and click the *Overview* entry in the menu on the left side.   
  The *Overview* page is displayed.

  ![Application overview](/Assets/Screenshots/Core1Platform/Azure/ApplicationOverview.png "[Application overview]")

7. Click the [Endpoints] button in the top bar.   
  The *Endpoints* window is displayed.

  ![Endpoints](/Assets/Screenshots/Core1Platform/Azure/Endpoints.png "[Endpoints]")

8. Copy the *OAuth 2.0 authorization endpoint (v2)* and the *OAuth 2.0 token endpoint (v2)* by clicking the ![Copy](/Assets/Icons/Copy01.png "[Copy]") (Copy) button in the corresponding column and save these endpoints in a secure location.

  > [Info] The *OAuth 2.0 authorization endpoint (v2)* and the *OAuth 2.0 token endpoint (v2)* are needed by Actindo for the SSO configuration.
