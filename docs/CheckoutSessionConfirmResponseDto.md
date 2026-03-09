
# CheckoutSessionConfirmResponseDto


## Properties

Name | Type
------------ | -------------
`sessionId` | string
`paymentIntentId` | string
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
import type { CheckoutSessionConfirmResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "sessionId": null,
  "paymentIntentId": null,
  "iveriParams": null,
  "iVeri3dsEndpoint": null,
  "sandboxMode": null,
  "status": null,
  "transactionId": null,
  "authCode": null,
  "amount": null,
  "currency": null,
  "reason": null,
} satisfies CheckoutSessionConfirmResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionConfirmResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


