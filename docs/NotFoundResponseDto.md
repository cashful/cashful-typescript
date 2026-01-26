
# NotFoundResponseDto


## Properties

Name | Type
------------ | -------------
`statusCode` | number
`message` | Array&lt;string&gt;
`error` | string

## Example

```typescript
import type { NotFoundResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "statusCode": 404,
  "message": null,
  "error": Not Found,
} satisfies NotFoundResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotFoundResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


