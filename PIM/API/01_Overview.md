# Overview

[comment]: <> (Diese Info gilt für alle APIs bzw. alle Module. Falls andere Module dokumentiert, darauf verweisen oder auf eine überordnete Ebene verschieben)

## Introduction

The *Actindo Core1 Platform* is built based on the API-first approach. With over 500 API endpoints, the Core1 is fully connective and integrative. Every part of the application is accessible through a set of documented API endpoints, which are all accessible through a variety of protocols. 

The Core1 is highly configurable and expandable, using not only the Actindo App Store, but also including self-developed modules and extensions. Therefore, every Actindo Core1 account is unique in its API configuration due to the individual construction of the installed and extended modules.

On this documentation, you will find a general API specification of the platform itself, as well as common API use cases and examples for different Actindo modules and extensions in the specified versions. Individual accounts have different module versions and vendor profiles. To access the full API documentation specific to you instance, log in to your Core1 instance and navigate to *Dev Tools > API*.

[comment]: <> (Double-check info. Wo kommt es her?)

The *Actindo Core1 Platform API* is a web REST API that uses the OpenAPI 3.0 Specification (OAS). 

[comment]: <> (Supports REST, SOAP, welche andere? Relevant hier?)

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

The *Actindo Core1 Platform API* accepts and returns json body requests. 

## Basic API architecture

[comment]: <> (Graphik)

## Basic API request workflow

[comment]: <> (Graphik)





