# AdminOperationsApi

All URIs are relative to *https://localhost/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addInventory**](AdminOperationsApi.md#addInventory) | **POST** /inventory | adds an inventory item


<a name="addInventory"></a>
# **addInventory**
> addInventory(inventoryItem)

adds an inventory item

Adds an item to the system

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.AdminOperationsApi;


AdminOperationsApi apiInstance = new AdminOperationsApi();
InventoryItem inventoryItem = new InventoryItem(); // InventoryItem | Inventory item to add
try {
    apiInstance.addInventory(inventoryItem);
} catch (ApiException e) {
    System.err.println("Exception when calling AdminOperationsApi#addInventory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventoryItem** | [**InventoryItem**](InventoryItem.md)| Inventory item to add | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

