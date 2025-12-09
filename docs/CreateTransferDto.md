
# CreateTransferDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`fromCustomerId` | string
`toCustomerId` | string
`amount` | number
`currency` | string
`description` | string

## Example

```typescript
import type { CreateTransferDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "fromCustomerId": null,
  "toCustomerId": null,
  "amount": null,
  "currency": null,
  "description": null,
} satisfies CreateTransferDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateTransferDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


