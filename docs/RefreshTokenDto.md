
# RefreshTokenDto


## Properties

Name | Type
------------ | -------------
`refreshToken` | string
`rotate` | boolean

## Example

```typescript
import type { RefreshTokenDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "refreshToken": refresh_token_123,
  "rotate": true,
} satisfies RefreshTokenDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RefreshTokenDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


