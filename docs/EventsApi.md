# EventsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listEvents**](EventsApi.md#listevents) | **GET** /api/canary/events | List Events |



## listEvents

> ListEventsResponseDto listEvents(merchantId, limit, offset, type, status, startDate, endDate)

List Events

Retrieves a log of all API events for debugging and logging.

### Example

```ts
import {
  Configuration,
  EventsApi,
} from '@cashful/typescript';
import type { ListEventsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventsApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // number | Maximum number of records to return (optional)
    limit: 50,
    // number | Number of records to skip (optional)
    offset: 0,
    // string | Filter by event type (optional)
    type: type_example,
    // 'pending' | 'delivered' | 'failed' | Filter by event status (optional)
    status: status_example,
    // string | Filter by start date (optional)
    startDate: startDate_example,
    // string | Filter by end date (optional)
    endDate: endDate_example,
  } satisfies ListEventsRequest;

  try {
    const data = await api.listEvents(body);
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
| **type** | `string` | Filter by event type | [Optional] [Defaults to `undefined`] |
| **status** | `pending`, `delivered`, `failed` | Filter by event status | [Optional] [Defaults to `undefined`] [Enum: pending, delivered, failed] |
| **startDate** | `string` | Filter by start date | [Optional] [Defaults to `undefined`] |
| **endDate** | `string` | Filter by end date | [Optional] [Defaults to `undefined`] |

### Return type

[**ListEventsResponseDto**](ListEventsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved events |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

