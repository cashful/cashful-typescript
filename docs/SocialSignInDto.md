
# SocialSignInDto


## Properties

Name | Type
------------ | -------------
`provider` | string
`callbackURL` | string
`newUserCallbackURL` | string
`errorCallbackURL` | string
`disableRedirect` | boolean
`idToken` | object
`scopes` | Array&lt;string&gt;
`requestSignUp` | boolean
`loginHint` | string
`additionalData` | string

## Example

```typescript
import type { SocialSignInDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "provider": google,
  "callbackURL": https://example.com/auth/callback,
  "newUserCallbackURL": https://example.com/auth/new-user,
  "errorCallbackURL": https://example.com/auth/error,
  "disableRedirect": false,
  "idToken": null,
  "scopes": ["email","profile"],
  "requestSignUp": false,
  "loginHint": user@example.com,
  "additionalData": additional_data,
} satisfies SocialSignInDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SocialSignInDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


