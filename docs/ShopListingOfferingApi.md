# \ShopListingOfferingApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetListingOffering**](ShopListingOfferingApi.md#GetListingOffering) | **Get** /v3/application/listings/{listing_id}/products/{product_id}/offerings/{product_offering_id} | 



## GetListingOffering

> ListingInventoryProductOffering GetListingOffering(ctx, listingId, productId, productOfferingId).Execute()





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
    listingId := int32(56) // int32 | 
    productId := int32(56) // int32 | 
    productOfferingId := int32(56) // int32 | 

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingOfferingApi.GetListingOffering(context.Background(), listingId, productId, productOfferingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingOfferingApi.GetListingOffering``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingOffering`: ListingInventoryProductOffering
    fmt.Fprintf(os.Stdout, "Response from `ShopListingOfferingApi.GetListingOffering`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** |  | 
**productId** | **int32** |  | 
**productOfferingId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingOfferingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ListingInventoryProductOffering**](ListingInventoryProductOffering.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

