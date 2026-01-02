# PaymentLinksApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPaymentLink**](PaymentLinksApi.md#createpaymentlink) | **POST** /api/canary/payment-links | Create Payment Link |
| [**listPaymentLinks**](PaymentLinksApi.md#listpaymentlinks) | **GET** /api/canary/payment-links | List Payment Links |
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
} from '@cashful-co/typescript';
import type { CreatePaymentLinkRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
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

[bearer](../README.md#bearer)

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


## listPaymentLinks

> ListPaymentLinksResponseDto listPaymentLinks(merchantId, limit, offset, active)

List Payment Links

Retrieves all payment links created by the merchant.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful-co/typescript';
import type { ListPaymentLinksRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new PaymentLinksApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // number | Maximum number of records to return (optional)
    limit: 8.14,
    // number | Number of records to skip (optional)
    offset: 8.14,
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
| **merchantId** | `string` | The ID of the merchant. This parameter is required. | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |
| **active** | `boolean` | Filter by active status | [Optional] [Defaults to `undefined`] |

### Return type

[**ListPaymentLinksResponseDto**](ListPaymentLinksResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

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


## updatePaymentLink

> any updatePaymentLink(id, updatePaymentLinkDto)

Update Payment Link

Updates a link\&#39;s details, most commonly to set active: false.

### Example

```ts
import {
  Configuration,
  PaymentLinksApi,
} from '@cashful-co/typescript';
import type { UpdatePaymentLinkRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
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

[bearer](../README.md#bearer)

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

