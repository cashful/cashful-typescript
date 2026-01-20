
# SessionDto


## Properties

Name | Type
------------ | -------------
`id` | string
`userId` | string
`expiresAt` | Date
`ipAddress` | string
`userAgent` | string

## Example

```typescript
import type { SessionDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "userId": null,
  "expiresAt": null,
  "ipAddress": null,
  "userAgent": null,
} satisfies SessionDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SessionDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


