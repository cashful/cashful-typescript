# ComplianceApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCompliance**](ComplianceApi.md#createcompliance) | **POST** /api/canary/compliance | Create Compliance info |
| [**listCompliance**](ComplianceApi.md#listcompliance) | **GET** /api/canary/compliance | List Compliance info for organization |
| [**updateCompliance**](ComplianceApi.md#updatecompliance) | **PATCH** /api/canary/compliance/{id} | Update Compliance info |



## createCompliance

> OrganizationComplianceResponseDto createCompliance(createOrganizationComplianceDto)

Create Compliance info

### Example

```ts
import {
  Configuration,
  ComplianceApi,
} from '@cashful/typescript';
import type { CreateComplianceRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceApi(config);

  const body = {
    // CreateOrganizationComplianceDto
    createOrganizationComplianceDto: ...,
  } satisfies CreateComplianceRequest;

  try {
    const data = await api.createCompliance(body);
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
| **createOrganizationComplianceDto** | [CreateOrganizationComplianceDto](CreateOrganizationComplianceDto.md) |  | |

### Return type

[**OrganizationComplianceResponseDto**](OrganizationComplianceResponseDto.md)

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


## listCompliance

> ListOrganizationComplianceResponseDto listCompliance(limit, offset, filter, sort, order)

List Compliance info for organization

### Example

```ts
import {
  Configuration,
  ComplianceApi,
} from '@cashful/typescript';
import type { ListComplianceRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceApi(config);

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
  } satisfies ListComplianceRequest;

  try {
    const data = await api.listCompliance(body);
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

### Return type

[**ListOrganizationComplianceResponseDto**](ListOrganizationComplianceResponseDto.md)

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


## updateCompliance

> updateCompliance(id, updateOrganizationComplianceDto)

Update Compliance info

### Example

```ts
import {
  Configuration,
  ComplianceApi,
} from '@cashful/typescript';
import type { UpdateComplianceRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ComplianceApi(config);

  const body = {
    // string
    id: id_example,
    // UpdateOrganizationComplianceDto
    updateOrganizationComplianceDto: ...,
  } satisfies UpdateComplianceRequest;

  try {
    const data = await api.updateCompliance(body);
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
| **updateOrganizationComplianceDto** | [UpdateOrganizationComplianceDto](UpdateOrganizationComplianceDto.md) |  | |

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
| **200** | Compliance updated |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

