# PaymentIntentsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPaymentIntent**](PaymentIntentsApi.md#createpaymentintent) | **POST** /api/canary/payment-intents | Create Off-Session Charge |
| [**retrievePaymentIntent**](PaymentIntentsApi.md#retrievepaymentintent) | **GET** /api/canary/payment-intents/{id} | Retrieve Payment Intent |



## createPaymentIntent

> PaymentIntentResponseDto createPaymentIntent(createPaymentIntentDto)

Create Off-Session Charge

Server-to-server API to charge a saved card. Used for subscriptions or recurring billing (a core gateway feature).

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful-co/typescript';
import type { CreatePaymentIntentRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentIntentsApi(config);

  const body = {
    // CreatePaymentIntentDto | Payment intent details
    createPaymentIntentDto: ...,
  } satisfies CreatePaymentIntentRequest;

  try {
    const data = await api.createPaymentIntent(body);
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
| **createPaymentIntentDto** | [CreatePaymentIntentDto](CreatePaymentIntentDto.md) | Payment intent details | |

### Return type

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Payment intent created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **402** | Payment declined |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrievePaymentIntent

> any retrievePaymentIntent(id)

Retrieve Payment Intent

Checks the status of a specific server-to-server charge.

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful-co/typescript';
import type { RetrievePaymentIntentRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentIntentsApi(config);

  const body = {
    // string | The unique identifier of the payment intent
    id: id_example,
  } satisfies RetrievePaymentIntentRequest;

  try {
    const data = await api.retrievePaymentIntent(body);
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
| **id** | `string` | The unique identifier of the payment intent | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved payment intent |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

