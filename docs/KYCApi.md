# KYCApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createKyc**](KYCApi.md#createkyc) | **POST** /api/canary/kyc | Create KYC info |
| [**getKyc**](KYCApi.md#getkyc) | **GET** /api/canary/kyc | Get KYC info for organization |
| [**updateKyc**](KYCApi.md#updatekyc) | **PATCH** /api/canary/kyc/{id} | Update KYC info |



## createKyc

> OrganizationKycResponseDto createKyc(createOrganizationKycDto)

Create KYC info

### Example

```ts
import {
  Configuration,
  KYCApi,
} from '@cashful-co/typescript';
import type { CreateKycRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KYCApi(config);

  const body = {
    // CreateOrganizationKycDto
    createOrganizationKycDto: ...,
  } satisfies CreateKycRequest;

  try {
    const data = await api.createKyc(body);
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
| **createOrganizationKycDto** | [CreateOrganizationKycDto](CreateOrganizationKycDto.md) |  | |

### Return type

[**OrganizationKycResponseDto**](OrganizationKycResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** |  |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getKyc

> OrganizationKycResponseDto getKyc(organizationId)

Get KYC info for organization

### Example

```ts
import {
  Configuration,
  KYCApi,
} from '@cashful-co/typescript';
import type { GetKycRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KYCApi(config);

  const body = {
    // string
    organizationId: organizationId_example,
  } satisfies GetKycRequest;

  try {
    const data = await api.getKyc(body);
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
| **organizationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**OrganizationKycResponseDto**](OrganizationKycResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateKyc

> updateKyc(id, updateOrganizationKycDto)

Update KYC info

### Example

```ts
import {
  Configuration,
  KYCApi,
} from '@cashful-co/typescript';
import type { UpdateKycRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new KYCApi(config);

  const body = {
    // string
    id: id_example,
    // UpdateOrganizationKycDto
    updateOrganizationKycDto: ...,
  } satisfies UpdateKycRequest;

  try {
    const data = await api.updateKyc(body);
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
| **id** | `string` |  | [Defaults to `undefined`] |
| **updateOrganizationKycDto** | [UpdateOrganizationKycDto](UpdateOrganizationKycDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | KYC updated |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

