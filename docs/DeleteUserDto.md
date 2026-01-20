
# DeleteUserDto


## Properties

Name | Type
------------ | -------------
`callbackURL` | string
`password` | string
`token` | string

## Example

```typescript
import type { DeleteUserDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "callbackURL": https://example.com/goodbye,
  "password": CurrentPassword123!,
  "token": delete_token_12345,
} satisfies DeleteUserDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeleteUserDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


