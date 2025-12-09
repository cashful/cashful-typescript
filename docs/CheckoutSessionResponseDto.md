
# CheckoutSessionResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`merchantId` | string
`customerId` | string
`sessionUrl` | string
`successUrl` | string
`cancelUrl` | string
`lineItems` | [Array&lt;LineItemDto&gt;](LineItemDto.md)
`totalAmount` | number
`currency` | string
`mode` | string
`status` | string
`expiresAt` | Date
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { CheckoutSessionResponseDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "merchantId": null,
  "customerId": null,
  "sessionUrl": null,
  "successUrl": null,
  "cancelUrl": null,
  "lineItems": null,
  "totalAmount": null,
  "currency": null,
  "mode": null,
  "status": null,
  "expiresAt": null,
  "metadata": {"orderId":"ORD-12345"},
} satisfies CheckoutSessionResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CheckoutSessionResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


