
# ChangeEmailResponseDto


## Properties

Name | Type
------------ | -------------
`status` | boolean
`message` | string
`user` | [SessionUserDto](SessionUserDto.md)

## Example

```typescript
import type { ChangeEmailResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "message": null,
  "user": null,
} satisfies ChangeEmailResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ChangeEmailResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


