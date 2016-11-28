# Nearby Outlets  
Returns the a list of the basic information of nearby outlets if a lat long is supplied
Otherwise will return a list of hero outlets decided by posboss


This the nearby outlets and the regulars object, are identical

### changelog

##Request
### End Point
  > GET mobile_api/v1/nearby_outlets

### Parameters

- **lat:** (Optional)
- **long:** (Optional)

### Example:
  > GET mobile_api/v1/nearby_outlets?lat=38.8977long=77.0365


##Response

###Status
  > 200 OK

###Payload

- nearby_outlets: (Array) 
 - **id:** (String) The outlets uuid
 - **lat:** () 
 - **long:** () 
 - **logo_image_url:** (String) url of the outlets Logo image
 - **name:** (string) name of the outlet


###example
```json
{
  "nearby_outlets" : [
    {
      "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
      "name": "Five Burrows",
      "lat": "",
      "long": "",
      "logo_image_url": "https://s3-ap-southeast-2.amazonaws.com/posboss-production/uploads/profiles/265a42f0-c444-0132-0c7d-021161b97956/medium.png"
    }
  ]
}
```
