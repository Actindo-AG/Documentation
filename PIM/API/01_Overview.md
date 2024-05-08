# Overview

[comment]: <> (Diese Info gilt für alle APIs bzw. alle Module. Falls andere Module dokumentiert, darauf verweisen oder auf eine überordnete Ebene verschieben)

In this section, an API documentation for the *Actindo Core1 Platform* is provided...

Use case - what it is used for

The *Actindo Core1 Platform* is highly configurable and expandable, using not only the Actindo App Store, but also including self-developed modules and extensions. Therefore, every *Actindo Core1 Platform* account is unique in its API configuration due to the individual construction of the installed and extended modules.

The *Actindo Core1 OpenAPI* is a web REST API that uses the OpenAPI 3.0 Specification (OAS). It is built based on the API-first approach. With over 500 API endpoints, the Core1 is fully connective and integrative. Every part of the application is accessible through a set of documented API endpoints, which are all accessible through a variety of protocols. 

[comment]: <> (Andere Kompatibilität? SOAP und andere unterstützt? Erwähnenswert? Allgemeine API info, die man noch erwähnen sollte?)

## API general requirements/setup / How the API works 

### Authentication

The *Actindo Core1 Platform* supports two workflows of the OAuth 2.0 protocol to retrieve an access token to make authenticated requests. For detailed information on the authentication flow, see [OAuth authorization flow](02_GetStarted.md#oauth-authorization-flow).

### Methods

The *POST* method is always used for all *Actindo Core1 OpenAPI* endpoints. All other methods are not relevant for communication with the Core1 platform.

### URI

URI stands for Uniform Resource Identifier. It represents the location of a web resource. 

In the *Actindo Core1 OpenAPI*, the URI has the following structure:

**https://your-workspace.actindo.com/API.endpoint**

- *your-workspace* represents the name of your instance.
- *API.endpoint* represents the API endpoint as described in this API reference documentation.

### Headers

Headers contain metadata in key-value pairs that are sent along with HTTP requests and responses. They are essential for the API calls, as they provide additional information for communication between client and server.

The following headers are required for communication with the *Actindo Core1 OpenAPI*:

| Key | Value |
|-----|-------|
| Content-Type  | application/json |
| Accept        | application/json |
| Authorization  | access token <br> See [Generate an access token](./02_GetStarted.md#step-3-generate-an-access-token) |

[comment]: <> (Unsicher, ob das stimmt, und wie authentication/authorization via header/request body funktioniert)

### Response codes

Generally, the *Actindo Core1 OpenAPI* uses the standard HTTP status codes to indicate the success of failure of the API requests. The most usual response codes returned are as follows: 

| Code | Description | Notes |
| ---- | ----------- | ------ |
| 200  | OK          |  Everything worked as expected      |
| 400  | Bad request | Unacceptable request, often due to missing required parameter or  header, e.g. Content-Type: application/json, or malformed json |
| 401  | Unauthorized | Authentication has failed, e.g. due to invalid or missing authentication credentials |
| 429  | Too many requests   | You sent too many requests in a given amount of time |
| 530 | Site frozen | The tenant is currently frozen due to maintenance work, module installations or updates |
| default | Generic error | - | 

For detailed information, see [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes "[https://en.wikipedia.org/wiki/List_of_HTTP_status_codes]").

### Format

The *Actindo Core1 Platform OpenAPI* accepts and returns json body requests. 

## Tools

You can use different software tools to submit your requests, either your own tool or a third-party tool, such as Postman. For a detailed description on how to set up Postman, see [Set up Postman](./07_SetUpPostman.md). 

Regardless of how you submit your requests, you always have to provide the following information:

- URI
- HTTP method 
- Headers
- Request body

[comment]: <> (In Postman habe ich session cookie eingestellt, daher brauche authentication nicht mehr. Wie funktioniert es sonst?)


[comment]: <> (Glossary?)
[comment]: <> (API architecture, API request workflow?)