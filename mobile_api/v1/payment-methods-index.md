# Get Payment Methods
Retrieves a list of payment methods for a customer

##Request
### End Point
  > GET mobile_api/v1/payment_methods

### Parameters.

##Response

###Status
  > 200 ok



### Parameters 

- **payment_methods:** (Array)

 - **card_type:** (String) Visa, Mastercard etc
 - **token:** (String) Braintree vault token used for making transactions with a cc
 -  **last_4:** (String) The last 4 digits of the CC


###Payload

```json
{
  "payment_methods": [
    {
      "card_type": "Visa",
      "last_4": "1111",
      "token": "8j334d"
    }
  ]
}
```

