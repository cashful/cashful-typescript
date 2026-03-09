
# BulkUpdateCustomersInputDto


## Properties

Name | Type
------------ | -------------
`ids` | Array&lt;string&gt;
`data` | object

## Example

```typescript
import type { BulkUpdateCustomersInputDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "ids": ["id_1","id_2"],
  "data": {"name":"Updated","metadata":{"tier":"gold"}},
} satisfies BulkUpdateCustomersInputDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkUpdateCustomersInputDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


