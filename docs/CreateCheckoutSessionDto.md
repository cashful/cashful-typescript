
# CreateCheckoutSessionDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`customerId` | string
`productId` | string
`successUrl` | string
`failureUrl` | string
`cancelUrl` | string
`lineItems` | [Array&lt;LineItemDto&gt;](LineItemDto.md)
`totalAmount` | number
`currency` | string
`mode` | string
`metadata` | { [key: string]: any; }
`hostedCheckoutConfig` | [HostedCheckoutConfigDto](HostedCheckoutConfigDto.md)

## Example

```typescript
import type { CreateCheckoutSessionDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "customerId": null,
  "productId": null,
  "successUrl": null,
  "failureUrl": null,
  "cancelUrl": null,
  "lineItems": null,
  "totalAmount": null,
  "currency": null,
  "mode": null,
  "metadata": {"orderId":"ORD-12345","source":"web"},
  "hostedCheckoutConfig": null,
} satisfies CreateCheckoutSessionDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateCheckoutSessionDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


