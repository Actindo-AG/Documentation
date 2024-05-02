# Get started

[comment]: <> (Diese Info gilt für alle APIs bzw. alle Module. Falls andere Module dokumentiert, darauf verweisen oder auf eine übergeordnete Ebene verschieben)

This API reference documentation provides general information on the main resources, such as products, and request samples to perform the most usual API calls. It is not meant to be comprehensive but to provide you with a starting point to understand how the *Actindo Core1 openAPI* works. 

A complete API documentation, organized by module, is available in the *Actindo Core1 Platform* under *Dev Tools > API > Module name*. The API documentation is automatically generated based on your specific module configuration. Therefore, the available modules, endpoints, and attributes contained in your *Actindo Core1 openAPI* documentation are the ones relevant for your current instance.


## Using the request samples

The request samples provided in this documentation are complete and ready to use, but they require some customization. 

Let's take the following request sample: 


    {
        "product": {
            "sku": "Single-product",
            "attributeSetId": 102,
            "_pim_art_name__actindo_basic__en_US": "Single product",
            "_pim_art_name__actindo_basic__de_DE": "Einzelprodukt",
            "_pim_products_description__actindo_basic__en_US": "This is a product description.",
            "_pim_products_description__actindo_basic__de_DE": "Das ist eine Produktbeschreibung."
        }
    }

Let's say you want to create a single product (that is, without variants), for example, a handbag. You market your products in your online shop to an English and Spanish speaking audience.


| Product       | Information  | Attribute      | Value    |
|---------------|--------------|----------------|----------| 
| **SKU**       | HNDBG-1      | sku            | HNDBG-1  |
| **Type**      | Accessories  | attributeSetId | 412 (s. notes) |
| **English Name** | Handbag   | _pim_art__online_shop__name_en_US  | Handbag  |
| **Spanish Name** | Bolso     | _pim_art__online_shop__name_es_ES  | Bolso |
| **English description**| Vegan leather crossbody handbag | _pim_products_description__online_shop__en_US | Vegan leather crossbody handbag |
| **Spanish description**| Bolso bandolera de cuero vegano | _pim_products_description__online_shop__de_DE | Bolso bandolera de cuero vegano |


The exemplary attributes and values provided in the request sample should be customized as follows: 

    {
        "product": {
            "sku": "HNDBG-1",
            "attributeSetId": 412,
            "_pim_art_name__online_shop__en_US": "Handbag",
            "_pim_art_name__online_shop__es_ES": "Bolso",
            "_pim_products_description__online_shop__en_US": "Vegan leather crossbody handbag",
            "_pim_products_description__online_shop__es_ES": "Bolso bandolera de cuero vegano"
        }
    }

**Notes**

- The *sku* is a required attribute to create a product. You can choose it freely depending on your SKU structure, as long it is a string, that is, a sequence of characters. For detailed information, see [The product object](./05_Products.md#the-product-object).
- The *attributeSetId* represents the product type and is required attribute to create a product. Attribute sets must be previously created in the *PIM* or the *DataHub* modules based on your product structure. For detailed information, see [Attribute sets](./03_KeyConcepts.md#attribute-sets).
-  The attributes provided are the standard Actindo attributes contained in the *PIM basic set*. If you have created you own attributes and attribute sets, the attribute names will probably differ. If desired, you can get a list of all attributes created in an attribute set via API, see [List the attributes in an attribute set](./04_EntityData.md#list-the-attributes-in-an-attribute-set).   
- The scope (in this case, online shop) and languages (en_US and es_ES) must also be specified accordingly. 


## OAuth authorization flow

The *Actindo Core1 Platform* uses the OAuth 2.0 open protocol to handle client authorization for API access. 

#### Prerequisites

- An app for client access is available. 
- A user has been created.
- The user has the appropriate rights.

For detailed information on user rights, see [User rights](to-be-determined) in the Core1 documentation.

### Step 1: Register your app

If you want to gain access to the Core1 from your app via API, first of all you have to register your app in the developer portal. 

*Dev Tools > Tab APP REGISTRATIONS*

![App registrations](../../Assets/Screenshots/PIM/API/AppRegistrations.png "[App registrations]")

1. Click the ![App registrations](../../Assets/Icons/Plus01.png "[App registrations]") button to add an app registration.
    The *Create* view is displayed.

    ![Create app registration](../../Assets/Screenshots/PIM/API/CreateAppRegistration.png "[Create app registration]")

2. Enter a name for your app registration in the *Name* field. For the application name, it is recommended to use the third-party app name.

3. Enter a valid client ID in the *Application (client) ID* field. You can freely define your client ID, although it is recommended to use a UUID generator tool, such as [UUID Generator](https://www.uuidgenerator.net/version4 "[https://www.uuidgenerator.net/version4]"), to generate a UUID (universally unique identifier).

    The client ID for the Core1 must comply with the following requirements:
    - between 4 and a 31 characters long  
    - allowed characters include upper and lower cases letters, numbers, and underscore
    - beginning with a letter  

[comment]: <> (Wahrscheinlich auch mit einer Zahl am Anfang möglich laut Oli. Evtl. von Devs oder ImSpecs testen/bestätigen lassen und dementsprechend anpassen! UI muss verbessert werden, da Toggle darunter auch nicht funktioniert.)

4. If available in your version, leave the toggle *Only authentication scopes open ID profile e-mail. You will not be able to call any methods besides getting profile data" disabled.

5. Enter an appropriate redirect URI in the *Redirect URI* field. For exemplary purposes, we are using https://oauthdebugger.com/debug. See the following screenshot for reference.

    ![App registration example](../../Assets/Screenshots/PIM/API/AppRegistrationExample.png "[App registration example]")

6. Click the [SAVE] button.  
    The app registration is saved. The client secret is displayed.

    > [Caution]   
    The client secret is displayed only once.  
    Make sure you copy it!


### Step 2: Get an authorization code

To be able to generate an access token for authentication, you need to get an authorization code first. 

Following the example provided in [Step 1: Register you app](#step-1-register-your-app), we describe the process in the https://oauthdebugger.com/ website. You can also use other third-party website or your own system. 

*OAuth debugger*

![OAuth debugger](../../Assets/Screenshots/PIM/API/OAuthDebugger.png "[OAuth debugger]")

> [Caution]  
    Before continuing, make sure you are not logged into your account. Otherwise, the authorization code will be linked to your user profile. That means that any API requests made subsequently will be made on your user's behalf.
    
1. Enter the authorization URI (Uniform Resource Identifier) in the *Authorize URI (required)* field. In this case, your URI should look like this:

    **https://your-workspace.actindo.com/Actindo.CoreModules.Auth.OAuth2.authorize**

    Replace *your-workspace* with the name of your instance. Bear in mind that the authorization is account-specific.

2. Enter **https://oauthdebugger.com/debug** in the *Redirect URI (required)* field.

3. Enter your client ID in the *Client ID (required)* field. You have defined your client ID previously in the app registration.

4. Enter **profile** in the *Scope (required)* field.

5. The *State* and *Nonce* fields are automatically generated.

6. Click the *code* checkbox in the *Response type (required)* section.

7. Select the *form_post* radio button in the *Response mode (required)* section. 

8. Click the [SEND REQUEST] button.  
    If the authentication flow is successful, OAuth debugger displays a success message with an authorization code, such as in the following example. 

    ![OAuth debugger success](../../Assets/Screenshots/PIM/API/OAuthDebuggerSuccess.png "[OAuth debugger success]")
    
9. Log in to the *Actindo Core1 Digital Operation Platforms* with the user credentials (username and password) you want to authorize for API access.  
    The authorization code is now linked to the logged in user.

    ![Core1 Login](../../Assets/Screenshots/PIM/API/Core1Login.png "[Core1 Login]")


### Step 3: Generate an access token

Once you have obtained an authorization code, you can generate an access token for authentication.

For the following steps, a command line tool curl is used.

The following parameters are required: 
- Authorization code
- Client ID
- Client secret

1. Send the token URL request to generate your access token, as displayed in the following request sample.  

    **Request sample**

        curl -X POST   https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken \
        -H 'Content-Type: application/x-www-form-urlencoded' \
        -H 'cache-control: no-cache' \
        -d 'grant_type=authorization_code&code=5471fdee60b8c9d571f137c0940dfeddfdc4dddb&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&redirect_uri=https%3A%2F%2Foauthdebugger.com%2Fdebug'

    Replace *[your-workspace]* with the name of your instance, and the example values with your client ID, client secret, and the authorization code that you have obtained in [Step 2: Get an authorization code](#step-2-get-an-authorization-code). 

2. An access token and a refresh token are generated, as displayed in the following response sample. 

    **Response sample**

        {"access_token":"EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"37e521b0ec5f035c86f0a2db09fe73cda934235e"}

3. Write down your access token and your refresh token. 
    > [Info]  Access (also called bearer) tokens are short-lived. You can generate further access tokens with your refresh token.

### Step 4: Send a test authentication request

You can now send a request to your Core1 instance to check that the access token is valid. For exemplary purposes, we are using a simple "ping-pong" authentication test. 

[comment]: <> (ping-pong method/test? Übliche standard Test-Prozedur? Hat das einen konkreten Namen?)

1. Send an authentication test request, as displayed in the following request sample.  

    **Request sample**

        curl -X POST \
        -H 'Authorization: Bearer EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2' \
        'https://[your-workspace].actindo.com/Actindo.CoreModules.Tools.TenantTest.ping?ping=42'

    Replace *your-workspace* with the name of your instance, and the example values with your access token (bearer) code that you have obtained in [Step 3: Generate an access token](#step-3-generate-an-access-token). 

2. If the access token is valid, a success response is returned, as displayed in the following response sample.

    **Response sample**

        {"pong":"42","success":true,"displayMessage":null,"displayMessageTitle":null,"error":null,"job_id":null}'



### Step 5: Generate an access token from refresh token

Access tokens are valid for a limited period of time. If your access token is expired, you can get a new one using your refresh token.

1. Send the token URL request to generate your access token, as displayed in the following request sample.  
    
    **Request sample** 

        curl -X POST 'https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken' \
        -H 'Content-Type: application/x-www-form-urlencoded' \
        -H 'cache-control: no-cache' \
        -d 'grant_type=refresh_token&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&refresh_token=37e521b0ec5f035c86f0a2db09fe73cda934235e'

    Replace *your-workspace* with the name of your instance, and the example values with your client ID, client secret, and the refresh token that you have obtained in [Step 3: Generate an access token](#step-3-generate-an-access-token).  


2. The access token is generated, as displayed in the following response sample. 

    **Response sample** 

        {"access_token":"3lUNK4D\/eiiVg4hM1iJ+lK1b6n+qNflykDyI+laWLQL3P8O8Xmuu3AkfmjnWYUaIdZ\/1r\/6ybfgh4IXHLOFZ0R78rZH89Hk7teOTpsGqPsreiguqOT92WklHU9pTBTNb","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"cca31dc1bdf4c85b892804424b3a5f3ee44368aa"}

    > [Info] 
    You also get a new refresh token.  
    Make sure you keep it safely for future reference!

        


[comment]: <> (Send your first request?)