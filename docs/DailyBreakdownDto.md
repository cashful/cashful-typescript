
# DailyBreakdownDto


## Properties

Name | Type
------------ | -------------
`date` | string
`count` | number
`sum` | number

## Example

```typescript
import type { DailyBreakdownDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "date": null,
  "count": null,
  "sum": null,
} satisfies DailyBreakdownDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DailyBreakdownDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


