# Overview

## Using the API

[comment]: <> (Alternativer Dateiname: Get started / Overview)

What can the API do?
What is required to use the API?


There are two ways to interact with the *Actindo Core1 Platform* - via user interface (user interactive requests) and via API (API requests). You can perform most of actions using both access methods. 

Both methods require authentication. If accessing the Core1 via user interface using a browser, you need to log into the system with your credentials. When the system receives valid credentials, it authenticates the user. The user interactive session is then started. If accessing the Core via API, you use a software, usually a third-party tool, to handle all communication with the system.


[comment]: <> (Benefits of API integration, if relevant to add?)

*Actindo Core1 Platform* uses the OpenAPI 3.0 Specification (OAS). 

[comment]: <> (Stimmt das so? Relevant zu erwähnen?)


## Authentication

| **Security Scheme Type** | **AuthorizationCode OAuth Flow** |
|-------------------------|----------------------|
| OAuth2 | **Authorization URL:** /Actindo.CoreModules.Auth.OAuth2.authorize |
|    | **Token URL:** /Actindo.CoreModules.Auth.OAuth2Token.getAccessToken |

The *Actindo Core1 Platform* supports two workflows of the OAuth2 protocol to retrieve an access token to make authenticated requests.



## Methods 

The *POST* method is always used for all Actindo API endpoints. All other methods are not relevant for communication with the Core1 platform.


## Response codes

The response codes correspond the standard HTTP status codes. For detailed information, see [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes "[https://en.wikipedia.org/wiki/List_of_HTTP_status_codes]").


Endpoint -> It varies depending on version!


## Required attributes  

Attributes can be required or optional. Required attributes must always be provided when sending a request. Required attributes are marked in bold.

## Format  

The *Actindo Core1 OpenAPI* endpoints accept requests in JSON format. 


---

[comment]: <> (type: "numeric"|"date": "<", "<=", ">", ">=", "=", "!="; type="list": "in"; type="string": "like"; type="all": "isNull","isNotNull")




