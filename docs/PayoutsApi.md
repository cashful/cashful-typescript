# PayoutsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPayout**](PayoutsApi.md#createpayout) | **POST** /api/canary/payouts | Create Payout |
| [**listPayouts**](PayoutsApi.md#listpayouts) | **GET** /api/canary/payouts | List Payouts |



## createPayout

> PayoutResponseDto createPayout(createPayoutDto)

Create Payout

Allows the merchant to move funds from their MerchantBalance (their earnings) to their external bank account.

### Example

```ts
import {
  Configuration,
  PayoutsApi,
} from '@cashful/typescript';
import type { CreatePayoutRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PayoutsApi(config);

  const body = {
    // CreatePayoutDto | Payout details
    createPayoutDto: ...,
  } satisfies CreatePayoutRequest;

  try {
    const data = await api.createPayout(body);
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
| **createPayoutDto** | [CreatePayoutDto](CreatePayoutDto.md) | Payout details | |

### Return type

[**PayoutResponseDto**](PayoutResponseDto.md)

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Payout created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **402** | Insufficient merchant balance |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPayouts

> ListPayoutsResponseDto listPayouts(limit, offset, filter, sort, order, merchantId, status)

List Payouts

Retrieves a list of all historical and pending payouts for the merchant.

### Example

```ts
import {
  Configuration,
  PayoutsApi,
} from '@cashful/typescript';
import type { ListPayoutsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PayoutsApi(config);

  const body = {
    // number | Maximum number of items to return (optional)
    limit: 50,
    // number | Number of items to skip (optional)
    offset: 0,
    // string | JSON string used for dynamic filtering (optional)
    filter: {"ids":["prod_123","prod_456"]},
    // string | Field name to sort by (optional)
    sort: createdAt,
    // string | Sort direction (optional)
    order: DESC,
    // string | The ID of the merchant whose payouts are being requested. If omitted, defaults to the authenticated merchant. (optional)
    merchantId: merchantId_example,
    // string | Filter by status (optional)
    status: status_example,
  } satisfies ListPayoutsRequest;

  try {
    const data = await api.listPayouts(body);
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
| **limit** | `number` | Maximum number of items to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of items to skip | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | JSON string used for dynamic filtering | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Field name to sort by | [Optional] [Defaults to `undefined`] |
| **order** | `string` | Sort direction | [Optional] [Defaults to `undefined`] |
| **merchantId** | `string` | The ID of the merchant whose payouts are being requested. If omitted, defaults to the authenticated merchant. | [Optional] [Defaults to `undefined`] |
| **status** | `string` | Filter by status | [Optional] [Defaults to `undefined`] |

### Return type

[**ListPayoutsResponseDto**](ListPayoutsResponseDto.md)

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved payouts |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

