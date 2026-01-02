# NotificationsApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**sendEmail**](NotificationsApi.md#sendemail) | **POST** /api/canary/notifications/email | Send an email notification |
| [**sendMultiChannelNotification**](NotificationsApi.md#sendmultichannelnotification) | **POST** /api/canary/notifications/multi-channel | Send notifications via multiple channels |
| [**sendNotification**](NotificationsApi.md#sendnotification) | **POST** /api/canary/notifications/send | Send a notification via specified channel |
| [**sendSms**](NotificationsApi.md#sendsms) | **POST** /api/canary/notifications/sms | Send an SMS notification |



## sendEmail

> SendEmail200Response sendEmail(sendEmailDto)

Send an email notification

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from '@cashful-co/typescript';
import type { SendEmailRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new NotificationsApi();

  const body = {
    // SendEmailDto
    sendEmailDto: ...,
  } satisfies SendEmailRequest;

  try {
    const data = await api.sendEmail(body);
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
| **sendEmailDto** | [SendEmailDto](SendEmailDto.md) |  | |

### Return type

[**SendEmail200Response**](SendEmail200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Email sent successfully |  -  |
| **400** | Bad request |  -  |
| **500** | Failed to send email |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendMultiChannelNotification

> SendMultiChannelNotification200Response sendMultiChannelNotification()

Send notifications via multiple channels

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from '@cashful-co/typescript';
import type { SendMultiChannelNotificationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new NotificationsApi();

  try {
    const data = await api.sendMultiChannelNotification();
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

[**SendMultiChannelNotification200Response**](SendMultiChannelNotification200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Notifications sent |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendNotification

> sendNotification(notificationDto)

Send a notification via specified channel

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from '@cashful-co/typescript';
import type { SendNotificationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new NotificationsApi();

  const body = {
    // NotificationDto
    notificationDto: ...,
  } satisfies SendNotificationRequest;

  try {
    const data = await api.sendNotification(body);
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
| **notificationDto** | [NotificationDto](NotificationDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Notification sent successfully |  -  |
| **400** | Bad request |  -  |
| **500** | Failed to send notification |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendSms

> SendSms200Response sendSms(sendSmsDto)

Send an SMS notification

### Example

```ts
import {
  Configuration,
  NotificationsApi,
} from '@cashful-co/typescript';
import type { SendSmsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new NotificationsApi();

  const body = {
    // SendSmsDto
    sendSmsDto: ...,
  } satisfies SendSmsRequest;

  try {
    const data = await api.sendSms(body);
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
| **sendSmsDto** | [SendSmsDto](SendSmsDto.md) |  | |

### Return type

[**SendSms200Response**](SendSms200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SMS sent successfully |  -  |
| **400** | Bad request |  -  |
| **500** | Failed to send SMS |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

