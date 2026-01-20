
# SendSmsDto


## Properties

Name | Type
------------ | -------------
`to` | object
`message` | string
`from` | string

## Example

```typescript
import type { SendSmsDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "to": +27123456789,
  "message": Your verification code is: 123456,
  "from": Cashful,
} satisfies SendSmsDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendSmsDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


