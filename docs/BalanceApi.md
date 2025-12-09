# BalanceApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getBalanceHistory**](BalanceApi.md#getbalancehistory) | **GET** /api/canary/balance/history | List Merchant Balance History |
| [**getMerchantBalance**](BalanceApi.md#getmerchantbalance) | **GET** /api/canary/balance | Get Merchant Balance |



## getBalanceHistory

> BalanceHistoryResponseDto getBalanceHistory(merchantId, transactionType, endDate, startDate, limit, offset)

List Merchant Balance History

A full ledger of all transactions, fees, and payouts for the merchant\&#39;s master account.

### Example

```ts
import {
  Configuration,
  BalanceApi,
} from '@cashful-co/typescript';
import type { GetBalanceHistoryRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BalanceApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // any | Filter by transaction type (e.g., \"credit\", \"debit\", \"fee\", \"payout\") (optional)
    transactionType: ...,
    // any | Filter transactions until this date (ISO 8601 format) (optional)
    endDate: ...,
    // any | Filter transactions from this date (ISO 8601 format) (optional)
    startDate: ...,
    // number | Maximum number of records to return (optional)
    limit: 8.14,
    // number | Number of records to skip (optional)
    offset: 8.14,
  } satisfies GetBalanceHistoryRequest;

  try {
    const data = await api.getBalanceHistory(body);
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
| **transactionType** | `any` | Filter by transaction type (e.g., \&quot;credit\&quot;, \&quot;debit\&quot;, \&quot;fee\&quot;, \&quot;payout\&quot;) | [Optional] [Defaults to `undefined`] |
| **endDate** | `any` | Filter transactions until this date (ISO 8601 format) | [Optional] [Defaults to `undefined`] |
| **startDate** | `any` | Filter transactions from this date (ISO 8601 format) | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |

### Return type

[**BalanceHistoryResponseDto**](BalanceHistoryResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved balance history |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMerchantBalance

> MerchantBalanceResponseDto getMerchantBalance()

Get Merchant Balance

Retrieves the merchant\&#39;s own master balance (their earnings) available for payouts.

### Example

```ts
import {
  Configuration,
  BalanceApi,
} from '@cashful-co/typescript';
import type { GetMerchantBalanceRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BalanceApi(config);

  try {
    const data = await api.getMerchantBalance();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**MerchantBalanceResponseDto**](MerchantBalanceResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved merchant balance |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

