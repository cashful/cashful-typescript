
# SendEmailDto


## Properties

Name | Type
------------ | -------------
`to` | object
`subject` | string
`template` | string
`context` | object
`html` | string
`text` | string
`from` | string
`cc` | object
`bcc` | object

## Example

```typescript
import type { SendEmailDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "to": user@example.com,
  "subject": Welcome to Cashful,
  "template": welcome,
  "context": {"name":"John Doe","activationLink":"https://example.com/activate"},
  "html": <p>Hello World</p>,
  "text": Hello World,
  "from": noreply@cashful.africa,
  "cc": ["admin@cashful.africa"],
  "bcc": ["archive@cashful.africa"],
} satisfies SendEmailDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendEmailDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


