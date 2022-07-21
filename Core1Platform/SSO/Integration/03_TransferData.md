[!!Set up SSO in Azure AD](./01_AzureADSetup.md)
[!!Provide user data for SSO](./02_ProvideUserData.md)


# Transfer data to Actindo

After the organization side configuration for SSO in Azure AD, Actindo needs to configure further settings to enable SSO. Therefore, a certain set of required data from the organization must be transferred to Actindo to complete the SSO configuration.

#### Prerequisites

- The Azure AD setup is completed, see [Set up SSO in Azure AD](./01_AzureADSetup.md).
- The data of all users who want to use SSO are provided, see [Provide user data for SSO](./02_ProvideUserData.md).

#### Procedure

1. Create a MPS ticket for Actindo.   

2. Include the following data:
- User data (userPrincipalName and ID) of each user who will use SSO
- Client secret value
- Application (client) ID
- OAuth 2.0 authorization endpoint (v2) and OAuth 2.0 token endpoint (v2)

3. Send the ticket with the required data to Actindo.   
  The SSO for Actindo will be configured.
