
# UpdateOrganizationDto


## Properties

Name | Type
------------ | -------------
`organizationId` | string
`data` | object

## Example

```typescript
import type { UpdateOrganizationDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "organizationId": org_12345,
  "data": null,
} satisfies UpdateOrganizationDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateOrganizationDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


