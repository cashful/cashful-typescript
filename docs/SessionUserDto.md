
# SessionUserDto


## Properties

Name | Type
------------ | -------------
`id` | string
`email` | string
`emailVerified` | boolean
`name` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { SessionUserDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "email": null,
  "emailVerified": null,
  "name": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies SessionUserDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SessionUserDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


