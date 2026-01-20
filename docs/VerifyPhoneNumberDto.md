
# VerifyPhoneNumberDto


## Properties

Name | Type
------------ | -------------
`phoneNumber` | string
`code` | string

## Example

```typescript
import type { VerifyPhoneNumberDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "phoneNumber": +1234567890,
  "code": 123456,
} satisfies VerifyPhoneNumberDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VerifyPhoneNumberDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


