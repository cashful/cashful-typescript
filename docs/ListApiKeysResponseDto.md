
# ListApiKeysResponseDto


## Properties

Name | Type
------------ | -------------
`apiKeys` | [Array&lt;ApiKey&gt;](ApiKey.md)

## Example

```typescript
import type { ListApiKeysResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "apiKeys": [{"id":"key_123","name":"My API Key"}],
} satisfies ListApiKeysResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListApiKeysResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


