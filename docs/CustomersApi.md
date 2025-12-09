# CustomersApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCustomer**](CustomersApi.md#createcustomer) | **POST** /api/canary/customers | Create Customer |
| [**getCustomerBalance**](CustomersApi.md#getcustomerbalance) | **GET** /api/canary/customers/{id}/balance | Get Customer\&#39;s Cash Balance |
| [**listCustomerPaymentMethods**](CustomersApi.md#listcustomerpaymentmethods) | **GET** /api/canary/customers/{id}/payment-methods | List Customer\&#39;s Payment Methods |
| [**listCustomerTransactions**](CustomersApi.md#listcustomertransactions) | **GET** /api/canary/customers/{id}/transactions | List Customer\&#39;s Cash Transactions |
| [**listCustomers**](CustomersApi.md#listcustomers) | **GET** /api/canary/customers | List Customers |
| [**retrieveCustomer**](CustomersApi.md#retrievecustomer) | **GET** /api/canary/customers/{id} | Retrieve Customer |
| [**updateCustomer**](CustomersApi.md#updatecustomer) | **PATCH** /api/canary/customers/{id} | Update Customer |



## createCustomer

> CustomerResponseDto createCustomer(createCustomerDto)

Create Customer

Creates a new customer object. This also provisions their \&quot;cash balance\&quot; feature (starting at 0).

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { CreateCustomerRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // CreateCustomerDto | Customer details
    createCustomerDto: ...,
  } satisfies CreateCustomerRequest;

  try {
    const data = await api.createCustomer(body);
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
| **createCustomerDto** | [CreateCustomerDto](CreateCustomerDto.md) | Customer details | |

### Return type

[**CustomerResponseDto**](CustomerResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Customer created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **409** | Customer with this email already exists |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCustomerBalance

> any getCustomerBalance(id)

Get Customer\&#39;s Cash Balance

Retrieves the real-time balance for a single customer\&#39;s \&quot;cash balance\&quot; (the \&quot;wallet-enabling\&quot; feature).

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { GetCustomerBalanceRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // string | The unique identifier of the customer
    id: id_example,
  } satisfies GetCustomerBalanceRequest;

  try {
    const data = await api.getCustomerBalance(body);
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
| **id** | `string` | The unique identifier of the customer | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved customer\&#39;s cash balance |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listCustomerPaymentMethods

> any listCustomerPaymentMethods(id)

List Customer\&#39;s Payment Methods

Shows all saved payment methods (cards, etc.) for a single customer.

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { ListCustomerPaymentMethodsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // string | The unique identifier of the customer
    id: id_example,
  } satisfies ListCustomerPaymentMethodsRequest;

  try {
    const data = await api.listCustomerPaymentMethods(body);
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
| **id** | `string` | The unique identifier of the customer | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved customer\&#39;s payment methods |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listCustomerTransactions

> ListCustomerTransactionsResponseDto listCustomerTransactions(id)

List Customer\&#39;s Cash Transactions

Provides the full transaction history for a single customer\&#39;s \&quot;cash balance\&quot; (Pay-Ins, Purchases, Transfers).

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { ListCustomerTransactionsRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // string | The unique identifier of the customer
    id: id_example,
  } satisfies ListCustomerTransactionsRequest;

  try {
    const data = await api.listCustomerTransactions(body);
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
| **id** | `string` | The unique identifier of the customer | [Defaults to `undefined`] |

### Return type

[**ListCustomerTransactionsResponseDto**](ListCustomerTransactionsResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved customer transactions |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listCustomers

> ListCustomersResponseDto listCustomers(merchantId, search, email, limit, offset)

List Customers

Retrieves a paginated list of all customers for the merchant.

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { ListCustomersRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // any | Search across customer fields (optional)
    search: ...,
    // any | Filter by email address (optional)
    email: ...,
    // number | Maximum number of records to return (optional)
    limit: 8.14,
    // number | Number of records to skip (optional)
    offset: 8.14,
  } satisfies ListCustomersRequest;

  try {
    const data = await api.listCustomers(body);
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
| **search** | `any` | Search across customer fields | [Optional] [Defaults to `undefined`] |
| **email** | `any` | Filter by email address | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |

### Return type

[**ListCustomersResponseDto**](ListCustomersResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved customers list |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrieveCustomer

> any retrieveCustomer(id)

Retrieve Customer

Gets the details for a single customer.

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { RetrieveCustomerRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // string | The unique identifier of the customer
    id: id_example,
  } satisfies RetrieveCustomerRequest;

  try {
    const data = await api.retrieveCustomer(body);
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
| **id** | `string` | The unique identifier of the customer | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved customer details |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateCustomer

> any updateCustomer(id, updateCustomerDto)

Update Customer

Updates a customer\&#39;s details (e.g., email, metadata).

### Example

```ts
import {
  Configuration,
  CustomersApi,
} from '@cashful-co/typescript';
import type { UpdateCustomerRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CustomersApi(config);

  const body = {
    // string | The unique identifier of the customer
    id: id_example,
    // UpdateCustomerDto | Customer update details
    updateCustomerDto: ...,
  } satisfies UpdateCustomerRequest;

  try {
    const data = await api.updateCustomer(body);
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
| **id** | `string` | The unique identifier of the customer | [Defaults to `undefined`] |
| **updateCustomerDto** | [UpdateCustomerDto](UpdateCustomerDto.md) | Customer update details | |

### Return type

**any**

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Customer updated successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **409** | Email already in use by another customer |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

