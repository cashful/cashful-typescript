# PaymentLinksApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPaymentLink**](PaymentLinksApi.md#createpaymentlink) | **POST** /api/canary/payment-links | Create Payment Link |
| [**deletePaymentLink**](PaymentLinksApi.md#deletepaymentlink) | **DELETE** /api/canary/payment-links/{id} | Delete Payment Link |
| [**listPaymentLinks**](PaymentLinksApi.md#listpaymentlinks) | **GET** /api/canary/payment-links | List Payment Links |
| [**retrievePaymentLink**](PaymentLinksApi.md#retrievepaymentlink) | **GET** /api/canary/payment-links/{id} | Retrieve Payment Link |
| [**updatePaymentLink**](PaymentLinksApi.md#updatepaymentlink) | **PATCH** /api/canary/payment-links/{id} | Update Payment Link |



## createPaymentLink

> PaymentLinkResponseDto createPaymentLink(createPaymentLinkDto)

Create Payment Link

Creates a re-usable hosted link. Can be used for: (1) Selling a product, or (2) as a \&quot;Pay-In\&quot; link for a customer.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful/typescript';
import type { CreatePaymentLinkRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentLinksApi(config);

  const body = {
    // CreatePaymentLinkDto | Payment link details
    createPaymentLinkDto: ...,
  } satisfies CreatePaymentLinkRequest;

  try {
    const data = await api.createPaymentLink(body);
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
| **createPaymentLinkDto** | [CreatePaymentLinkDto](CreatePaymentLinkDto.md) | Payment link details | |

### Return type

[**PaymentLinkResponseDto**](PaymentLinkResponseDto.md)

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Payment link created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deletePaymentLink

> deletePaymentLink(id)

Delete Payment Link

Soft-deletes a payment link.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful/typescript';
import type { DeletePaymentLinkRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentLinksApi(config);

  const body = {
    // string | The unique identifier of the payment link
    id: id_example,
  } satisfies DeletePaymentLinkRequest;

  try {
    const data = await api.deletePaymentLink(body);
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
| **id** | `string` | The unique identifier of the payment link | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Payment link deleted successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPaymentLinks

> ListPaymentLinksResponseDto listPaymentLinks(limit, offset, filter, sort, order, merchantId, active)

List Payment Links

Retrieves all payment links created by the merchant.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful/typescript';
import type { ListPaymentLinksRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentLinksApi(config);

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
    // string | The ID of the merchant whose payment links are being requested. If omitted, defaults to the authenticated merchant. (optional)
    merchantId: merchantId_example,
    // boolean | Filter by active status (optional)
    active: true,
  } satisfies ListPaymentLinksRequest;

  try {
    const data = await api.listPaymentLinks(body);
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
| **merchantId** | `string` | The ID of the merchant whose payment links are being requested. If omitted, defaults to the authenticated merchant. | [Optional] [Defaults to `undefined`] |
| **active** | `boolean` | Filter by active status | [Optional] [Defaults to `undefined`] |

### Return type

[**ListPaymentLinksResponseDto**](ListPaymentLinksResponseDto.md)

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved payment links |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrievePaymentLink

> PaymentLinkResponseDto retrievePaymentLink(id)

Retrieve Payment Link

Retrieves a single payment link by ID.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful/typescript';
import type { RetrievePaymentLinkRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentLinksApi(config);

  const body = {
    // string | The unique identifier of the payment link
    id: id_example,
  } satisfies RetrievePaymentLinkRequest;

  try {
    const data = await api.retrievePaymentLink(body);
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
| **id** | `string` | The unique identifier of the payment link | [Defaults to `undefined`] |

### Return type

[**PaymentLinkResponseDto**](PaymentLinkResponseDto.md)

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Payment link retrieved successfully |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updatePaymentLink

> any updatePaymentLink(id, updatePaymentLinkDto)

Update Payment Link

Updates a link\&#39;s details, most commonly to set active: false.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful/typescript';
import type { UpdatePaymentLinkRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKey
    apiKey: "YOUR API KEY",
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentLinksApi(config);

  const body = {
    // string | The unique identifier of the payment link
    id: id_example,
    // UpdatePaymentLinkDto | Payment link update details
    updatePaymentLinkDto: ...,
  } satisfies UpdatePaymentLinkRequest;

  try {
    const data = await api.updatePaymentLink(body);
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
| **id** | `string` | The unique identifier of the payment link | [Defaults to `undefined`] |
| **updatePaymentLinkDto** | [UpdatePaymentLinkDto](UpdatePaymentLinkDto.md) | Payment link update details | |

### Return type

**any**

### Authorization

[apiKey](../README.md#apiKey), [bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Payment link updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

