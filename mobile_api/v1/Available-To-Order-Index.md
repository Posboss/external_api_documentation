# Available To Order
Returns whether the outlet is open and the user is able to order, a reason for why ordering is not available (e.g. closed)  can be returned if ordering is not available.

##Request
### End Point
  > mobile_api/v1/:outlet_uuid/available_to_order

### Parameters

none

### Example:
> GET mobile_api/v1/:outlet_uuid/available_to_order

##Response
###Status
  > 200 OK

###Payload
- **available_to_order:** (boolean)
- **reason:** (string)

###Example
```json
{
  "available_to_order" : false,
  "reason": "It is night time"
}
```
