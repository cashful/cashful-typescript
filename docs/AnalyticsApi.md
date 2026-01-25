# AnalyticsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getAnalytics**](AnalyticsApi.md#getanalytics) | **GET** /api/canary/analytics | Get Analytics |
| [**getAnalyticsSummary**](AnalyticsApi.md#getanalyticssummary) | **GET** /api/canary/analytics/summary | Get Analytics Summary |



## getAnalytics

> AnalyticsResponseDto getAnalytics(merchantId)

Get Analytics

Retrieves transaction volume and customer growth metrics for the merchant.

### Example

```ts
import {
  Configuration,
  AnalyticsApi,
} from '@cashful/typescript';
import type { GetAnalyticsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AnalyticsApi(config);

  const body = {
    // string | The unique identifier of the merchant. If not provided, defaults to the authenticated user\'s active organization. (optional)
    merchantId: merchant_123,
  } satisfies GetAnalyticsRequest;

  try {
    const data = await api.getAnalytics(body);
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
| **merchantId** | `string` | The unique identifier of the merchant. If not provided, defaults to the authenticated user\&#39;s active organization. | [Optional] [Defaults to `undefined`] |

### Return type

[**AnalyticsResponseDto**](AnalyticsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved analytics |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAnalyticsSummary

> AnalyticsSummaryDto getAnalyticsSummary(merchantId)

Get Analytics Summary

Retrieves a quick summary of key metrics for the merchant.

### Example

```ts
import {
  Configuration,
  AnalyticsApi,
} from '@cashful/typescript';
import type { GetAnalyticsSummaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AnalyticsApi(config);

  const body = {
    // string | The unique identifier of the merchant. If not provided, defaults to the authenticated user\'s active organization. (optional)
    merchantId: merchant_123,
  } satisfies GetAnalyticsSummaryRequest;

  try {
    const data = await api.getAnalyticsSummary(body);
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
| **merchantId** | `string` | The unique identifier of the merchant. If not provided, defaults to the authenticated user\&#39;s active organization. | [Optional] [Defaults to `undefined`] |

### Return type

[**AnalyticsSummaryDto**](AnalyticsSummaryDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved analytics summary |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

