# ACTION
Returns all outlets.

### changelog

##Request
### End Point
  > GET mobile_api/v1/outlets

### Parameters

none

### Example:
  > mobile_api/v1/outlets


##Response

###Status
  > 200 OK

###Payload

A list of outlets and metadata:

- **xxx:** TODO Rob

###Example
```json
{
  "outlets" : [
    {
      "logo_image_url" : "https://posboss-production.s3.amazonaws.com/uploads/items/0f6aa180-0c48-0131-9fc5-064f8ffec43c/medium.png?1380577747",
      "name" : "Coffee 86",
      "promotional_slogan" : "Best coffee in Wellington",
      "street_address" : "123 Lambton Quay, Wellington",
      "uuid" : "DD2A3476-AE5D-4232-B85B-E0E03803BC0D",
      "available_to_order" : true,
      "menu_last_updated_at" : "2015-11-03T17:16:16+13:00",
	   "opening_hours" : "12:30 - 5:00 Sunday,...",
	   "telephone" : "555-5555"
    },
  ]
}
```
