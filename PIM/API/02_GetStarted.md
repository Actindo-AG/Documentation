# Get started


## Using the Actindo Core1 OpenAPI



## OAuth authorization flow

The Core1 uses the OAuth 2.0 open protocol to handle client authorization for API access. 

### Prerequisite

- An app for client access is available. 
- A user has been created.
- The user has the appropriate rights, see [User rights](add-link-to-Core1-docu).

[comment]: <> (to be completed)

### Step 1: Register your app

If you want to gain access to the Core1 from your app via API, first of all you have to register your app in the developer portal. 

*Dev Tools > Tab APP REGISTRATION*

![App registrations](../../Assets/Screenshots/PIM/API/AppRegistrations.png "[App registrations]")

1. Click the ![App registrations](../../Assets/Icons/Plus01.png "[App registrations]") button to add an app registration.
    The *Create* view is displayed.

    ![Create app registration](../../Assets/Screenshots/PIM/API/CreateAppRegistration.png "[Create app registration]")

2. Enter a name for your app registration in the *Name* field. For the application name, it is recommended to use the third-party app name.

3. Enter a valid client ID in the *Application (client) ID* field. You can freely define your client ID, although it is recommended to use a UUID generator tool, such as [UUID Generator](https://www.uuidgenerator.net/version4 "[https://www.uuidgenerator.net/version4]"), to generate a UUID (universally unique identifier).

    The client ID for the Core1 must comply with the following requirements:
    - between 4 and a 31 characters long  
    - allowed characters include upper and lower cases letters, numbers, underscore, and hyphen
    - beginning with a letter  

[comment]: <> (Underscore und hyphen? Stimmt das? Wahrscheinlich auch mit einer Zahl am Anfang möglich. Evtl. von Devs oder ImSpecs testen/bestätigen lassen und dementsprechend anpassen!)

4. If available in your version, leave the toggle *Only authentication scopes open ID profile e-mail. You will not be able to call any methods besides getting profile data" disabled.

5. Enter an appropriate redirect URI in the *Redirect URI* field. For exemplary purposes, we are using https://oauthdebugger.com/debug. See the following screenshot for reference.

    ![App registration example](../../Assets/Screenshots/PIM/API/AppRegistrationExample.png "[App registration example]")

6. Click the [SAVE] button.  
    The app registration is saved. The client secret is displayed.

    > [Caution]   
    The client secret is displayed only once.  
    Make sure you copy it!


## Step 2: Get an authorization code

To be able to generate an access token for authentication, you need to get an authorization code first. 

Following the example provided in [Step 1: Register you app](#step-1-register-your-app), go to the https://oauthdebugger.com/ website.

*OAuth debugger*

![OAuth debugger](../../Assets/Screenshots/PIM/API/OAuthDebugger.png "[OAuth debugger]")

> [Caution]  
    Before continuing, make sure you are not logged into the account anymore. Otherwise, the system will create credentials that can make requests on your users' behalf.
    When logging in, make sure to use the correct API user credentials instead of your personal account.

1. Enter the authorization URI (Uniform Resource Identifier) in the *Authorize URI (required)* field. In this case, you URI should look like this:

    **https://your-workspace.actindo.com/Actindo.CoreModules.Auth.OAuth2.authorize**

    Replace *your-workspace* with the name of your instance. Bear in mind that the authorization is account-specific.

2. Enter **https://oauthdebugger.com/debug** in the *Redirect URI (required)* field.

3. Enter your client ID in the *Client ID (required)* field. You have defined your client ID previously in the app registration.

4. Enter **profile** in the *Scope (required)* field.

5. The *State* and *Nonce* fields are automatically filled.

6. Click the *code* checkbox in the *Response type (required)* section.

7. Select the *form_post* radio button in the *Response mode (required)* section. 

[comment]: <> (form post oder query? Check video)

8. Click the [SEND REQUEST] button.  
    If the authentication flow is successful, OAuth debugger displays as success message with an authorization code, such as in the following example. 

    ![OAuth debugger success](../../Assets/Screenshots/PIM/API/OAuthDebuggerSuccess.png "[OAuth debugger success]")
    
9. Log in to your *Actindo Core1 Digital Operation Platforms* with your credentials (username and authorization code).  
    The authorization code is now linked to the logged in user.

    ![Core1 Login](../../Assets/Screenshots/PIM/API/Core1Login.png "[Core1 Login]")

[comment]: <> (Stimmt das so? Check video und ausführlicher formulieren!)


## Step 3: Generate an access token

Once you have obtained an authorization code, you can generate an access token for authentication.

The following parameters are required: 
- Authorization code
- Client ID
- Client secret

1. Send the Token URL request to generate you access token, as displayed in the following request sample.  
    Replace *your-workspace* with the name of your instance, and the example values with your client ID, client secret, and the authorization code that you have obtained in [Step 2: Get an authorization code](#step-2-get-an-authorization-code). 

    **Request sample**

        curl -X POST   https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken \
        -H 'Content-Type: application/x-www-form-urlencoded' \
        -H 'cache-control: no-cache' \
        -d 'grant_type=authorization_code&code=5471fdee60b8c9d571f137c0940dfeddfdc4dddb&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&redirect_uri=https%3A%2F%2Foauthdebugger.com%2Fdebug'

    The access token is generated, as displayed in the following response sample.

    **Response sample**

        {"access_token":"EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"37e521b0ec5f035c86f0a2db09fe73cda934235e"}

2. Write down you access token and your refresh token. 
    You can now log in to your *Actindo Core1 Digital Operations Platform* instance with your credentials (username and access token). 

    > [Info]  Access (also called bearer) tokens are short-lived. You can generate further access tokens with your refresh token.
    
[comment]: <> (Unsicher, dass es hier schon kommt. Evtl. in Step 4? Check video!)


## Step 4: Send a test authentication request

Send a test authentication request to your Core1 instance to check that the access token is valid.

1. Send the Token URL request to generate you access token, as displayed in the following request sample.  
    Replace *your-workspace* with the name of your instance, and the example values with your access token (bearer) code that you have obtained in [Step 3: Generate an access token](#step-3-generate-an-access-token). 

    **Request sample**

        curl -X POST \
        -H 'Authorization: Bearer EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2' \
        'https://[your-workspace].actindo.com/Actindo.CoreModules.Tools.TenantTest.ping?ping=42'


    If the access token is valid, a success response is returned, as displayed in the following response sample.

    **Response sample**

        {"pong":"42","success":true,"displayMessage":null,"displayMessageTitle":null,"error":null,"job_id":null}'



## Step 5: Generate an access token from refresh token

Access tokens are valid for a limited period of time. If your access token is expired, you can get a new one using your refresh token.

1. Send the Token URL request to generate you access token, as displayed in the following request sample.  
    Replace *your-workspace* with the name of your instance, and the example values with your client ID, client secret, and the refresh token that you have obtained in [Step 3: Generate an access token](#step-3-generate-an-access-token).  

    **Request sample** 

        curl -X POST 'https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken' \
        -H 'Content-Type: application/x-www-form-urlencoded' \
        -H 'cache-control: no-cache' \
        -d 'grant_type=refresh_token&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&refresh_token=37e521b0ec5f035c86f0a2db09fe73cda934235e'


    The access token is generated, as displayed in the following response sample. 

    **Response sample** 

        {"access_token":"3lUNK4D\/eiiVg4hM1iJ+lK1b6n+qNflykDyI+laWLQL3P8O8Xmuu3AkfmjnWYUaIdZ\/1r\/6ybfgh4IXHLOFZ0R78rZH89Hk7teOTpsGqPsreiguqOT92WklHU9pTBTNb","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"cca31dc1bdf4c85b892804424b3a5f3ee44368aa"}

    > [Info] 
    You also get a new refresh token.  
    Make sure you keep it safely for future reference!

        


## Send your first request

1. Authorization
2. Header/Format
3. Find out required fields
4. Find out required fields id
5. Send request

[comment]: <> (to be completed)
