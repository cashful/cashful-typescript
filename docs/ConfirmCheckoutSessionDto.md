
# ConfirmCheckoutSessionDto


## Properties

Name | Type
------------ | -------------
`evervaultEncryptedCard` | [EvervaultEncryptedCardDto](EvervaultEncryptedCardDto.md)
`maskedPan` | string
`tokenizeCard` | boolean
`firstName` | string
`lastName` | string
`phoneNumber` | string
`paymentDescription` | string
`merchantName` | string
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { ConfirmCheckoutSessionDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "evervaultEncryptedCard": null,
  "maskedPan": null,
  "tokenizeCard": null,
  "firstName": null,
  "lastName": null,
  "phoneNumber": null,
  "paymentDescription": null,
  "merchantName": null,
  "metadata": null,
} satisfies ConfirmCheckoutSessionDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConfirmCheckoutSessionDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


