
# InitiatePaymentDto


## Properties

Name | Type
------------ | -------------
`amount` | number
`currency` | string
`merchantId` | string
`evervaultEncryptedCard` | [EvervaultEncryptedCardDto](EvervaultEncryptedCardDto.md)
`paymentIntentId` | string
`maskedPan` | string
`tokenizeCard` | boolean
`firstName` | string
`lastName` | string
`phoneNumber` | string
`paymentDescription` | string
`merchantName` | string
`metadata` | object

## Example

```typescript
import type { InitiatePaymentDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "amount": 10000,
  "currency": ZAR,
  "merchantId": mer_abc123,
  "evervaultEncryptedCard": null,
  "paymentIntentId": pi_xyz789,
  "maskedPan": ************1234,
  "tokenizeCard": null,
  "firstName": John,
  "lastName": Doe,
  "phoneNumber": +27123456789,
  "paymentDescription": Payment for order #12345,
  "merchantName": Acme Store,
  "metadata": {"orderId":"12345","customField":"value"},
} satisfies InitiatePaymentDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InitiatePaymentDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


