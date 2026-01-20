
# PresignedUploadResponseDto


## Properties

Name | Type
------------ | -------------
`uploadUrl` | string
`fileId` | string
`key` | string
`expiresAt` | Date

## Example

```typescript
import type { PresignedUploadResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "uploadUrl": null,
  "fileId": null,
  "key": null,
  "expiresAt": null,
} satisfies PresignedUploadResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PresignedUploadResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


