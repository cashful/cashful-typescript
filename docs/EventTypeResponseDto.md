
# EventTypeResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`description` | string
`isActive` | boolean

## Example

```typescript
import type { EventTypeResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "description": null,
  "isActive": null,
} satisfies EventTypeResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EventTypeResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


