# PetsApi

All URIs are relative to *http://petstore.swagger.io/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createPets**](PetsApi.md#createPets) | **POST** /pets | Create a pet |


<a name="createPets"></a>
# **createPets**
> createPets(createPetData)

Create a pet

### Example
```java
// Import classes:
import com.github.dhslrl321.openapi.invoker.ApiClient;
import com.github.dhslrl321.openapi.invoker.ApiException;
import com.github.dhslrl321.openapi.invoker.Configuration;
import com.github.dhslrl321.openapi.invoker.models.*;
import com.github.dhslrl321.openapi.PetsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://petstore.swagger.io/v1");

    PetsApi apiInstance = new PetsApi(defaultClient);
    CreatePetData createPetData = new CreatePetData(); // CreatePetData | 
    try {
      apiInstance.createPets(createPetData);
    } catch (ApiException e) {
      System.err.println("Exception when calling PetsApi#createPets");
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
| **createPetData** | [**CreatePetData**](CreatePetData.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Null response |  -  |
| **0** | unexpected error |  -  |

