
# PayoutResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`amount` | number
`currency` | string
`status` | string
`bankAccount` | string
`description` | string
`metadata` | { [key: string]: any; }
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PayoutResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "amount": null,
  "currency": null,
  "status": null,
  "bankAccount": null,
  "description": null,
  "metadata": {"orderId":"12345"},
  "createdAt": null,
  "updatedAt": null,
} satisfies PayoutResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PayoutResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


