
# RequestUploadUrlDto


## Properties

Name | Type
------------ | -------------
`filename` | string
`mimeType` | string
`tags` | Array&lt;string&gt;
`relatedEntityId` | string
`relatedEntityType` | string
`isPublic` | boolean

## Example

```typescript
import type { RequestUploadUrlDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "filename": null,
  "mimeType": image/png,
  "tags": ["compliance","identity-document"],
  "relatedEntityId": null,
  "relatedEntityType": null,
  "isPublic": null,
} satisfies RequestUploadUrlDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RequestUploadUrlDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


