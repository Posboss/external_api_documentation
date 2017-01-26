# Order History

Returns the orders of the customer in date order (newest first). For the outlet it returns the same information as the outlets API returns, and should match the schema exactly.

## Request

### End Point
> GET mobile_api/v1/order_history

### Parameters

none

## Response

### Status

200 ok

### Payload

    {
      "order_history": [
        {
          "date": "2017-01-26T11:01:54+13:00",
          "outlet": {
            "hero_image_url": "/assets/missing.png",
            "logo_image_url": "/assets/missing.png",
            "name": "Meta Kiehn I",
            "opening_hours": [
              {
                "days": "Monday-Friday",
                "hours": "9-5"
              }
            ],
            "uuid": "cea92020-c577-0134-fdab-745c89b8cc09",
            "available_to_order": true,
            "menu_last_updated_at": "2017-01-26T11:01:54+13:00",
            "venue_type": null,
            "street_address": null,
            "phone_number": null,
            "website_url": null,
            "facebook_url": null,
            "instagram_url": "",
            "twitter_url": ""
          },
          "order_items": []
        },
        {
          "date": "2017-01-26T14:25:59+13:00",
          "outlet": {
            "hero_image_url": "/assets/missing.png",
            "logo_image_url": "/assets/missing.png",
            "name": "Marion McLaughlin",
            "opening_hours": [
              {
                "days": "Monday-Friday",
                "hours": "9-5"
              }
            ],
            "uuid": "50b64490-c594-0134-fe0b-745c89b8cc09",
            "available_to_order": true,
            "menu_last_updated_at": "2017-01-26T14:25:58+13:00",
            "venue_type": null,
            "street_address": null,
            "phone_number": null,
            "website_url": null,
            "facebook_url": null,
            "instagram_url": "",
            "twitter_url": ""
          },
          "order_items": [
            {
              "item_uuid": "50cecbe0-c594-0134-fe0e-745c89b8cc09",
              "item_name": "Practical Linen Shirt",
              "notes": "MyString",
              "multiplier": "2.0",
              "order_item_mods": [
                "5808aad2-b706-559d-b491-a84d873e1385",
                "78088452-057d-5f3b-a8a0-9c215c0d85df"
              ]
            }
          ]
        }
      ]
    }
