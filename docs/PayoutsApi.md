# PayoutsApi

All URIs are relative to *http://localhost:3000*

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
} from '@cashful-co/typescript';
import type { CreatePayoutRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
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

[bearer](../README.md#bearer)

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

> ListPayoutsResponseDto listPayouts(merchantId, status, limit, offset)

List Payouts

Retrieves a list of all historical and pending payouts for the merchant.

### Example

```ts
import {
  Configuration,
  PayoutsApi,
} from '@cashful-co/typescript';
import type { ListPayoutsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PayoutsApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // any | Filter by status (optional)
    status: ...,
    // number | Maximum number of records to return (optional)
    limit: 8.14,
    // number | Number of records to skip (optional)
    offset: 8.14,
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
| **merchantId** | `string` | The ID of the merchant. This parameter is required. | [Defaults to `undefined`] |
| **status** | `any` | Filter by status | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |

### Return type

[**ListPayoutsResponseDto**](ListPayoutsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

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

