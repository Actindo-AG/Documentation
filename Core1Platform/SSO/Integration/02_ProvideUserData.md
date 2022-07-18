# Provide user data for SSO

For the SSO setup in Azure AD, it is required to configure several settings in Azure AD on the organization side for SSO and to provide the required data for the Actindo side configuration. The procedure to provide the user data is described below.

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

3. Click the *Users* entry in the side menu on the left.   
  You are redirected to the *Users* page of your Azure AD.

4. Click the *All users* entry in the side menu on the left.   
  The *All users* page is displayed.

  ![All users](/Assets/Screenshots/Core1Platform/Azure/AllUsers.png "[All users]")

5. Click the *Bulk operations* drop-down list in the top bar.   
  The *Bulk operations* menu is displayed.

  ![Bulk operations](/Assets/Screenshots/Core1Platform/Azure/BulkOperations.png "[Bulk operations]")

6. Click the *Download users* entry in the *Bulk operations* menu.   
  A list with all users is automatically exported as a csv file.

7. Click the *Bulk Operation results* entry in the side menu on the left.   
  The *Bulk Operation results* page with the exported user list is displayed.

  ![Bulk operation results](/Assets/Screenshots/Core1Platform/Azure/BulkOperationResults.png "[Bulk operation results]")

8. Click the exported user list.   
  The *Bulk user export (preview)* page with details to the user list is displayed.

  ![Bulk user export](/Assets/Screenshots/Core1Platform/Azure/BulkUserExport.png "[Bulk user export]")

9. Click the [Download results] button in the *Result* column of the corresponding row.   
  The user list is downloaded.

10. Open the downloaded csv file in a spreadsheet program, for instance in Excel.   
  The user list with all users is displayed in the spreadsheet program.

  ![User list](/Assets/Screenshots/Core1Platform/UserList.png "[User list]")

11. Copy the data in the columns *userPrincipalName* and *Id* for all users that will use SSO and save this data in a secure location.   

  > [Info] The *UserPrincipalName* and the *Id* of each user are needed by Actindo for the SSO configuration.
