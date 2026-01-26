
# HostedCheckoutConfigDto


## Properties

Name | Type
------------ | -------------
`merchantId` | string
`merchantAlias` | string
`merchantLegalName` | string
`merchantAvatarTextPlaceholder` | string
`merchantAvatarUrl` | string
`requireContact` | boolean
`requireAddress` | boolean
`taxRate` | number
`embedMode` | boolean
`embedOrigin` | string

## Example

```typescript
import type { HostedCheckoutConfigDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "merchantId": null,
  "merchantAlias": null,
  "merchantLegalName": null,
  "merchantAvatarTextPlaceholder": null,
  "merchantAvatarUrl": null,
  "requireContact": null,
  "requireAddress": null,
  "taxRate": null,
  "embedMode": null,
  "embedOrigin": null,
} satisfies HostedCheckoutConfigDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as HostedCheckoutConfigDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


