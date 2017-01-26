# Pending Accounts Payment 

The account payments that will occurr at the next billing cycle

##Request
### End Point
  > GET mobile_api/v1/pending_account_payments

##Response

###Status
  > 200 OK

###Payload

- **pending_account_payments:(Array)**
 - **number_of_transactions:** (Integer) - How many payments the user made this week
 - **outlet_id:** (String) The outlet id this payment will be made to
 - **preferred_name:** (String, null)
 - **currency:** (String) 'NZD'
 - **tax_inclusive:** (String)
 - **tax_exclusive:** (String)
 - **tax_rate:** (String)
 - **tax_amount:** (String)

###Example

```
json
{
  "customer" : {
    "id": "E9A3450B-B94A-43FB-A085-E33E25D2EE00",
    "preferred_name": "Eminem",
    "name": "Marshall Mathers",
    "email": "eminem@gmail.com",
    "phone_number": "021 111 1111"
  }
}
```
