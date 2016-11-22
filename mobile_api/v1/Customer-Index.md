# Customer

Returns the customer that is logged in

##Request
### End Point
  > GET mobile_api/v1/customer

##Response

###Status
  > 200 OK

###Payload

- **customer:**
 - **id:** (String) - Uuid
 - **preferred_name:** (String, null)
 - **name:** (String)
 - **email_address:** (String)
 - **phone_number:** (String, null)

###Example

```
json
{
  "customer" : {
    "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
    "preferred_name": "Eminem",
    "name": "Marshall Mathers",
    "email": "eminem@gmail.com",
    "phone_number": "021 111 1111"
  }
}
```
