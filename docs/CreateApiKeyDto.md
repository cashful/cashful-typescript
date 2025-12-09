
# CreateApiKeyDto


## Properties

Name | Type
------------ | -------------
`name` | string
`expiresIn` | number
`prefix` | string
`metadata` | object

## Example

```typescript
import type { CreateApiKeyDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": My API Key,
  "expiresIn": 3600,
  "prefix": pk_live_,
  "metadata": {"env":"production"},
} satisfies CreateApiKeyDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateApiKeyDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


