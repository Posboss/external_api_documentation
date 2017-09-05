# Regulars  Index
Returns the current customer's regular outlets

### changelog

## Request
### End Point
  > GET mobile_api/v1/regulars

### Parameters

none

### Example:
  > GET mobile_api/v1/regulars

## Response

### Status
  > 200 OK

### Payload

A list of customers regular outlets:

- **regulars**: (Array)
 - **uuid:** (String) an Outlet UUID
 - **lat:** (String) WGS-84 latitude of the outlet
 - **long:** (String) WGS-84 longitude of the outlet
 - **logo_image_url:** (String) url of the outlet's Logo image
 - **hero_image_url:** (String) url of the hero image for the outlet
 - **name:** (string) name of the outlet

###Example
```json
{
  "regulars": [
    {
      "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
      "name": "Five Boroughs",
      "lat": "45.909304",
      "long": "-9.074411",
      "logo_image_url": "https://posboss-feature.s3.amazonaws.com/uploads/outlets/25a04190-7536-0133-ddbf-022efe9defe5/large.jpg?1504474941",
      "hero_image_url": "https://posboss-feature.s3.amazonaws.com/uploads/outlets/25a04190-7536-0133-ddbf-022efe9defe5/hero_image/large.jpg?1504576015"
    }
  ]
}
```
