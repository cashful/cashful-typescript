
# UpdateCustomerDto


## Properties

Name | Type
------------ | -------------
`email` | string
`name` | string
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { UpdateCustomerDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "email": null,
  "name": null,
  "metadata": {"customField":"value","orderId":"12345"},
} satisfies UpdateCustomerDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateCustomerDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


