# PublicOperationsApi

All URIs are relative to *https://localhost/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**searchInventory**](PublicOperationsApi.md#searchInventory) | **GET** /inventory | searches inventory


<a name="searchInventory"></a>
# **searchInventory**
> List&lt;InventoryItem&gt; searchInventory(searchString, skip, limit)

searches inventory

By passing in the appropriate options, you can search for available inventory in the system 

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PublicOperationsApi;


PublicOperationsApi apiInstance = new PublicOperationsApi();
String searchString = "searchString_example"; // String | pass an optional search string for looking up inventory
Integer skip = 56; // Integer | number of records to skip for pagination
Integer limit = 56; // Integer | maximum number of records to return
try {
    List<InventoryItem> result = apiInstance.searchInventory(searchString, skip, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PublicOperationsApi#searchInventory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **searchString** | **String**| pass an optional search string for looking up inventory | [optional]
 **skip** | **Integer**| number of records to skip for pagination | [optional]
 **limit** | **Integer**| maximum number of records to return | [optional]

### Return type

[**List&lt;InventoryItem&gt;**](InventoryItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

