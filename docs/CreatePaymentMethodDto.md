
# CreatePaymentMethodDto


## Properties

Name | Type
------------ | -------------
`customerId` | string
`type` | string
`isDefault` | boolean
`cardNumber` | string
`brand` | string
`last4` | string
`expiryMonth` | number
`expiryYear` | number

## Example

```typescript
import type { CreatePaymentMethodDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "customerId": null,
  "type": null,
  "isDefault": null,
  "cardNumber": null,
  "brand": null,
  "last4": null,
  "expiryMonth": null,
  "expiryYear": null,
} satisfies CreatePaymentMethodDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreatePaymentMethodDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


