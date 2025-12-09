
# CreatePayoutDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`amount` | number
`currency` | string
`bankAccount` | string
`description` | string
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { CreatePayoutDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "amount": null,
  "currency": null,
  "bankAccount": null,
  "description": null,
  "metadata": {"orderId":"12345"},
} satisfies CreatePayoutDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreatePayoutDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


