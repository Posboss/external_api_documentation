# Regulars  Index
Returns the current customers regular outlets

### changelog

##Request
### End Point
  > GET mobile_api/v1/regulars

### Parameters

none

### Example:
  > GET mobile_api/v1/regulars


##Response

###Status
  > 200 OK

###Payload

A list of customers regulars:

- customer_regulars: (Array) 
 - **id:** (String) The outlets uuid
 - **lat:** () 
 - **long:** () 
 - **logo_image_url:** (String) url of the outlets Logo image
 - **name:** (string) name of the outlet

###Example
```json
{
  "regulars" : [
    {
      "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
      "name": "Five Burrows",
      "lat": "",
      "long": "",
      "logo_image_url": "https://eat24-files-live.s3.amazonaws.com/cuisines/v4/cafe.jpg?Signature=7lRr4TRudF64MCWz9U54Ovw9BbM%3D&Expires=1479941955&AWSAccessKeyId=AKIAIEJ2GCCJRT63TBYA"
    }
  ]
}
```
