# @cashful/typescript@0.8.0

A TypeScript SDK client for the api.cashful.africa API.

## Usage

First, install the SDK from npm.

```bash
npm install @cashful/typescript --save
```

Next, try it out.


```ts
import {
  Configuration,
  AnalyticsApi,
} from '@cashful/typescript';
import type { GetAnalyticsRequest } from '@cashful/typescript';

async function example() {
  console.log("🚀 Testing @cashful/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AnalyticsApi(config);

  const body = {
    // string | The unique identifier of the merchant. If not provided, defaults to the authenticated user\'s active organization. (optional)
    merchantId: merchant_123,
  } satisfies GetAnalyticsRequest;

  try {
    const data = await api.getAnalytics(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```


## Documentation

### API Endpoints

All URIs are relative to *https://api.cashful.africa*

| Class | Method | HTTP request | Description
| ----- | ------ | ------------ | -------------
*AnalyticsApi* | [**getAnalytics**](docs/AnalyticsApi.md#getanalytics) | **GET** /api/canary/analytics | Get Analytics
*AnalyticsApi* | [**getAnalyticsSummary**](docs/AnalyticsApi.md#getanalyticssummary) | **GET** /api/canary/analytics/summary | Get Analytics Summary
*AuthenticationApi* | [**acceptInvitation**](docs/AuthenticationApi.md#acceptinvitation) | **POST** /api/canary/authentication/organization/accept-invitation | Accept Invitation
*AuthenticationApi* | [**cancelInvitation**](docs/AuthenticationApi.md#cancelinvitation) | **POST** /api/canary/authentication/organization/cancel-invitation | Cancel Invitation
*AuthenticationApi* | [**changeEmail**](docs/AuthenticationApi.md#changeemail) | **POST** /api/canary/authentication/change-email | Change Email
*AuthenticationApi* | [**changePassword**](docs/AuthenticationApi.md#changepassword) | **POST** /api/canary/authentication/change-password | Change Password
*AuthenticationApi* | [**checkSlug**](docs/AuthenticationApi.md#checkslug) | **POST** /api/canary/authentication/organization/check-slug | Check Slug
*AuthenticationApi* | [**createApiKey**](docs/AuthenticationApi.md#createapikey) | **POST** /api/canary/authentication/api-key/create | Create API Key
*AuthenticationApi* | [**createOrganization**](docs/AuthenticationApi.md#createorganization) | **POST** /api/canary/authentication/organization/create | Create Organization
*AuthenticationApi* | [**deleteApiKey**](docs/AuthenticationApi.md#deleteapikey) | **POST** /api/canary/authentication/api-key/delete | Delete API Key
*AuthenticationApi* | [**deleteOrganization**](docs/AuthenticationApi.md#deleteorganization) | **POST** /api/canary/authentication/organization/delete | Delete Organization
*AuthenticationApi* | [**deleteUser**](docs/AuthenticationApi.md#deleteuser) | **POST** /api/canary/authentication/delete-user | Delete User
*AuthenticationApi* | [**forgetPassword**](docs/AuthenticationApi.md#forgetpassword) | **POST** /api/canary/authentication/forget-password | Forget Password
*AuthenticationApi* | [**getAccessToken**](docs/AuthenticationApi.md#getaccesstoken) | **POST** /api/canary/authentication/get-access-token | Get Access Token
*AuthenticationApi* | [**getActiveMember**](docs/AuthenticationApi.md#getactivemember) | **GET** /api/canary/authentication/organization/get-active-member | Get Active Member
*AuthenticationApi* | [**getActiveMemberRole**](docs/AuthenticationApi.md#getactivememberrole) | **GET** /api/canary/authentication/organization/get-active-member-role | Get Active Member Role
*AuthenticationApi* | [**getApiKey**](docs/AuthenticationApi.md#getapikey) | **GET** /api/canary/authentication/api-key/get | Get API Key
*AuthenticationApi* | [**getInvitation**](docs/AuthenticationApi.md#getinvitation) | **GET** /api/canary/authentication/organization/get-invitation | Get Invitation
*AuthenticationApi* | [**getJSONWebKeySet**](docs/AuthenticationApi.md#getjsonwebkeyset) | **GET** /api/canary/authentication/jwks | Get the JSON Web Key Set
*AuthenticationApi* | [**getJSONWebToken**](docs/AuthenticationApi.md#getjsonwebtoken) | **GET** /api/canary/authentication/token | Get a JWT token
*AuthenticationApi* | [**getOrganization**](docs/AuthenticationApi.md#getorganization) | **GET** /api/canary/authentication/organization/get-full-organization | Get Full Organization
*AuthenticationApi* | [**getSession**](docs/AuthenticationApi.md#getsession) | **GET** /api/canary/authentication/get-session | Get Session
*AuthenticationApi* | [**hasPermission**](docs/AuthenticationApi.md#haspermission) | **POST** /api/canary/authentication/organization/has-permission | Has Permission
*AuthenticationApi* | [**inviteMember**](docs/AuthenticationApi.md#invitemember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member
*AuthenticationApi* | [**isUsernameAvailable**](docs/AuthenticationApi.md#isusernameavailable) | **POST** /api/canary/authentication/is-username-available | Check Username Availability
*AuthenticationApi* | [**leaveOrganization**](docs/AuthenticationApi.md#leaveorganization) | **POST** /api/canary/authentication/organization/leave | Leave Organization
*AuthenticationApi* | [**linkSocial**](docs/AuthenticationApi.md#linksocial) | **POST** /api/canary/authentication/link-social | Link Social Account
*AuthenticationApi* | [**listAccounts**](docs/AuthenticationApi.md#listaccounts) | **GET** /api/canary/authentication/list-accounts | List Linked Accounts
*AuthenticationApi* | [**listApiKeys**](docs/AuthenticationApi.md#listapikeys) | **GET** /api/canary/authentication/api-key/list | List API Keys
*AuthenticationApi* | [**listMembers**](docs/AuthenticationApi.md#listmembers) | **GET** /api/canary/authentication/organization/list-members | List Members
*AuthenticationApi* | [**listOrganizationInvitations**](docs/AuthenticationApi.md#listorganizationinvitations) | **GET** /api/canary/authentication/organization/list-invitations | List Invitations
*AuthenticationApi* | [**listOrganizations**](docs/AuthenticationApi.md#listorganizations) | **GET** /api/canary/authentication/organization/list | List Organizations
*AuthenticationApi* | [**listUserInvitations**](docs/AuthenticationApi.md#listuserinvitations) | **GET** /api/canary/authentication/organization/list-user-invitations | List User Invitations
*AuthenticationApi* | [**listUserSessions**](docs/AuthenticationApi.md#listusersessions) | **GET** /api/canary/authentication/list-sessions | List User Sessions
*AuthenticationApi* | [**ok**](docs/AuthenticationApi.md#ok) | **GET** /api/canary/authentication/ok | Health Check
*AuthenticationApi* | [**refreshToken**](docs/AuthenticationApi.md#refreshtoken) | **POST** /api/canary/authentication/refresh-token | Refresh Token
*AuthenticationApi* | [**rejectInvitation**](docs/AuthenticationApi.md#rejectinvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation
*AuthenticationApi* | [**removeMember**](docs/AuthenticationApi.md#removemember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member
*AuthenticationApi* | [**requestPasswordReset**](docs/AuthenticationApi.md#requestpasswordreset) | **POST** /api/canary/authentication/request-password-reset | Request Password Reset
*AuthenticationApi* | [**requestPhonePasswordReset**](docs/AuthenticationApi.md#requestphonepasswordreset) | **POST** /api/canary/authentication/phone-number/request-password-reset | Request Password Reset via Phone
*AuthenticationApi* | [**resetPassword**](docs/AuthenticationApi.md#resetpassword) | **POST** /api/canary/authentication/reset-password | Reset Password
*AuthenticationApi* | [**resetPasswordCallback**](docs/AuthenticationApi.md#resetpasswordcallback) | **GET** /api/canary/authentication/reset-password/{token} | Reset Password Callback
*AuthenticationApi* | [**resetPhonePassword**](docs/AuthenticationApi.md#resetphonepassword) | **POST** /api/canary/authentication/phone-number/reset-password | Reset Password with Phone
*AuthenticationApi* | [**revokeOtherSessions**](docs/AuthenticationApi.md#revokeothersessions) | **POST** /api/canary/authentication/revoke-other-sessions | Revoke Other Sessions
*AuthenticationApi* | [**revokeSession**](docs/AuthenticationApi.md#revokesession) | **POST** /api/canary/authentication/revoke-session | Revoke Session
*AuthenticationApi* | [**revokeSessions**](docs/AuthenticationApi.md#revokesessions) | **POST** /api/canary/authentication/revoke-sessions | Revoke All Sessions
*AuthenticationApi* | [**sendPhoneOTP**](docs/AuthenticationApi.md#sendphoneotp) | **POST** /api/canary/authentication/phone-number/send-otp | Send OTP to Phone
*AuthenticationApi* | [**sendVerificationEmail**](docs/AuthenticationApi.md#sendverificationemail) | **POST** /api/canary/authentication/send-verification-email | Send Verification Email
*AuthenticationApi* | [**setActiveOrganization**](docs/AuthenticationApi.md#setactiveorganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization
*AuthenticationApi* | [**signInEmail**](docs/AuthenticationApi.md#signinemail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email
*AuthenticationApi* | [**signInPhoneNumber**](docs/AuthenticationApi.md#signinphonenumber) | **POST** /api/canary/authentication/sign-in/phone-number | Sign in with Phone Number
*AuthenticationApi* | [**signOut**](docs/AuthenticationApi.md#signout) | **POST** /api/canary/authentication/sign-out | Sign out
*AuthenticationApi* | [**signUpEmail**](docs/AuthenticationApi.md#signupemail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email
*AuthenticationApi* | [**socialSignIn**](docs/AuthenticationApi.md#socialsignin) | **POST** /api/canary/authentication/sign-in/social | Sign in with social provider
*AuthenticationApi* | [**unlinkAccount**](docs/AuthenticationApi.md#unlinkaccount) | **POST** /api/canary/authentication/unlink-account | Unlink Social Account
*AuthenticationApi* | [**updateApiKey**](docs/AuthenticationApi.md#updateapikey) | **POST** /api/canary/authentication/api-key/update | Update API Key
*AuthenticationApi* | [**updateMemberRole**](docs/AuthenticationApi.md#updatememberrole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role
*AuthenticationApi* | [**updateOrganization**](docs/AuthenticationApi.md#updateorganization) | **POST** /api/canary/authentication/organization/update | Update Organization
*AuthenticationApi* | [**updateUser**](docs/AuthenticationApi.md#updateuser) | **POST** /api/canary/authentication/update-user | Update User
*AuthenticationApi* | [**verifyApiKey**](docs/AuthenticationApi.md#verifyapikey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key
*AuthenticationApi* | [**verifyEmail**](docs/AuthenticationApi.md#verifyemail) | **GET** /api/canary/authentication/verify-email | Verify Email
*AuthenticationApi* | [**verifyPhoneNumber**](docs/AuthenticationApi.md#verifyphonenumber) | **POST** /api/canary/authentication/phone-number/verify | Verify Phone Number
*BalanceApi* | [**getBalanceHistory**](docs/BalanceApi.md#getbalancehistory) | **GET** /api/canary/balance/history | List Merchant Balance History
*BalanceApi* | [**getMerchantBalance**](docs/BalanceApi.md#getmerchantbalance) | **GET** /api/canary/balance | Get Merchant Balance
*CheckoutsApi* | [**createCheckoutSession**](docs/CheckoutsApi.md#createcheckoutsession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout
*CheckoutsApi* | [**listCheckoutSessions**](docs/CheckoutsApi.md#listcheckoutsessions) | **GET** /api/canary/checkout/sessions | List Checkout Sessions
*CheckoutsApi* | [**retrieveCheckoutSession**](docs/CheckoutsApi.md#retrievecheckoutsession) | **GET** /api/canary/checkout/sessions/{id} | Retrieve Checkout Session
*ComplianceApi* | [**createCompliance**](docs/ComplianceApi.md#createcompliance) | **POST** /api/canary/compliance | Create Compliance info
*ComplianceApi* | [**getCompliance**](docs/ComplianceApi.md#getcompliance) | **GET** /api/canary/compliance | Get Compliance info for organization
*ComplianceApi* | [**updateCompliance**](docs/ComplianceApi.md#updatecompliance) | **PATCH** /api/canary/compliance/{id} | Update Compliance info
*CustomersApi* | [**createCustomer**](docs/CustomersApi.md#createcustomer) | **POST** /api/canary/customers | Create Customer
*CustomersApi* | [**getCustomerBalance**](docs/CustomersApi.md#getcustomerbalance) | **GET** /api/canary/customers/{id}/balance | Get Customer\&#39;s Cash Balance
*CustomersApi* | [**listCustomerPaymentMethods**](docs/CustomersApi.md#listcustomerpaymentmethods) | **GET** /api/canary/customers/{id}/payment-methods | List Customer\&#39;s Payment Methods
*CustomersApi* | [**listCustomerTransactions**](docs/CustomersApi.md#listcustomertransactions) | **GET** /api/canary/customers/{id}/transactions | List Customer\&#39;s Cash Transactions
*CustomersApi* | [**listCustomers**](docs/CustomersApi.md#listcustomers) | **GET** /api/canary/customers | List Customers
*CustomersApi* | [**retrieveCustomer**](docs/CustomersApi.md#retrievecustomer) | **GET** /api/canary/customers/{id} | Retrieve Customer
*CustomersApi* | [**updateCustomer**](docs/CustomersApi.md#updatecustomer) | **PATCH** /api/canary/customers/{id} | Update Customer
*EventsApi* | [**listEvents**](docs/EventsApi.md#listevents) | **GET** /api/canary/events | List Events
*HealthApi* | [**checkHealth**](docs/HealthApi.md#checkhealth) | **GET** /api/canary/health | Health check endpoint
*NotificationsApi* | [**sendEmail**](docs/NotificationsApi.md#sendemail) | **POST** /api/canary/notifications/email | Send an email notification
*NotificationsApi* | [**sendMultiChannelNotification**](docs/NotificationsApi.md#sendmultichannelnotification) | **POST** /api/canary/notifications/multi-channel | Send notifications via multiple channels
*NotificationsApi* | [**sendNotification**](docs/NotificationsApi.md#sendnotification) | **POST** /api/canary/notifications/send | Send a notification via specified channel
*NotificationsApi* | [**sendSms**](docs/NotificationsApi.md#sendsms) | **POST** /api/canary/notifications/sms | Send an SMS notification
*PaymentIntentsApi* | [**cancelPaymentIntent**](docs/PaymentIntentsApi.md#cancelpaymentintent) | **POST** /api/canary/payment-intents/{id}/cancel | Cancel Payment Intent
*PaymentIntentsApi* | [**confirmPaymentIntent**](docs/PaymentIntentsApi.md#confirmpaymentintent) | **POST** /api/canary/payment-intents/{id}/confirm | Confirm Payment Intent
*PaymentIntentsApi* | [**createPaymentIntent**](docs/PaymentIntentsApi.md#createpaymentintent) | **POST** /api/canary/payment-intents | Create Payment Intent
*PaymentIntentsApi* | [**listPaymentIntents**](docs/PaymentIntentsApi.md#listpaymentintents) | **GET** /api/canary/payment-intents | List Payment Intents
*PaymentIntentsApi* | [**retrievePaymentIntent**](docs/PaymentIntentsApi.md#retrievepaymentintent) | **GET** /api/canary/payment-intents/{id} | Retrieve Payment Intent
*PaymentLinksApi* | [**createPaymentLink**](docs/PaymentLinksApi.md#createpaymentlink) | **POST** /api/canary/payment-links | Create Payment Link
*PaymentLinksApi* | [**listPaymentLinks**](docs/PaymentLinksApi.md#listpaymentlinks) | **GET** /api/canary/payment-links | List Payment Links
*PaymentLinksApi* | [**retrievePaymentLink**](docs/PaymentLinksApi.md#retrievepaymentlink) | **GET** /api/canary/payment-links/{id} | Retrieve Payment Link
*PaymentLinksApi* | [**updatePaymentLink**](docs/PaymentLinksApi.md#updatepaymentlink) | **PATCH** /api/canary/payment-links/{id} | Update Payment Link
*PaymentMethodsApi* | [**deletePaymentMethod**](docs/PaymentMethodsApi.md#deletepaymentmethod) | **DELETE** /api/canary/payment-methods/{id} | Delete Payment Method
*PaymentMethodsApi* | [**listPaymentMethods**](docs/PaymentMethodsApi.md#listpaymentmethods) | **GET** /api/canary/payment-methods | List Payment Methods
*PaymentMethodsApi* | [**retrievePaymentMethod**](docs/PaymentMethodsApi.md#retrievepaymentmethod) | **GET** /api/canary/payment-methods/{id} | Retrieve Payment Method
*PayoutsApi* | [**createPayout**](docs/PayoutsApi.md#createpayout) | **POST** /api/canary/payouts | Create Payout
*PayoutsApi* | [**listPayouts**](docs/PayoutsApi.md#listpayouts) | **GET** /api/canary/payouts | List Payouts
*ProductsApi* | [**createProduct**](docs/ProductsApi.md#createproduct) | **POST** /api/canary/products | Create Product
*ProductsApi* | [**listProducts**](docs/ProductsApi.md#listproducts) | **GET** /api/canary/products | List Products
*ProductsApi* | [**retrieveMultipleProducts**](docs/ProductsApi.md#retrievemultipleproducts) | **POST** /api/canary/products/multiple | Retrieve Multiple Products by ID
*ProductsApi* | [**retrieveProduct**](docs/ProductsApi.md#retrieveproduct) | **GET** /api/canary/products/{id} | Retrieve Product
*ProductsApi* | [**updateProduct**](docs/ProductsApi.md#updateproduct) | **PATCH** /api/canary/products/{id} | Update Product
*PurchasesApi* | [**createPurchase**](docs/PurchasesApi.md#createpurchase) | **POST** /api/canary/purchases | Buy with Cash Balance
*StorageApi* | [**confirmUpload**](docs/StorageApi.md#confirmupload) | **POST** /api/canary/storage/confirm-upload | Confirm that a file upload was completed
*StorageApi* | [**deleteFile**](docs/StorageApi.md#deletefile) | **DELETE** /api/canary/storage/{id} | Delete a file
*StorageApi* | [**getDownloadUrl**](docs/StorageApi.md#getdownloadurl) | **GET** /api/canary/storage/{id}/download-url | Get a presigned download URL for a file
*StorageApi* | [**getFileDetails**](docs/StorageApi.md#getfiledetails) | **GET** /api/canary/storage/{id} | Get file details
*StorageApi* | [**listFiles**](docs/StorageApi.md#listfiles) | **GET** /api/canary/storage | List files
*StorageApi* | [**requestUploadUrl**](docs/StorageApi.md#requestuploadurl) | **POST** /api/canary/storage/upload-url | Request a presigned URL for file upload
*TransfersApi* | [**createTransfer**](docs/TransfersApi.md#createtransfer) | **POST** /api/canary/transfers | Create P2P Transfer
*TransfersApi* | [**listTransfers**](docs/TransfersApi.md#listtransfers) | **GET** /api/canary/transfers | List Transfers
*WebhooksApi* | [**createWebhookEndpoint**](docs/WebhooksApi.md#createwebhookendpoint) | **POST** /api/canary/webhook-endpoints | Create Webhook Endpoint
*WebhooksApi* | [**deleteWebhookEndpoint**](docs/WebhooksApi.md#deletewebhookendpoint) | **DELETE** /api/canary/webhook-endpoints/{id} | Delete Webhook Endpoint
*WebhooksApi* | [**listWebhookEndpoints**](docs/WebhooksApi.md#listwebhookendpoints) | **GET** /api/canary/webhook-endpoints | List Webhook Endpoints


### Models

- [AcceptInvitationDto](docs/AcceptInvitationDto.md)
- [AcceptInvitationResponseDto](docs/AcceptInvitationResponseDto.md)
- [AdminCreateUserDto](docs/AdminCreateUserDto.md)
- [AdminCreateUserResponseDto](docs/AdminCreateUserResponseDto.md)
- [AdminGetUserDto](docs/AdminGetUserDto.md)
- [AdminGetUserResponseDto](docs/AdminGetUserResponseDto.md)
- [AdminListUserSessionsDto](docs/AdminListUserSessionsDto.md)
- [AdminListUserSessionsResponseDto](docs/AdminListUserSessionsResponseDto.md)
- [AdminRemoveUserDto](docs/AdminRemoveUserDto.md)
- [AdminRemoveUserResponseDto](docs/AdminRemoveUserResponseDto.md)
- [AdminRevokeUserSessionDto](docs/AdminRevokeUserSessionDto.md)
- [AdminRevokeUserSessionResponseDto](docs/AdminRevokeUserSessionResponseDto.md)
- [AdminRevokeUserSessionsDto](docs/AdminRevokeUserSessionsDto.md)
- [AdminRevokeUserSessionsResponseDto](docs/AdminRevokeUserSessionsResponseDto.md)
- [AdminSetUserPasswordDto](docs/AdminSetUserPasswordDto.md)
- [AdminSetUserPasswordResponseDto](docs/AdminSetUserPasswordResponseDto.md)
- [AdminUpdateUserDto](docs/AdminUpdateUserDto.md)
- [AdminUpdateUserResponseDto](docs/AdminUpdateUserResponseDto.md)
- [AnalyticsResponseDto](docs/AnalyticsResponseDto.md)
- [AnalyticsSummaryDto](docs/AnalyticsSummaryDto.md)
- [ApiKey](docs/ApiKey.md)
- [BadRequestResponseDto](docs/BadRequestResponseDto.md)
- [BalanceHistoryResponseDto](docs/BalanceHistoryResponseDto.md)
- [BalanceTransactionDto](docs/BalanceTransactionDto.md)
- [BanUserDto](docs/BanUserDto.md)
- [BanUserResponseDto](docs/BanUserResponseDto.md)
- [BaseDto](docs/BaseDto.md)
- [CancelInvitationDto](docs/CancelInvitationDto.md)
- [CancelInvitationResponseDto](docs/CancelInvitationResponseDto.md)
- [ChangeEmailDto](docs/ChangeEmailDto.md)
- [ChangeEmailResponseDto](docs/ChangeEmailResponseDto.md)
- [ChangePasswordDto](docs/ChangePasswordDto.md)
- [ChangePasswordResponseDto](docs/ChangePasswordResponseDto.md)
- [CheckSlugDto](docs/CheckSlugDto.md)
- [CheckSlugResponseDto](docs/CheckSlugResponseDto.md)
- [CheckoutSessionResponseDto](docs/CheckoutSessionResponseDto.md)
- [ConfirmUploadDto](docs/ConfirmUploadDto.md)
- [CreateApiKeyDto](docs/CreateApiKeyDto.md)
- [CreateApiKeyResponseDto](docs/CreateApiKeyResponseDto.md)
- [CreateBalanceDto](docs/CreateBalanceDto.md)
- [CreateCheckoutSessionDto](docs/CreateCheckoutSessionDto.md)
- [CreateCustomerDto](docs/CreateCustomerDto.md)
- [CreateOrganizationComplianceDto](docs/CreateOrganizationComplianceDto.md)
- [CreateOrganizationDto](docs/CreateOrganizationDto.md)
- [CreateOrganizationResponseDto](docs/CreateOrganizationResponseDto.md)
- [CreatePaymentIntentDto](docs/CreatePaymentIntentDto.md)
- [CreatePaymentLinkDto](docs/CreatePaymentLinkDto.md)
- [CreatePaymentMethodDto](docs/CreatePaymentMethodDto.md)
- [CreatePayoutDto](docs/CreatePayoutDto.md)
- [CreateProductDto](docs/CreateProductDto.md)
- [CreatePurchaseDto](docs/CreatePurchaseDto.md)
- [CreateTransferDto](docs/CreateTransferDto.md)
- [CreateWebhookEndpointDto](docs/CreateWebhookEndpointDto.md)
- [CustomerBalanceDto](docs/CustomerBalanceDto.md)
- [CustomerPaymentMethodDto](docs/CustomerPaymentMethodDto.md)
- [CustomerResponseDto](docs/CustomerResponseDto.md)
- [CustomerStatsDto](docs/CustomerStatsDto.md)
- [CustomerTransactionDto](docs/CustomerTransactionDto.md)
- [DailyBreakdownDto](docs/DailyBreakdownDto.md)
- [DebitReturnResponseDto](docs/DebitReturnResponseDto.md)
- [DeleteApiKeyDto](docs/DeleteApiKeyDto.md)
- [DeleteApiKeyResponseDto](docs/DeleteApiKeyResponseDto.md)
- [DeleteOrganizationDto](docs/DeleteOrganizationDto.md)
- [DeleteOrganizationResponseDto](docs/DeleteOrganizationResponseDto.md)
- [DeleteUserDto](docs/DeleteUserDto.md)
- [DeleteUserResponseDto](docs/DeleteUserResponseDto.md)
- [EventResponseDto](docs/EventResponseDto.md)
- [EvervaultEncryptedCardDto](docs/EvervaultEncryptedCardDto.md)
- [FileDto](docs/FileDto.md)
- [ForbiddenResponseDto](docs/ForbiddenResponseDto.md)
- [ForgotPasswordDto](docs/ForgotPasswordDto.md)
- [ForgotPasswordResponseDto](docs/ForgotPasswordResponseDto.md)
- [GetAccessTokenDto](docs/GetAccessTokenDto.md)
- [GetAccessTokenResponseDto](docs/GetAccessTokenResponseDto.md)
- [GetActiveMemberResponseDto](docs/GetActiveMemberResponseDto.md)
- [GetActiveMemberRoleResponseDto](docs/GetActiveMemberRoleResponseDto.md)
- [GetApiKeyResponseDto](docs/GetApiKeyResponseDto.md)
- [GetFullOrganizationResponseDto](docs/GetFullOrganizationResponseDto.md)
- [GetInvitationResponseDto](docs/GetInvitationResponseDto.md)
- [GetJsonWebKeySetResponseDto](docs/GetJsonWebKeySetResponseDto.md)
- [GetJsonWebTokenResponseDto](docs/GetJsonWebTokenResponseDto.md)
- [GetSessionResponseDto](docs/GetSessionResponseDto.md)
- [HasPermissionDto](docs/HasPermissionDto.md)
- [HasPermissionResponseDto](docs/HasPermissionResponseDto.md)
- [HostedCheckoutConfigDto](docs/HostedCheckoutConfigDto.md)
- [IVeriHealthCheckResponseDto](docs/IVeriHealthCheckResponseDto.md)
- [ImpersonateUserDto](docs/ImpersonateUserDto.md)
- [ImpersonateUserResponseDto](docs/ImpersonateUserResponseDto.md)
- [InitiatePaymentDto](docs/InitiatePaymentDto.md)
- [InitiatePaymentResponseDto](docs/InitiatePaymentResponseDto.md)
- [InternalServerErrorResponseDto](docs/InternalServerErrorResponseDto.md)
- [InvitationDto](docs/InvitationDto.md)
- [InviteMemberDto](docs/InviteMemberDto.md)
- [InviteMemberResponseDto](docs/InviteMemberResponseDto.md)
- [IsUsernameAvailableDto](docs/IsUsernameAvailableDto.md)
- [IsUsernameAvailableResponseDto](docs/IsUsernameAvailableResponseDto.md)
- [IveriParamsDto](docs/IveriParamsDto.md)
- [JwkDto](docs/JwkDto.md)
- [LeaveOrganizationDto](docs/LeaveOrganizationDto.md)
- [LeaveOrganizationResponseDto](docs/LeaveOrganizationResponseDto.md)
- [LineItemDto](docs/LineItemDto.md)
- [LinkSocialDto](docs/LinkSocialDto.md)
- [LinkSocialResponseDto](docs/LinkSocialResponseDto.md)
- [ListAccountsResponseDto](docs/ListAccountsResponseDto.md)
- [ListApiKeysResponseDto](docs/ListApiKeysResponseDto.md)
- [ListCheckoutSessionsResponseDto](docs/ListCheckoutSessionsResponseDto.md)
- [ListCustomerPaymentMethodsResponseDto](docs/ListCustomerPaymentMethodsResponseDto.md)
- [ListCustomerTransactionsResponseDto](docs/ListCustomerTransactionsResponseDto.md)
- [ListCustomersResponseDto](docs/ListCustomersResponseDto.md)
- [ListEventsResponseDto](docs/ListEventsResponseDto.md)
- [ListFilesResponseDto](docs/ListFilesResponseDto.md)
- [ListInvitationsResponseDto](docs/ListInvitationsResponseDto.md)
- [ListMembersResponseDto](docs/ListMembersResponseDto.md)
- [ListOrganizationComplianceResponseDto](docs/ListOrganizationComplianceResponseDto.md)
- [ListPaymentIntentsResponseDto](docs/ListPaymentIntentsResponseDto.md)
- [ListPaymentLinksResponseDto](docs/ListPaymentLinksResponseDto.md)
- [ListPaymentMethodsResponseDto](docs/ListPaymentMethodsResponseDto.md)
- [ListPayoutsResponseDto](docs/ListPayoutsResponseDto.md)
- [ListProductsResponseDto](docs/ListProductsResponseDto.md)
- [ListSessionsResponseDto](docs/ListSessionsResponseDto.md)
- [ListTransfersResponseDto](docs/ListTransfersResponseDto.md)
- [ListUserInvitationsResponseDto](docs/ListUserInvitationsResponseDto.md)
- [ListUsersResponseDto](docs/ListUsersResponseDto.md)
- [ListWebhookEndpointsResponseDto](docs/ListWebhookEndpointsResponseDto.md)
- [MemberDto](docs/MemberDto.md)
- [MerchantBalanceResponseDto](docs/MerchantBalanceResponseDto.md)
- [MetricStatsDto](docs/MetricStatsDto.md)
- [NotFoundResponseDto](docs/NotFoundResponseDto.md)
- [NotificationDto](docs/NotificationDto.md)
- [OrganizationComplianceResponseDto](docs/OrganizationComplianceResponseDto.md)
- [OrganizationDto](docs/OrganizationDto.md)
- [PaginationResponseDto](docs/PaginationResponseDto.md)
- [PaymentIntentResponseDto](docs/PaymentIntentResponseDto.md)
- [PaymentLinkResponseDto](docs/PaymentLinkResponseDto.md)
- [PaymentMethodResponseDto](docs/PaymentMethodResponseDto.md)
- [PayoutResponseDto](docs/PayoutResponseDto.md)
- [PresignedDownloadResponseDto](docs/PresignedDownloadResponseDto.md)
- [PresignedUploadResponseDto](docs/PresignedUploadResponseDto.md)
- [ProductResponseDto](docs/ProductResponseDto.md)
- [PurchaseResponseDto](docs/PurchaseResponseDto.md)
- [RefreshTokenDto](docs/RefreshTokenDto.md)
- [RefreshTokenResponseDto](docs/RefreshTokenResponseDto.md)
- [RejectInvitationDto](docs/RejectInvitationDto.md)
- [RejectInvitationResponseDto](docs/RejectInvitationResponseDto.md)
- [RemoveMemberDto](docs/RemoveMemberDto.md)
- [RemoveMemberResponseDto](docs/RemoveMemberResponseDto.md)
- [RequestPasswordResetDto](docs/RequestPasswordResetDto.md)
- [RequestPasswordResetResponseDto](docs/RequestPasswordResetResponseDto.md)
- [RequestPhonePasswordResetDto](docs/RequestPhonePasswordResetDto.md)
- [RequestPhonePasswordResetResponseDto](docs/RequestPhonePasswordResetResponseDto.md)
- [RequestUploadUrlDto](docs/RequestUploadUrlDto.md)
- [ResetPasswordCallbackResponseDto](docs/ResetPasswordCallbackResponseDto.md)
- [ResetPasswordDto](docs/ResetPasswordDto.md)
- [ResetPasswordResponseDto](docs/ResetPasswordResponseDto.md)
- [ResetPhonePasswordDto](docs/ResetPhonePasswordDto.md)
- [ResetPhonePasswordResponseDto](docs/ResetPhonePasswordResponseDto.md)
- [RetrieveMultipleProductsDto](docs/RetrieveMultipleProductsDto.md)
- [RevokeSessionDto](docs/RevokeSessionDto.md)
- [RevokeSessionResponseDto](docs/RevokeSessionResponseDto.md)
- [SendEmail200Response](docs/SendEmail200Response.md)
- [SendEmailDto](docs/SendEmailDto.md)
- [SendMultiChannelNotification200Response](docs/SendMultiChannelNotification200Response.md)
- [SendPhoneOTPDto](docs/SendPhoneOTPDto.md)
- [SendPhoneOTPResponseDto](docs/SendPhoneOTPResponseDto.md)
- [SendSms200Response](docs/SendSms200Response.md)
- [SendSmsDto](docs/SendSmsDto.md)
- [SendVerificationEmailDto](docs/SendVerificationEmailDto.md)
- [SendVerificationEmailResponseDto](docs/SendVerificationEmailResponseDto.md)
- [SessionDto](docs/SessionDto.md)
- [SessionUserDto](docs/SessionUserDto.md)
- [SetActiveOrganizationDto](docs/SetActiveOrganizationDto.md)
- [SetActiveOrganizationResponseDto](docs/SetActiveOrganizationResponseDto.md)
- [SetRoleDto](docs/SetRoleDto.md)
- [SetRoleResponseDto](docs/SetRoleResponseDto.md)
- [SignInDto](docs/SignInDto.md)
- [SignInPhoneNumberDto](docs/SignInPhoneNumberDto.md)
- [SignInResponseDto](docs/SignInResponseDto.md)
- [SignOutResponseDto](docs/SignOutResponseDto.md)
- [SignUpDto](docs/SignUpDto.md)
- [SignUpResponseDto](docs/SignUpResponseDto.md)
- [SocialSignInDto](docs/SocialSignInDto.md)
- [StopImpersonatingResponseDto](docs/StopImpersonatingResponseDto.md)
- [TimeframeMetricsDto](docs/TimeframeMetricsDto.md)
- [TransferResponseDto](docs/TransferResponseDto.md)
- [UnauthorizedResponseDto](docs/UnauthorizedResponseDto.md)
- [UnbanUserDto](docs/UnbanUserDto.md)
- [UnbanUserResponseDto](docs/UnbanUserResponseDto.md)
- [UnlinkAccountDto](docs/UnlinkAccountDto.md)
- [UnlinkAccountResponseDto](docs/UnlinkAccountResponseDto.md)
- [UpdateApiKeyDto](docs/UpdateApiKeyDto.md)
- [UpdateApiKeyResponseDto](docs/UpdateApiKeyResponseDto.md)
- [UpdateBalanceDto](docs/UpdateBalanceDto.md)
- [UpdateCheckoutSessionDto](docs/UpdateCheckoutSessionDto.md)
- [UpdateCheckoutSessionResponseDto](docs/UpdateCheckoutSessionResponseDto.md)
- [UpdateCustomerDto](docs/UpdateCustomerDto.md)
- [UpdateMemberRoleDto](docs/UpdateMemberRoleDto.md)
- [UpdateMemberRoleResponseDto](docs/UpdateMemberRoleResponseDto.md)
- [UpdateOrganizationComplianceDto](docs/UpdateOrganizationComplianceDto.md)
- [UpdateOrganizationDto](docs/UpdateOrganizationDto.md)
- [UpdateOrganizationResponseDto](docs/UpdateOrganizationResponseDto.md)
- [UpdatePaymentLinkDto](docs/UpdatePaymentLinkDto.md)
- [UpdatePayoutDto](docs/UpdatePayoutDto.md)
- [UpdateProductDto](docs/UpdateProductDto.md)
- [UpdateUserDto](docs/UpdateUserDto.md)
- [UpdateUserResponseDto](docs/UpdateUserResponseDto.md)
- [UpdateWebhookEndpointDto](docs/UpdateWebhookEndpointDto.md)
- [VerifyApiKeyDto](docs/VerifyApiKeyDto.md)
- [VerifyApiKeyResponseDto](docs/VerifyApiKeyResponseDto.md)
- [VerifyEmailResponseDto](docs/VerifyEmailResponseDto.md)
- [VerifyPhoneNumberDto](docs/VerifyPhoneNumberDto.md)
- [VerifyPhoneNumberResponseDto](docs/VerifyPhoneNumberResponseDto.md)
- [WebhookEndpointResponseDto](docs/WebhookEndpointResponseDto.md)

### Authorization


Authentication schemes defined for the API:
<a id="bearer"></a>
#### bearer


- **Type**: HTTP Bearer Token authentication (JWT)

## About

This TypeScript SDK client supports the [Fetch API](https://fetch.spec.whatwg.org/)
and is automatically generated by the
[OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `0.8.0`
- Package version: `0.8.0`
- Generator version: `7.17.0`
- Build package: `org.openapitools.codegen.languages.TypeScriptFetchClientCodegen`

The generated npm module supports the following:

- Environments
  * Node.js
  * Webpack
  * Browserify
- Language levels
  * ES5 - you must have a Promises/A+ library installed
  * ES6
- Module systems
  * CommonJS
  * ES6 module system

For more information, please visit [https://cashful.africa](https://cashful.africa)

## Development

### Building

To build the TypeScript source code, you need to have Node.js and npm installed.
After cloning the repository, navigate to the project directory and run:

```bash
npm install
npm run build
```

### Publishing

Once you've built the package, you can publish it to npm:

```bash
npm publish
```

## License

[]()
