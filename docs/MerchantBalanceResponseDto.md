
# MerchantBalanceResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`merchantId` | string
`amount` | number
`currency` | string
`available` | number
`pending` | number

## Example

```typescript
import type { MerchantBalanceResponseDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "merchantId": null,
  "amount": null,
  "currency": null,
  "available": null,
  "pending": null,
} satisfies MerchantBalanceResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MerchantBalanceResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


