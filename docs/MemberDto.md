
# MemberDto


## Properties

Name | Type
------------ | -------------
`id` | string
`userId` | string
`organizationId` | string
`role` | string
`createdAt` | string

## Example

```typescript
import type { MemberDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": mem_12345,
  "userId": user_12345,
  "organizationId": org_12345,
  "role": member,
  "createdAt": 2024-01-01T00:00:00Z,
} satisfies MemberDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MemberDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


