
# EventResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`type` | string
`data` | object
`relatedEntityId` | string
`relatedEntityType` | string
`createdAt` | Date

## Example

```typescript
import type { EventResponseDto } from '@cashful-co/typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "type": null,
  "data": {"key":"value"},
  "relatedEntityId": null,
  "relatedEntityType": null,
  "createdAt": null,
} satisfies EventResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EventResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


