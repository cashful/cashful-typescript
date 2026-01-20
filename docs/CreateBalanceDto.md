
# CreateBalanceDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`amount` | number
`currency` | string

## Example

```typescript
import type { CreateBalanceDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "merchantId": merchant_123,
  "amount": 1000,
  "currency": ZAR,
} satisfies CreateBalanceDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateBalanceDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


