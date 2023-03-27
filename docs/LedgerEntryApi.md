# \LedgerEntryApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetShopPaymentAccountLedgerEntries**](LedgerEntryApi.md#GetShopPaymentAccountLedgerEntries) | **Get** /v3/application/shops/{shop_id}/payment-account/ledger-entries | 
[**GetShopPaymentAccountLedgerEntry**](LedgerEntryApi.md#GetShopPaymentAccountLedgerEntry) | **Get** /v3/application/shops/{shop_id}/payment-account/ledger-entries/{ledger_entry_id} | 



## GetShopPaymentAccountLedgerEntries

> PaymentAccountLedgerEntries GetShopPaymentAccountLedgerEntries(ctx, shopId).MinCreated(minCreated).MaxCreated(maxCreated).Limit(limit).Offset(offset).Execute()





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
    minCreated := int32(56) // int32 | The earliest unix timestamp for when a record was created.
    maxCreated := int32(56) // int32 | The latest unix timestamp for when a record was created.
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.LedgerEntryApi.GetShopPaymentAccountLedgerEntries(context.Background(), shopId).MinCreated(minCreated).MaxCreated(maxCreated).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `LedgerEntryApi.GetShopPaymentAccountLedgerEntries``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopPaymentAccountLedgerEntries`: PaymentAccountLedgerEntries
    fmt.Fprintf(os.Stdout, "Response from `LedgerEntryApi.GetShopPaymentAccountLedgerEntries`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopPaymentAccountLedgerEntriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **minCreated** | **int32** | The earliest unix timestamp for when a record was created. | 
 **maxCreated** | **int32** | The latest unix timestamp for when a record was created. | 
 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**PaymentAccountLedgerEntries**](PaymentAccountLedgerEntries.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopPaymentAccountLedgerEntry

> PaymentAccountLedgerEntry GetShopPaymentAccountLedgerEntry(ctx, shopId, ledgerEntryId).Execute()





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
    ledgerEntryId := int32(56) // int32 | The unique ID of the shop owner ledger entry.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.LedgerEntryApi.GetShopPaymentAccountLedgerEntry(context.Background(), shopId, ledgerEntryId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `LedgerEntryApi.GetShopPaymentAccountLedgerEntry``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopPaymentAccountLedgerEntry`: PaymentAccountLedgerEntry
    fmt.Fprintf(os.Stdout, "Response from `LedgerEntryApi.GetShopPaymentAccountLedgerEntry`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**ledgerEntryId** | **int32** | The unique ID of the shop owner ledger entry. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopPaymentAccountLedgerEntryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**PaymentAccountLedgerEntry**](PaymentAccountLedgerEntry.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

