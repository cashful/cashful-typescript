
# PurchaseResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`customerId` | string
`productId` | string
`amount` | number
`currency` | string
`status` | string
`customerBalanceBefore` | number
`customerBalanceAfter` | number
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PurchaseResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "customerId": null,
  "productId": null,
  "amount": null,
  "currency": null,
  "status": null,
  "customerBalanceBefore": null,
  "customerBalanceAfter": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies PurchaseResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PurchaseResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


