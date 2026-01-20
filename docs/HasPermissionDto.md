
# HasPermissionDto


## Properties

Name | Type
------------ | -------------
`permission` | object
`resource` | string
`organizationId` | string

## Example

```typescript
import type { HasPermissionDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "permission": read:users,
  "resource": organization:org_123,
  "organizationId": org_12345,
} satisfies HasPermissionDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as HasPermissionDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


