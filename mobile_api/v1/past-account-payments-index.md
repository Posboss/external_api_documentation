# Past Accounts Payment

The past 10 payments made by the customer

## Request

### End Point

> GET mobile_api/v1/past_account_payments

## Response

### Status

> 200 OK

### Payload

* **past_account_payments:(Array)**
* **outlet_id:** (String) The id of the outlet this payment was to
* **outlet_name:** (String) The name of the outlet this payment was made to
* **currency:** (String) 'NZD'
* **tax_inclusive:** (Decimal)
* **tax_exclusive:** (Decimal)
* **tax_rate:** (String)
* **tax_amount:** (Decimal)
* **success:** (Boolean) Whether the payment was successful or not
* **processor_response_text:** (String) The status of the payment
* **occurred_at:** (String) The date the payment was made

### Example

```json
{
  "past_account_payments": [
    {
      "outlet_id": "ca32bab0-c5aa-0134-f355-20c9d0852053",
      "outlet_name": "posBoss Cafe",
      "currency": "NZD",
      "tax_amount": 1.5,
      "tax_exclusive": 8.5,
      "tax_inclusive": 10.0,
      "tax_rate": "15.0",
      "success": true,
      "processor_response_text": "Approved",
      "occurred_at": "2017-01-26T11:01:54+13:00"
    }
  ]
}
```
