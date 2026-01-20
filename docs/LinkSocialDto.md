
# LinkSocialDto


## Properties

Name | Type
------------ | -------------
`provider` | string
`accessToken` | string
`refreshToken` | string
`idToken` | string
`expiresAt` | number

## Example

```typescript
import type { LinkSocialDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "provider": google,
  "accessToken": ya29.access_token,
  "refreshToken": refresh_token_123,
  "idToken": id_token_123,
  "expiresAt": 1640995200,
} satisfies LinkSocialDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LinkSocialDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


