
# NotificationDto


## Properties

Name | Type
------------ | -------------
`channel` | string
`email` | [SendEmailDto](SendEmailDto.md)
`sms` | [SendSmsDto](SendSmsDto.md)

## Example

```typescript
import type { NotificationDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "channel": email,
  "email": null,
  "sms": null,
} satisfies NotificationDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotificationDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


