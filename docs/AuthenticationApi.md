# AuthenticationApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**acceptInvitation**](AuthenticationApi.md#acceptinvitation) | **POST** /api/canary/authentication/organization/accept-invitation | Accept Invitation |
| [**cancelInvitation**](AuthenticationApi.md#cancelinvitation) | **POST** /api/canary/authentication/organization/cancel-invitation | Cancel Invitation |
| [**changeEmail**](AuthenticationApi.md#changeemail) | **POST** /api/canary/authentication/change-email | Change Email |
| [**changePassword**](AuthenticationApi.md#changepassword) | **POST** /api/canary/authentication/change-password | Change Password |
| [**checkSlug**](AuthenticationApi.md#checkslug) | **POST** /api/canary/authentication/organization/check-slug | Check Slug |
| [**createApiKey**](AuthenticationApi.md#createapikey) | **POST** /api/canary/authentication/api-key/create | Create API Key |
| [**createOrganization**](AuthenticationApi.md#createorganization) | **POST** /api/canary/authentication/organization/create | Create Organization |
| [**deleteApiKey**](AuthenticationApi.md#deleteapikey) | **POST** /api/canary/authentication/api-key/delete | Delete API Key |
| [**deleteOrganization**](AuthenticationApi.md#deleteorganization) | **POST** /api/canary/authentication/organization/delete | Delete Organization |
| [**deleteUser**](AuthenticationApi.md#deleteuser) | **POST** /api/canary/authentication/delete-user | Delete User |
| [**forgetPassword**](AuthenticationApi.md#forgetpassword) | **POST** /api/canary/authentication/forget-password | Forget Password |
| [**getActiveMember**](AuthenticationApi.md#getactivemember) | **GET** /api/canary/authentication/organization/get-active-member | Get Active Member |
| [**getActiveMemberRole**](AuthenticationApi.md#getactivememberrole) | **GET** /api/canary/authentication/organization/get-active-member-role | Get Active Member Role |
| [**getInvitation**](AuthenticationApi.md#getinvitation) | **GET** /api/canary/authentication/organization/get-invitation | Get Invitation |
| [**getOrganization**](AuthenticationApi.md#getorganization) | **GET** /api/canary/authentication/organization/get-full-organization | Get Full Organization |
| [**getSession**](AuthenticationApi.md#getsession) | **GET** /api/canary/authentication/get-session | Get Session |
| [**hasPermission**](AuthenticationApi.md#haspermission) | **POST** /api/canary/authentication/organization/has-permission | Has Permission |
| [**inviteMember**](AuthenticationApi.md#invitemember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member |
| [**leaveOrganization**](AuthenticationApi.md#leaveorganization) | **POST** /api/canary/authentication/organization/leave | Leave Organization |
| [**listApiKeys**](AuthenticationApi.md#listapikeys) | **GET** /api/canary/authentication/api-key/list | List API Keys |
| [**listMembers**](AuthenticationApi.md#listmembers) | **GET** /api/canary/authentication/organization/list-members | List Members |
| [**listOrganizationInvitations**](AuthenticationApi.md#listorganizationinvitations) | **GET** /api/canary/authentication/organization/list-invitations | List Invitations |
| [**listOrganizations**](AuthenticationApi.md#listorganizations) | **GET** /api/canary/authentication/organization/list | List Organizations |
| [**listUserInvitations**](AuthenticationApi.md#listuserinvitations) | **GET** /api/canary/authentication/organization/list-user-invitations | List User Invitations |
| [**listUserSessions**](AuthenticationApi.md#listusersessions) | **GET** /api/canary/authentication/list-sessions | List User Sessions |
| [**rejectInvitation**](AuthenticationApi.md#rejectinvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation |
| [**removeMember**](AuthenticationApi.md#removemember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member |
| [**requestPasswordReset**](AuthenticationApi.md#requestpasswordreset) | **POST** /api/canary/authentication/request-password-reset | Request Password Reset |
| [**resetPassword**](AuthenticationApi.md#resetpassword) | **POST** /api/canary/authentication/reset-password | Reset Password |
| [**resetPasswordCallback**](AuthenticationApi.md#resetpasswordcallback) | **GET** /api/canary/authentication/reset-password/{token} | Reset Password Callback |
| [**revokeSession**](AuthenticationApi.md#revokesession) | **POST** /api/canary/authentication/revoke-session | Revoke Session |
| [**sendVerificationEmail**](AuthenticationApi.md#sendverificationemail) | **POST** /api/canary/authentication/send-verification-email | Send Verification Email |
| [**setActiveOrganization**](AuthenticationApi.md#setactiveorganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization |
| [**signInEmail**](AuthenticationApi.md#signinemail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email |
| [**signOut**](AuthenticationApi.md#signout) | **POST** /api/canary/authentication/sign-out | Sign out |
| [**signUpEmail**](AuthenticationApi.md#signupemail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email |
| [**updateApiKey**](AuthenticationApi.md#updateapikey) | **POST** /api/canary/authentication/api-key/update | Update API Key |
| [**updateMemberRole**](AuthenticationApi.md#updatememberrole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role |
| [**updateOrganization**](AuthenticationApi.md#updateorganization) | **POST** /api/canary/authentication/organization/update | Update Organization |
| [**updateUser**](AuthenticationApi.md#updateuser) | **POST** /api/canary/authentication/update-user | Update User |
| [**verifyApiKey**](AuthenticationApi.md#verifyapikey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key |
| [**verifyEmail**](AuthenticationApi.md#verifyemail) | **GET** /api/canary/authentication/verify-email | Verify Email |



## acceptInvitation

> AcceptInvitationResponseDto acceptInvitation(acceptInvitationDto)

Accept Invitation

Accept an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { AcceptInvitationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**AcceptInvitationResponseDto**](AcceptInvitationResponseDto.md)

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

> CancelInvitationResponseDto cancelInvitation(cancelInvitationDto)

Cancel Invitation

Cancel an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { CancelInvitationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**CancelInvitationResponseDto**](CancelInvitationResponseDto.md)

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


## changeEmail

> ChangeEmailResponseDto changeEmail(changeEmailDto)

Change Email

Change the email address of the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ChangeEmailRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // ChangeEmailDto
    changeEmailDto: ...,
  } satisfies ChangeEmailRequest;

  try {
    const data = await api.changeEmail(body);
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
| **changeEmailDto** | [ChangeEmailDto](ChangeEmailDto.md) |  | |

### Return type

[**ChangeEmailResponseDto**](ChangeEmailResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Email change request processed successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## changePassword

> ChangePasswordResponseDto changePassword(changePasswordDto)

Change Password

Change the password of the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ChangePasswordRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // ChangePasswordDto
    changePasswordDto: ...,
  } satisfies ChangePasswordRequest;

  try {
    const data = await api.changePassword(body);
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
| **changePasswordDto** | [ChangePasswordDto](ChangePasswordDto.md) |  | |

### Return type

[**ChangePasswordResponseDto**](ChangePasswordResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Password changed successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## checkSlug

> CheckSlugResponseDto checkSlug(checkSlugDto)

Check Slug

Check if organization slug is available

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { CheckSlugRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // CheckSlugDto
    checkSlugDto: ...,
  } satisfies CheckSlugRequest;

  try {
    const data = await api.checkSlug(body);
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
| **checkSlugDto** | [CheckSlugDto](CheckSlugDto.md) |  | |

### Return type

[**CheckSlugResponseDto**](CheckSlugResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Slug check completed |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createApiKey

> CreateApiKeyResponseDto createApiKey(createApiKeyDto)

Create API Key

Create a new API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { CreateApiKeyRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**CreateApiKeyResponseDto**](CreateApiKeyResponseDto.md)

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

> CreateOrganizationResponseDto createOrganization(createOrganizationDto)

Create Organization

Create a new organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { CreateOrganizationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**CreateOrganizationResponseDto**](CreateOrganizationResponseDto.md)

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

> DeleteApiKeyResponseDto deleteApiKey(deleteApiKeyDto)

Delete API Key

Delete an API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { DeleteApiKeyRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**DeleteApiKeyResponseDto**](DeleteApiKeyResponseDto.md)

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

> DeleteOrganizationResponseDto deleteOrganization(deleteOrganizationDto)

Delete Organization

Delete an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { DeleteOrganizationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**DeleteOrganizationResponseDto**](DeleteOrganizationResponseDto.md)

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


## deleteUser

> DeleteUserResponseDto deleteUser(deleteUserDto)

Delete User

Delete the current user\&#39;s account

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { DeleteUserRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // DeleteUserDto
    deleteUserDto: ...,
  } satisfies DeleteUserRequest;

  try {
    const data = await api.deleteUser(body);
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
| **deleteUserDto** | [DeleteUserDto](DeleteUserDto.md) |  | |

### Return type

[**DeleteUserResponseDto**](DeleteUserResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User deletion processed successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## forgetPassword

> ForgotPasswordResponseDto forgetPassword(forgotPasswordDto)

Forget Password

Send a password reset email to the user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ForgetPasswordRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**ForgotPasswordResponseDto**](ForgotPasswordResponseDto.md)

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


## getActiveMember

> GetActiveMemberResponseDto getActiveMember(organizationId)

Get Active Member

Get the member details of the active organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { GetActiveMemberRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | Filter by organization ID (optional)
    organizationId: org_12345,
  } satisfies GetActiveMemberRequest;

  try {
    const data = await api.getActiveMember(body);
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
| **organizationId** | `string` | Filter by organization ID | [Optional] [Defaults to `undefined`] |

### Return type

[**GetActiveMemberResponseDto**](GetActiveMemberResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Active member retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getActiveMemberRole

> GetActiveMemberRoleResponseDto getActiveMemberRole(organizationId)

Get Active Member Role

Get the role of the current user in the active organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { GetActiveMemberRoleRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | Filter by organization ID (optional)
    organizationId: org_12345,
  } satisfies GetActiveMemberRoleRequest;

  try {
    const data = await api.getActiveMemberRole(body);
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
| **organizationId** | `string` | Filter by organization ID | [Optional] [Defaults to `undefined`] |

### Return type

[**GetActiveMemberRoleResponseDto**](GetActiveMemberRoleResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Active member role retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getInvitation

> GetInvitationResponseDto getInvitation(invitationId)

Get Invitation

Get an invitation by ID

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { GetInvitationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | The ID of the invitation to get
    invitationId: inv_12345,
  } satisfies GetInvitationRequest;

  try {
    const data = await api.getInvitation(body);
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
| **invitationId** | `string` | The ID of the invitation to get | [Defaults to `undefined`] |

### Return type

[**GetInvitationResponseDto**](GetInvitationResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Invitation retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getOrganization

> GetFullOrganizationResponseDto getOrganization(organizationId)

Get Full Organization

Get the full organization details

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { GetOrganizationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | The organization ID to get (optional)
    organizationId: org_12345,
  } satisfies GetOrganizationRequest;

  try {
    const data = await api.getOrganization(body);
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
| **organizationId** | `string` | The organization ID to get | [Optional] [Defaults to `undefined`] |

### Return type

[**GetFullOrganizationResponseDto**](GetFullOrganizationResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
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
} from '@cashful-co/typescript';
import type { GetSessionRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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


## hasPermission

> HasPermissionResponseDto hasPermission(hasPermissionDto)

Has Permission

Check if a user has permission

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { HasPermissionRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // HasPermissionDto
    hasPermissionDto: ...,
  } satisfies HasPermissionRequest;

  try {
    const data = await api.hasPermission(body);
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
| **hasPermissionDto** | [HasPermissionDto](HasPermissionDto.md) |  | |

### Return type

[**HasPermissionResponseDto**](HasPermissionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Permission check completed |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## inviteMember

> InviteMemberResponseDto inviteMember(inviteMemberDto)

Invite Member

Invite a user to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { InviteMemberRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**InviteMemberResponseDto**](InviteMemberResponseDto.md)

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


## leaveOrganization

> LeaveOrganizationResponseDto leaveOrganization(leaveOrganizationDto)

Leave Organization

Leave an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { LeaveOrganizationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // LeaveOrganizationDto
    leaveOrganizationDto: ...,
  } satisfies LeaveOrganizationRequest;

  try {
    const data = await api.leaveOrganization(body);
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
| **leaveOrganizationDto** | [LeaveOrganizationDto](LeaveOrganizationDto.md) |  | |

### Return type

[**LeaveOrganizationResponseDto**](LeaveOrganizationResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Left organization successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listApiKeys

> ListApiKeysResponseDto listApiKeys()

List API Keys

List all API keys for the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ListApiKeysRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**ListApiKeysResponseDto**](ListApiKeysResponseDto.md)

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


## listMembers

> ListMembersResponseDto listMembers(organizationId)

List Members

List all members of an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ListMembersRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | Filter by organization ID (optional)
    organizationId: org_12345,
  } satisfies ListMembersRequest;

  try {
    const data = await api.listMembers(body);
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
| **organizationId** | `string` | Filter by organization ID | [Optional] [Defaults to `undefined`] |

### Return type

[**ListMembersResponseDto**](ListMembersResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Members listed successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrganizationInvitations

> ListInvitationsResponseDto listOrganizationInvitations(organizationId)

List Invitations

List all invitations a user has received

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ListOrganizationInvitationsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | Filter by organization ID (optional)
    organizationId: org_12345,
  } satisfies ListOrganizationInvitationsRequest;

  try {
    const data = await api.listOrganizationInvitations(body);
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
| **organizationId** | `string` | Filter by organization ID | [Optional] [Defaults to `undefined`] |

### Return type

[**ListInvitationsResponseDto**](ListInvitationsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Invitations listed successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrganizations

> Array&lt;OrganizationDto&gt; listOrganizations(include)

List Organizations

List all organizations for the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ListOrganizationsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // boolean | Include additional organization data (optional)
    include: true,
  } satisfies ListOrganizationsRequest;

  try {
    const data = await api.listOrganizations(body);
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
| **include** | `boolean` | Include additional organization data | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;OrganizationDto&gt;**](OrganizationDto.md)

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


## listUserInvitations

> ListUserInvitationsResponseDto listUserInvitations(status)

List User Invitations

List all invitations a user has received

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ListUserInvitationsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | Filter by status (optional)
    status: pending,
  } satisfies ListUserInvitationsRequest;

  try {
    const data = await api.listUserInvitations(body);
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
| **status** | `string` | Filter by status | [Optional] [Defaults to `undefined`] |

### Return type

[**ListUserInvitationsResponseDto**](ListUserInvitationsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User invitations listed successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listUserSessions

> ListSessionsResponseDto listUserSessions()

List User Sessions

List all active sessions for the user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ListUserSessionsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.listUserSessions();
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

[**ListSessionsResponseDto**](ListSessionsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Sessions listed successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## rejectInvitation

> RejectInvitationResponseDto rejectInvitation(rejectInvitationDto)

Reject Invitation

Reject an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { RejectInvitationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**RejectInvitationResponseDto**](RejectInvitationResponseDto.md)

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

> RemoveMemberResponseDto removeMember(removeMemberDto)

Remove Member

Remove a member from an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { RemoveMemberRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**RemoveMemberResponseDto**](RemoveMemberResponseDto.md)

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


## requestPasswordReset

> RequestPasswordResetResponseDto requestPasswordReset(requestPasswordResetDto)

Request Password Reset

Send a password reset email to the user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { RequestPasswordResetRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // RequestPasswordResetDto
    requestPasswordResetDto: ...,
  } satisfies RequestPasswordResetRequest;

  try {
    const data = await api.requestPasswordReset(body);
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
| **requestPasswordResetDto** | [RequestPasswordResetDto](RequestPasswordResetDto.md) |  | |

### Return type

[**RequestPasswordResetResponseDto**](RequestPasswordResetResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Password reset email sent successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resetPassword

> ResetPasswordResponseDto resetPassword(resetPasswordDto)

Reset Password

Reset the user\&#39;s password using a token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ResetPasswordRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**ResetPasswordResponseDto**](ResetPasswordResponseDto.md)

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


## resetPasswordCallback

> ResetPasswordCallbackResponseDto resetPasswordCallback(callbackURL, token)

Reset Password Callback

Redirects user to callback URL with token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { ResetPasswordCallbackRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // string
    callbackURL: callbackURL_example,
    // string
    token: token_example,
  } satisfies ResetPasswordCallbackRequest;

  try {
    const data = await api.resetPasswordCallback(body);
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
| **callbackURL** | `string` |  | [Defaults to `undefined`] |
| **token** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ResetPasswordCallbackResponseDto**](ResetPasswordCallbackResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Password reset token validated |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## revokeSession

> RevokeSessionResponseDto revokeSession(revokeSessionDto)

Revoke Session

Revoke a specific session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { RevokeSessionRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // RevokeSessionDto
    revokeSessionDto: ...,
  } satisfies RevokeSessionRequest;

  try {
    const data = await api.revokeSession(body);
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
| **revokeSessionDto** | [RevokeSessionDto](RevokeSessionDto.md) |  | |

### Return type

[**RevokeSessionResponseDto**](RevokeSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Session revoked successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendVerificationEmail

> SendVerificationEmailResponseDto sendVerificationEmail(sendVerificationEmailDto)

Send Verification Email

Send a verification email to the user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { SendVerificationEmailRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // SendVerificationEmailDto
    sendVerificationEmailDto: ...,
  } satisfies SendVerificationEmailRequest;

  try {
    const data = await api.sendVerificationEmail(body);
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
| **sendVerificationEmailDto** | [SendVerificationEmailDto](SendVerificationEmailDto.md) |  | |

### Return type

[**SendVerificationEmailResponseDto**](SendVerificationEmailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Verification email sent successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## setActiveOrganization

> SetActiveOrganizationResponseDto setActiveOrganization(setActiveOrganizationDto)

Set Active Organization

Set the active organization for the current session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { SetActiveOrganizationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**SetActiveOrganizationResponseDto**](SetActiveOrganizationResponseDto.md)

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

> SignInResponseDto signInEmail(signInDto)

Sign in with email

Authenticate a user using email and password

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { SignInEmailRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**SignInResponseDto**](SignInResponseDto.md)

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

> SignOutResponseDto signOut()

Sign out

Sign out the current user and invalidate the session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { SignOutRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**SignOutResponseDto**](SignOutResponseDto.md)

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

> SignUpResponseDto signUpEmail(signUpDto)

Sign up with email

Create a new user account using email and password

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { SignUpEmailRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**SignUpResponseDto**](SignUpResponseDto.md)

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

> UpdateApiKeyResponseDto updateApiKey(updateApiKeyDto)

Update API Key

Update an API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { UpdateApiKeyRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**UpdateApiKeyResponseDto**](UpdateApiKeyResponseDto.md)

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

> UpdateMemberRoleResponseDto updateMemberRole(updateMemberRoleDto)

Update Member Role

Update a member\&#39;s role in an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { UpdateMemberRoleRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**UpdateMemberRoleResponseDto**](UpdateMemberRoleResponseDto.md)

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

> UpdateOrganizationResponseDto updateOrganization(updateOrganizationDto)

Update Organization

Update an organization\&#39;s details

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { UpdateOrganizationRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**UpdateOrganizationResponseDto**](UpdateOrganizationResponseDto.md)

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


## updateUser

> UpdateUserResponseDto updateUser(updateUserDto)

Update User

Update the current user\&#39;s information

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { UpdateUserRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // UpdateUserDto
    updateUserDto: ...,
  } satisfies UpdateUserRequest;

  try {
    const data = await api.updateUser(body);
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
| **updateUserDto** | [UpdateUserDto](UpdateUserDto.md) |  | |

### Return type

[**UpdateUserResponseDto**](UpdateUserResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## verifyApiKey

> VerifyApiKeyResponseDto verifyApiKey(verifyApiKeyDto)

Verify API Key

Verify an API key

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { VerifyApiKeyRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
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

[**VerifyApiKeyResponseDto**](VerifyApiKeyResponseDto.md)

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


## verifyEmail

> VerifyEmailResponseDto verifyEmail(token, callbackURL)

Verify Email

Verify the email of a user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful-co/typescript';
import type { VerifyEmailRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // string
    token: token_example,
    // string (optional)
    callbackURL: callbackURL_example,
  } satisfies VerifyEmailRequest;

  try {
    const data = await api.verifyEmail(body);
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
| **token** | `string` |  | [Defaults to `undefined`] |
| **callbackURL** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**VerifyEmailResponseDto**](VerifyEmailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Email verified successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

