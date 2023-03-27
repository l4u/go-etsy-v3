# \ShopListingVariationImageApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetListingVariationImages**](ShopListingVariationImageApi.md#GetListingVariationImages) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/variation-images | 
[**UpdateVariationImages**](ShopListingVariationImageApi.md#UpdateVariationImages) | **Post** /v3/application/shops/{shop_id}/listings/{listing_id}/variation-images | 



## GetListingVariationImages

> ListingVariationImages GetListingVariationImages(ctx, shopId, listingId).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/l4u/go-etsyv3"
)

func main() {
    shopId := int32(56) // int32 | The unique positive non-zero numeric ID for an Etsy Shop.
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingVariationImageApi.GetListingVariationImages(context.Background(), shopId, listingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingVariationImageApi.GetListingVariationImages``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingVariationImages`: ListingVariationImages
    fmt.Fprintf(os.Stdout, "Response from `ShopListingVariationImageApi.GetListingVariationImages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingVariationImagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListingVariationImages**](ListingVariationImages.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateVariationImages

> ListingVariationImages UpdateVariationImages(ctx, shopId, listingId).UpdateVariationImagesRequest(updateVariationImagesRequest).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/l4u/go-etsyv3"
)

func main() {
    shopId := int32(56) // int32 | The unique positive non-zero numeric ID for an Etsy Shop.
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    updateVariationImagesRequest := *openapiclient.NewUpdateVariationImagesRequest([]openapiclient.UpdateVariationImagesRequestVariationImagesInner{*openapiclient.NewUpdateVariationImagesRequestVariationImagesInner(int32(123), int32(123), int32(123))}) // UpdateVariationImagesRequest |  (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingVariationImageApi.UpdateVariationImages(context.Background(), shopId, listingId).UpdateVariationImagesRequest(updateVariationImagesRequest).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingVariationImageApi.UpdateVariationImages``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateVariationImages`: ListingVariationImages
    fmt.Fprintf(os.Stdout, "Response from `ShopListingVariationImageApi.UpdateVariationImages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateVariationImagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateVariationImagesRequest** | [**UpdateVariationImagesRequest**](UpdateVariationImagesRequest.md) |  | 

### Return type

[**ListingVariationImages**](ListingVariationImages.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

