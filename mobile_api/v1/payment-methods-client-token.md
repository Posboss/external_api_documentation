# Client Token
Get the client token used to create payment nonces with braintree 
see [Braintree Overview Doc](https://developers.braintreepayments.com/start/overview)

##Request
### End Point
  > GET mobile_api/v1/payment_methods/client_token

##Response

###Status
  > 201 Created

###Payload

client_token: (String) The braintree client token used to get the payment method_nonce

###Example
```json
{
  "client_token": "eyJ2ZXJzaW9uI....=="
}
```
