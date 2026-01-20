
# ChangePasswordResponseDto


## Properties

Name | Type
------------ | -------------
`token` | string
`user` | [SessionUserDto](SessionUserDto.md)

## Example

```typescript
import type { ChangePasswordResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "token": new_session_token_12345,
  "user": null,
} satisfies ChangePasswordResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ChangePasswordResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


