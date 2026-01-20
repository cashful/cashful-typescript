
# ResetPhonePasswordDto


## Properties

Name | Type
------------ | -------------
`phoneNumber` | string
`code` | string
`newPassword` | string

## Example

```typescript
import type { ResetPhonePasswordDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "phoneNumber": +1234567890,
  "code": 123456,
  "newPassword": NewStrongPassword123!,
} satisfies ResetPhonePasswordDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ResetPhonePasswordDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


