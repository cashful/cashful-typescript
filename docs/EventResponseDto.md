
# EventResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`webhookEndpointId` | string
`type` | string
`data` | object
`status` | string
`attempts` | number
`relatedEntityId` | string
`relatedEntityType` | string
`lastAttemptAt` | Date
`nextRetryAt` | Date
`deliveredAt` | Date
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { EventResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "webhookEndpointId": null,
  "type": null,
  "data": {"key":"value"},
  "status": null,
  "attempts": null,
  "relatedEntityId": null,
  "relatedEntityType": null,
  "lastAttemptAt": null,
  "nextRetryAt": null,
  "deliveredAt": null,
  "createdAt": null,
  "updatedAt": null,
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


