
# CreatePaymentIntentDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`customerId` | string
`paymentMethodId` | string
`amount` | number
`currency` | string
`description` | string
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { CreatePaymentIntentDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "customerId": null,
  "paymentMethodId": null,
  "amount": null,
  "currency": null,
  "description": null,
  "metadata": {"customField":"value","orderId":"12345"},
} satisfies CreatePaymentIntentDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreatePaymentIntentDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


