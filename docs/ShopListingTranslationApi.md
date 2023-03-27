# \ShopListingTranslationApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateListingTranslation**](ShopListingTranslationApi.md#CreateListingTranslation) | **Post** /v3/application/shops/{shop_id}/listings/{listing_id}/translations/{language} | 
[**GetListingTranslation**](ShopListingTranslationApi.md#GetListingTranslation) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/translations/{language} | 
[**UpdateListingTranslation**](ShopListingTranslationApi.md#UpdateListingTranslation) | **Put** /v3/application/shops/{shop_id}/listings/{listing_id}/translations/{language} | 



## CreateListingTranslation

> ListingTranslation CreateListingTranslation(ctx, shopId, listingId, language).Title(title).Description(description).Tags(tags).Execute()





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
    language := "language_example" // string | The IETF language tag for the language of this translation. Ex: `de`, `en`, `es`, `fr`, `it`, `ja`, `nl`, `pl`, `pt`.
    title := "title_example" // string | The title of the Listing of this Translation.
    description := "description_example" // string | The description of the Listing of this Translation.
    tags := []string{"Inner_example"} // []string | The tags of the Listing of this Translation. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingTranslationApi.CreateListingTranslation(context.Background(), shopId, listingId, language).Title(title).Description(description).Tags(tags).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingTranslationApi.CreateListingTranslation``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateListingTranslation`: ListingTranslation
    fmt.Fprintf(os.Stdout, "Response from `ShopListingTranslationApi.CreateListingTranslation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**language** | **string** | The IETF language tag for the language of this translation. Ex: &#x60;de&#x60;, &#x60;en&#x60;, &#x60;es&#x60;, &#x60;fr&#x60;, &#x60;it&#x60;, &#x60;ja&#x60;, &#x60;nl&#x60;, &#x60;pl&#x60;, &#x60;pt&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateListingTranslationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **title** | **string** | The title of the Listing of this Translation. | 
 **description** | **string** | The description of the Listing of this Translation. | 
 **tags** | **[]string** | The tags of the Listing of this Translation. | 

### Return type

[**ListingTranslation**](ListingTranslation.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingTranslation

> ListingTranslation GetListingTranslation(ctx, shopId, listingId, language).Execute()





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
    language := "language_example" // string | The IETF language tag for the language of this translation. Ex: `de`, `en`, `es`, `fr`, `it`, `ja`, `nl`, `pl`, `pt`.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingTranslationApi.GetListingTranslation(context.Background(), shopId, listingId, language).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingTranslationApi.GetListingTranslation``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingTranslation`: ListingTranslation
    fmt.Fprintf(os.Stdout, "Response from `ShopListingTranslationApi.GetListingTranslation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**language** | **string** | The IETF language tag for the language of this translation. Ex: &#x60;de&#x60;, &#x60;en&#x60;, &#x60;es&#x60;, &#x60;fr&#x60;, &#x60;it&#x60;, &#x60;ja&#x60;, &#x60;nl&#x60;, &#x60;pl&#x60;, &#x60;pt&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingTranslationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ListingTranslation**](ListingTranslation.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateListingTranslation

> ListingTranslation UpdateListingTranslation(ctx, shopId, listingId, language).Title(title).Description(description).Tags(tags).Execute()





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
    language := "language_example" // string | The IETF language tag for the language of this translation. Ex: `de`, `en`, `es`, `fr`, `it`, `ja`, `nl`, `pl`, `pt`.
    title := "title_example" // string | The title of the Listing of this Translation.
    description := "description_example" // string | The description of the Listing of this Translation.
    tags := []string{"Inner_example"} // []string | The tags of the Listing of this Translation. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingTranslationApi.UpdateListingTranslation(context.Background(), shopId, listingId, language).Title(title).Description(description).Tags(tags).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingTranslationApi.UpdateListingTranslation``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateListingTranslation`: ListingTranslation
    fmt.Fprintf(os.Stdout, "Response from `ShopListingTranslationApi.UpdateListingTranslation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**language** | **string** | The IETF language tag for the language of this translation. Ex: &#x60;de&#x60;, &#x60;en&#x60;, &#x60;es&#x60;, &#x60;fr&#x60;, &#x60;it&#x60;, &#x60;ja&#x60;, &#x60;nl&#x60;, &#x60;pl&#x60;, &#x60;pt&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateListingTranslationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **title** | **string** | The title of the Listing of this Translation. | 
 **description** | **string** | The description of the Listing of this Translation. | 
 **tags** | **[]string** | The tags of the Listing of this Translation. | 

### Return type

[**ListingTranslation**](ListingTranslation.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

