# Get started

[comment]: <> (Diese Info gilt für alle APIs bzw. alle Module. Falls andere Module dokumentiert, darauf verweisen oder auf eine übergeordnete Ebene verschieben)

This API reference documentation provides general information on the main resources, such as products, and request samples to perform the most usual API calls. It is not meant to be exhaustive, but to provide you with a starting point to understand how the *Actindo Core1 OpenAPI* works. 

A complete API documentation, organized by module, is available in the *Actindo Core1 Platform* under *Dev Tools > API > Tab API > Module name*. The API documentation is automatically generated based on your specific module configuration. Therefore, the available modules, endpoints, and attributes contained in your *Actindo Core1 OpenAPI* documentation are the ones relevant for your current instance.


## How to use the request samples

The request samples provided in this documentation are complete and ready to use, but they require some customization. 

In the following, an example is given using one of the request samples provided in the API reference documentation. 



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

You want to create a single product (that is, without variants), for example, a handbag. You market your products in your online shop to English and Spanish-speaking customers. 


| Product       | Information  | Attribute key     | Value    |
|---------------|--------------|----------------|----------| 
| **SKU**       | HNDBG-1      | sku            | HNDBG-1  |
| **Type**      | Accessories  | attributeSetId | 412 (see **Notes** below) |
| **English name** | Handbag   | _pim_art_name__online_shop__en_US  | Handbag  |
| **Spanish name** | Bolso     | _pim_art_name__online_shop__es_ES  | Bolso |
| **English description** | Vegan leather crossbody handbag | _pim_products_description__online_shop__en_US | Vegan leather crossbody handbag |
| **Spanish description** | Bolso bandolera de cuero vegano | _pim_products_description__online_shop__de_DE | Bolso bandolera de cuero vegano |


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

- The *"sku"* is a required attribute to create a product. You can choose it freely depending on your SKU structure, as long it is a string, that is, a sequence of characters. For detailed information, see [The product object](./05_ManageProducts.md#the-product-object).
- The *"attributeSetId"* represents the product type and is a required attribute to create a product. Attribute sets must be previously created in the *PIM* or the *DataHub* modules based on your product structure. For detailed information, see [Attribute sets](./03_KeyConcepts.md#attribute-sets). To find out the attribute set, or any other entity, ID, see [Retrieve entity data](./04_RetrieveEntityData.md).
-  The attributes provided are the standard Actindo attributes contained in the *PIM basic set*. If you have created your own attributes and attribute sets, the attribute names will probably differ. If desired, you can get a list of all attributes created in an attribute set via API, see [List the attributes in an attribute set](./04_RetrieveEntityData.md#list-the-attributes-in-an-attribute-set).   
- The scope (with the key *online_shop* in this example) and languages (language codes *en_US* and *es_ES*) must also be specified accordingly. 



## Set up the OAuth authorization

The *Actindo Core1 Platform* uses the OAuth 2.0 open protocol to handle client authorization for API access. To make authenticated API requests, you need to set up the OAuth authorization first.


### Step 1 &ndash; Register the client app

If you want to gain access to the *Actindo Core1 Platform* from an external app via API, first of all you have to register the client app in the developer portal. 

#### Prerequisites

- An app for client access is available. 
- A user has been created.
- The user has the appropriate rights.

#### Procedure

*Dev Tools > API > Tab APP REGISTRATIONS*

![App registrations](../../Assets/Screenshots/PIM/API/AppRegistrations.png "[App registrations]")

1. Click the ![App registrations](../../Assets/Icons/Plus01.png "[App registrations]") button to add an app registration.  
    The *Create* view is displayed.

    ![Create app registration](../../Assets/Screenshots/PIM/API/CreateAppRegistration.png "[Create app registration]")

2. Enter a name for the app registration in the *Name* field. For the sake of clarity, it is recommended to use the client app name.

3. Enter a valid client ID in the *Application (client) ID* field. You can freely define your client ID, but it is recommended to use a UUID generator tool, such as [UUID Generator](https://www.uuidgenerator.net/version4 "[https://www.uuidgenerator.net/version4]"), to generate a UUID (universally unique identifier).

    The client ID for the *Actindo Core1 Platform* must comply with the following requirements:
    - between 4 and 31 characters long  
    - allowed characters include upper and lower cases letters, numbers, and underscore
    - beginning with a letter  

[comment]: <> (Andreas: Kannst du bitte die Information oben bestätigen bzw. verbessern? Laut Oli ist es wahrscheinlich auch mit einer Zahl am Anfang möglich. UI muss verbessert werden, da Toggle darunter auch nicht wirklich funktioniert.)

4. If available in your version, leave the *Only authentication scopes open ID profile email. You will not be able to call any methods besides getting profile data* toggle disabled.

5. Enter an appropriate redirect URI in the *Redirect URI* field. For exemplary purposes, [https://oauthdebugger.com/debug](https://oauthdebugger.com/debug/ "[https://oauthdebugger.com/debug]") is used. See the following screenshot for reference.

    ![App registration example](../../Assets/Screenshots/PIM/API/AppRegistrationExample.png "[App registration example]")

6. Click the [SAVE] button.  
    The app registration is saved. The client secret is displayed.

    > [Caution]   
    The client secret is displayed only once.  
    Make sure you copy it and keep it safe for future reference.


### Step 2 &ndash; Get an authorization code

An authorization code is a temporary code provided by an authorization server. This code is then used by the client app to exchange for an access token. Once you have the access token, you can send authenticated requests and access the information via API. 

Bear in mind that you need to get an authorization code for each instance you want to access via API.

> [Caution]  
    Before continuing, make sure you are not logged into your system instance. Otherwise, the authorization code will be linked to your user profile. That means that any API requests made subsequently will be made on your user's behalf.

Following the example provided in [Step 1 &ndash; Register the client app](#step-1-–-register-the-client-app), the process is described using the [https://oauthdebugger.com/](https://oauthdebugger.com/ "[https://oauthdebugger.com/]") website. You can also use another third-party website or your own system. 

#### Prerequisites

You have registered the client app, see [Step 1 &ndash; Register the client app](#step-1-–-register-the-client-app).

#### Procedure

*OAuth debugger*

![OAuth debugger](../../Assets/Screenshots/PIM/API/OAuthDebugger.png "[OAuth debugger]")

1. Enter the authorization URI (Uniform Resource Identifier) in the *Authorize URI (required)* field. In this case, your URI should look like this:

    **https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2.authorize**

    Replace *[your-workspace]* with the name of your instance. Bear in mind that the authorization is instance-specific.

2. Enter **https://oauthdebugger.com/debug** in the *Redirect URI (required)* field.

3. Enter your client ID in the *Client ID (required)* field. You have defined your client ID previously in the client app registration.

4. Enter **profile** in the *Scope (required)* field.

5. Leave the *State* and *Nonce* fields as they are. They are automatically generated.

6. Click the *code* checkbox in the *Response type (required)* section.

7. Select the *form_post* radio button in the *Response mode (required)* section. 

8. Click the [SEND REQUEST] button.  
    If the authorization flow is successful, OAuth debugger displays a success message with an authorization code, such as in the following screenshot: 

    ![OAuth debugger success](../../Assets/Screenshots/PIM/API/OAuthDebuggerSuccess.png "[OAuth debugger success]")
    
9. Log in to the *Actindo Core1 Platform* with the user credentials (username and password) you want to authorize for API access.  
    The authorization code is now linked to the logged in user.

    ![Core1 Login](../../Assets/Screenshots/PIM/API/Core1Login.png "[Core1 Login]")

[comment]: <> (Andreas: Stimmt der letzter Schritt? Braucht man sonst einen Schritt dazwischen, z.B. Benutzer mit speziellen Rechten erstellen? Oder solange ein beliebiger Benutzer den authorization flow durchgeführt hat, kann er danach API requests senden?)



### Step 3 &ndash; Generate an access token

Once you have obtained an authorization code, you can generate an access token for authentication.

Use a cURL command line tool for the following steps.

#### Prerequisites

- You have your client ID. You have defined it when registering the client app.
- Your have your client secret. It is displayed when saving the app registration, see [Step 1 &ndash; Register the client app](#step-1-–-register-the-client-app).
- You have your authorization code. You have obtained it in [Step 2 &ndash; Get an authorization code](#step-2-–-get-an-authorization-code).

#### Procedure

1. Send the token URL request to generate your access token, as displayed in the following request sample.  

    **Request sample**

        curl -X POST   https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken \
        -H 'Content-Type: application/x-www-form-urlencoded' \
        -H 'cache-control: no-cache' \
        -d 'grant_type=authorization_code&code=5471fdee60b8c9d571f137c0940dfeddfdc4dddb&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&redirect_uri=https%3A%2F%2Foauthdebugger.com%2Fdebug'

    Replace *[your-workspace]* with the name of your instance, and the example values with your client ID, client secret, and authorization code. 

    An access token and a refresh token are returned, as displayed in the following response sample. 

    **Response sample**

        {"access_token":"EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"37e521b0ec5f035c86f0a2db09fe73cda934235e"}

2. Copy and save your access token and your refresh token. 

    > [Info]  Access (also called bearer) tokens are short-lived. You can generate further access tokens with your refresh token. Make sure you keep it safe for future reference.


### Step 4 &ndash; Send a test authentication request

You can now send a request to your *Actindo Core1 Platform* instance to check that the access token is valid. For exemplary purposes, we are using a simple "ping-pong" authentication test. 

#### Prerequisites

You have an access token, see [Step 3 &ndash; Generate an access token](#step-3-–-generate-an-access-token).

#### Procedure

1. Send an authentication test request, as displayed in the following request sample.  

    **Request sample**

        curl -X POST \
        -H 'Authorization: Bearer EYqSCcJOoBgbOxgHJpU3stvliosc+EGEFQ60QplUPjNuCOTfoebG2kvUg5sb574TjI94aEUMBG0I2DS+LulBQj+sXGIl3FX+3QFICEDb1Sw+HzfO1K34QhB60rkULlN2' \
        'https://[your-workspace].actindo.com/Actindo.CoreModules.Tools.TenantTest.ping?ping=42'

    Replace *[your-workspace]* with the name of your instance, and the example values with your access (bearer) token that you have obtained in [Step 3 &ndash; Generate an access token](#step-3-–-generate-an-access-token). 

    If the access token is valid, a success response is returned, as displayed in the following response sample.

    **Response sample**

        {"pong":"42","success":true,"displayMessage":null,"displayMessageTitle":null,"error":null,"job_id":null}'


### Step 5 &ndash; Generate an access token from refresh token

Access tokens are valid for a limited period of time. If your access token is expired, you can get a new one using your refresh token.

#### Prerequisites

You have a refresh token. You have obtained it when generating an access token, see [Step 3 &ndash; Generate an access token](#step-3-–-generate-an-access-token).

#### Procedure

1. Send the token URL request to generate your access token, as displayed in the following request sample.  
    
    **Request sample** 

        curl -X POST 'https://[your-workspace].actindo.com/Actindo.CoreModules.Auth.OAuth2Token.getAccessToken' \
        -H 'Content-Type: application/x-www-form-urlencoded' \
        -H 'cache-control: no-cache' \
        -d 'grant_type=refresh_token&client_id=myclientid&client_secret=1U-YdJpAD67huXxmy0c7Cg__&refresh_token=37e521b0ec5f035c86f0a2db09fe73cda934235e'

    Replace *[your-workspace]* with the name of your instance, and the example values with your client ID, client secret, and the refresh token that you have obtained in [Step 3 &ndash; Generate an access token](#step-3-–-generate-an-access-token).  


    The access token is generated, as displayed in the following response sample. 

    **Response sample** 

        {"access_token":"3lUNK4D\/eiiVg4hM1iJ+lK1b6n+qNflykDyI+laWLQL3P8O8Xmuu3AkfmjnWYUaIdZ\/1r\/6ybfgh4IXHLOFZ0R78rZH89Hk7teOTpsGqPsreiguqOT92WklHU9pTBTNb","expires_in":3600,"token_type":"bearer","scope":"none","refresh_token":"cca31dc1bdf4c85b892804424b3a5f3ee44368aa"}

    > [Info] 
    You also get a new refresh token.  
    Make sure you copy it and keep it safe for future reference.


## Make an API call

Once the authorization flow is successfully completed, you are ready to start making API calls. 

To make an API call to the *Actindo Core1 OpenAPI*, you need to follow the step-by-step sequence below: 

| Step   | Description | Further information |
| :----: | ------------------ | ------------ |
| 1      | Find the endpoint you want to address | Find the relevant use case, for instance in [Create products](./05_ManageProducts.md) or [Create variant products](./06_ManageVariantProducts.md). <br> For a complete list of endpoints, refer to the API documentation of your instance under *Dev Tools > API > Tab API > Module name*. |
| 2      | Check the required attributes | Find the relevant definitions depending on the request you want to send, for instance in [Create products](./05_ManageProducts.md) or [Create variant products](./06_ManageVariantProducts.md). <br> For a complete list of attributes, refer to the API documentation of your instance under *Dev Tools > API > Tab API > Module name*. |
| 3      | Discover the required entity ID(s) | See [Retrieve entity data](./04_RetrieveEntityData.md). | 
| 4      | Create your request payload | Find practical request samples, for instance in [Create products](./05_ManageProducts.md) or [Create variant products](./06_ManageVariantProducts.md). |
| 5      | Send your request | If using an external tool, such as Postman, you need to set it up first. For detailed information, see [Set up Postman](07_SetUpPostman.md). |
| 6      | Interpret the response | See [Response bodies](./01_Overview.md#response-bodies). |