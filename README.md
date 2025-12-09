# @cashful-co/typescript-sdk@0.0.1

A TypeScript SDK client for the localhost API.

## Usage

First, install the SDK from npm.

```bash
npm install @cashful-co/typescript-sdk --save
```

Next, try it out.


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


## Documentation

### API Endpoints

All URIs are relative to *http://localhost:3000*

| Class | Method | HTTP request | Description
| ----- | ------ | ------------ | -------------
*AuthenticationApi* | [**acceptInvitation**](docs/AuthenticationApi.md#acceptinvitation) | **POST** /api/canary/authentication/organization/accept-invitation | Accept Invitation
*AuthenticationApi* | [**cancelInvitation**](docs/AuthenticationApi.md#cancelinvitation) | **POST** /api/canary/authentication/organization/cancel-invitation | Cancel Invitation
*AuthenticationApi* | [**createApiKey**](docs/AuthenticationApi.md#createapikey) | **POST** /api/canary/authentication/api-key/create | Create API Key
*AuthenticationApi* | [**createOrganization**](docs/AuthenticationApi.md#createorganization) | **POST** /api/canary/authentication/organization/create | Create Organization
*AuthenticationApi* | [**deleteApiKey**](docs/AuthenticationApi.md#deleteapikey) | **POST** /api/canary/authentication/api-key/delete | Delete API Key
*AuthenticationApi* | [**deleteOrganization**](docs/AuthenticationApi.md#deleteorganization) | **POST** /api/canary/authentication/organization/delete | Delete Organization
*AuthenticationApi* | [**forgetPassword**](docs/AuthenticationApi.md#forgetpassword) | **POST** /api/canary/authentication/forget-password | Forget Password
*AuthenticationApi* | [**getSession**](docs/AuthenticationApi.md#getsession) | **GET** /api/canary/authentication/get-session | Get Session
*AuthenticationApi* | [**inviteMember**](docs/AuthenticationApi.md#invitemember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member
*AuthenticationApi* | [**listApiKeys**](docs/AuthenticationApi.md#listapikeys) | **GET** /api/canary/authentication/api-key/list | List API Keys
*AuthenticationApi* | [**listOrganizations**](docs/AuthenticationApi.md#listorganizations) | **GET** /api/canary/authentication/organization/list | List Organizations
*AuthenticationApi* | [**rejectInvitation**](docs/AuthenticationApi.md#rejectinvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation
*AuthenticationApi* | [**removeMember**](docs/AuthenticationApi.md#removemember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member
*AuthenticationApi* | [**resetPassword**](docs/AuthenticationApi.md#resetpassword) | **POST** /api/canary/authentication/reset-password | Reset Password
*AuthenticationApi* | [**setActiveOrganization**](docs/AuthenticationApi.md#setactiveorganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization
*AuthenticationApi* | [**signInEmail**](docs/AuthenticationApi.md#signinemail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email
*AuthenticationApi* | [**signOut**](docs/AuthenticationApi.md#signout) | **POST** /api/canary/authentication/sign-out | Sign out
*AuthenticationApi* | [**signUpEmail**](docs/AuthenticationApi.md#signupemail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email
*AuthenticationApi* | [**updateApiKey**](docs/AuthenticationApi.md#updateapikey) | **POST** /api/canary/authentication/api-key/update | Update API Key
*AuthenticationApi* | [**updateMemberRole**](docs/AuthenticationApi.md#updatememberrole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role
*AuthenticationApi* | [**updateOrganization**](docs/AuthenticationApi.md#updateorganization) | **POST** /api/canary/authentication/organization/update | Update Organization
*AuthenticationApi* | [**verifyApiKey**](docs/AuthenticationApi.md#verifyapikey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key
*BalanceApi* | [**getBalanceHistory**](docs/BalanceApi.md#getbalancehistory) | **GET** /api/canary/balance/history | List Merchant Balance History
*BalanceApi* | [**getMerchantBalance**](docs/BalanceApi.md#getmerchantbalance) | **GET** /api/canary/balance | Get Merchant Balance
*CheckoutsApi* | [**createCheckoutSession**](docs/CheckoutsApi.md#createcheckoutsession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout
*CustomersApi* | [**createCustomer**](docs/CustomersApi.md#createcustomer) | **POST** /api/canary/customers | Create Customer
*CustomersApi* | [**getCustomerBalance**](docs/CustomersApi.md#getcustomerbalance) | **GET** /api/canary/customers/{id}/balance | Get Customer\&#39;s Cash Balance
*CustomersApi* | [**listCustomerPaymentMethods**](docs/CustomersApi.md#listcustomerpaymentmethods) | **GET** /api/canary/customers/{id}/payment-methods | List Customer\&#39;s Payment Methods
*CustomersApi* | [**listCustomerTransactions**](docs/CustomersApi.md#listcustomertransactions) | **GET** /api/canary/customers/{id}/transactions | List Customer\&#39;s Cash Transactions
*CustomersApi* | [**listCustomers**](docs/CustomersApi.md#listcustomers) | **GET** /api/canary/customers | List Customers
*CustomersApi* | [**retrieveCustomer**](docs/CustomersApi.md#retrievecustomer) | **GET** /api/canary/customers/{id} | Retrieve Customer
*CustomersApi* | [**updateCustomer**](docs/CustomersApi.md#updatecustomer) | **PATCH** /api/canary/customers/{id} | Update Customer
*EventsApi* | [**listEvents**](docs/EventsApi.md#listevents) | **GET** /api/canary/events | List Events
*HealthApi* | [**checkHealth**](docs/HealthApi.md#checkhealth) | **GET** /api/canary/health | Health check endpoint
*PaymentIntentsApi* | [**createPaymentIntent**](docs/PaymentIntentsApi.md#createpaymentintent) | **POST** /api/canary/payment-intents | Create Off-Session Charge
*PaymentIntentsApi* | [**retrievePaymentIntent**](docs/PaymentIntentsApi.md#retrievepaymentintent) | **GET** /api/canary/payment-intents/{id} | Retrieve Payment Intent
*PaymentLinksApi* | [**createPaymentLink**](docs/PaymentLinksApi.md#createpaymentlink) | **POST** /api/canary/payment-links | Create Payment Link
*PaymentLinksApi* | [**listPaymentLinks**](docs/PaymentLinksApi.md#listpaymentlinks) | **GET** /api/canary/payment-links | List Payment Links
*PaymentLinksApi* | [**updatePaymentLink**](docs/PaymentLinksApi.md#updatepaymentlink) | **PATCH** /api/canary/payment-links/{id} | Update Payment Link
*PaymentMethodsApi* | [**deletePaymentMethod**](docs/PaymentMethodsApi.md#deletepaymentmethod) | **DELETE** /api/canary/payment-methods/{id} | Delete Payment Method
*PaymentMethodsApi* | [**retrievePaymentMethod**](docs/PaymentMethodsApi.md#retrievepaymentmethod) | **GET** /api/canary/payment-methods/{id} | Retrieve Payment Method
*PayoutsApi* | [**createPayout**](docs/PayoutsApi.md#createpayout) | **POST** /api/canary/payouts | Create Payout
*PayoutsApi* | [**listPayouts**](docs/PayoutsApi.md#listpayouts) | **GET** /api/canary/payouts | List Payouts
*ProductsApi* | [**createProduct**](docs/ProductsApi.md#createproduct) | **POST** /api/canary/products | Create Product
*ProductsApi* | [**listProducts**](docs/ProductsApi.md#listproducts) | **GET** /api/canary/products | List Products
*ProductsApi* | [**updateProduct**](docs/ProductsApi.md#updateproduct) | **PATCH** /api/canary/products/{id} | Update Product
*PurchasesApi* | [**createPurchase**](docs/PurchasesApi.md#createpurchase) | **POST** /api/canary/purchases | Buy with Cash Balance
*TransfersApi* | [**createTransfer**](docs/TransfersApi.md#createtransfer) | **POST** /api/canary/transfers | Create P2P Transfer
*WebhooksApi* | [**createWebhookEndpoint**](docs/WebhooksApi.md#createwebhookendpoint) | **POST** /api/canary/webhook-endpoints | Create Webhook Endpoint
*WebhooksApi* | [**deleteWebhookEndpoint**](docs/WebhooksApi.md#deletewebhookendpoint) | **DELETE** /api/canary/webhook-endpoints/{id} | Delete Webhook Endpoint
*WebhooksApi* | [**listWebhookEndpoints**](docs/WebhooksApi.md#listwebhookendpoints) | **GET** /api/canary/webhook-endpoints | List Webhook Endpoints


### Models

- [AcceptInvitationDto](docs/AcceptInvitationDto.md)
- [BalanceHistoryResponseDto](docs/BalanceHistoryResponseDto.md)
- [BalanceTransactionDto](docs/BalanceTransactionDto.md)
- [BanUserDto](docs/BanUserDto.md)
- [BaseDto](docs/BaseDto.md)
- [CancelInvitationDto](docs/CancelInvitationDto.md)
- [CheckoutSessionResponseDto](docs/CheckoutSessionResponseDto.md)
- [CreateApiKeyDto](docs/CreateApiKeyDto.md)
- [CreateBalanceDto](docs/CreateBalanceDto.md)
- [CreateCheckoutSessionDto](docs/CreateCheckoutSessionDto.md)
- [CreateCustomerDto](docs/CreateCustomerDto.md)
- [CreateOrganizationDto](docs/CreateOrganizationDto.md)
- [CreatePaymentIntentDto](docs/CreatePaymentIntentDto.md)
- [CreatePaymentLinkDto](docs/CreatePaymentLinkDto.md)
- [CreatePaymentMethodDto](docs/CreatePaymentMethodDto.md)
- [CreatePayoutDto](docs/CreatePayoutDto.md)
- [CreateProductDto](docs/CreateProductDto.md)
- [CreatePurchaseDto](docs/CreatePurchaseDto.md)
- [CreateTransferDto](docs/CreateTransferDto.md)
- [CreateWebhookEndpointDto](docs/CreateWebhookEndpointDto.md)
- [CustomerResponseDto](docs/CustomerResponseDto.md)
- [CustomerTransactionDto](docs/CustomerTransactionDto.md)
- [DeleteApiKeyDto](docs/DeleteApiKeyDto.md)
- [DeleteOrganizationDto](docs/DeleteOrganizationDto.md)
- [ErrorResponseDto](docs/ErrorResponseDto.md)
- [EventResponseDto](docs/EventResponseDto.md)
- [ForgotPasswordDto](docs/ForgotPasswordDto.md)
- [GetSessionResponseDto](docs/GetSessionResponseDto.md)
- [ImpersonateUserDto](docs/ImpersonateUserDto.md)
- [InviteMemberDto](docs/InviteMemberDto.md)
- [LineItemDto](docs/LineItemDto.md)
- [ListCustomerTransactionsResponseDto](docs/ListCustomerTransactionsResponseDto.md)
- [ListCustomersResponseDto](docs/ListCustomersResponseDto.md)
- [ListEventsResponseDto](docs/ListEventsResponseDto.md)
- [ListPaymentLinksResponseDto](docs/ListPaymentLinksResponseDto.md)
- [ListPayoutsResponseDto](docs/ListPayoutsResponseDto.md)
- [ListProductsResponseDto](docs/ListProductsResponseDto.md)
- [ListWebhookEndpointsResponseDto](docs/ListWebhookEndpointsResponseDto.md)
- [MerchantBalanceResponseDto](docs/MerchantBalanceResponseDto.md)
- [PaginationResponseDto](docs/PaginationResponseDto.md)
- [PaymentIntentResponseDto](docs/PaymentIntentResponseDto.md)
- [PaymentLinkResponseDto](docs/PaymentLinkResponseDto.md)
- [PaymentMethodResponseDto](docs/PaymentMethodResponseDto.md)
- [PayoutResponseDto](docs/PayoutResponseDto.md)
- [ProductResponseDto](docs/ProductResponseDto.md)
- [PurchaseResponseDto](docs/PurchaseResponseDto.md)
- [RejectInvitationDto](docs/RejectInvitationDto.md)
- [RemoveMemberDto](docs/RemoveMemberDto.md)
- [ResetPasswordDto](docs/ResetPasswordDto.md)
- [SessionDto](docs/SessionDto.md)
- [SessionUserDto](docs/SessionUserDto.md)
- [SetActiveOrganizationDto](docs/SetActiveOrganizationDto.md)
- [SetRoleDto](docs/SetRoleDto.md)
- [SignInDto](docs/SignInDto.md)
- [SignUpDto](docs/SignUpDto.md)
- [TransferResponseDto](docs/TransferResponseDto.md)
- [UnbanUserDto](docs/UnbanUserDto.md)
- [UpdateApiKeyDto](docs/UpdateApiKeyDto.md)
- [UpdateCustomerDto](docs/UpdateCustomerDto.md)
- [UpdateMemberRoleDto](docs/UpdateMemberRoleDto.md)
- [UpdateOrganizationDto](docs/UpdateOrganizationDto.md)
- [UpdatePaymentLinkDto](docs/UpdatePaymentLinkDto.md)
- [UpdatePayoutDto](docs/UpdatePayoutDto.md)
- [UpdateProductDto](docs/UpdateProductDto.md)
- [UpdateWebhookEndpointDto](docs/UpdateWebhookEndpointDto.md)
- [VerifyApiKeyDto](docs/VerifyApiKeyDto.md)
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

- API version: `1.0.0`
- Package version: `0.0.1`
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
