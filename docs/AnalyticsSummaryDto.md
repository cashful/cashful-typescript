
# AnalyticsSummaryDto


## Properties

Name | Type
------------ | -------------
`balance` | number
`customers` | number
`transactions` | number
`members` | number

## Example

```typescript
import type { AnalyticsSummaryDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "balance": null,
  "customers": null,
  "transactions": null,
  "members": null,
} satisfies AnalyticsSummaryDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AnalyticsSummaryDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


