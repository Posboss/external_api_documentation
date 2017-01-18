# Available To Order
Returns whether the outlet is open and the user is able to order

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
  "available_to_order" : false
}
```
