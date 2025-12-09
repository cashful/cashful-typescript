# AuthenticationApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**acceptInvitation**](AuthenticationApi.md#acceptinvitation) | **POST** /api/canary/authentication/organization/accept-invitation | Accept Invitation |
| [**cancelInvitation**](AuthenticationApi.md#cancelinvitation) | **POST** /api/canary/authentication/organization/cancel-invitation | Cancel Invitation |
| [**createApiKey**](AuthenticationApi.md#createapikey) | **POST** /api/canary/authentication/api-key/create | Create API Key |
| [**createOrganization**](AuthenticationApi.md#createorganization) | **POST** /api/canary/authentication/organization/create | Create Organization |
| [**deleteApiKey**](AuthenticationApi.md#deleteapikey) | **POST** /api/canary/authentication/api-key/delete | Delete API Key |
| [**deleteOrganization**](AuthenticationApi.md#deleteorganization) | **POST** /api/canary/authentication/organization/delete | Delete Organization |
| [**forgetPassword**](AuthenticationApi.md#forgetpassword) | **POST** /api/canary/authentication/forget-password | Forget Password |
| [**getSession**](AuthenticationApi.md#getsession) | **GET** /api/canary/authentication/get-session | Get Session |
| [**inviteMember**](AuthenticationApi.md#invitemember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member |
| [**listApiKeys**](AuthenticationApi.md#listapikeys) | **GET** /api/canary/authentication/api-key/list | List API Keys |
| [**listOrganizations**](AuthenticationApi.md#listorganizations) | **GET** /api/canary/authentication/organization/list | List Organizations |
| [**rejectInvitation**](AuthenticationApi.md#rejectinvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation |
| [**removeMember**](AuthenticationApi.md#removemember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member |
| [**resetPassword**](AuthenticationApi.md#resetpassword) | **POST** /api/canary/authentication/reset-password | Reset Password |
| [**setActiveOrganization**](AuthenticationApi.md#setactiveorganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization |
| [**signInEmail**](AuthenticationApi.md#signinemail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email |
| [**signOut**](AuthenticationApi.md#signout) | **POST** /api/canary/authentication/sign-out | Sign out |
| [**signUpEmail**](AuthenticationApi.md#signupemail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email |
| [**updateApiKey**](AuthenticationApi.md#updateapikey) | **POST** /api/canary/authentication/api-key/update | Update API Key |
| [**updateMemberRole**](AuthenticationApi.md#updatememberrole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role |
| [**updateOrganization**](AuthenticationApi.md#updateorganization) | **POST** /api/canary/authentication/organization/update | Update Organization |
| [**verifyApiKey**](AuthenticationApi.md#verifyapikey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key |



## acceptInvitation

> acceptInvitation(acceptInvitationDto)

Accept Invitation

Accept an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { AcceptInvitationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // AcceptInvitationDto
    acceptInvitationDto: ...,
  } satisfies AcceptInvitationRequest;

  try {
    const data = await api.acceptInvitation(body);
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
| **acceptInvitationDto** | [AcceptInvitationDto](AcceptInvitationDto.md) |  | |

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
| **200** | Invitation accepted successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## cancelInvitation

> cancelInvitation(cancelInvitationDto)

Cancel Invitation

Cancel an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { CancelInvitationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // CancelInvitationDto
    cancelInvitationDto: ...,
  } satisfies CancelInvitationRequest;

  try {
    const data = await api.cancelInvitation(body);
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
| **cancelInvitationDto** | [CancelInvitationDto](CancelInvitationDto.md) |  | |

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
| **200** | Invitation cancelled successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createApiKey

> createApiKey(createApiKeyDto)

Create API Key

Create a new API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { CreateApiKeyRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // CreateApiKeyDto
    createApiKeyDto: ...,
  } satisfies CreateApiKeyRequest;

  try {
    const data = await api.createApiKey(body);
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
| **createApiKeyDto** | [CreateApiKeyDto](CreateApiKeyDto.md) |  | |

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
| **200** | API key created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createOrganization

> createOrganization(createOrganizationDto)

Create Organization

Create a new organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { CreateOrganizationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // CreateOrganizationDto
    createOrganizationDto: ...,
  } satisfies CreateOrganizationRequest;

  try {
    const data = await api.createOrganization(body);
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
| **createOrganizationDto** | [CreateOrganizationDto](CreateOrganizationDto.md) |  | |

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
| **200** | Organization created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteApiKey

> deleteApiKey(deleteApiKeyDto)

Delete API Key

Delete an API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { DeleteApiKeyRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // DeleteApiKeyDto
    deleteApiKeyDto: ...,
  } satisfies DeleteApiKeyRequest;

  try {
    const data = await api.deleteApiKey(body);
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
| **deleteApiKeyDto** | [DeleteApiKeyDto](DeleteApiKeyDto.md) |  | |

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
| **200** | API key deleted successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteOrganization

> deleteOrganization(deleteOrganizationDto)

Delete Organization

Delete an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { DeleteOrganizationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // DeleteOrganizationDto
    deleteOrganizationDto: ...,
  } satisfies DeleteOrganizationRequest;

  try {
    const data = await api.deleteOrganization(body);
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
| **deleteOrganizationDto** | [DeleteOrganizationDto](DeleteOrganizationDto.md) |  | |

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
| **200** | Organization deleted successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## forgetPassword

> forgetPassword(forgotPasswordDto)

Forget Password

Send a password reset email to the user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { ForgetPasswordRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const api = new AuthenticationApi();

  const body = {
    // ForgotPasswordDto
    forgotPasswordDto: ...,
  } satisfies ForgetPasswordRequest;

  try {
    const data = await api.forgetPassword(body);
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
| **forgotPasswordDto** | [ForgotPasswordDto](ForgotPasswordDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Password reset email sent |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSession

> GetSessionResponseDto getSession()

Get Session

Retrieve the current user session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { GetSessionRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.getSession();
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

[**GetSessionResponseDto**](GetSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Session retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## inviteMember

> inviteMember(inviteMemberDto)

Invite Member

Invite a user to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { InviteMemberRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // InviteMemberDto
    inviteMemberDto: ...,
  } satisfies InviteMemberRequest;

  try {
    const data = await api.inviteMember(body);
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
| **inviteMemberDto** | [InviteMemberDto](InviteMemberDto.md) |  | |

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
| **200** | Member invited successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listApiKeys

> listApiKeys()

List API Keys

List all API keys for the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { ListApiKeysRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.listApiKeys();
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

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | API keys listed successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrganizations

> listOrganizations()

List Organizations

List all organizations for the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { ListOrganizationsRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.listOrganizations();
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

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organizations listed successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## rejectInvitation

> rejectInvitation(rejectInvitationDto)

Reject Invitation

Reject an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { RejectInvitationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // RejectInvitationDto
    rejectInvitationDto: ...,
  } satisfies RejectInvitationRequest;

  try {
    const data = await api.rejectInvitation(body);
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
| **rejectInvitationDto** | [RejectInvitationDto](RejectInvitationDto.md) |  | |

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
| **200** | Invitation rejected successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## removeMember

> removeMember(removeMemberDto)

Remove Member

Remove a member from an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { RemoveMemberRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // RemoveMemberDto
    removeMemberDto: ...,
  } satisfies RemoveMemberRequest;

  try {
    const data = await api.removeMember(body);
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
| **removeMemberDto** | [RemoveMemberDto](RemoveMemberDto.md) |  | |

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
| **200** | Member removed successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resetPassword

> resetPassword(resetPasswordDto)

Reset Password

Reset the user\&#39;s password using a token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { ResetPasswordRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const api = new AuthenticationApi();

  const body = {
    // ResetPasswordDto
    resetPasswordDto: ...,
  } satisfies ResetPasswordRequest;

  try {
    const data = await api.resetPassword(body);
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
| **resetPasswordDto** | [ResetPasswordDto](ResetPasswordDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Password reset successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setActiveOrganization

> setActiveOrganization(setActiveOrganizationDto)

Set Active Organization

Set the active organization for the current session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { SetActiveOrganizationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // SetActiveOrganizationDto
    setActiveOrganizationDto: ...,
  } satisfies SetActiveOrganizationRequest;

  try {
    const data = await api.setActiveOrganization(body);
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
| **setActiveOrganizationDto** | [SetActiveOrganizationDto](SetActiveOrganizationDto.md) |  | |

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
| **200** | Active organization set successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## signInEmail

> signInEmail(signInDto)

Sign in with email

Authenticate a user using email and password

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { SignInEmailRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const api = new AuthenticationApi();

  const body = {
    // SignInDto
    signInDto: ...,
  } satisfies SignInEmailRequest;

  try {
    const data = await api.signInEmail(body);
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
| **signInDto** | [SignInDto](SignInDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User signed in successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## signOut

> signOut()

Sign out

Sign out the current user and invalidate the session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { SignOutRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.signOut();
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

`void` (Empty response body)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User signed out successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## signUpEmail

> signUpEmail(signUpDto)

Sign up with email

Create a new user account using email and password

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { SignUpEmailRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const api = new AuthenticationApi();

  const body = {
    // SignUpDto
    signUpDto: ...,
  } satisfies SignUpEmailRequest;

  try {
    const data = await api.signUpEmail(body);
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
| **signUpDto** | [SignUpDto](SignUpDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateApiKey

> updateApiKey(updateApiKeyDto)

Update API Key

Update an API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { UpdateApiKeyRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // UpdateApiKeyDto
    updateApiKeyDto: ...,
  } satisfies UpdateApiKeyRequest;

  try {
    const data = await api.updateApiKey(body);
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
| **updateApiKeyDto** | [UpdateApiKeyDto](UpdateApiKeyDto.md) |  | |

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
| **200** | API key updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateMemberRole

> updateMemberRole(updateMemberRoleDto)

Update Member Role

Update a member\&#39;s role in an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { UpdateMemberRoleRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // UpdateMemberRoleDto
    updateMemberRoleDto: ...,
  } satisfies UpdateMemberRoleRequest;

  try {
    const data = await api.updateMemberRole(body);
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
| **updateMemberRoleDto** | [UpdateMemberRoleDto](UpdateMemberRoleDto.md) |  | |

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
| **200** | Member role updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateOrganization

> updateOrganization(updateOrganizationDto)

Update Organization

Update an organization\&#39;s details

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { UpdateOrganizationRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // UpdateOrganizationDto
    updateOrganizationDto: ...,
  } satisfies UpdateOrganizationRequest;

  try {
    const data = await api.updateOrganization(body);
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
| **updateOrganizationDto** | [UpdateOrganizationDto](UpdateOrganizationDto.md) |  | |

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
| **200** | Organization updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## verifyApiKey

> verifyApiKey(verifyApiKeyDto)

Verify API Key

Verify an API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript-sdk';
import type { VerifyApiKeyRequest } from '@cashful-co/typescript-sdk';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript-sdk SDK...");
  const api = new AuthenticationApi();

  const body = {
    // VerifyApiKeyDto
    verifyApiKeyDto: ...,
  } satisfies VerifyApiKeyRequest;

  try {
    const data = await api.verifyApiKey(body);
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
| **verifyApiKeyDto** | [VerifyApiKeyDto](VerifyApiKeyDto.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | API key verified successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

