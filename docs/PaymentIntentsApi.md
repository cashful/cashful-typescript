# PaymentIntentsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**cancelPaymentIntent**](PaymentIntentsApi.md#cancelpaymentintent) | **POST** /api/canary/payment-intents/{id}/cancel | Cancel Payment Intent |
| [**confirmPaymentIntent**](PaymentIntentsApi.md#confirmpaymentintent) | **POST** /api/canary/payment-intents/{id}/confirm | Confirm Payment Intent |
| [**createPaymentIntent**](PaymentIntentsApi.md#createpaymentintent) | **POST** /api/canary/payment-intents | Create Payment Intent |
| [**listPaymentIntents**](PaymentIntentsApi.md#listpaymentintents) | **GET** /api/canary/payment-intents | List Payment Intents |
| [**retrievePaymentIntent**](PaymentIntentsApi.md#retrievepaymentintent) | **GET** /api/canary/payment-intents/{id} | Retrieve Payment Intent |



## cancelPaymentIntent

> PaymentIntentResponseDto cancelPaymentIntent(id)

Cancel Payment Intent

Cancels a payment intent that has not yet succeeded or failed.

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful/typescript';
import type { CancelPaymentIntentRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentIntentsApi(config);

  const body = {
    // string | The unique identifier of the payment intent
    id: id_example,
  } satisfies CancelPaymentIntentRequest;

  try {
    const data = await api.cancelPaymentIntent(body);
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

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Payment intent canceled |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## confirmPaymentIntent

> PaymentIntentResponseDto confirmPaymentIntent(id)

Confirm Payment Intent

Confirms a payment intent that requires confirmation. This initiates the actual payment processing.

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful/typescript';
import type { ConfirmPaymentIntentRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentIntentsApi(config);

  const body = {
    // string | The unique identifier of the payment intent
    id: id_example,
  } satisfies ConfirmPaymentIntentRequest;

  try {
    const data = await api.confirmPaymentIntent(body);
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

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Payment intent confirmed and processing |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createPaymentIntent

> PaymentIntentResponseDto createPaymentIntent(createPaymentIntentDto)

Create Payment Intent

Creates a payment intent for off-session charges. Used for subscriptions, recurring billing, or server-to-server payments with saved cards.

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful/typescript';
import type { CreatePaymentIntentRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## listPaymentIntents

> listPaymentIntents(merchantId, limit, offset, status)

List Payment Intents

Lists payment intents for a specific merchant with pagination and filtering.

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful/typescript';
import type { ListPaymentIntentsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentIntentsApi(config);

  const body = {
    // string | Filter by merchant ID
    merchantId: merchantId_example,
    // number | Maximum number of records to return (optional)
    limit: 8.14,
    // number | Number of records to skip (optional)
    offset: 8.14,
    // 'initiation' | 'requires_payment_method' | 'requires_confirmation' | 'requires_action' | 'processing' | 'requires_capture' | 'succeeded' | 'failed' | 'canceled' | Filter by status (optional)
    status: status_example,
  } satisfies ListPaymentIntentsRequest;

  try {
    const data = await api.listPaymentIntents(body);
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
| **merchantId** | `string` | Filter by merchant ID | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `50`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `0`] |
| **status** | `initiation`, `requires_payment_method`, `requires_confirmation`, `requires_action`, `processing`, `requires_capture`, `succeeded`, `failed`, `canceled` | Filter by status | [Optional] [Defaults to `undefined`] [Enum: initiation, requires_payment_method, requires_confirmation, requires_action, processing, requires_capture, succeeded, failed, canceled] |

### Return type

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved payment intents |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrievePaymentIntent

> PaymentIntentResponseDto retrievePaymentIntent(id)

Retrieve Payment Intent

Retrieves the current state of a specific payment intent.

### Example

```ts
import {
  Configuration,
  PaymentIntentsApi,
} from '@cashful/typescript';
import type { RetrievePaymentIntentRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

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

