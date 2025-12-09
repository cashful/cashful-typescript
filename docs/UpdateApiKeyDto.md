
# UpdateApiKeyDto


## Properties

Name | Type
------------ | -------------
`keyId` | string
`name` | string
`enabled` | boolean
`metadata` | object

## Example

```typescript
import type { UpdateApiKeyDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "keyId": key_12345,
  "name": My Updated API Key,
  "enabled": true,
  "metadata": {"env":"production"},
} satisfies UpdateApiKeyDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateApiKeyDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


