
# EvervaultEncryptedCardDto


## Properties

Name | Type
------------ | -------------
`pAN` | string
`expiryDate` | string
`cardSecurityCode` | string
`cardholderName` | string

## Example

```typescript
import type { EvervaultEncryptedCardDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "pAN": ev:encrypted:ABC123...,
  "expiryDate": ev:encrypted:DEF456...,
  "cardSecurityCode": ev:encrypted:GHI789...,
  "cardholderName": ev:encrypted:JKL012...,
} satisfies EvervaultEncryptedCardDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EvervaultEncryptedCardDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


