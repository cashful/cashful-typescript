
# PaymentLinkResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`url` | string
`productId` | string
`customerId` | string
`amount` | number
`currency` | string
`mode` | string
`active` | boolean
`successUrl` | string
`cancelUrl` | string
`metadata` | { [key: string]: any; }
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PaymentLinkResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "url": null,
  "productId": null,
  "customerId": null,
  "amount": null,
  "currency": null,
  "mode": null,
  "active": null,
  "successUrl": null,
  "cancelUrl": null,
  "metadata": {"customField":"value"},
  "createdAt": null,
  "updatedAt": null,
} satisfies PaymentLinkResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentLinkResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


