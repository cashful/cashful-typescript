
# FileDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`key` | string
`bucket` | string
`filename` | string
`mimeType` | string
`size` | number
`tags` | Array&lt;string&gt;
`status` | string
`checksum` | string
`isPublic` | boolean
`relatedEntityId` | string
`relatedEntityType` | string
`uploadedById` | string

## Example

```typescript
import type { FileDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "key": null,
  "bucket": null,
  "filename": null,
  "mimeType": null,
  "size": null,
  "tags": null,
  "status": null,
  "checksum": null,
  "isPublic": null,
  "relatedEntityId": null,
  "relatedEntityType": null,
  "uploadedById": null,
} satisfies FileDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as FileDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


