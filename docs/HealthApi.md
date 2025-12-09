# HealthApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**checkHealth**](HealthApi.md#checkhealth) | **GET** /api/canary/health | Health check endpoint |



## checkHealth

> any checkHealth()

Health check endpoint

Performs a health check on the application and external dependencies

### Example

```ts
import {
  Configuration,
  HealthApi,
} from '@cashful-co/typescript';
import type { CheckHealthRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new HealthApi();

  try {
    const data = await api.checkHealth();
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

**any**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Application and all dependencies are healthy |  -  |
| **503** | One or more health checks failed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

