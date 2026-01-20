
# ChangeEmailDto


## Properties

Name | Type
------------ | -------------
`newEmail` | string
`callbackURL` | string

## Example

```typescript
import type { ChangeEmailDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "newEmail": newemail@example.com,
  "callbackURL": https://example.com/callback,
} satisfies ChangeEmailDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ChangeEmailDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


