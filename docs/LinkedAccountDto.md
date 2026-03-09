
# LinkedAccountDto


## Properties

Name | Type
------------ | -------------
`id` | string
`accountId` | string
`providerId` | string
`userId` | string
`accessToken` | string
`refreshToken` | string
`idToken` | string
`accessTokenExpiresAt` | Date
`refreshTokenExpiresAt` | Date
`scope` | string
`password` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { LinkedAccountDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "accountId": null,
  "providerId": null,
  "userId": null,
  "accessToken": null,
  "refreshToken": null,
  "idToken": null,
  "accessTokenExpiresAt": null,
  "refreshTokenExpiresAt": null,
  "scope": null,
  "password": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies LinkedAccountDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LinkedAccountDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


