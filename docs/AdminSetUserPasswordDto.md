
# AdminSetUserPasswordDto


## Properties

Name | Type
------------ | -------------
`userId` | string
`newPassword` | string

## Example

```typescript
import type { AdminSetUserPasswordDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "userId": user_12345,
  "newPassword": NewStrongPassword123!,
} satisfies AdminSetUserPasswordDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AdminSetUserPasswordDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


