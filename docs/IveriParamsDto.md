
# IveriParamsDto


## Properties

Name | Type
------------ | -------------
`applicationID` | string
`returnUrl` | string
`merchantReference` | string
`amount` | string
`currency` | string

## Example

```typescript
import type { IveriParamsDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "applicationID": APP123,
  "returnUrl": https://api.example.com/api/iveri/debit-return,
  "merchantReference": pi_xyz789,
  "amount": 10000,
  "currency": ZAR,
} satisfies IveriParamsDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IveriParamsDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


