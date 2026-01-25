# AuthenticationApi

All URIs are relative to *https://api.cashful.africa*

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
| [**getAccessToken**](AuthenticationApi.md#getaccesstoken) | **POST** /api/canary/authentication/get-access-token | Get Access Token |
| [**getActiveMember**](AuthenticationApi.md#getactivemember) | **GET** /api/canary/authentication/organization/get-active-member | Get Active Member |
| [**getActiveMemberRole**](AuthenticationApi.md#getactivememberrole) | **GET** /api/canary/authentication/organization/get-active-member-role | Get Active Member Role |
| [**getApiKey**](AuthenticationApi.md#getapikey) | **GET** /api/canary/authentication/api-key/get | Get API Key |
| [**getInvitation**](AuthenticationApi.md#getinvitation) | **GET** /api/canary/authentication/organization/get-invitation | Get Invitation |
| [**getJSONWebKeySet**](AuthenticationApi.md#getjsonwebkeyset) | **GET** /api/canary/authentication/jwks | Get the JSON Web Key Set |
| [**getJSONWebToken**](AuthenticationApi.md#getjsonwebtoken) | **GET** /api/canary/authentication/token | Get a JWT token |
| [**getOrganization**](AuthenticationApi.md#getorganization) | **GET** /api/canary/authentication/organization/get-full-organization | Get Full Organization |
| [**getSession**](AuthenticationApi.md#getsession) | **GET** /api/canary/authentication/get-session | Get Session |
| [**hasPermission**](AuthenticationApi.md#haspermission) | **POST** /api/canary/authentication/organization/has-permission | Has Permission |
| [**inviteMember**](AuthenticationApi.md#invitemember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member |
| [**isUsernameAvailable**](AuthenticationApi.md#isusernameavailable) | **POST** /api/canary/authentication/is-username-available | Check Username Availability |
| [**leaveOrganization**](AuthenticationApi.md#leaveorganization) | **POST** /api/canary/authentication/organization/leave | Leave Organization |
| [**linkSocial**](AuthenticationApi.md#linksocial) | **POST** /api/canary/authentication/link-social | Link Social Account |
| [**listAccounts**](AuthenticationApi.md#listaccounts) | **GET** /api/canary/authentication/list-accounts | List Linked Accounts |
| [**listApiKeys**](AuthenticationApi.md#listapikeys) | **GET** /api/canary/authentication/api-key/list | List API Keys |
| [**listMembers**](AuthenticationApi.md#listmembers) | **GET** /api/canary/authentication/organization/list-members | List Members |
| [**listOrganizationInvitations**](AuthenticationApi.md#listorganizationinvitations) | **GET** /api/canary/authentication/organization/list-invitations | List Invitations |
| [**listOrganizations**](AuthenticationApi.md#listorganizations) | **GET** /api/canary/authentication/organization/list | List Organizations |
| [**listUserInvitations**](AuthenticationApi.md#listuserinvitations) | **GET** /api/canary/authentication/organization/list-user-invitations | List User Invitations |
| [**listUserSessions**](AuthenticationApi.md#listusersessions) | **GET** /api/canary/authentication/list-sessions | List User Sessions |
| [**ok**](AuthenticationApi.md#ok) | **GET** /api/canary/authentication/ok | Health Check |
| [**refreshToken**](AuthenticationApi.md#refreshtoken) | **POST** /api/canary/authentication/refresh-token | Refresh Token |
| [**rejectInvitation**](AuthenticationApi.md#rejectinvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation |
| [**removeMember**](AuthenticationApi.md#removemember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member |
| [**requestPasswordReset**](AuthenticationApi.md#requestpasswordreset) | **POST** /api/canary/authentication/request-password-reset | Request Password Reset |
| [**requestPhonePasswordReset**](AuthenticationApi.md#requestphonepasswordreset) | **POST** /api/canary/authentication/phone-number/request-password-reset | Request Password Reset via Phone |
| [**resetPassword**](AuthenticationApi.md#resetpassword) | **POST** /api/canary/authentication/reset-password | Reset Password |
| [**resetPasswordCallback**](AuthenticationApi.md#resetpasswordcallback) | **GET** /api/canary/authentication/reset-password/{token} | Reset Password Callback |
| [**resetPhonePassword**](AuthenticationApi.md#resetphonepassword) | **POST** /api/canary/authentication/phone-number/reset-password | Reset Password with Phone |
| [**revokeOtherSessions**](AuthenticationApi.md#revokeothersessions) | **POST** /api/canary/authentication/revoke-other-sessions | Revoke Other Sessions |
| [**revokeSession**](AuthenticationApi.md#revokesession) | **POST** /api/canary/authentication/revoke-session | Revoke Session |
| [**revokeSessions**](AuthenticationApi.md#revokesessions) | **POST** /api/canary/authentication/revoke-sessions | Revoke All Sessions |
| [**sendPhoneOTP**](AuthenticationApi.md#sendphoneotp) | **POST** /api/canary/authentication/phone-number/send-otp | Send OTP to Phone |
| [**sendVerificationEmail**](AuthenticationApi.md#sendverificationemail) | **POST** /api/canary/authentication/send-verification-email | Send Verification Email |
| [**setActiveOrganization**](AuthenticationApi.md#setactiveorganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization |
| [**signInEmail**](AuthenticationApi.md#signinemail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email |
| [**signInPhoneNumber**](AuthenticationApi.md#signinphonenumber) | **POST** /api/canary/authentication/sign-in/phone-number | Sign in with Phone Number |
| [**signOut**](AuthenticationApi.md#signout) | **POST** /api/canary/authentication/sign-out | Sign out |
| [**signUpEmail**](AuthenticationApi.md#signupemail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email |
| [**socialSignIn**](AuthenticationApi.md#socialsignin) | **POST** /api/canary/authentication/sign-in/social | Sign in with social provider |
| [**unlinkAccount**](AuthenticationApi.md#unlinkaccount) | **POST** /api/canary/authentication/unlink-account | Unlink Social Account |
| [**updateApiKey**](AuthenticationApi.md#updateapikey) | **POST** /api/canary/authentication/api-key/update | Update API Key |
| [**updateMemberRole**](AuthenticationApi.md#updatememberrole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role |
| [**updateOrganization**](AuthenticationApi.md#updateorganization) | **POST** /api/canary/authentication/organization/update | Update Organization |
| [**updateUser**](AuthenticationApi.md#updateuser) | **POST** /api/canary/authentication/update-user | Update User |
| [**verifyApiKey**](AuthenticationApi.md#verifyapikey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key |
| [**verifyEmail**](AuthenticationApi.md#verifyemail) | **GET** /api/canary/authentication/verify-email | Verify Email |
| [**verifyPhoneNumber**](AuthenticationApi.md#verifyphonenumber) | **POST** /api/canary/authentication/phone-number/verify | Verify Phone Number |



## acceptInvitation

> AcceptInvitationResponseDto acceptInvitation(acceptInvitationDto)

Accept Invitation

Accept an invitation to an organization

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { AcceptInvitationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { CancelInvitationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ChangeEmailRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ChangePasswordRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { CheckSlugRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { CreateApiKeyRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { CreateOrganizationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { DeleteApiKeyRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { DeleteOrganizationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { DeleteUserRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ForgetPasswordRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## getAccessToken

> GetAccessTokenResponseDto getAccessToken(getAccessTokenDto)

Get Access Token

Get current access token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { GetAccessTokenRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // GetAccessTokenDto
    getAccessTokenDto: ...,
  } satisfies GetAccessTokenRequest;

  try {
    const data = await api.getAccessToken(body);
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
| **getAccessTokenDto** | [GetAccessTokenDto](GetAccessTokenDto.md) |  | |

### Return type

[**GetAccessTokenResponseDto**](GetAccessTokenResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Access token retrieved successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
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
} from '@cashful/typescript';
import type { GetActiveMemberRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { GetActiveMemberRoleRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## getApiKey

> GetApiKeyResponseDto getApiKey(id)

Get API Key

Retrieve a specific API key by ID

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { GetApiKeyRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // string | The ID of API key to retrieve
    id: key_12345,
  } satisfies GetApiKeyRequest;

  try {
    const data = await api.getApiKey(body);
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
| **id** | `string` | The ID of API key to retrieve | [Defaults to `undefined`] |

### Return type

[**GetApiKeyResponseDto**](GetApiKeyResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | API key retrieved successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
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
} from '@cashful/typescript';
import type { GetInvitationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## getJSONWebKeySet

> GetJsonWebKeySetResponseDto getJSONWebKeySet()

Get the JSON Web Key Set

Get the JSON Web Key Set

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { GetJSONWebKeySetRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.getJSONWebKeySet();
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

[**GetJsonWebKeySetResponseDto**](GetJsonWebKeySetResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | JSON Web Key Set retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getJSONWebToken

> GetJsonWebTokenResponseDto getJSONWebToken()

Get a JWT token

Get a JWT token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { GetJSONWebTokenRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.getJSONWebToken();
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

[**GetJsonWebTokenResponseDto**](GetJsonWebTokenResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
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
} from '@cashful/typescript';
import type { GetOrganizationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { GetSessionRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { HasPermissionRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { InviteMemberRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## isUsernameAvailable

> IsUsernameAvailableResponseDto isUsernameAvailable(isUsernameAvailableDto)

Check Username Availability

Check if username is available for signup

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { IsUsernameAvailableRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // IsUsernameAvailableDto
    isUsernameAvailableDto: ...,
  } satisfies IsUsernameAvailableRequest;

  try {
    const data = await api.isUsernameAvailable(body);
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
| **isUsernameAvailableDto** | [IsUsernameAvailableDto](IsUsernameAvailableDto.md) |  | |

### Return type

[**IsUsernameAvailableResponseDto**](IsUsernameAvailableResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Username availability checked |  -  |
| **400** | Bad Request - Invalid input |  -  |
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
} from '@cashful/typescript';
import type { LeaveOrganizationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## linkSocial

> LinkSocialResponseDto linkSocial(linkSocialDto)

Link Social Account

Link a social account to existing user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { LinkSocialRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // LinkSocialDto
    linkSocialDto: ...,
  } satisfies LinkSocialRequest;

  try {
    const data = await api.linkSocial(body);
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
| **linkSocialDto** | [LinkSocialDto](LinkSocialDto.md) |  | |

### Return type

[**LinkSocialResponseDto**](LinkSocialResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Social account linked successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listAccounts

> ListAccountsResponseDto listAccounts()

List Linked Accounts

List all linked social accounts

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { ListAccountsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.listAccounts();
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

[**ListAccountsResponseDto**](ListAccountsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Linked accounts listed successfully |  -  |
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
} from '@cashful/typescript';
import type { ListApiKeysRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ListMembersRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ListOrganizationInvitationsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ListOrganizationsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ListUserInvitationsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { ListUserSessionsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## ok

> string ok()

Health Check

Check if the authentication API is working

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { OkRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  try {
    const data = await api.ok();
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

**string**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | API is working |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## refreshToken

> RefreshTokenResponseDto refreshToken(refreshTokenDto)

Refresh Token

Refresh authentication token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { RefreshTokenRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // RefreshTokenDto
    refreshTokenDto: ...,
  } satisfies RefreshTokenRequest;

  try {
    const data = await api.refreshToken(body);
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
| **refreshTokenDto** | [RefreshTokenDto](RefreshTokenDto.md) |  | |

### Return type

[**RefreshTokenResponseDto**](RefreshTokenResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Token refreshed successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
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
} from '@cashful/typescript';
import type { RejectInvitationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { RemoveMemberRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { RequestPasswordResetRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## requestPhonePasswordReset

> RequestPhonePasswordResetResponseDto requestPhonePasswordReset(requestPhonePasswordResetDto)

Request Password Reset via Phone

Request password reset via phone number

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { RequestPhonePasswordResetRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // RequestPhonePasswordResetDto
    requestPhonePasswordResetDto: ...,
  } satisfies RequestPhonePasswordResetRequest;

  try {
    const data = await api.requestPhonePasswordReset(body);
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
| **requestPhonePasswordResetDto** | [RequestPhonePasswordResetDto](RequestPhonePasswordResetDto.md) |  | |

### Return type

[**RequestPhonePasswordResetResponseDto**](RequestPhonePasswordResetResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Password reset requested successfully |  -  |
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
} from '@cashful/typescript';
import type { ResetPasswordRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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

> ResetPasswordCallbackResponseDto resetPasswordCallback(token, callbackURL)

Reset Password Callback

Redirects user to callback URL with token

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { ResetPasswordCallbackRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // string
    token: token_example,
    // string | The URL to redirect user to reset their password
    callbackURL: https://example.com/reset-password,
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
| **token** | `string` |  | [Defaults to `undefined`] |
| **callbackURL** | `string` | The URL to redirect user to reset their password | [Defaults to `undefined`] |

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


## resetPhonePassword

> ResetPhonePasswordResponseDto resetPhonePassword(resetPhonePasswordDto)

Reset Password with Phone

Reset password using phone verification

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { ResetPhonePasswordRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // ResetPhonePasswordDto
    resetPhonePasswordDto: ...,
  } satisfies ResetPhonePasswordRequest;

  try {
    const data = await api.resetPhonePassword(body);
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
| **resetPhonePasswordDto** | [ResetPhonePasswordDto](ResetPhonePasswordDto.md) |  | |

### Return type

[**ResetPhonePasswordResponseDto**](ResetPhonePasswordResponseDto.md)

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


## revokeOtherSessions

> RevokeSessionResponseDto revokeOtherSessions()

Revoke Other Sessions

Revoke all sessions except the current one

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { RevokeOtherSessionsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.revokeOtherSessions();
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

[**RevokeSessionResponseDto**](RevokeSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Other sessions revoked successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
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
} from '@cashful/typescript';
import type { RevokeSessionRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## revokeSessions

> RevokeSessionResponseDto revokeSessions()

Revoke All Sessions

Revoke all sessions for the current user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { RevokeSessionsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.revokeSessions();
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

[**RevokeSessionResponseDto**](RevokeSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | All sessions revoked successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendPhoneOTP

> SendPhoneOTPResponseDto sendPhoneOTP(sendPhoneOTPDto)

Send OTP to Phone

Send one-time password to phone number

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { SendPhoneOTPRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // SendPhoneOTPDto
    sendPhoneOTPDto: ...,
  } satisfies SendPhoneOTPRequest;

  try {
    const data = await api.sendPhoneOTP(body);
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
| **sendPhoneOTPDto** | [SendPhoneOTPDto](SendPhoneOTPDto.md) |  | |

### Return type

[**SendPhoneOTPResponseDto**](SendPhoneOTPResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OTP sent successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
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
} from '@cashful/typescript';
import type { SendVerificationEmailRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { SetActiveOrganizationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { SignInEmailRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## signInPhoneNumber

> SignInResponseDto signInPhoneNumber(signInPhoneNumberDto)

Sign in with Phone Number

Sign in using phone number and password

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { SignInPhoneNumberRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // SignInPhoneNumberDto
    signInPhoneNumberDto: ...,
  } satisfies SignInPhoneNumberRequest;

  try {
    const data = await api.signInPhoneNumber(body);
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
| **signInPhoneNumberDto** | [SignInPhoneNumberDto](SignInPhoneNumberDto.md) |  | |

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
| **200** | Signed in with phone number successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## signOut

> SignOutResponseDto signOut(body)

Sign out

Sign out the current user and invalidate the session

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { SignOutRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // object
    body: Object,
  } satisfies SignOutRequest;

  try {
    const data = await api.signOut(body);
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
| **body** | `object` |  | |

### Return type

[**SignOutResponseDto**](SignOutResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
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
} from '@cashful/typescript';
import type { SignUpEmailRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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


## socialSignIn

> SignInResponseDto socialSignIn(socialSignInDto)

Sign in with social provider

Sign in with a social provider (OAuth, etc.)

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { SocialSignInRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // SocialSignInDto
    socialSignInDto: ...,
  } satisfies SocialSignInRequest;

  try {
    const data = await api.socialSignIn(body);
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
| **socialSignInDto** | [SocialSignInDto](SocialSignInDto.md) |  | |

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
| **200** | Successfully signed in with social provider |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## unlinkAccount

> UnlinkAccountResponseDto unlinkAccount(unlinkAccountDto)

Unlink Social Account

Unlink a social account from user

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { UnlinkAccountRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // UnlinkAccountDto
    unlinkAccountDto: ...,
  } satisfies UnlinkAccountRequest;

  try {
    const data = await api.unlinkAccount(body);
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
| **unlinkAccountDto** | [UnlinkAccountDto](UnlinkAccountDto.md) |  | |

### Return type

[**UnlinkAccountResponseDto**](UnlinkAccountResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Social account unlinked successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
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
} from '@cashful/typescript';
import type { UpdateApiKeyRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { UpdateMemberRoleRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { UpdateOrganizationRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { UpdateUserRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { VerifyApiKeyRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
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
} from '@cashful/typescript';
import type { VerifyEmailRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // string | The token to verify email
    token: verify_token_12345,
    // string | The URL to redirect to after email verification (optional)
    callbackURL: https://example.com/callback,
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
| **token** | `string` | The token to verify email | [Defaults to `undefined`] |
| **callbackURL** | `string` | The URL to redirect to after email verification | [Optional] [Defaults to `undefined`] |

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


## verifyPhoneNumber

> VerifyPhoneNumberResponseDto verifyPhoneNumber(verifyPhoneNumberDto)

Verify Phone Number

Verify phone number with OTP code

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@cashful/typescript';
import type { VerifyPhoneNumberRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const api = new AuthenticationApi();

  const body = {
    // VerifyPhoneNumberDto
    verifyPhoneNumberDto: ...,
  } satisfies VerifyPhoneNumberRequest;

  try {
    const data = await api.verifyPhoneNumber(body);
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
| **verifyPhoneNumberDto** | [VerifyPhoneNumberDto](VerifyPhoneNumberDto.md) |  | |

### Return type

[**VerifyPhoneNumberResponseDto**](VerifyPhoneNumberResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number verified successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

