# Get Payment Methods
Retrieves a list of payment methods for a customer

##Request
### End Point
  > GETJ mobile_api/v1/payment_methods

### Parameters.

##Response

###Status
  > 200 ok



### Parameters 

- **payment_methods:** (Array)

 -  **card_type:** (String) Visa, Mastercard etc
 - **token:** (String) Braintree vault token used for making transactions with a cc
 -  **image_url:** (String) Url to a cute image of the CC type


###Payload

```json
{
  "payment_methods": [
    {
      "card_type": "Visa",
      "image_url": "https://assets.braintreegateway.com/payment_method_logo/visa.png?environment=sandbox",
      "token": "8j334d"
    }
  ]
}
```

