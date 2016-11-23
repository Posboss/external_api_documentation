# Nearby Outlets  
Returns the 

### changelog

##Request
### End Point
  > GET mobile_api/v1/regulars

### Parameters

- **lat:** 
- **long:**

### Example:
  > GET mobile_api/v1/regulars?lat=38.8977long=77.0365


##Response

###Status
  > 200 OK

###Payload

- nearby_outlets: (Array) 
 - **id:** (String) The outlets uuid
 - **lat:** () 
 - **long:** () 
 - **image_url:** (String) url of the outlets hero image
 - **name:** (string) name of the outlet


###example
```json
{
  "nearby_outlets" : [
    {
      "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
      "name": "Eminem",
      "lat": "Marshall Mathers",
      "long": "eminem@gmail.com",
      "image_url": "https://eat24-files-live.s3.amazonaws.com/cuisines/v4/cafe.jpg?Signature=7lRr4TRudF64MCWz9U54Ovw9BbM%3D&Expires=1479941955&AWSAccessKeyId=AKIAIEJ2GCCJRT63TBYA"
    }
  ]
}
```
