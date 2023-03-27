# \ReviewApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetReviewsByListing**](ReviewApi.md#GetReviewsByListing) | **Get** /v3/application/listings/{listing_id}/reviews | 
[**GetReviewsByShop**](ReviewApi.md#GetReviewsByShop) | **Get** /v3/application/shops/{shop_id}/reviews | 



## GetReviewsByListing

> ListingReviews GetReviewsByListing(ctx, listingId).Limit(limit).Offset(offset).MinCreated(minCreated).MaxCreated(maxCreated).Execute()





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
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)
    minCreated := int32(56) // int32 | The earliest unix timestamp for when a record was created. (optional)
    maxCreated := int32(56) // int32 | The latest unix timestamp for when a record was created. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ReviewApi.GetReviewsByListing(context.Background(), listingId).Limit(limit).Offset(offset).MinCreated(minCreated).MaxCreated(maxCreated).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ReviewApi.GetReviewsByListing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetReviewsByListing`: ListingReviews
    fmt.Fprintf(os.Stdout, "Response from `ReviewApi.GetReviewsByListing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReviewsByListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]
 **minCreated** | **int32** | The earliest unix timestamp for when a record was created. | 
 **maxCreated** | **int32** | The latest unix timestamp for when a record was created. | 

### Return type

[**ListingReviews**](ListingReviews.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetReviewsByShop

> TransactionReviews GetReviewsByShop(ctx, shopId).Limit(limit).Offset(offset).MinCreated(minCreated).MaxCreated(maxCreated).Execute()





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
    shopId := int32(56) // int32 | The unique positive non-zero numeric ID for an Etsy Shop.
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)
    minCreated := int32(56) // int32 | The earliest unix timestamp for when a record was created. (optional)
    maxCreated := int32(56) // int32 | The latest unix timestamp for when a record was created. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ReviewApi.GetReviewsByShop(context.Background(), shopId).Limit(limit).Offset(offset).MinCreated(minCreated).MaxCreated(maxCreated).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ReviewApi.GetReviewsByShop``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetReviewsByShop`: TransactionReviews
    fmt.Fprintf(os.Stdout, "Response from `ReviewApi.GetReviewsByShop`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReviewsByShopRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]
 **minCreated** | **int32** | The earliest unix timestamp for when a record was created. | 
 **maxCreated** | **int32** | The latest unix timestamp for when a record was created. | 

### Return type

[**TransactionReviews**](TransactionReviews.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

