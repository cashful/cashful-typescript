# PurchasesApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPurchase**](PurchasesApi.md#createpurchase) | **POST** /api/canary/purchases | Buy with Cash Balance |



## createPurchase

> PurchaseResponseDto createPurchase(createPurchaseDto)

Buy with Cash Balance

(Wallet-Enabling) Spends a product using the CustomerBalance as the source. Atomically debits the CustomerBalance and credits the MerchantBalance.

### Example

```ts
import {
  Configuration,
  PurchasesApi,
} from '@cashful-co/typescript-sdk';
import type { CreatePurchaseRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PurchasesApi(config);

  const body = {
    // CreatePurchaseDto | Purchase details
    createPurchaseDto: ...,
  } satisfies CreatePurchaseRequest;

  try {
    const data = await api.createPurchase(body);
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
| **createPurchaseDto** | [CreatePurchaseDto](CreatePurchaseDto.md) | Purchase details | |

### Return type

[**PurchaseResponseDto**](PurchaseResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Purchase created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **402** | Insufficient customer balance |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

