
# JwkDto


## Properties

Name | Type
------------ | -------------
`kid` | string
`kty` | string
`alg` | string
`use` | string
`n` | string
`e` | string
`crv` | string
`x` | string
`y` | string

## Example

```typescript
import type { JwkDto } from '@cashful/typescript'

// TODO: Update the object below with actual values
const example = {
  "kid": null,
  "kty": null,
  "alg": null,
  "use": null,
  "n": null,
  "e": null,
  "crv": null,
  "x": null,
  "y": null,
} satisfies JwkDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as JwkDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


