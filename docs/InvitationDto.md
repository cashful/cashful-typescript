
# InvitationDto


## Properties

Name | Type
------------ | -------------
`id` | string
`organizationId` | string
`email` | string
`role` | string
`status` | string
`expiresAt` | string
`createdAt` | string
`inviterId` | string

## Example

```typescript
import type { InvitationDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": inv_12345,
  "organizationId": org_12345,
  "email": user@example.com,
  "role": member,
  "status": pending,
  "expiresAt": 2024-01-01T00:00:00Z,
  "createdAt": 2024-01-01T00:00:00Z,
  "inviterId": user_67890,
} satisfies InvitationDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InvitationDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


