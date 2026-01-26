
# PaymentLinkResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`description` | string
`merchantId` | string
`url` | string
`lineItems` | [Array&lt;LineItemDto&gt;](LineItemDto.md)
`customerId` | string
`totalAmount` | number
`currency` | string
`mode` | string
`active` | boolean
`successUrl` | string
`cancelUrl` | string
`metadata` | { [key: string]: any; }
`hostedCheckoutConfig` | [HostedCheckoutConfigDto](HostedCheckoutConfigDto.md)
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date

## Example

```typescript
import type { PaymentLinkResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "description": null,
  "merchantId": null,
  "url": null,
  "lineItems": null,
  "customerId": null,
  "totalAmount": null,
  "currency": null,
  "mode": null,
  "active": null,
  "successUrl": null,
  "cancelUrl": null,
  "metadata": {"customField":"value"},
  "hostedCheckoutConfig": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
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


