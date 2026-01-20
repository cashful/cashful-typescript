
# ApiKey


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`name` | string
`prefix` | string
`userId` | string
`enabled` | boolean
`rateLimitEnabled` | boolean
`rateLimitTimeWindow` | number
`rateLimitMax` | number
`requestCount` | number
`remaining` | number
`lastRequest` | Date
`expiresAt` | Date
`metadata` | object
`permissions` | string

## Example

```typescript
import type { ApiKey } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "name": null,
  "prefix": null,
  "userId": null,
  "enabled": null,
  "rateLimitEnabled": null,
  "rateLimitTimeWindow": null,
  "rateLimitMax": null,
  "requestCount": null,
  "remaining": null,
  "lastRequest": null,
  "expiresAt": null,
  "metadata": null,
  "permissions": null,
} satisfies ApiKey

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApiKey
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


