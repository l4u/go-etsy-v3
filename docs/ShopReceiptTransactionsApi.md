# \ShopReceiptTransactionsApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetShopReceiptTransaction**](ShopReceiptTransactionsApi.md#GetShopReceiptTransaction) | **Get** /v3/application/shops/{shop_id}/transactions/{transaction_id} | 
[**GetShopReceiptTransactionsByListing**](ShopReceiptTransactionsApi.md#GetShopReceiptTransactionsByListing) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/transactions | 
[**GetShopReceiptTransactionsByReceipt**](ShopReceiptTransactionsApi.md#GetShopReceiptTransactionsByReceipt) | **Get** /v3/application/shops/{shop_id}/receipts/{receipt_id}/transactions | 
[**GetShopReceiptTransactionsByShop**](ShopReceiptTransactionsApi.md#GetShopReceiptTransactionsByShop) | **Get** /v3/application/shops/{shop_id}/transactions | 



## GetShopReceiptTransaction

> ShopReceiptTransaction GetShopReceiptTransaction(ctx, shopId, transactionId).Execute()





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
    transactionId := int32(56) // int32 | The unique numeric ID for a transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopReceiptTransactionsApi.GetShopReceiptTransaction(context.Background(), shopId, transactionId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopReceiptTransactionsApi.GetShopReceiptTransaction``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopReceiptTransaction`: ShopReceiptTransaction
    fmt.Fprintf(os.Stdout, "Response from `ShopReceiptTransactionsApi.GetShopReceiptTransaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**transactionId** | **int32** | The unique numeric ID for a transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopReceiptTransactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopReceiptTransaction**](ShopReceiptTransaction.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopReceiptTransactionsByListing

> ShopReceiptTransactions GetShopReceiptTransactionsByListing(ctx, shopId, listingId).Limit(limit).Offset(offset).Execute()





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
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopReceiptTransactionsApi.GetShopReceiptTransactionsByListing(context.Background(), shopId, listingId).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopReceiptTransactionsApi.GetShopReceiptTransactionsByListing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopReceiptTransactionsByListing`: ShopReceiptTransactions
    fmt.Fprintf(os.Stdout, "Response from `ShopReceiptTransactionsApi.GetShopReceiptTransactionsByListing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopReceiptTransactionsByListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**ShopReceiptTransactions**](ShopReceiptTransactions.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopReceiptTransactionsByReceipt

> ShopReceiptTransactions GetShopReceiptTransactionsByReceipt(ctx, shopId, receiptId).Execute()





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
    receiptId := int32(56) // int32 | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopReceiptTransactionsApi.GetShopReceiptTransactionsByReceipt(context.Background(), shopId, receiptId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopReceiptTransactionsApi.GetShopReceiptTransactionsByReceipt``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopReceiptTransactionsByReceipt`: ShopReceiptTransactions
    fmt.Fprintf(os.Stdout, "Response from `ShopReceiptTransactionsApi.GetShopReceiptTransactionsByReceipt`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**receiptId** | **int32** | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopReceiptTransactionsByReceiptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopReceiptTransactions**](ShopReceiptTransactions.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopReceiptTransactionsByShop

> ShopReceiptTransactions GetShopReceiptTransactionsByShop(ctx, shopId).Limit(limit).Offset(offset).Execute()





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

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopReceiptTransactionsApi.GetShopReceiptTransactionsByShop(context.Background(), shopId).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopReceiptTransactionsApi.GetShopReceiptTransactionsByShop``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopReceiptTransactionsByShop`: ShopReceiptTransactions
    fmt.Fprintf(os.Stdout, "Response from `ShopReceiptTransactionsApi.GetShopReceiptTransactionsByShop`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopReceiptTransactionsByShopRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**ShopReceiptTransactions**](ShopReceiptTransactions.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

