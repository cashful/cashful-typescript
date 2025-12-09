
# CreatePaymentLinkDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`productId` | string
`customerId` | string
`amount` | number
`currency` | string
`mode` | string
`successUrl` | string
`cancelUrl` | string
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { CreatePaymentLinkDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "productId": null,
  "customerId": null,
  "amount": null,
  "currency": null,
  "mode": null,
  "successUrl": null,
  "cancelUrl": null,
  "metadata": {"customField":"value","orderId":"12345"},
} satisfies CreatePaymentLinkDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreatePaymentLinkDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


