
# SignInDto


## Properties

Name | Type
------------ | -------------
`email` | string
`password` | string

## Example

```typescript
import type { SignInDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "email": john.doe@example.com,
  "password": StrongPassword123!,
} satisfies SignInDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SignInDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


