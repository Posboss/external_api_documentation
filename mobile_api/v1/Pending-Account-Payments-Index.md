# Pending Accounts Payment

The account payments that will occur at the next billing cycle

## Request
### End Point
  > GET mobile_api/v1/pending_account_payments

## Response

### Status
  > 200 OK

### Payload

- **pending_account_payments:(Array)**
 - **number_of_transactions:** (Integer) - How many payments the user made this week
 - **outlet_id:** (String) The outlet id this payment will be made to
 - **outlet_name:** (String) The name of the outlet this payment will be made to
 - **preferred_name:** (String, null)
 - **currency:** (String) 'NZD'
 - **tax_inclusive:** (Decimal)
 - **tax_exclusive:** (Decimal)
 - **tax_rate:** (String)
 - **tax_amount:** (Decimal)

### Example

```json

{
  "pending_account_payments":[
    {
      "number_of_transactions": 1,
      "outlet_id": "ca32bab0-c5aa-0134-f355-20c9d0852053",
      "outlet_name": "posBoss Cafe",
      "currency": "NZD",
      "tax_amount": 1.5,
      "tax_exclusive": 8.5,
      "tax_inclusive": 10.0,
      "tax_rate": "15.0"
    }
  ]
}
```
