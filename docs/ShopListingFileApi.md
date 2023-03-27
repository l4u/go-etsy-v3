# \ShopListingFileApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteListingFile**](ShopListingFileApi.md#DeleteListingFile) | **Delete** /v3/application/shops/{shop_id}/listings/{listing_id}/files/{listing_file_id} | 
[**GetAllListingFiles**](ShopListingFileApi.md#GetAllListingFiles) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/files | 
[**GetListingFile**](ShopListingFileApi.md#GetListingFile) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/files/{listing_file_id} | 
[**UploadListingFile**](ShopListingFileApi.md#UploadListingFile) | **Post** /v3/application/shops/{shop_id}/listings/{listing_id}/files | 



## DeleteListingFile

> DeleteListingFile(ctx, shopId, listingId, listingFileId).Execute()





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
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    listingFileId := int32(56) // int32 | The unique numeric ID of a file associated with a digital listing.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopListingFileApi.DeleteListingFile(context.Background(), shopId, listingId, listingFileId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingFileApi.DeleteListingFile``: %v\n", err)
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
**listingFileId** | **int32** | The unique numeric ID of a file associated with a digital listing. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteListingFileRequest struct via the builder pattern


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


## GetAllListingFiles

> ShopListingFiles GetAllListingFiles(ctx, listingId, shopId).Execute()





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
    shopId := int32(56) // int32 | The unique positive non-zero numeric ID for an Etsy Shop.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingFileApi.GetAllListingFiles(context.Background(), listingId, shopId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingFileApi.GetAllListingFiles``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetAllListingFiles`: ShopListingFiles
    fmt.Fprintf(os.Stdout, "Response from `ShopListingFileApi.GetAllListingFiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAllListingFilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopListingFiles**](ShopListingFiles.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingFile

> ShopListingFile GetListingFile(ctx, shopId, listingId, listingFileId).Execute()





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
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    listingFileId := int32(56) // int32 | The unique numeric ID of a file associated with a digital listing.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingFileApi.GetListingFile(context.Background(), shopId, listingId, listingFileId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingFileApi.GetListingFile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingFile`: ShopListingFile
    fmt.Fprintf(os.Stdout, "Response from `ShopListingFileApi.GetListingFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**listingFileId** | **int32** | The unique numeric ID of a file associated with a digital listing. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ShopListingFile**](ShopListingFile.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UploadListingFile

> ShopListingFile UploadListingFile(ctx, shopId, listingId).ListingFileId(listingFileId).File(file).Name(name).Rank(rank).Execute()





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
    listingId := int32(56) // int32 | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction.
    listingFileId := int32(56) // int32 | The unique numeric ID of a file associated with a digital listing. (optional)
    file := os.NewFile(1234, "some_file") // *os.File | A binary file to upload. (optional)
    name := "name_example" // string | The file name string of a file to upload (optional)
    rank := int32(56) // int32 | The positive non-zero numeric position in the images displayed in a listing, with rank 1 images appearing in the left-most position in a listing. (optional) (default to 1)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingFileApi.UploadListingFile(context.Background(), shopId, listingId).ListingFileId(listingFileId).File(file).Name(name).Rank(rank).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingFileApi.UploadListingFile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UploadListingFile`: ShopListingFile
    fmt.Fprintf(os.Stdout, "Response from `ShopListingFileApi.UploadListingFile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUploadListingFileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **listingFileId** | **int32** | The unique numeric ID of a file associated with a digital listing. | 
 **file** | ***os.File** | A binary file to upload. | 
 **name** | **string** | The file name string of a file to upload | 
 **rank** | **int32** | The positive non-zero numeric position in the images displayed in a listing, with rank 1 images appearing in the left-most position in a listing. | [default to 1]

### Return type

[**ShopListingFile**](ShopListingFile.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

