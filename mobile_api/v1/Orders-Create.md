# Orders
Creates a new order for an outlet and a customer

##Request
### End Point
  > POST mobile_api/v1/outlets/:outlet_uuid/orders

### Parameters

- **order:**
  - **date** An ISO timestamp of when the order was created
  - **order_items**
    - **item_uuid**
    - **notes**
    - **multiplier** How many of this order item were ordered
    - **modifications** A list of modification uuids
    - **order_item_mod_groups**
      - **uuid** uuid of the mod group, as the same mod can be in multiple groups
      - **order_item_mods** List of mod uuids

### Example:
  > mobile_api/v1/outlets/1427DFF5-53CF-44BB-BF47-420F1D1D0F99/orders
  
###Example
```json
{
  "order": {
    "date": "2018-03-30T03:30:58.425Z",
    "order_items": [
      {
        "item_uuid": "ea6822b7-848f-4de5-8ae8-8926073cbd42",
        "notes": "Put the mustard on the side",
        "multiplier": 2,
        "order_item_mod_groups": [
          {
            "uuid": "f7beae9f-4907-5357-aedb-0a445d409af6",
            "order_item_mods": [
              "463cc4e3-e557-4603-be0d-173100ff4fd7",
              "fced228f-dc72-4be5-b2fe-d0d52e2f7ba6"
            ]
          },
          {
            "uuid": "a2b381cf-3352-5409-880b-0c51be85af1a",
            "order_item_mods": [
              "99bf24be-1675-5b5d-ad93-bffc94776535",
              "793dca56-bf22-5f77-a56e-a97bfa0241c8"
            ]
          }
        ]
      }      
    ]
  }
}
```

##Response

###Status
  > 201 Created

###Payload

none


