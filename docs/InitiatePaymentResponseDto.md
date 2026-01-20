
# InitiatePaymentResponseDto


## Properties

Name | Type
------------ | -------------
`iveriParams` | [IveriParamsDto](IveriParamsDto.md)
`iVeri3dsEndpoint` | string

## Example

```typescript
import type { InitiatePaymentResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "iveriParams": null,
  "iVeri3dsEndpoint": https://portal.nedsecure.co.za/threedsecure/EnrollmentInitial,
} satisfies InitiatePaymentResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InitiatePaymentResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


