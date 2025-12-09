
# ProductResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`merchantId` | string
`name` | string
`description` | string
`amount` | number
`currency` | string
`active` | boolean
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { ProductResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "merchantId": null,
  "name": null,
  "description": null,
  "amount": null,
  "currency": null,
  "active": null,
  "metadata": {"sku":"PROD-001"},
} satisfies ProductResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProductResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


