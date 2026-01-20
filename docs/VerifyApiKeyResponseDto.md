
# VerifyApiKeyResponseDto


## Properties

Name | Type
------------ | -------------
`valid` | boolean
`key` | object

## Example

```typescript
import type { VerifyApiKeyResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "valid": false,
  "key": {"id":"key_123","name":"My API Key"},
} satisfies VerifyApiKeyResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VerifyApiKeyResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


