# StorageApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**confirmUpload**](StorageApi.md#confirmupload) | **POST** /api/canary/storage/confirm-upload | Confirm that a file upload was completed |
| [**deleteFile**](StorageApi.md#deletefile) | **DELETE** /api/canary/storage/{id} | Delete a file |
| [**getDownloadUrl**](StorageApi.md#getdownloadurl) | **GET** /api/canary/storage/{id}/download-url | Get a presigned download URL for a file |
| [**getFileDetails**](StorageApi.md#getfiledetails) | **GET** /api/canary/storage/{id} | Get file details |
| [**listFiles**](StorageApi.md#listfiles) | **GET** /api/canary/storage | List files |
| [**requestUploadUrl**](StorageApi.md#requestuploadurl) | **POST** /api/canary/storage/upload-url | Request a presigned URL for file upload |



## confirmUpload

> FileDto confirmUpload(confirmUploadDto)

Confirm that a file upload was completed

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { ConfirmUploadRequest } from '@cashful/typescript';

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
  } satisfies ConfirmUploadRequest;

  try {
    const data = await api.confirmUpload(body);
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


## deleteFile

> deleteFile(id)

Delete a file

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { DeleteFileRequest } from '@cashful/typescript';

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
  } satisfies DeleteFileRequest;

  try {
    const data = await api.deleteFile(body);
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


## getDownloadUrl

> PresignedDownloadResponseDto getDownloadUrl(id)

Get a presigned download URL for a file

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { GetDownloadUrlRequest } from '@cashful/typescript';

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
  } satisfies GetDownloadUrlRequest;

  try {
    const data = await api.getDownloadUrl(body);
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


## getFileDetails

> FileDto getFileDetails(id)

Get file details

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { GetFileDetailsRequest } from '@cashful/typescript';

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
  } satisfies GetFileDetailsRequest;

  try {
    const data = await api.getFileDetails(body);
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


## listFiles

> ListFilesResponseDto listFiles(limit, offset, tag, status, relatedEntityId, relatedEntityType)

List files

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { ListFilesRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
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
  } satisfies ListFilesRequest;

  try {
    const data = await api.listFiles(body);
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


## requestUploadUrl

> PresignedUploadResponseDto requestUploadUrl(requestUploadUrlDto)

Request a presigned URL for file upload

### Example

```ts
import {
  Configuration,
  StorageApi,
} from '@cashful/typescript';
import type { RequestUploadUrlRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StorageApi(config);

  const body = {
    // RequestUploadUrlDto
    requestUploadUrlDto: {"filename":"iphone-15.png","mimeType":"image/png","isPublic":true,"tags":["product","image"],"relatedEntityId":"product_123","relatedEntityType":"product"},
  } satisfies RequestUploadUrlRequest;

  try {
    const data = await api.requestUploadUrl(body);
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

