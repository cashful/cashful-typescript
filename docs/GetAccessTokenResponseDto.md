
# GetAccessTokenResponseDto


## Properties

Name | Type
------------ | -------------
`token` | string
`expiresAt` | string

## Example

```typescript
import type { GetAccessTokenResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "token": current_access_token_123,
  "expiresAt": 2024-01-01T00:00:00Z,
} satisfies GetAccessTokenResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetAccessTokenResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


