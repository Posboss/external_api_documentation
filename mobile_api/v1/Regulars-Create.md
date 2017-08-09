# Regular Create
Create a new connection between an outlet and a customer

### changelog

##Request
### End Point
  > POST mobile_api/v1/regulars

### Parameters

**outlet_id:** (String, Required) The id of the outlet to be added as regular

none

### Example:
  > POST mobile_api/v1/regulars

```json
{
  "regulars" : [
    {
      "outlet_id": "df878a02-ef85-5a07-a5d0-2dc5fe6036a5"
    },
    {
      "outlet_id": "f5740122-55e4-51c5-b88a-954571418ab4"
    }
  ]
}
```

##Response

###Status
  > 200 OK

###Payload


###Example
```json
```
