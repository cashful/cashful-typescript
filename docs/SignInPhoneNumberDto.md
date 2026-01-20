
# SignInPhoneNumberDto


## Properties

Name | Type
------------ | -------------
`phoneNumber` | string
`password` | string
`callbackURL` | string

## Example

```typescript
import type { SignInPhoneNumberDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "phoneNumber": +1234567890,
  "password": StrongPassword123!,
  "callbackURL": https://example.com/callback,
} satisfies SignInPhoneNumberDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SignInPhoneNumberDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


