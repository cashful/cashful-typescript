
# CustomerPaymentMethodDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`customerId` | string
`type` | string
`brand` | string
`last4` | string
`expiryMonth` | number
`expiryYear` | number
`isDefault` | boolean

## Example

```typescript
import type { CustomerPaymentMethodDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "customerId": null,
  "type": null,
  "brand": null,
  "last4": null,
  "expiryMonth": null,
  "expiryYear": null,
  "isDefault": null,
} satisfies CustomerPaymentMethodDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomerPaymentMethodDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


