# Customer Create
Creates a new customer in the database with a google device id.
Alternatively returns the customer if the device has already been recorded.

##Request
### End Point
  > POST mobile_api/v1/customers

### Parameters

**device_id:** (String, Required) The id of the current device

### Example:
  > POST mobile_api/v1/customers

```json
{
  "customer" : [
    {
      "device_id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
    }
  ]
}
```

##Response
###Status
  > 200 OK

###Payload
- **Customer:** (object)
  - **Id:**

###Example
```json
{
  "customer" : {
      "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
      "device_id": "3AB5B680-3144-42AD-96F2-58B6C3E19C28"
    }
}
```
