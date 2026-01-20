
# SignInDto


## Properties

Name | Type
------------ | -------------
`email` | string
`password` | string
`callbackURL` | string
`rememberMe` | boolean

## Example

```typescript
import type { SignInDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "email": john.doe@example.com,
  "password": StrongPassword123!,
  "callbackURL": https://example.com/auth/callback,
  "rememberMe": true,
} satisfies SignInDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SignInDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


