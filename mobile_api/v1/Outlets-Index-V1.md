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

**hero_image_url:** (String, Url) - The url of a  hero shot of the premise,  food, or other to show off the outlet.

**logo_image_url:** (String, Url) - The url of the  outlets logo

**name:** (String, Url) - The name of the outlet

**Venue type:** (String) -   [ Bar, Cafe, Resturant, Other ]  What do you want to see here @paperkite?

**Opening hours:**  (String,) - User entered string with opening hours

**phone_number:**  (String)  - Phone Number to contact the outlet

**street_address:** (String) -

**website_url:** (String) -

**facebook_url:** (String) -

**instagram_url:** (String) -

**twitter_url:** (String) -

**uuid:** (String) - The id of the resource

**available_to_order:** (Boolean) - Does this outlet have mobile ordering enabled

**menu_last_updated_at:** (String, DateTime) - The last time the menu was updated


###Example
```json
{
  "outlets" : [
    {
      "logo_image_url" : "https://s3-ap-southeast-2.amazonaws.com/posboss-production/uploads/profiles/265a42f0-c444-0132-0c7d-021161b97956/medium.png",
      "hero_image_url" : "https://posboss-production.s3.amazonaws.com/uploads/items/0f6aa180-0c48-0131-9fc5-064f8ffec43c/medium.png?1380577747",
      "name" : "Coffee 86",
      "opening_hours" : "12:30 - 5:00 Sunday,...",
      "phone_number" : "555-5555",
      "street_address" : "123 Lambton Quay, Wellington",
      "website_url" : "https://www.coffee86.co.nz",
      "facebook_url" : "https://facebook.com/cafe86nz",
      "instagram_url" : "https://instagram.com/cafe86nz",
      "twitter_url" : "https://twitter.com/cafe86nz",
      "uuid" : "DD2A3476-AE5D-4232-B85B-E0E03803BC0D",
      "available_to_order" : true,
      "menu_last_updated_at" : "2015-11-03T17:16:16+13:00"
    }
  ]
}
```
