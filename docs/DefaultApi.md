# DefaultApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**clientsClientIdDelete**](DefaultApi.md#clientsClientIdDelete) | **DELETE** /clients/{clientId} | Delete a client by ID |
| [**clientsClientIdGet**](DefaultApi.md#clientsClientIdGet) | **GET** /clients/{clientId} | Get a client by ID |
| [**clientsClientIdPut**](DefaultApi.md#clientsClientIdPut) | **PUT** /clients/{clientId} | Update a client by ID |
| [**clientsGet**](DefaultApi.md#clientsGet) | **GET** /clients | Get all clients |
| [**clientsPost**](DefaultApi.md#clientsPost) | **POST** /clients | Create new client |
| [**contractsContractIdDelete**](DefaultApi.md#contractsContractIdDelete) | **DELETE** /contracts/{contractId} | Delete a contract by ID |
| [**contractsContractIdGet**](DefaultApi.md#contractsContractIdGet) | **GET** /contracts/{contractId} | Get a contract by ID |
| [**contractsContractIdPut**](DefaultApi.md#contractsContractIdPut) | **PUT** /contracts/{contractId} | Update a contract by ID |
| [**contractsGet**](DefaultApi.md#contractsGet) | **GET** /contracts | Get all contracts |
| [**contractsPost**](DefaultApi.md#contractsPost) | **POST** /contracts | Create new contract |
| [**employeesEmployeeIdDelete**](DefaultApi.md#employeesEmployeeIdDelete) | **DELETE** /employees/{employeeId} | Delete an employee by ID |
| [**employeesEmployeeIdGet**](DefaultApi.md#employeesEmployeeIdGet) | **GET** /employees/{employeeId} | Get an employee by ID |
| [**employeesEmployeeIdPut**](DefaultApi.md#employeesEmployeeIdPut) | **PUT** /employees/{employeeId} | Update an employee by ID |
| [**employeesGet**](DefaultApi.md#employeesGet) | **GET** /employees | Get all employees |
| [**employeesPost**](DefaultApi.md#employeesPost) | **POST** /employees | Create new employee |
| [**historyGet**](DefaultApi.md#historyGet) | **GET** /history | Get all history |
| [**historyHistoryIdDelete**](DefaultApi.md#historyHistoryIdDelete) | **DELETE** /history/{historyId} | Delete an employee contract assignment by ID |
| [**historyHistoryIdGet**](DefaultApi.md#historyHistoryIdGet) | **GET** /history/{historyId} | Get an employee contract asignment by ID |
| [**historyHistoryIdPut**](DefaultApi.md#historyHistoryIdPut) | **PUT** /history/{historyId} | Update an employee contract assignment by ID |
| [**historyPost**](DefaultApi.md#historyPost) | **POST** /history | Create new employee contract assignment |


<a name="clientsClientIdDelete"></a>
# **clientsClientIdDelete**
> clientsClientIdDelete(clientId)

Delete a client by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer clientId = 56; // Integer | Numeric ID of the client
    try {
      apiInstance.clientsClientIdDelete(clientId);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#clientsClientIdDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **clientId** | **Integer**| Numeric ID of the client | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="clientsClientIdGet"></a>
# **clientsClientIdGet**
> Client clientsClientIdGet(clientId)

Get a client by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer clientId = 56; // Integer | Numeric ID of the client
    try {
      Client result = apiInstance.clientsClientIdGet(clientId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#clientsClientIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **clientId** | **Integer**| Numeric ID of the client | |

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="clientsClientIdPut"></a>
# **clientsClientIdPut**
> Client clientsClientIdPut(clientId, clientsPostRequest)

Update a client by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer clientId = 56; // Integer | Numeric ID of the client
    ClientsPostRequest clientsPostRequest = new ClientsPostRequest(); // ClientsPostRequest | 
    try {
      Client result = apiInstance.clientsClientIdPut(clientId, clientsPostRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#clientsClientIdPut");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **clientId** | **Integer**| Numeric ID of the client | |
| **clientsPostRequest** | [**ClientsPostRequest**](ClientsPostRequest.md)|  | |

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="clientsGet"></a>
# **clientsGet**
> List&lt;Client&gt; clientsGet()

Get all clients

Retrieves all clients

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      List<Client> result = apiInstance.clientsGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#clientsGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;Client&gt;**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="clientsPost"></a>
# **clientsPost**
> Client clientsPost(clientsPostRequest)

Create new client

Add a new client with given name and url

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    ClientsPostRequest clientsPostRequest = new ClientsPostRequest(); // ClientsPostRequest | 
    try {
      Client result = apiInstance.clientsPost(clientsPostRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#clientsPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **clientsPostRequest** | [**ClientsPostRequest**](ClientsPostRequest.md)|  | |

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="contractsContractIdDelete"></a>
# **contractsContractIdDelete**
> contractsContractIdDelete(contractId)

Delete a contract by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer contractId = 56; // Integer | Numeric ID of the contract
    try {
      apiInstance.contractsContractIdDelete(contractId);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#contractsContractIdDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **contractId** | **Integer**| Numeric ID of the contract | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="contractsContractIdGet"></a>
# **contractsContractIdGet**
> Contract contractsContractIdGet(contractId)

Get a contract by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer contractId = 56; // Integer | Numeric ID of the contract
    try {
      Contract result = apiInstance.contractsContractIdGet(contractId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#contractsContractIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **contractId** | **Integer**| Numeric ID of the contract | |

### Return type

[**Contract**](Contract.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="contractsContractIdPut"></a>
# **contractsContractIdPut**
> Contract contractsContractIdPut(contractId, contractPatch)

Update a contract by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer contractId = 56; // Integer | Numeric ID of the contract
    ContractPatch contractPatch = new ContractPatch(); // ContractPatch | 
    try {
      Contract result = apiInstance.contractsContractIdPut(contractId, contractPatch);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#contractsContractIdPut");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **contractId** | **Integer**| Numeric ID of the contract | |
| **contractPatch** | [**ContractPatch**](ContractPatch.md)|  | |

### Return type

[**Contract**](Contract.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="contractsGet"></a>
# **contractsGet**
> List&lt;Contract&gt; contractsGet()

Get all contracts

Retrieves all contracts

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      List<Contract> result = apiInstance.contractsGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#contractsGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;Contract&gt;**](Contract.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="contractsPost"></a>
# **contractsPost**
> Contract contractsPost(contractPatch)

Create new contract

Add a new contract with fields

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    ContractPatch contractPatch = new ContractPatch(); // ContractPatch | 
    try {
      Contract result = apiInstance.contractsPost(contractPatch);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#contractsPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **contractPatch** | [**ContractPatch**](ContractPatch.md)|  | |

### Return type

[**Contract**](Contract.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="employeesEmployeeIdDelete"></a>
# **employeesEmployeeIdDelete**
> employeesEmployeeIdDelete(employeeId)

Delete an employee by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer employeeId = 56; // Integer | Numeric ID of the employee
    try {
      apiInstance.employeesEmployeeIdDelete(employeeId);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#employeesEmployeeIdDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **employeeId** | **Integer**| Numeric ID of the employee | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="employeesEmployeeIdGet"></a>
# **employeesEmployeeIdGet**
> Employee employeesEmployeeIdGet(employeeId)

Get an employee by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer employeeId = 56; // Integer | Numeric ID of the employee
    try {
      Employee result = apiInstance.employeesEmployeeIdGet(employeeId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#employeesEmployeeIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **employeeId** | **Integer**| Numeric ID of the employee | |

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="employeesEmployeeIdPut"></a>
# **employeesEmployeeIdPut**
> Employee employeesEmployeeIdPut(employeeId, employeesPostRequest)

Update an employee by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer employeeId = 56; // Integer | Numeric ID of the employee
    EmployeesPostRequest employeesPostRequest = new EmployeesPostRequest(); // EmployeesPostRequest | 
    try {
      Employee result = apiInstance.employeesEmployeeIdPut(employeeId, employeesPostRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#employeesEmployeeIdPut");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **employeeId** | **Integer**| Numeric ID of the employee | |
| **employeesPostRequest** | [**EmployeesPostRequest**](EmployeesPostRequest.md)|  | |

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="employeesGet"></a>
# **employeesGet**
> List&lt;Employee&gt; employeesGet()

Get all employees

Retrieves all employees

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      List<Employee> result = apiInstance.employeesGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#employeesGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;Employee&gt;**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="employeesPost"></a>
# **employeesPost**
> Employee employeesPost(employeesPostRequest)

Create new employee

Add a new employee with given name and github username

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    EmployeesPostRequest employeesPostRequest = new EmployeesPostRequest(); // EmployeesPostRequest | 
    try {
      Employee result = apiInstance.employeesPost(employeesPostRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#employeesPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **employeesPostRequest** | [**EmployeesPostRequest**](EmployeesPostRequest.md)|  | |

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="historyGet"></a>
# **historyGet**
> List&lt;History&gt; historyGet(employeeId, clientId, contractId)

Get all history

Retrieves all employee contract assignment history

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer employeeId = 56; // Integer | numerical employee identifier
    Integer clientId = 56; // Integer | numerical client identifier
    Integer contractId = 56; // Integer | numerical contract identifier
    try {
      List<History> result = apiInstance.historyGet(employeeId, clientId, contractId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#historyGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **employeeId** | **Integer**| numerical employee identifier | [optional] |
| **clientId** | **Integer**| numerical client identifier | [optional] |
| **contractId** | **Integer**| numerical contract identifier | [optional] |

### Return type

[**List&lt;History&gt;**](History.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="historyHistoryIdDelete"></a>
# **historyHistoryIdDelete**
> historyHistoryIdDelete(historyId)

Delete an employee contract assignment by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer historyId = 56; // Integer | Numeric ID of the employee contract assignment
    try {
      apiInstance.historyHistoryIdDelete(historyId);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#historyHistoryIdDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **historyId** | **Integer**| Numeric ID of the employee contract assignment | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="historyHistoryIdGet"></a>
# **historyHistoryIdGet**
> History historyHistoryIdGet(historyId)

Get an employee contract asignment by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer historyId = 56; // Integer | Numeric ID of the employee contract assignment
    try {
      History result = apiInstance.historyHistoryIdGet(historyId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#historyHistoryIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **historyId** | **Integer**| Numeric ID of the employee contract assignment | |

### Return type

[**History**](History.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="historyHistoryIdPut"></a>
# **historyHistoryIdPut**
> Contract historyHistoryIdPut(historyId, historyPatch)

Update an employee contract assignment by ID

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer historyId = 56; // Integer | Numeric ID of the employee contract assignment
    HistoryPatch historyPatch = new HistoryPatch(); // HistoryPatch | 
    try {
      Contract result = apiInstance.historyHistoryIdPut(historyId, historyPatch);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#historyHistoryIdPut");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **historyId** | **Integer**| Numeric ID of the employee contract assignment | |
| **historyPatch** | [**HistoryPatch**](HistoryPatch.md)|  | |

### Return type

[**Contract**](Contract.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a name="historyPost"></a>
# **historyPost**
> History historyPost(historyPatch)

Create new employee contract assignment

Add a new contract assignment with fields

### Example
```java
// Import classes:
import com.boxboat.simpletracker.api.ApiClient;
import com.boxboat.simpletracker.api.ApiException;
import com.boxboat.simpletracker.api.Configuration;
import com.boxboat.simpletracker.api.models.*;
import com.boxboat.simpletracker.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    HistoryPatch historyPatch = new HistoryPatch(); // HistoryPatch | 
    try {
      History result = apiInstance.historyPost(historyPatch);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#historyPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **historyPatch** | [**HistoryPatch**](HistoryPatch.md)|  | |

### Return type

[**History**](History.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

