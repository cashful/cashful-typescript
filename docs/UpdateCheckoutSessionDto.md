
# UpdateCheckoutSessionDto


## Properties

Name | Type
------------ | -------------
`status` | string
`successUrl` | string
`failureUrl` | string
`cancelUrl` | string
`metadata` | { [key: string]: any; }
`hostedCheckoutConfig` | [HostedCheckoutConfigDto](HostedCheckoutConfigDto.md)

## Example

```typescript
import type { UpdateCheckoutSessionDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "status": null,
  "successUrl": null,
  "failureUrl": null,
  "cancelUrl": null,
  "metadata": {"orderId":"ORD-12345"},
  "hostedCheckoutConfig": null,
} satisfies UpdateCheckoutSessionDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateCheckoutSessionDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


