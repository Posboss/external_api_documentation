# Update Customer

Updates the current logged in customer

## Request
### End Point
  > PUT mobile_api/v1/customer

### Parameters

- **customer:**
  - **preferred_name:** (String, null)
  - **name:** (String)
  - **email:** (String)
  - **phone_number:** (String, null)
  - **emoji:** (String, null)


## Response

```json
{
  "customer": {
    "preferred_name": "Eminem",
    "name": "Marshall Mathers",
    "email": "eminem@gmail.com",
    "phone_number": "021 111 1111",
    "emoji": "🍆"
  }
}
```

### Status
  > 200 OK

### Payload

- **customer:**
 - **id:** (String) - Uuid
 - **preferred_name:** (String,  null)
 - **name:** (String)
 - **email_address:** (String, null)
 - **phone_number:** (String, null)
 - **emoji:** (String)

### Example

```json
{
  "customer": {
    "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
    "preferred_name": "Eminem",
    "name": "Marshall Mathers",
    "email": "eminem@gmail.com",
    "phone_number": "021 111 1111",
    "emoji": "🍆"
  }
}
```
