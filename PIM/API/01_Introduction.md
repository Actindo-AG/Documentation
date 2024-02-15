# Introduction

## General information

API vs UI   
Nutzen/Vorteil 


OpenAPI V3 format


## Authentication

**Security Scheme Type**: OAuth2  
**authorizationCode OAuth Flow**  
Authorization URL: /Actindo.CoreModules.Auth.OAuth2.authorize  
Token URL: /Actindo.CoreModules.Auth.OAuth2Token.getAccessToken  




How to pass parameters in JSON format in Postman?
Add the following to the headers: "Content-Type: application/json". This setting specifies that the data being sent in the request body is in JSON format.


## Best practices

To send requests to the *Actindo Core1 Platform* API endpoints, you need to use an external API tool, such as Postman. For detailed information on download, configuration and basic functions, see the [Postman](https://www.postman.com/ "[https://www.postman.com/]") website.

- Postman

[comment]: <> (Braucht man configuration?)

https://actindo.atlassian.net/wiki/spaces/CW/pages/33193985/How+to+configure+postman+and+make+an+API+call


- Collections
- Calls 
    - vordefinieren (Vorlagen) 
    - exportieren 
    - share (Cloud)

## Methods 

The *POST* method is always used for all Actindo API endpoints. All other methods are not relevant for communication with the Core1 platform.


## Response codes

The response codes correspond the standard HTTP status codes. For detailed information, see [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes "[https://en.wikipedia.org/wiki/List_of_HTTP_status_codes]").
