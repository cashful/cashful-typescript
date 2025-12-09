
# ListProductsResponseDto


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;ProductResponseDto&gt;](ProductResponseDto.md)
`pagination` | [PaginationResponseDto](PaginationResponseDto.md)

## Example

```typescript
import type { ListProductsResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "pagination": null,
} satisfies ListProductsResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListProductsResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


