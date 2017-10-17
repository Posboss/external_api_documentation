# Available To Order
Returns whether the outlet is open and the user is able to order, a reason for why ordering is not available (e.g. closed)  can (optionallu) be returned if ordering is not available.

##Request
### End Point
  > mobile_api/v1/outlets/:outlet_uuid/available_to_order

### Parameters

none

### Example:
> GET mobile_api/v1/outlets/:outlet_uuid/available_to_order

##Response
###Status
  > 200 OK

###Payload
- **code:** (string) one of the following [ 
      "mobile_ordering_disabled",
      "no_mobile_ordering",
      "closed",
      "available"
    ]
- **available:** (boolean) required whether or not this place is available to order
- **message:** (string) required

###Example
```json
{
  "available_to_order" : false,
  "reason": "It is night time"
}
```
