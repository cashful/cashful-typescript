
# InternalAnalyticsInsightsDto


## Properties

Name | Type
------------ | -------------
`organizations` | number
`customers` | number
`savedPaymentMethods` | number
`transactions` | number
`totalAvailableBalance` | number
`totalPendingBalance` | number

## Example

```typescript
import type { InternalAnalyticsInsightsDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "organizations": null,
  "customers": null,
  "savedPaymentMethods": null,
  "transactions": null,
  "totalAvailableBalance": null,
  "totalPendingBalance": null,
} satisfies InternalAnalyticsInsightsDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InternalAnalyticsInsightsDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


