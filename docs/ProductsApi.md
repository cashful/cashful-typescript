# ProductsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createProduct**](ProductsApi.md#createproduct) | **POST** /api/canary/products | Create Product |
| [**listProducts**](ProductsApi.md#listproducts) | **GET** /api/canary/products | List Products |
| [**retrieveProduct**](ProductsApi.md#retrieveproduct) | **GET** /api/canary/products/{id} | Retrieve Product |
| [**updateProduct**](ProductsApi.md#updateproduct) | **PATCH** /api/canary/products/{id} | Update Product |



## createProduct

> ProductResponseDto createProduct(createProductDto)

Create Product

Defines a product in the merchant\&#39;s catalog (e.g., \&quot;Airtime,\&quot; \&quot;Data\&quot;).

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@cashful/typescript';
import type { CreateProductRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductsApi(config);

  const body = {
    // CreateProductDto | Product details
    createProductDto: ...,
  } satisfies CreateProductRequest;

  try {
    const data = await api.createProduct(body);
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
| **createProductDto** | [CreateProductDto](CreateProductDto.md) | Product details | |

### Return type

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Product created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listProducts

> ListProductsResponseDto listProducts(limit, offset, merchantId, active)

List Products

Retrieves all products in the merchant\&#39;s catalog.

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@cashful/typescript';
import type { ListProductsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductsApi(config);

  const body = {
    // number | Maximum number of records to return (optional)
    limit: 50,
    // number | Number of records to skip (optional)
    offset: 0,
    // string | The ID of the merchant whose products are being requested. If not provided, the products of the authenticated merchant will be returned. (optional)
    merchantId: merchantId_example,
    // boolean | Filter by active status (optional)
    active: true,
  } satisfies ListProductsRequest;

  try {
    const data = await api.listProducts(body);
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
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |
| **merchantId** | `string` | The ID of the merchant whose products are being requested. If not provided, the products of the authenticated merchant will be returned. | [Optional] [Defaults to `undefined`] |
| **active** | `boolean` | Filter by active status | [Optional] [Defaults to `undefined`] |

### Return type

[**ListProductsResponseDto**](ListProductsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved products |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrieveProduct

> ProductResponseDto retrieveProduct(id)

Retrieve Product

Retrieves a single product by ID.

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@cashful/typescript';
import type { RetrieveProductRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductsApi(config);

  const body = {
    // string | The unique identifier of the product
    id: id_example,
  } satisfies RetrieveProductRequest;

  try {
    const data = await api.retrieveProduct(body);
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
| **id** | `string` | The unique identifier of the product | [Defaults to `undefined`] |

### Return type

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved product |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateProduct

> ProductResponseDto updateProduct(id, updateProductDto)

Update Product

Updates a product\&#39;s name, description, or metadata.

### Example

```ts
import {
  Configuration,
  ProductsApi,
} from '@cashful/typescript';
import type { UpdateProductRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ProductsApi(config);

  const body = {
    // string | The unique identifier of the product
    id: id_example,
    // UpdateProductDto | Product update details
    updateProductDto: ...,
  } satisfies UpdateProductRequest;

  try {
    const data = await api.updateProduct(body);
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
| **id** | `string` | The unique identifier of the product | [Defaults to `undefined`] |
| **updateProductDto** | [UpdateProductDto](UpdateProductDto.md) | Product update details | |

### Return type

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Product updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

