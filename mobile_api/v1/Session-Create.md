# Session Create

Takes a google id_token and returns posboss access_token used to access all the rest of the posboss mobile apis.

## High Level Overview

User wants to use a posboss resource.

App presents a google login form.

User enters email and password.

User approves permissions from google.

Google returns a id_token to the app.

The app sends the id_token to the server at POST mobile_api/v1/sessions

Server verifies the id_token with google.

Server then returns a auth token for the device.

THe app can now use this auth token for all futher requests


### End Point
 > POST mobile_api/v1/sessions

### Parameters

**token:** (String, Required) - Base64 encoded JWT token return from google as id_token


## Response

### payload
auth_token: The authtoken that can be used to authenticate all other requests by adding  as param to all other requests

###Example
```json
{
  "auth_token": "c_N98-s6pyNvRvoKbMDx"
}
```
