
# WebhookEndpointResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`merchantId` | string
`url` | string
`events` | Array&lt;string&gt;
`active` | boolean
`metadata` | { [key: string]: any; }
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { WebhookEndpointResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "merchantId": null,
  "url": null,
  "events": null,
  "active": null,
  "metadata": {"environment":"production"},
  "createdAt": null,
  "updatedAt": null,
} satisfies WebhookEndpointResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookEndpointResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


