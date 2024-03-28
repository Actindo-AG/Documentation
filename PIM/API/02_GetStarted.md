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

[comment]: <> (Was soll das heißen? Use some canonical name, such as "Testaccount for oauthdebugger.com")

3. Enter a valid client ID in the *Application (client) ID* field. For the client ID, it is recommended to use a UUID generator tool, such as [UUID Generator](https://www.uuidgenerator.net/version4 "[https://www.uuidgenerator.net/version4]"), to generate a UUID (universally unique identifier).

    The client ID for the Core1 must comply with the following requirements:
    - between 4 and a 31 characters long  
    - allowed characters include upper and lower cases letters, numbers, underscore, and hyphen
    - beginning with a letter  

[comment]: <> (begins with a letter??? Im Beispiel ist es eine Nummer! S. Screenshot)

4. If necessary, enable the toggle *Only authentication scopes open ID profile e-mail. You will not be able to call any methods besides getting profile data".

[comment]: <> (Was macht den Toggle? Ist es relevant oder kann es hier ignoriert werden?)

5. Enter https://oauthdebugger.com/debug in the *Redirect URI* field. See the following screenshot as an example.

    ![App registration example](../../Assets/Screenshots/PIM/API/AppRegistrationExample.png "[App registration example]")

6. Click the [SAVE] button.  
    The client secret is displayed **once**.  
    Make sure you copy it!


## Step 2 Get an authorization code

To be able to generate an access token for authentication, you need to get an authorization code first. As the Core1 works with the OAuth 2.0 authentication protocol, go to the https://oauthdebugger.com/ website.

*OAuth debugger*

![OAuth debugger](../../Assets/Screenshots/PIM/API/OAuthDebugger.png "[OAuth debugger]")

> [Caution]  
    Before continuing, make sure you are **NOT** logged into the account anymore. Otherwise, the system will create credentials that can make requests on **your** users' behalf.
    When logging in, make sure to use the correct API user credentials instead of your personal account.

1. Enter the authorization URI (Uniform Resource Identifier) in the *Authorize URI (required)* field. In this case, you URI should look like this:

    **https://your-workspace.actindo.com/Actindo.CoreModules.Auth.OAuth2.authorize**

    Replace *your-workspace* with the name of your instance. Bear in mind that the authorization is account-specific.

2. Enter **https://oauthdebugger.com/debug** in the *Redirect URI (required)* field.

3. Enter your client ID in the *Client ID (required)* field. You have defined your client ID previously in the app registration.

4. Enter **none** in the *Scope (required)* field.

5. *State* is an optional value and can therefore be ignored here.

6. Enter xxx in the *Nonce* (or number used once) field.

[comment]: <> (Nonce: a number that uniquely identifies each call to the REST API private endpoints. Bedeutung? Wo kommt den Code her?)

7. Click the *code* checkbox in the *Response type (required)* section.

8. Select the *form_post* radio button in the *Response mode (required)* section.

9. Click the [SEND REQUEST] button.  
    If the authentication flow is successful, OAuth displays as success message with an authorization code, such as in the following example. 

    ![OAuth debugger success](../../Assets/Screenshots/PIM/API/OAuthDebuggerSuccess.png "[OAuth debugger success]")
    
    > [Info] If the value **none** for the *Scope field* returns the "An unsupported scope was requested" error, try setting the value to **profile**.

[comment]: <> (Mehr Info zum Ergebnis benötigt!)


## Step 3: Generate an access token

Once you have obtained an authorization code, you can generate an access token for authentication.

The following parameters are required: 
- Authorization code
- Client ID
- Client secret

**Request sample** (?)


    curl -X POST   https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken \
    -H 'Content-Type: application/x-www-form-urlencoded' \
    -H 'cache-control: no-cache' \
    -d 'grant_type=authorization_code&code=5471fdee60b8c9d571f137c0940dfeddfdc4dddb&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&redirect_uri=https%3A%2F%2Foauthdebugger.com%2Fdebug'


**Response sample** (?)

    {"access_token":"EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"37e521b0ec5f035c86f0a2db09fe73cda934235e"}


## Step 4: Try the authentication via API ?

[comment]: <> (Try the authentication via API?)

**Request sample** (?)

        curl -X POST \
        -H 'Authorization: Bearer EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2' \
        'https://[your-workspace].actindo.com/Actindo.CoreModules.Tools.TenantTest.ping?ping=42'


**Response sample** (?)


        {"pong":"42","success":true,"displayMessage":null,"displayMessageTitle":null,"error":null,"job_id":null}'

Alternatively, you can try to log in with your credentials in the Core1.

![Core1 Login](../../Assets/Screenshots/PIM/API/Core1Login.png "[Core1 Login]")


## Step 5: Get authorization token from refresh token

Authorization tokens are valid for a limited period of time. If your authorization token is expired, you can get a new one using your refresh token.

**Request sample** (?)

    curl -X POST 'https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken' \
    -H 'Content-Type: application/x-www-form-urlencoded' \
    -H 'cache-control: no-cache' \
    -d 'grant_type=refresh_token&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&refresh_token=37e521b0ec5f035c86f0a2db09fe73cda934235e'

**Response sample** (?)

    {"access_token":"3lUNK4D\/eiiVg4hM1iJ+lK1b6n+qNflykDyI+laWLQL3P8O8Xmuu3AkfmjnWYUaIdZ\/1r\/6ybfgh4IXHLOFZ0R78rZH89Hk7teOTpsGqPsreiguqOT92WklHU9pTBTNb","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"cca31dc1bdf4c85b892804424b3a5f3ee44368aa"}

> [Info] You also get a new refresh token which you need to keep!


## Send your first request

1. Authorization
2. Header/Format
3. Find out required fields
4. Find out required fields id
5. Send request
