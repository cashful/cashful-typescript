
# UpdateProductDto


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`amount` | number
`active` | boolean
`imageId` | string
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { UpdateProductDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "description": null,
  "amount": null,
  "active": null,
  "imageId": null,
  "metadata": {"sku":"PROD-001"},
} satisfies UpdateProductDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateProductDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


