
# BalanceTransactionDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`merchantId` | string
`type` | string
`amount` | number
`currency` | string
`description` | string
`relatedEntityId` | string
`relatedEntityType` | string
`balanceAfter` | number

## Example

```typescript
import type { BalanceTransactionDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "merchantId": null,
  "type": null,
  "amount": null,
  "currency": null,
  "description": null,
  "relatedEntityId": null,
  "relatedEntityType": null,
  "balanceAfter": null,
} satisfies BalanceTransactionDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BalanceTransactionDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


