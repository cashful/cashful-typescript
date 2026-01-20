
# PaymentMethodResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`customerId` | string
`type` | string
`provider` | string
`brand` | string
`last4` | string
`expiryMonth` | number
`expiryYear` | number
`phoneNumber` | string
`isDefault` | boolean
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { PaymentMethodResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "customerId": null,
  "type": null,
  "provider": null,
  "brand": null,
  "last4": null,
  "expiryMonth": null,
  "expiryYear": null,
  "phoneNumber": null,
  "isDefault": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies PaymentMethodResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentMethodResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


