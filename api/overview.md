# Overview

This describe overview of API.

## Schema

All API access is over HTTPS. All data of request and response is JSON format.  
Endpoint is ``https://<service-domain>``.  

note.
Development environment is ``http://{version}-dot-<service-domain>.appspot.com/``.

## API Group

API is consist of following groups.

- Authentication API
- Common API
- Account API

### Authentication API

Endpoint Prefix: ``<service-domain>/auth/``

Authentication API provide login & signup functions.
Common & Account APIs are require JSON Web Token(JWT) that login API published.

### Common API

Endpoint Prefix: <service-domain>/common/

Common API provide account-shared data access.

### Account API

Endpoint Prefix: <service-domain>/account/

Account API provide account-oriented data access.

Account API always have account-id after endpoint prefix,
like ``<service-domain>/account/{account-id}``.

User can access only the endpoint of account he belongs.


## Authentication

API authentication system is JWT that login API published.
If authentication required API is called without or invalid JWT, return ``403 Forbidden``.

Login

```
curl -X POST "<service-domain>/auth/login" -H "Content-Type: application/json" -d "{ \"email\": \"user@example.com\", \"password\": \"userpassword\"}"
```

Call API With JWT

```
curl -X GET "<service-domain>/common/something" -H "Authorization: Bearer JWT-String-Here"
```
