
# OrganizationDto


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`slug` | string
`logo` | string
`createdAt` | string
`metadata` | object

## Example

```typescript
import type { OrganizationDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": org_12345,
  "name": Acme Corp,
  "slug": acme-corp,
  "logo": https://example.com/logo.png,
  "createdAt": 2024-01-01T00:00:00Z,
  "metadata": {"plan":"pro"},
} satisfies OrganizationDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OrganizationDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


