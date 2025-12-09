
# CreatePurchaseDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`customerId` | string
`productId` | string
`amount` | number
`currency` | string
`quantity` | number

## Example

```typescript
import type { CreatePurchaseDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "customerId": null,
  "productId": null,
  "amount": null,
  "currency": null,
  "quantity": null,
} satisfies CreatePurchaseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreatePurchaseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


