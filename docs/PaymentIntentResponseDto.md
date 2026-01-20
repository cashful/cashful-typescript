
# PaymentIntentResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`customerId` | string
`paymentMethodId` | string
`amount` | number
`currency` | string
`status` | string
`mode` | string
`description` | string
`metadata` | { [key: string]: any; }
`idempotencyKey` | string
`expiresAt` | Date
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date

## Example

```typescript
import type { PaymentIntentResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "customerId": null,
  "paymentMethodId": null,
  "amount": null,
  "currency": null,
  "status": null,
  "mode": null,
  "description": null,
  "metadata": {"orderId":"12345"},
  "idempotencyKey": null,
  "expiresAt": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
} satisfies PaymentIntentResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentIntentResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


