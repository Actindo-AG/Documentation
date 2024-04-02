# Overview

## Introduction

In order for our *Actindo Core1 Digital Operations Platform* to fit into our technology driven era, it has to be fully connective and integrative. This is why our platform is built with the API-first strategy in mind. Every part of the application is accessible through a set of documented API endpoints, which are all accessible through a variety of protocols. 

**Available APIs**  

The *Actindo Core1 Digital Operations Platform* is highly configurable and expandable, using not only the Actindo App Store, but including self-developed modules and extensions. Therefore, every Actindo Core1 account is unique in its APIs due to the individual construction of the installed and extended modules.  

On this page, you will find the API specification of the platform itself, as well as all Actindo modules and extensions in their latest versions. Individual accounts have different versions and vendor profiles. Please log in and navigate to Dev Tools > API in order to get the full documentation connected to your specific account. 

[comment]: <> (Info aus webseite oben - anpassen hier!)

Info to be included:
- Web API
- REST(ful) API
- accepts and returns json body requests
- uses standard HTTP responses codes
- authentication
- verbs (methods) 

[comment]: <> (Endpoint -> It varies depending on version!)

The API allows you to integrate your external app with the *Actindo Core1 Digital Operations Platform*.

[comment]: <> (Benefits of API integration, if relevant to add?)

[comment]: <> (What is required to use the API?)

*Actindo Core1 Platform* uses the OpenAPI 3.0 Specification (OAS). 

[comment]: <> (Stimmt das so? Relevant zu erwähnen?)


## Authentication

The *Actindo Core1 Platform* supports two workflows of the OAuth 2.0 protocol to retrieve an access token to make authenticated requests. For detailed information on the authentication flow, see [OAuth authorization flow](02_GetStarted.md#oauth-authorization-flow).

## Methods 

The *POST* method is always used for all *Actindo Core1 OpenAPI* endpoints. All other methods are not relevant for communication with the Core1 platform.

## Response codes

Generally, the *Actindo Core1 OpenAPI* uses the standard HTTP status codes to indicate the success of failure of the API requests.  The most usual response codes returned are as follows: 

| Code | Description | Notes |
| ---- | ----------- | ------ |
| 200  | OK          |  Everything worked as expected      |
| 400  | Bad request | Unacceptable request, often due to missing required parameter or  header, e.g. Content-Type: application/json, or malformed json |
| 401  | Unauthorized | Authentication has failed, e.g. due to invalid or missing authentication credentials |
| 429  | Too many requests   | You sent too many requests in a given amount of time |
| 530 | Site frozen | The tenant is currently frozen due to maintenance work, module installations or updates |
| default | Generic error | - | 

For detailed information, see [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes "[https://en.wikipedia.org/wiki/List_of_HTTP_status_codes]").

## Format  

The *Actindo Core1 OpenAPI* endpoints accept requests in JSON format. 

## Basic API architecture

[comment]: <> (Graphik)

## Basic API request workflow

[comment]: <> (Graphik)

---

[comment]: <> (type: "numeric"|"date": "<", "<=", ">", ">=", "=", "!="; type="list": "in"; type="string": "like"; type="all": "isNull","isNotNull")




