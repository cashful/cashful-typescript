# CheckoutsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCheckoutSession**](CheckoutsApi.md#createcheckoutsession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout |



## createCheckoutSession

> CheckoutSessionResponseDto createCheckoutSession(createCheckoutSessionDto)

Create Hosted Checkout

Creates a hosted payment page. Used for: (1) A standard e-commerce purchase, or (2) a \&quot;Pay-In\&quot; to fund a CustomerBalance.

### Example

```ts
import {
  Configuration,
  CheckoutsApi,
} from '@cashful-co/typescript-sdk';
import type { CreateCheckoutSessionRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CheckoutsApi(config);

  const body = {
    // CreateCheckoutSessionDto | Checkout session details
    createCheckoutSessionDto: ...,
  } satisfies CreateCheckoutSessionRequest;

  try {
    const data = await api.createCheckoutSession(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createCheckoutSessionDto** | [CreateCheckoutSessionDto](CreateCheckoutSessionDto.md) | Checkout session details | |

### Return type

[**CheckoutSessionResponseDto**](CheckoutSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Checkout session created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

