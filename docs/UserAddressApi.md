# \UserAddressApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteUserAddress**](UserAddressApi.md#DeleteUserAddress) | **Delete** /v3/application/user/addresses/{user_address_id} | 
[**GetUserAddress**](UserAddressApi.md#GetUserAddress) | **Get** /v3/application/user/addresses/{user_address_id} | 
[**GetUserAddresses**](UserAddressApi.md#GetUserAddresses) | **Get** /v3/application/user/addresses | 



## DeleteUserAddress

> DeleteUserAddress(ctx, userAddressId).Execute()





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
    userAddressId := int32(56) // int32 | The numeric ID of the user's address.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.UserAddressApi.DeleteUserAddress(context.Background(), userAddressId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `UserAddressApi.DeleteUserAddress``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userAddressId** | **int32** | The numeric ID of the user&#39;s address. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteUserAddressRequest struct via the builder pattern


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


## GetUserAddress

> UserAddress GetUserAddress(ctx, userAddressId).Execute()





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
    userAddressId := int32(56) // int32 | The numeric ID of the user's address.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.UserAddressApi.GetUserAddress(context.Background(), userAddressId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `UserAddressApi.GetUserAddress``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetUserAddress`: UserAddress
    fmt.Fprintf(os.Stdout, "Response from `UserAddressApi.GetUserAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userAddressId** | **int32** | The numeric ID of the user&#39;s address. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**UserAddress**](UserAddress.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserAddresses

> UserAddresses GetUserAddresses(ctx).Limit(limit).Offset(offset).Execute()





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
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.UserAddressApi.GetUserAddresses(context.Background()).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `UserAddressApi.GetUserAddresses``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetUserAddresses`: UserAddresses
    fmt.Fprintf(os.Stdout, "Response from `UserAddressApi.GetUserAddresses`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetUserAddressesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**UserAddresses**](UserAddresses.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

