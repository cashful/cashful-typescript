
# PaginationResponseDto


## Properties

Name | Type
------------ | -------------
`limit` | number
`offset` | number
`total` | number
`hasMore` | boolean

## Example

```typescript
import type { PaginationResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "limit": 50,
  "offset": 0,
  "total": 150,
  "hasMore": true,
} satisfies PaginationResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaginationResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


