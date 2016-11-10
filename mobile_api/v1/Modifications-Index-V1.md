# Modications
Returns all Modifcations  from the current mobile menu for an outlet.

##Request
### End Point
  > GET mobile_api/v1/outlets/:outlet_uuid/modifications

### Parameters

none

### Example:
  > mobile_api/v1/outlets/1427DFF5-53CF-44BB-BF47-420F1D1D0F99/modifications


##Response

###Status
  > 200 OK

###Payload

A list of Modifications:

- **modification:** (Object) The Mod
  - **uuid:** (String)
  - **name:** (String) Name of the mod
  - **price:** (Object) The Mod's price
    - **uuid:** (String)
    - **currency:** (String) 'NZD'
    - **tax_inclusive:** (String)
    - **tax_exclusive:** (String)
    - **tax_rate:** (String)
    - **tax_amount:** (String)


###Example
```json
{ 
  "modifications": [
    {
      "uuid" : "cd622410-0c46-0131-9f85-064f8ffec43c",
      "name" : "Cinnamon",
      "price" : {
        "currency" : "NZD",
        "tax_inclusive" : "0.0",
        "tax_exclusive" : "0.0",
        "uuid" : "47B5B0BA-104F-43EF-8F07-307960D104CA",
        "tax_rate" : "15",
        "tax_amount" : "0.0"
      }
    },
    {
      "uuid" : "0F55AADD-825C-4450-A148-6A2C0F0D07C4",
      "name" : "Chocolate",
      "price" : {
        "currency" : "NZD",
        "tax_inclusive" : "0.0",
        "tax_exclusive" : "0.0",
        "uuid" : "359E659F-A20F-45DC-A5E5-611EE178F038",
        "tax_rate" : "15",
        "tax_amount" : "0.0"
      }
    },
    {
      "uuid" : "0BBCBA7E-F146-4710-91E9-CFAD9DA89F36",
      "name" : "T/A",
      "price" : {
        "currency" : "NZD",
        "tax_inclusive" : "0.2",
        "tax_exclusive" : "0.17",
        "uuid" : "94A75C80-16CC-4054-A196-D23CED588443",
        "tax_rate" : "15",
        "tax_amount" : "0.03"
      }
    }
  ]
}
```
