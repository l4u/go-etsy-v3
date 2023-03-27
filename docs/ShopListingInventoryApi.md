# \ShopListingInventoryApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetListingInventory**](ShopListingInventoryApi.md#GetListingInventory) | **Get** /v3/application/listings/{listing_id}/inventory | 
[**UpdateListingInventory**](ShopListingInventoryApi.md#UpdateListingInventory) | **Put** /v3/application/listings/{listing_id}/inventory | 



## GetListingInventory

> ListingInventoryWithAssociations GetListingInventory(ctx, listingId).ShowDeleted(showDeleted).Includes(includes).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    showDeleted := true // bool | A boolean value for inventory whether to include deleted products and their offerings. Default value is false. (optional)
    includes := "includes_example" // string | An enumerated string that attaches a valid association. Default value is null. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingInventoryApi.GetListingInventory(context.Background(), listingId).ShowDeleted(showDeleted).Includes(includes).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingInventoryApi.GetListingInventory``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingInventory`: ListingInventoryWithAssociations
    fmt.Fprintf(os.Stdout, "Response from `ShopListingInventoryApi.GetListingInventory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingInventoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **showDeleted** | **bool** | A boolean value for inventory whether to include deleted products and their offerings. Default value is false. | 
 **includes** | **string** | An enumerated string that attaches a valid association. Default value is null. | 

### Return type

[**ListingInventoryWithAssociations**](ListingInventoryWithAssociations.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateListingInventory

> ListingInventory UpdateListingInventory(ctx, listingId).UpdateListingInventoryRequest(updateListingInventoryRequest).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    updateListingInventoryRequest := *openapiclient.NewUpdateListingInventoryRequest([]openapiclient.UpdateListingInventoryRequestProductsInner{*openapiclient.NewUpdateListingInventoryRequestProductsInner([]openapiclient.UpdateListingInventoryRequestProductsInnerOfferingsInner{*openapiclient.NewUpdateListingInventoryRequestProductsInnerOfferingsInner(float32(123), int32(123), false)})}) // UpdateListingInventoryRequest |  (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingInventoryApi.UpdateListingInventory(context.Background(), listingId).UpdateListingInventoryRequest(updateListingInventoryRequest).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingInventoryApi.UpdateListingInventory``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateListingInventory`: ListingInventory
    fmt.Fprintf(os.Stdout, "Response from `ShopListingInventoryApi.UpdateListingInventory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateListingInventoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateListingInventoryRequest** | [**UpdateListingInventoryRequest**](UpdateListingInventoryRequest.md) |  | 

### Return type

[**ListingInventory**](ListingInventory.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

