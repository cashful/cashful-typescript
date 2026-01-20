
# DebitReturnResponseDto


## Properties

Name | Type
------------ | -------------
`status` | string
`merchantReference` | string
`paymentIntentId` | string
`transactionId` | string
`authCode` | string
`reason` | string
`amount` | number
`currency` | string

## Example

```typescript
import type { DebitReturnResponseDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "status": succeeded,
  "merchantReference": pi_xyz789,
  "paymentIntentId": pi_xyz789,
  "transactionId": txn_abc123,
  "authCode": AUTH123456,
  "reason": Insufficient funds,
  "amount": 10000,
  "currency": ZAR,
} satisfies DebitReturnResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DebitReturnResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


