
# CreateEventDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`type` | string
`data` | object
`relatedEntityId` | string
`relatedEntityType` | string

## Example

```typescript
import type { CreateEventDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "type": null,
  "data": null,
  "relatedEntityId": null,
  "relatedEntityType": null,
} satisfies CreateEventDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CreateEventDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


