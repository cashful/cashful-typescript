# TransfersApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTransfer**](TransfersApi.md#createtransfer) | **POST** /api/canary/transfers | Create P2P Transfer |
| [**listTransfers**](TransfersApi.md#listtransfers) | **GET** /api/canary/transfers | List Transfers |



## createTransfer

> TransferResponseDto createTransfer(createTransferDto)

Create P2P Transfer

(Wallet-Enabling) Moves funds from one CustomerBalance to another CustomerBalance. This is the P2P feature.

### Example

```ts
import {
  Configuration,
  TransfersApi,
} from '@cashful/typescript';
import type { CreateTransferRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TransfersApi(config);

  const body = {
    // CreateTransferDto | Transfer details
    createTransferDto: ...,
  } satisfies CreateTransferRequest;

  try {
    const data = await api.createTransfer(body);
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
| **createTransferDto** | [CreateTransferDto](CreateTransferDto.md) | Transfer details | |

### Return type

[**TransferResponseDto**](TransferResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Transfer created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **402** | Insufficient sender balance |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTransfers

> ListTransfersResponseDto listTransfers(limit, offset, merchantId)

List Transfers

Lists transfers for a specific merchant with pagination.

### Example

```ts
import {
  Configuration,
  TransfersApi,
} from '@cashful/typescript';
import type { ListTransfersRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TransfersApi(config);

  const body = {
    // number | Maximum number of items to return (optional)
    limit: 50,
    // number | Number of items to skip (optional)
    offset: 0,
    // string | Filter by merchant ID. If omitted, defaults to the authenticated merchant. (optional)
    merchantId: merchantId_example,
  } satisfies ListTransfersRequest;

  try {
    const data = await api.listTransfers(body);
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
| **merchantId** | `string` | Filter by merchant ID. If omitted, defaults to the authenticated merchant. | [Optional] [Defaults to `undefined`] |

### Return type

[**ListTransfersResponseDto**](ListTransfersResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved transfers |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

