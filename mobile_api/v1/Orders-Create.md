# Orders
Creates a new order for an outlet and a customer

##Request
### End Point
  > GET mobile_api/v1/outlets/:outlet_uuid/orders

### Parameters

- **order:**
  - **uuid**
  - **date** A timestamp of when the order was created
  - **order_items**
    - **uuid**
    - **item_uuid**
    - **notes**
    - **multiplier** How many of this order item were ordered
    - **modifications** A list of modification uuids

### Example:
  > mobile_api/v1/outlets/1427DFF5-53CF-44BB-BF47-420F1D1D0F99/modifications


##Response

###Status
  > 201 Created

###Payload

none


###Example
```json
{
  "order": {
    "uuid": "5fe71fa1-4087-41bf-87e5-9453cec6a3c8",
    "date": "2016-11-30T11:01:00+13:00",
    "order_items": [
      {
        "uuid": "e006e302-7758-4b78-92f8-0866bfdbac43",
        "item_uuid": "ea6822b7-848f-4de5-8ae8-8926073cbd42",
        "notes": "Put the mustard on the side",
        "multiplier": 2,
        "modifications": [
          "463cc4e3-e557-4603-be0d-173100ff4fd7",
          "fced428f-db72-4be5-b2ce-d0d52e2f7ba6"
        ]
      }      
    ]
  }
}
```
