# Customer 

Returns the customer that is logged in

### changelog

##Request
### End Point
  > GET mobile_api/v1/customer

### Parameters

### Example:
  > mobile_api/v1/outlets


##Response

###Status
  > 200 OK

###Payload

**id:** (String) - Uuid 
**preferred_name:** (String, Optional) 
**name:** (String) 
**email_address:** (String) 
**phone_number:** (String, Optional) 

###Example

```json
{
  "customer" : {
    {
      "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
      "preferred_name": "Eminem",
      "name": "Marshall Mathers",
      "email": "eminem@gmail.com",
      "phone_number": "021 111 1111"
    }
  }
}
```
