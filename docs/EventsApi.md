# EventsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEvent**](EventsApi.md#createevent) | **POST** /api/canary/events | Create Event |
| [**listEventTypes**](EventsApi.md#listeventtypes) | **GET** /api/canary/events/types | List Event Types |
| [**listEvents**](EventsApi.md#listevents) | **GET** /api/canary/events | List Events |



## createEvent

> createEvent(createEventDto)

Create Event

Records a new event and triggers associated webhooks.

### Example

```ts
import {
  Configuration,
  EventsApi,
} from '@cashful/typescript';
import type { CreateEventRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventsApi(config);

  const body = {
    // CreateEventDto
    createEventDto: ...,
  } satisfies CreateEventRequest;

  try {
    const data = await api.createEvent(body);
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
| **createEventDto** | [CreateEventDto](CreateEventDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Event successfully created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listEventTypes

> ListEventTypesResponseDto listEventTypes()

List Event Types

Retrieves all available event types that can be sent or subscribed to.

### Example

```ts
import {
  Configuration,
  EventsApi,
} from '@cashful/typescript';
import type { ListEventTypesRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventsApi(config);

  try {
    const data = await api.listEventTypes();
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

[**ListEventTypesResponseDto**](ListEventTypesResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved event types |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listEvents

> ListEventsResponseDto listEvents(merchantId, limit, offset, filter, sort, order, type, status, startDate, endDate)

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
    // string | The ID of the merchant whose events are being requested. This parameter is required.
    merchantId: merchantId_example,
    // number | Maximum number of records to return (optional)
    limit: 50,
    // number | Number of records to skip (optional)
    offset: 0,
    // string | JSON string used for dynamic filtering (optional)
    filter: {"ids":["prod_123","prod_456"]},
    // string | Field name to sort by (optional)
    sort: createdAt,
    // string | Sort direction (ASC or DESC) (optional)
    order: DESC,
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
| **merchantId** | `string` | The ID of the merchant whose events are being requested. This parameter is required. | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |
| **filter** | `string` | JSON string used for dynamic filtering | [Optional] [Defaults to `undefined`] |
| **sort** | `string` | Field name to sort by | [Optional] [Defaults to `undefined`] |
| **order** | `string` | Sort direction (ASC or DESC) | [Optional] [Defaults to `undefined`] |
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

