
# UpdatePaymentLinkDto


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`active` | boolean
`totalAmount` | number
`successUrl` | string
`cancelUrl` | string
`metadata` | { [key: string]: any; }
`hostedCheckoutConfig` | [HostedCheckoutConfigDto](HostedCheckoutConfigDto.md)

## Example

```typescript
import type { UpdatePaymentLinkDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "description": null,
  "active": null,
  "totalAmount": null,
  "successUrl": null,
  "cancelUrl": null,
  "metadata": {"orderId":"12345"},
  "hostedCheckoutConfig": null,
} satisfies UpdatePaymentLinkDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdatePaymentLinkDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


