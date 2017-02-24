# Item index
Returns all items from the current mobile menu for an outlet.

### changelog

##Request
### End Point
  > GET mobile_api/v1/outlets/outlet_uuid:/items

### Parameters

none

### Example:
  > mobile_api/v1/outlets/1427DFF5-53CF-44BB-BF47-420F1D1D0F99/items


##Response

###Status
  > 200 OK

###Payload

A list of items:

- **image_url:** (String) URL of the image
- **name:** (String) Name of the item
- **description:** (String) Description of the item
- **uuid:** (String)
- **price:** (Object) The Mod's price
	- **uuid:** (String)
	- **currency:** (String) 'NZD'
	- **tax_inclusive:** (String)
	- **tax_exclusive:** (String)
	- **tax_rate:** (String)
	- **tax_amount:** (String)
- **item_mod_groups:** (Array) List of mod groups
	- **uuid:** (String)
	- **name:** (String) Name of mod group
	- **required_mod_count:** : (Number) How many of the selected mods are required, (1 
	- **sort_order:** (Number) 0-based index for this mod group
  for required, 0 for optional)
	- **item_mods:** (Array) List of item mods
		- **uuid:** (String) The uuid of the item mod itself
		- **favourite:** (Bool) - Is this mod on by default
		- **sort_order:** (Number) 0-based index for this item mod
		- **modification_uuid:** (String) The Mod uuid this links up with


###Example
```json
{
 "items": [
    {
      "image_url" : "https://posboss-production.s3.amazonaws.com/uploads/items/0f6aa180-0c48-0131-9fc5-064f8ffec43c/medium.png?1380577747",
      "name" : "Cappuccino",
      "description" : "Wellington's finest Cappuccino with freshly roasted beans ",
      "uuid" : "0f6aa180-0c48-0131-9fc5-064f8ffec43c",
      "price" : {
        "uuid" : "E83A7B49-F4E2-44DD-89AF-DC904F3CF876",
        "currency" : "NZD",
        "tax_inclusive" : "4.0",
        "tax_exclusive" : "3.4",
        "tax_rate" : "15",
        "tax_amount" : "0.6"
      },
      "item_mod_groups" : [
        {
          "uuid" : "100090b0-0c48-0131-9fd5-064f8ffec43c",
          "name" : "Dusting",
          "sort_order" : 0,
          "required_mod_count" :1 ,
          "item_mods" : [
            {
              "uuid" : "960161c6-8493-5459-9e12-4a68085d0487",
              "favourite" : true,
              "sort_order" : 0,
              "modification_uuid" : "cd622410-0c46-0131-9f85-064f8ffec43c"
            },
            {
              "uuid" : "6a023620-e4bd-5407-ab4f-435f880c1660",
              "favourite" : false,
              "sort_order" : 1,
              "modification_uuid" : "0F55AADD-825C-4450-A148-6A2C0F0D07C4"
            }
          ]
        },
        {
          "uuid" : "DEA6F22C-331C-4CC9-9E78-BAA80F8EBF05",
          "name" : "Optional Modifications",
          "sort_order" : 1,
          "required_mod_count": 0,
          "item_mods" : [
            {
              "uuid" : "34edaabf-2a75-53df-93ce-03449f04b69d",
              "favourite" : false,
              "sort_order" : 0,
              "modification_uuid" :"0BBCBA7E-F146-4710-91E9-CFAD9DA89F36"
            },
            {
              "uuid" : "b0f4eefd-c4a0-5776-b968-7b46e16357ac",
              "favourite" : false,
              "sort_order" : 1,
              "modification_uuid" : "278F4E3B-A1F4-4E67-AAE7-CA1B75BC2EF1"
            }
          ]
        }
      ]
    }
  ]
}
