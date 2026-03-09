
# UpdateFileDto


## Properties

Name | Type
------------ | -------------
`tags` | Array&lt;string&gt;
`status` | string
`isPublic` | boolean
`relatedEntityId` | string
`relatedEntityType` | string

## Example

```typescript
import type { UpdateFileDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "tags": null,
  "status": null,
  "isPublic": null,
  "relatedEntityId": null,
  "relatedEntityType": null,
} satisfies UpdateFileDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateFileDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


