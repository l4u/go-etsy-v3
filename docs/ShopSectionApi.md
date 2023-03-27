# \ShopSectionApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateShopSection**](ShopSectionApi.md#CreateShopSection) | **Post** /v3/application/shops/{shop_id}/sections | 
[**DeleteShopSection**](ShopSectionApi.md#DeleteShopSection) | **Delete** /v3/application/shops/{shop_id}/sections/{shop_section_id} | 
[**GetShopSection**](ShopSectionApi.md#GetShopSection) | **Get** /v3/application/shops/{shop_id}/sections/{shop_section_id} | 
[**GetShopSections**](ShopSectionApi.md#GetShopSections) | **Get** /v3/application/shops/{shop_id}/sections | 
[**UpdateShopSection**](ShopSectionApi.md#UpdateShopSection) | **Put** /v3/application/shops/{shop_id}/sections/{shop_section_id} | 



## CreateShopSection

> ShopSection CreateShopSection(ctx, shopId).Title(title).Execute()





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
    title := "title_example" // string | The title string for a shop section.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopSectionApi.CreateShopSection(context.Background(), shopId).Title(title).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopSectionApi.CreateShopSection``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateShopSection`: ShopSection
    fmt.Fprintf(os.Stdout, "Response from `ShopSectionApi.CreateShopSection`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateShopSectionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **title** | **string** | The title string for a shop section. | 

### Return type

[**ShopSection**](ShopSection.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteShopSection

> DeleteShopSection(ctx, shopId, shopSectionId).Execute()





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
    shopSectionId := int32(56) // int32 | The numeric ID of a section in a specific Etsy shop.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopSectionApi.DeleteShopSection(context.Background(), shopId, shopSectionId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopSectionApi.DeleteShopSection``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shopSectionId** | **int32** | The numeric ID of a section in a specific Etsy shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteShopSectionRequest struct via the builder pattern


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


## GetShopSection

> ShopSection GetShopSection(ctx, shopId, shopSectionId).Execute()





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
    shopSectionId := int32(56) // int32 | The numeric ID of a section in a specific Etsy shop.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopSectionApi.GetShopSection(context.Background(), shopId, shopSectionId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopSectionApi.GetShopSection``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopSection`: ShopSection
    fmt.Fprintf(os.Stdout, "Response from `ShopSectionApi.GetShopSection`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shopSectionId** | **int32** | The numeric ID of a section in a specific Etsy shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopSectionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopSection**](ShopSection.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopSections

> ShopSections GetShopSections(ctx, shopId).Execute()





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

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopSectionApi.GetShopSections(context.Background(), shopId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopSectionApi.GetShopSections``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopSections`: ShopSections
    fmt.Fprintf(os.Stdout, "Response from `ShopSectionApi.GetShopSections`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopSectionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ShopSections**](ShopSections.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateShopSection

> ShopSection UpdateShopSection(ctx, shopId, shopSectionId).Title(title).Execute()





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
    shopSectionId := int32(56) // int32 | The numeric ID of a section in a specific Etsy shop.
    title := "title_example" // string | The title string for a shop section.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopSectionApi.UpdateShopSection(context.Background(), shopId, shopSectionId).Title(title).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopSectionApi.UpdateShopSection``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateShopSection`: ShopSection
    fmt.Fprintf(os.Stdout, "Response from `ShopSectionApi.UpdateShopSection`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shopSectionId** | **int32** | The numeric ID of a section in a specific Etsy shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateShopSectionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **title** | **string** | The title string for a shop section. | 

### Return type

[**ShopSection**](ShopSection.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

