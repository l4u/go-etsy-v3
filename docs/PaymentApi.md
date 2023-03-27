# \PaymentApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetPaymentAccountLedgerEntryPayments**](PaymentApi.md#GetPaymentAccountLedgerEntryPayments) | **Get** /v3/application/shops/{shop_id}/payment-account/ledger-entries/payments | 
[**GetPayments**](PaymentApi.md#GetPayments) | **Get** /v3/application/shops/{shop_id}/payments | 
[**GetShopPaymentByReceiptId**](PaymentApi.md#GetShopPaymentByReceiptId) | **Get** /v3/application/shops/{shop_id}/receipts/{receipt_id}/payments | 



## GetPaymentAccountLedgerEntryPayments

> Payments GetPaymentAccountLedgerEntryPayments(ctx, shopId).LedgerEntryIds(ledgerEntryIds).Execute()





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
    ledgerEntryIds := []int32{int32(123)} // []int32 | 

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PaymentApi.GetPaymentAccountLedgerEntryPayments(context.Background(), shopId).LedgerEntryIds(ledgerEntryIds).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PaymentApi.GetPaymentAccountLedgerEntryPayments``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetPaymentAccountLedgerEntryPayments`: Payments
    fmt.Fprintf(os.Stdout, "Response from `PaymentApi.GetPaymentAccountLedgerEntryPayments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPaymentAccountLedgerEntryPaymentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ledgerEntryIds** | **[]int32** |  | 

### Return type

[**Payments**](Payments.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPayments

> Payments GetPayments(ctx, shopId).PaymentIds(paymentIds).Execute()





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
    paymentIds := []int32{int32(123)} // []int32 | A comma-separated array of Payment IDs numbers.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PaymentApi.GetPayments(context.Background(), shopId).PaymentIds(paymentIds).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PaymentApi.GetPayments``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetPayments`: Payments
    fmt.Fprintf(os.Stdout, "Response from `PaymentApi.GetPayments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPaymentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **paymentIds** | **[]int32** | A comma-separated array of Payment IDs numbers. | 

### Return type

[**Payments**](Payments.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopPaymentByReceiptId

> Payments GetShopPaymentByReceiptId(ctx, shopId, receiptId).Execute()





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
    receiptId := int32(56) // int32 | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PaymentApi.GetShopPaymentByReceiptId(context.Background(), shopId, receiptId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PaymentApi.GetShopPaymentByReceiptId``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopPaymentByReceiptId`: Payments
    fmt.Fprintf(os.Stdout, "Response from `PaymentApi.GetShopPaymentByReceiptId`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**receiptId** | **int32** | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopPaymentByReceiptIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Payments**](Payments.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

