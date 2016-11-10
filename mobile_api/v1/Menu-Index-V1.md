# ACTION
Returns the current mobile menu structure for an outlet. The response payload contains uuids of items on the menu.

### changelog

##Request
### End Point
  > GET mobile_api/v1/outlets/:outlet_uuid/menu

### Parameters

**outlet_uuid:** The uuid of the customers whose menu should be returned

### Example:
  > mobile_api/v1/outlets/1427DFF5-53CF-44BB-BF47-420F1D1D0F99/menu


##Response

###Status
  > 200 OK

###Payload

- **uuid:** (String) The uuid of the mobile menu
- **last_updated_at:** (String) RFC3339 Timestamp of last time menu was saved
- **pages:** (Array of Objects)
  - **name:** (String) - The page name
  - **sections:** (Array of objects)
    - **name:** (String) Title of this section
    - **sort_order:** (Number) 0-based index for display of this section
    - **section_items:** (Array) List of item uuids in this section


###Example
```json
{
  "menu": {
    "uuid": "E3CABE53-B9E4-420A-BBEA-E72E4F233BC1",
    "last_updated_at": "2015-11-03T17:16:16+13:00",
    "pages": [
      {
        "name": "Coffee",
        "sections" : [
          {
            "uuid" : "98FAFE91-3610-44BE-9E83-F73A1465C2CE",
            "name" : "Hot Drinks",
            "sort_order" : 0,
            "section_items" : [
              "BDEFC7DF-5716-4E25-8335-1B10A53DBA19",
              "064ABFF6-5BF0-47E5-B37C-27C67C66A2A0"
            ]
          }
        ]
      }
    ]
  }
}
```
