# Available To Order
Returns whether the outlet is open and the user is able to order, a reason for why ordering is not available (e.g. closed)  can be returned if ordering is not available.

##Request
### End Point
  > mobile_api/v1/available_to_order/:outlet_uuid

### Parameters

none

### Example:
> GET mobile_api/v1/available_to_order/:outlet_uuid

##Response
###Status
  > 200 OK

###Payload
- **available_to_order:** (boolean)

###Example
```json
{
  "available_to_order" : false,
  "reason": "It is night time"
}
```
