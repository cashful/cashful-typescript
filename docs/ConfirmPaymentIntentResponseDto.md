
# ConfirmPaymentIntentResponseDto


## Properties

Name | Type
------------ | -------------
`paymentIntent` | [PaymentIntentResponseDto](PaymentIntentResponseDto.md)
`iveriParams` | object
`iVeri3dsEndpoint` | string
`sandboxMode` | boolean
`status` | string
`transactionId` | string
`authCode` | string
`amount` | number
`currency` | string
`reason` | string

## Example

```typescript
import type { ConfirmPaymentIntentResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "paymentIntent": null,
  "iveriParams": null,
  "iVeri3dsEndpoint": null,
  "sandboxMode": null,
  "status": null,
  "transactionId": null,
  "authCode": null,
  "amount": null,
  "currency": null,
  "reason": null,
} satisfies ConfirmPaymentIntentResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConfirmPaymentIntentResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


