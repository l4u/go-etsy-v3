# \ShopListingImageApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteListingImage**](ShopListingImageApi.md#DeleteListingImage) | **Delete** /v3/application/shops/{shop_id}/listings/{listing_id}/images/{listing_image_id} | 
[**GetListingImage**](ShopListingImageApi.md#GetListingImage) | **Get** /v3/application/listings/{listing_id}/images/{listing_image_id} | 
[**GetListingImageDeprecated**](ShopListingImageApi.md#GetListingImageDeprecated) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/images/{listing_image_id} | 
[**GetListingImages**](ShopListingImageApi.md#GetListingImages) | **Get** /v3/application/listings/{listing_id}/images | 
[**GetListingImagesDeprecated**](ShopListingImageApi.md#GetListingImagesDeprecated) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/images | 
[**UploadListingImage**](ShopListingImageApi.md#UploadListingImage) | **Post** /v3/application/shops/{shop_id}/listings/{listing_id}/images | 



## DeleteListingImage

> DeleteListingImage(ctx, shopId, listingId, listingImageId).Execute()





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
    listingImageId := int32(56) // int32 | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopListingImageApi.DeleteListingImage(context.Background(), shopId, listingId, listingImageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingImageApi.DeleteListingImage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**listingImageId** | **int32** | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteListingImageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

 (empty response body)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingImage

> ListingImage GetListingImage(ctx, listingId, listingImageId).Execute()





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
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    listingImageId := int32(56) // int32 | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingImageApi.GetListingImage(context.Background(), listingId, listingImageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingImageApi.GetListingImage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingImage`: ListingImage
    fmt.Fprintf(os.Stdout, "Response from `ShopListingImageApi.GetListingImage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**listingImageId** | **int32** | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingImageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListingImage**](ListingImage.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingImageDeprecated

> ListingImage GetListingImageDeprecated(ctx, shopId, listingId, listingImageId).Execute()





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
    listingImageId := int32(56) // int32 | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingImageApi.GetListingImageDeprecated(context.Background(), shopId, listingId, listingImageId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingImageApi.GetListingImageDeprecated``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingImageDeprecated`: ListingImage
    fmt.Fprintf(os.Stdout, "Response from `ShopListingImageApi.GetListingImageDeprecated`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**listingImageId** | **int32** | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingImageDeprecatedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ListingImage**](ListingImage.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingImages

> ListingImages GetListingImages(ctx, listingId).Execute()





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
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingImageApi.GetListingImages(context.Background(), listingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingImageApi.GetListingImages``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingImages`: ListingImages
    fmt.Fprintf(os.Stdout, "Response from `ShopListingImageApi.GetListingImages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingImagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ListingImages**](ListingImages.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingImagesDeprecated

> ListingImages GetListingImagesDeprecated(ctx, shopId, listingId).Execute()





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
    resp, r, err := apiClient.ShopListingImageApi.GetListingImagesDeprecated(context.Background(), shopId, listingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingImageApi.GetListingImagesDeprecated``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingImagesDeprecated`: ListingImages
    fmt.Fprintf(os.Stdout, "Response from `ShopListingImageApi.GetListingImagesDeprecated`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingImagesDeprecatedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListingImages**](ListingImages.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UploadListingImage

> ListingImage UploadListingImage(ctx, shopId, listingId).Image(image).ListingImageId(listingImageId).Rank(rank).Overwrite(overwrite).IsWatermarked(isWatermarked).AltText(altText).Execute()





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
    image := os.NewFile(1234, "some_file") // *os.File | The file name string of a file to upload (optional)
    listingImageId := int32(56) // int32 | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. (optional)
    rank := int32(56) // int32 | The positive non-zero numeric position in the images displayed in a listing, with rank 1 images appearing in the left-most position in a listing. (optional) (default to 1)
    overwrite := true // bool | When true, this request replaces the existing image at a given rank. (optional) (default to false)
    isWatermarked := true // bool | When true, indicates that the uploaded image has a watermark. (optional) (default to false)
    altText := "altText_example" // string | Alt text for the listing image. (optional) (default to "")

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingImageApi.UploadListingImage(context.Background(), shopId, listingId).Image(image).ListingImageId(listingImageId).Rank(rank).Overwrite(overwrite).IsWatermarked(isWatermarked).AltText(altText).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingImageApi.UploadListingImage``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UploadListingImage`: ListingImage
    fmt.Fprintf(os.Stdout, "Response from `ShopListingImageApi.UploadListingImage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUploadListingImageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **image** | ***os.File** | The file name string of a file to upload | 
 **listingImageId** | **int32** | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. | 
 **rank** | **int32** | The positive non-zero numeric position in the images displayed in a listing, with rank 1 images appearing in the left-most position in a listing. | [default to 1]
 **overwrite** | **bool** | When true, this request replaces the existing image at a given rank. | [default to false]
 **isWatermarked** | **bool** | When true, indicates that the uploaded image has a watermark. | [default to false]
 **altText** | **string** | Alt text for the listing image. | [default to &quot;&quot;]

### Return type

[**ListingImage**](ListingImage.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

