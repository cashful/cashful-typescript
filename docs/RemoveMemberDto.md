
# RemoveMemberDto


## Properties

Name | Type
------------ | -------------
`memberId` | string
`organizationId` | string

## Example

```typescript
import type { RemoveMemberDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "memberId": mem_12345,
  "organizationId": org_12345,
} satisfies RemoveMemberDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RemoveMemberDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


