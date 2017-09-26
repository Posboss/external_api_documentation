# Session Refresh

Takes an a refresh_token from /mobile_api/v1/sessions and returns a new auth_token 


### End Point
 > POST mobile_api/v1/sessions/refresh

### Parameters

**refresh_token:** (String, Required) - Refresh_token from /mobile_api/v1/sessions 


## Response

### payload
auth_token: The new authtoken that can be used to authenticate all other requests by adding  as param to all other requests

###Example
```json
{
  "auth_token": "c_N98-s6pyNvRvoKbMDx"
}
```
