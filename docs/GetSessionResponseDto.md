
# GetSessionResponseDto


## Properties

Name | Type
------------ | -------------
`session` | [SessionDto](SessionDto.md)
`user` | [SessionUserDto](SessionUserDto.md)

## Example

```typescript
import type { GetSessionResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "session": null,
  "user": null,
} satisfies GetSessionResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GetSessionResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


