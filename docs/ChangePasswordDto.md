
# ChangePasswordDto


## Properties

Name | Type
------------ | -------------
`newPassword` | string
`currentPassword` | string
`revokeOtherSessions` | boolean

## Example

```typescript
import type { ChangePasswordDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "newPassword": NewStrongPassword123!,
  "currentPassword": CurrentPassword123!,
  "revokeOtherSessions": true,
} satisfies ChangePasswordDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ChangePasswordDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


