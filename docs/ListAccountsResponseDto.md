
# ListAccountsResponseDto


## Properties

Name | Type
------------ | -------------
`accounts` | [Array&lt;LinkedAccountDto&gt;](LinkedAccountDto.md)

## Example

```typescript
import type { ListAccountsResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "accounts": null,
} satisfies ListAccountsResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListAccountsResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


