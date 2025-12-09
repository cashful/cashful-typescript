# PaymentMethodsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deletePaymentMethod**](PaymentMethodsApi.md#deletepaymentmethod) | **DELETE** /api/canary/payment-methods/{id} | Delete Payment Method |
| [**retrievePaymentMethod**](PaymentMethodsApi.md#retrievepaymentmethod) | **GET** /api/canary/payment-methods/{id} | Retrieve Payment Method |



## deletePaymentMethod

> any deletePaymentMethod(id)

Delete Payment Method

Detaches and deletes a saved payment method from a customer.

### Example

```ts
import {
  Configuration,
  PaymentMethodsApi,
} from '@cashful-co/typescript-sdk';
import type { DeletePaymentMethodRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentMethodsApi(config);

  const body = {
    // string | The unique identifier of the payment method
    id: id_example,
  } satisfies DeletePaymentMethodRequest;

  try {
    const data = await api.deletePaymentMethod(body);
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
| **id** | `string` | The unique identifier of the payment method | [Defaults to `undefined`] |

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
| **200** | Payment method successfully deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrievePaymentMethod

> PaymentMethodResponseDto retrievePaymentMethod(id)

Retrieve Payment Method

Gets the non-sensitive details of a saved card (e.g., brand, last 4).

### Example

```ts
import {
  Configuration,
  PaymentMethodsApi,
} from '@cashful-co/typescript-sdk';
import type { RetrievePaymentMethodRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentMethodsApi(config);

  const body = {
    // string | The unique identifier of the payment method
    id: id_example,
  } satisfies RetrievePaymentMethodRequest;

  try {
    const data = await api.retrievePaymentMethod(body);
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
| **id** | `string` | The unique identifier of the payment method | [Defaults to `undefined`] |

### Return type

[**PaymentMethodResponseDto**](PaymentMethodResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved payment method details |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

