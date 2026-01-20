# StorageApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**storageControllerConfirmUploadCanary**](StorageApi.md#storagecontrollerconfirmuploadcanary) | **POST** /api/canary/storage/confirm-upload | Confirm that a file upload was completed |
| [**storageControllerDeleteCanary**](StorageApi.md#storagecontrollerdeletecanary) | **DELETE** /api/canary/storage/{id} | Delete a file |
| [**storageControllerGetDownloadUrlCanary**](StorageApi.md#storagecontrollergetdownloadurlcanary) | **GET** /api/canary/storage/{id}/download-url | Get a presigned download URL for a file |
| [**storageControllerListCanary**](StorageApi.md#storagecontrollerlistcanary) | **GET** /api/canary/storage | List files |
| [**storageControllerRequestUploadUrlCanary**](StorageApi.md#storagecontrollerrequestuploadurlcanary) | **POST** /api/canary/storage/upload-url | Request a presigned URL for file upload |
| [**storageControllerRetrieveCanary**](StorageApi.md#storagecontrollerretrievecanary) | **GET** /api/canary/storage/{id} | Get file details |



## storageControllerConfirmUploadCanary

> FileDto storageControllerConfirmUploadCanary(confirmUploadDto)

Confirm that a file upload was completed

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { StorageControllerConfirmUploadCanaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // ConfirmUploadDto
    confirmUploadDto: {"fileId":"file_abc123xyz","checksum":"sha256:a1b2c3d4e5f6...","size":245760},
  } satisfies StorageControllerConfirmUploadCanaryRequest;

  try {
    const data = await api.storageControllerConfirmUploadCanary(body);
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
| **confirmUploadDto** | [ConfirmUploadDto](ConfirmUploadDto.md) |  | |

### Return type

[**FileDto**](FileDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## storageControllerDeleteCanary

> storageControllerDeleteCanary(id)

Delete a file

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { StorageControllerDeleteCanaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // string | File ID
    id: id_example,
  } satisfies StorageControllerDeleteCanaryRequest;

  try {
    const data = await api.storageControllerDeleteCanary(body);
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
| **id** | `string` | File ID | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## storageControllerGetDownloadUrlCanary

> PresignedDownloadResponseDto storageControllerGetDownloadUrlCanary(id)

Get a presigned download URL for a file

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { StorageControllerGetDownloadUrlCanaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // string | File ID
    id: id_example,
  } satisfies StorageControllerGetDownloadUrlCanaryRequest;

  try {
    const data = await api.storageControllerGetDownloadUrlCanary(body);
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
| **id** | `string` | File ID | [Defaults to `undefined`] |

### Return type

[**PresignedDownloadResponseDto**](PresignedDownloadResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## storageControllerListCanary

> ListFilesResponseDto storageControllerListCanary(merchantId, limit, offset, tag, status, relatedEntityId, relatedEntityType)

List files

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { StorageControllerListCanaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // number | Maximum number of records to return (optional)
    limit: 50,
    // number | Number of records to skip (optional)
    offset: 0,
    // string | Filter by tag (optional)
    tag: tag_example,
    // 'pending' | 'uploaded' | 'failed' | 'deleted' (optional)
    status: status_example,
    // string (optional)
    relatedEntityId: relatedEntityId_example,
    // string (optional)
    relatedEntityType: relatedEntityType_example,
  } satisfies StorageControllerListCanaryRequest;

  try {
    const data = await api.storageControllerListCanary(body);
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
| **tag** | `string` | Filter by tag | [Optional] [Defaults to `undefined`] |
| **status** | `pending`, `uploaded`, `failed`, `deleted` |  | [Optional] [Defaults to `undefined`] [Enum: pending, uploaded, failed, deleted] |
| **relatedEntityId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **relatedEntityType** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**ListFilesResponseDto**](ListFilesResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## storageControllerRequestUploadUrlCanary

> PresignedUploadResponseDto storageControllerRequestUploadUrlCanary(requestUploadUrlDto)

Request a presigned URL for file upload

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { StorageControllerRequestUploadUrlCanaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // RequestUploadUrlDto
    requestUploadUrlDto: {"filename":"identity-document.pdf","mimeType":"application/pdf","tags":["compliance","identity-document"],"relatedEntityId":"compliance_info_123","relatedEntityType":"complianceInfo"},
  } satisfies StorageControllerRequestUploadUrlCanaryRequest;

  try {
    const data = await api.storageControllerRequestUploadUrlCanary(body);
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
| **requestUploadUrlDto** | [RequestUploadUrlDto](RequestUploadUrlDto.md) |  | |

### Return type

[**PresignedUploadResponseDto**](PresignedUploadResponseDto.md)

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
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## storageControllerRetrieveCanary

> FileDto storageControllerRetrieveCanary(id)

Get file details

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { StorageControllerRetrieveCanaryRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // string | File ID
    id: id_example,
  } satisfies StorageControllerRetrieveCanaryRequest;

  try {
    const data = await api.storageControllerRetrieveCanary(body);
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
| **id** | `string` | File ID | [Defaults to `undefined`] |

### Return type

[**FileDto**](FileDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

