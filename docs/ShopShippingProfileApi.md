# \ShopShippingProfileApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateShopShippingProfile**](ShopShippingProfileApi.md#CreateShopShippingProfile) | **Post** /v3/application/shops/{shop_id}/shipping-profiles | 
[**CreateShopShippingProfileDestination**](ShopShippingProfileApi.md#CreateShopShippingProfileDestination) | **Post** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/destinations | 
[**CreateShopShippingProfileUpgrade**](ShopShippingProfileApi.md#CreateShopShippingProfileUpgrade) | **Post** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/upgrades | 
[**DeleteShopShippingProfile**](ShopShippingProfileApi.md#DeleteShopShippingProfile) | **Delete** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id} | 
[**DeleteShopShippingProfileDestination**](ShopShippingProfileApi.md#DeleteShopShippingProfileDestination) | **Delete** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/destinations/{shipping_profile_destination_id} | 
[**DeleteShopShippingProfileUpgrade**](ShopShippingProfileApi.md#DeleteShopShippingProfileUpgrade) | **Delete** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/upgrades/{upgrade_id} | 
[**GetShippingCarriers**](ShopShippingProfileApi.md#GetShippingCarriers) | **Get** /v3/application/shipping-carriers | 
[**GetShopShippingProfile**](ShopShippingProfileApi.md#GetShopShippingProfile) | **Get** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id} | 
[**GetShopShippingProfileDestinationsByShippingProfile**](ShopShippingProfileApi.md#GetShopShippingProfileDestinationsByShippingProfile) | **Get** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/destinations | 
[**GetShopShippingProfileUpgrades**](ShopShippingProfileApi.md#GetShopShippingProfileUpgrades) | **Get** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/upgrades | 
[**GetShopShippingProfiles**](ShopShippingProfileApi.md#GetShopShippingProfiles) | **Get** /v3/application/shops/{shop_id}/shipping-profiles | 
[**UpdateShopShippingProfile**](ShopShippingProfileApi.md#UpdateShopShippingProfile) | **Put** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id} | 
[**UpdateShopShippingProfileDestination**](ShopShippingProfileApi.md#UpdateShopShippingProfileDestination) | **Put** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/destinations/{shipping_profile_destination_id} | 
[**UpdateShopShippingProfileUpgrade**](ShopShippingProfileApi.md#UpdateShopShippingProfileUpgrade) | **Put** /v3/application/shops/{shop_id}/shipping-profiles/{shipping_profile_id}/upgrades/{upgrade_id} | 



## CreateShopShippingProfile

> ShopShippingProfile CreateShopShippingProfile(ctx, shopId).Title(title).OriginCountryIso(originCountryIso).PrimaryCost(primaryCost).SecondaryCost(secondaryCost).MinProcessingTime(minProcessingTime).MaxProcessingTime(maxProcessingTime).ProcessingTimeUnit(processingTimeUnit).DestinationCountryIso(destinationCountryIso).DestinationRegion(destinationRegion).OriginPostalCode(originPostalCode).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()





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
    title := "title_example" // string | The name string of this shipping profile.
    originCountryIso := "originCountryIso_example" // string | The ISO code of the country from which the listing ships.
    primaryCost := float32(3.4) // float32 | The cost of shipping to this country/region alone, measured in the store's default currency.
    secondaryCost := float32(3.4) // float32 | The cost of shipping to this country/region with another item, measured in the store's default currency.
    minProcessingTime := int32(56) // int32 | The minimum time required to process to ship listings with this shipping profile.
    maxProcessingTime := int32(56) // int32 | The maximum processing time the listing needs to ship.
    processingTimeUnit := "processingTimeUnit_example" // string | The unit used to represent how long a processing time is. A week is equivalent to 5 business days. If none is provided, the unit is set to \\\"business_days\\\". (optional) (default to "business_days")
    destinationCountryIso := "destinationCountryIso_example" // string | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. (optional)
    destinationRegion := "destinationRegion_example" // string | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If `none`, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. (optional) (default to "none")
    originPostalCode := "originPostalCode_example" // string | The postal code string (not necessarily a number) for the location from which the listing ships. Required if the `origin_country_iso` is `US` or `CA`. (optional) (default to "")
    shippingCarrierId := int32(56) // int32 | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with `mail_class`** if `min_delivery_days` and `max_delivery_days` are null. (optional) (default to 0)
    mailClass := "mailClass_example" // string | The unique ID string of a shipping carrier's mail class, which is used to calculate an estimated delivery date. **Required with `shipping_carrier_id`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    minDeliveryDays := int32(56) // int32 | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `max_delivery_days`** if `mail_class` is null. (optional)
    maxDeliveryDays := int32(56) // int32 | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `min_delivery_days`** if `mail_class` is null. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.CreateShopShippingProfile(context.Background(), shopId).Title(title).OriginCountryIso(originCountryIso).PrimaryCost(primaryCost).SecondaryCost(secondaryCost).MinProcessingTime(minProcessingTime).MaxProcessingTime(maxProcessingTime).ProcessingTimeUnit(processingTimeUnit).DestinationCountryIso(destinationCountryIso).DestinationRegion(destinationRegion).OriginPostalCode(originPostalCode).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.CreateShopShippingProfile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateShopShippingProfile`: ShopShippingProfile
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.CreateShopShippingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateShopShippingProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **title** | **string** | The name string of this shipping profile. | 
 **originCountryIso** | **string** | The ISO code of the country from which the listing ships. | 
 **primaryCost** | **float32** | The cost of shipping to this country/region alone, measured in the store&#39;s default currency. | 
 **secondaryCost** | **float32** | The cost of shipping to this country/region with another item, measured in the store&#39;s default currency. | 
 **minProcessingTime** | **int32** | The minimum time required to process to ship listings with this shipping profile. | 
 **maxProcessingTime** | **int32** | The maximum processing time the listing needs to ship. | 
 **processingTimeUnit** | **string** | The unit used to represent how long a processing time is. A week is equivalent to 5 business days. If none is provided, the unit is set to \\\&quot;business_days\\\&quot;. | [default to &quot;business_days&quot;]
 **destinationCountryIso** | **string** | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. | 
 **destinationRegion** | **string** | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If &#x60;none&#x60;, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. | [default to &quot;none&quot;]
 **originPostalCode** | **string** | The postal code string (not necessarily a number) for the location from which the listing ships. Required if the &#x60;origin_country_iso&#x60; is &#x60;US&#x60; or &#x60;CA&#x60;. | [default to &quot;&quot;]
 **shippingCarrierId** | **int32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [default to 0]
 **mailClass** | **string** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **minDeliveryDays** | **int32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 
 **maxDeliveryDays** | **int32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 

### Return type

[**ShopShippingProfile**](ShopShippingProfile.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateShopShippingProfileDestination

> ShopShippingProfileDestination CreateShopShippingProfileDestination(ctx, shopId, shippingProfileId).PrimaryCost(primaryCost).SecondaryCost(secondaryCost).DestinationCountryIso(destinationCountryIso).DestinationRegion(destinationRegion).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    primaryCost := float32(3.4) // float32 | The cost of shipping to this country/region alone, measured in the store's default currency.
    secondaryCost := float32(3.4) // float32 | The cost of shipping to this country/region with another item, measured in the store's default currency.
    destinationCountryIso := "destinationCountryIso_example" // string | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. (optional)
    destinationRegion := "destinationRegion_example" // string | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If `none`, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. (optional) (default to "none")
    shippingCarrierId := int32(56) // int32 | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with `mail_class`** if `min_delivery_days` and `max_delivery_days` are null. (optional) (default to 0)
    mailClass := "mailClass_example" // string | The unique ID string of a shipping carrier's mail class, which is used to calculate an estimated delivery date. **Required with `shipping_carrier_id`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    minDeliveryDays := int32(56) // int32 | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `max_delivery_days`** if `mail_class` is null. (optional)
    maxDeliveryDays := int32(56) // int32 | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `min_delivery_days`** if `mail_class` is null. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.CreateShopShippingProfileDestination(context.Background(), shopId, shippingProfileId).PrimaryCost(primaryCost).SecondaryCost(secondaryCost).DestinationCountryIso(destinationCountryIso).DestinationRegion(destinationRegion).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.CreateShopShippingProfileDestination``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateShopShippingProfileDestination`: ShopShippingProfileDestination
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.CreateShopShippingProfileDestination`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateShopShippingProfileDestinationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **primaryCost** | **float32** | The cost of shipping to this country/region alone, measured in the store&#39;s default currency. | 
 **secondaryCost** | **float32** | The cost of shipping to this country/region with another item, measured in the store&#39;s default currency. | 
 **destinationCountryIso** | **string** | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. | 
 **destinationRegion** | **string** | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If &#x60;none&#x60;, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. | [default to &quot;none&quot;]
 **shippingCarrierId** | **int32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [default to 0]
 **mailClass** | **string** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **minDeliveryDays** | **int32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 
 **maxDeliveryDays** | **int32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 

### Return type

[**ShopShippingProfileDestination**](ShopShippingProfileDestination.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateShopShippingProfileUpgrade

> ShopShippingProfileUpgrade CreateShopShippingProfileUpgrade(ctx, shopId, shippingProfileId).Type_(type_).UpgradeName(upgradeName).Price(price).SecondaryPrice(secondaryPrice).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    type_ := "type__example" // string | The type of the shipping upgrade. Domestic (0) or international (1).
    upgradeName := "upgradeName_example" // string | Name for the shipping upgrade shown to shoppers at checkout, e.g. USPS Priority.
    price := float32(3.4) // float32 | Additional cost of adding the shipping upgrade.
    secondaryPrice := float32(3.4) // float32 | Additional cost of adding the shipping upgrade for each additional item.
    shippingCarrierId := int32(56) // int32 | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with `mail_class`** if `min_delivery_days` and `max_delivery_days` are null. (optional) (default to 0)
    mailClass := "mailClass_example" // string | The unique ID string of a shipping carrier's mail class, which is used to calculate an estimated delivery date. **Required with `shipping_carrier_id`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    minDeliveryDays := int32(56) // int32 | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `max_delivery_days`** if `mail_class` is null. (optional)
    maxDeliveryDays := int32(56) // int32 | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `min_delivery_days`** if `mail_class` is null. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.CreateShopShippingProfileUpgrade(context.Background(), shopId, shippingProfileId).Type_(type_).UpgradeName(upgradeName).Price(price).SecondaryPrice(secondaryPrice).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.CreateShopShippingProfileUpgrade``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateShopShippingProfileUpgrade`: ShopShippingProfileUpgrade
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.CreateShopShippingProfileUpgrade`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateShopShippingProfileUpgradeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **type_** | **string** | The type of the shipping upgrade. Domestic (0) or international (1). | 
 **upgradeName** | **string** | Name for the shipping upgrade shown to shoppers at checkout, e.g. USPS Priority. | 
 **price** | **float32** | Additional cost of adding the shipping upgrade. | 
 **secondaryPrice** | **float32** | Additional cost of adding the shipping upgrade for each additional item. | 
 **shippingCarrierId** | **int32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [default to 0]
 **mailClass** | **string** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **minDeliveryDays** | **int32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 
 **maxDeliveryDays** | **int32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 

### Return type

[**ShopShippingProfileUpgrade**](ShopShippingProfileUpgrade.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteShopShippingProfile

> DeleteShopShippingProfile(ctx, shopId, shippingProfileId).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopShippingProfileApi.DeleteShopShippingProfile(context.Background(), shopId, shippingProfileId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.DeleteShopShippingProfile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteShopShippingProfileRequest struct via the builder pattern


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


## DeleteShopShippingProfileDestination

> DeleteShopShippingProfileDestination(ctx, shopId, shippingProfileId, shippingProfileDestinationId).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    shippingProfileDestinationId := int32(56) // int32 | The numeric ID of the shipping profile destination in the [shipping profile](/documentation/reference#tag/Shop-ShippingProfile) associated with the listing.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopShippingProfileApi.DeleteShopShippingProfileDestination(context.Background(), shopId, shippingProfileId, shippingProfileDestinationId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.DeleteShopShippingProfileDestination``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 
**shippingProfileDestinationId** | **int32** | The numeric ID of the shipping profile destination in the [shipping profile](/documentation/reference#tag/Shop-ShippingProfile) associated with the listing. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteShopShippingProfileDestinationRequest struct via the builder pattern


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


## DeleteShopShippingProfileUpgrade

> DeleteShopShippingProfileUpgrade(ctx, shopId, shippingProfileId, upgradeId).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the shipping profile.
    upgradeId := int32(56) // int32 | The numeric ID that is associated with a shipping upgrade

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopShippingProfileApi.DeleteShopShippingProfileUpgrade(context.Background(), shopId, shippingProfileId, upgradeId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.DeleteShopShippingProfileUpgrade``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the shipping profile. | 
**upgradeId** | **int32** | The numeric ID that is associated with a shipping upgrade | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteShopShippingProfileUpgradeRequest struct via the builder pattern


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


## GetShippingCarriers

> ShippingCarriers GetShippingCarriers(ctx).OriginCountryIso(originCountryIso).Execute()





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
    originCountryIso := "originCountryIso_example" // string | The ISO code of the country from which the listing ships.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.GetShippingCarriers(context.Background()).OriginCountryIso(originCountryIso).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.GetShippingCarriers``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShippingCarriers`: ShippingCarriers
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.GetShippingCarriers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetShippingCarriersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **originCountryIso** | **string** | The ISO code of the country from which the listing ships. | 

### Return type

[**ShippingCarriers**](ShippingCarriers.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopShippingProfile

> ShopShippingProfile GetShopShippingProfile(ctx, shopId, shippingProfileId).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.GetShopShippingProfile(context.Background(), shopId, shippingProfileId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.GetShopShippingProfile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopShippingProfile`: ShopShippingProfile
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.GetShopShippingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopShippingProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopShippingProfile**](ShopShippingProfile.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopShippingProfileDestinationsByShippingProfile

> ShopShippingProfileDestinations GetShopShippingProfileDestinationsByShippingProfile(ctx, shopId, shippingProfileId).Limit(limit).Offset(offset).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.GetShopShippingProfileDestinationsByShippingProfile(context.Background(), shopId, shippingProfileId).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.GetShopShippingProfileDestinationsByShippingProfile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopShippingProfileDestinationsByShippingProfile`: ShopShippingProfileDestinations
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.GetShopShippingProfileDestinationsByShippingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopShippingProfileDestinationsByShippingProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**ShopShippingProfileDestinations**](ShopShippingProfileDestinations.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopShippingProfileUpgrades

> ShopShippingProfileUpgrades GetShopShippingProfileUpgrades(ctx, shopId, shippingProfileId).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.GetShopShippingProfileUpgrades(context.Background(), shopId, shippingProfileId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.GetShopShippingProfileUpgrades``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopShippingProfileUpgrades`: ShopShippingProfileUpgrades
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.GetShopShippingProfileUpgrades`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopShippingProfileUpgradesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopShippingProfileUpgrades**](ShopShippingProfileUpgrades.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetShopShippingProfiles

> ShopShippingProfiles GetShopShippingProfiles(ctx, shopId).Execute()





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

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.GetShopShippingProfiles(context.Background(), shopId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.GetShopShippingProfiles``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetShopShippingProfiles`: ShopShippingProfiles
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.GetShopShippingProfiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetShopShippingProfilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ShopShippingProfiles**](ShopShippingProfiles.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateShopShippingProfile

> ShopShippingProfile UpdateShopShippingProfile(ctx, shopId, shippingProfileId).Title(title).OriginCountryIso(originCountryIso).MinProcessingTime(minProcessingTime).MaxProcessingTime(maxProcessingTime).ProcessingTimeUnit(processingTimeUnit).OriginPostalCode(originPostalCode).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    title := "title_example" // string | The name string of this shipping profile. (optional)
    originCountryIso := "originCountryIso_example" // string | The ISO code of the country from which the listing ships. (optional)
    minProcessingTime := int32(56) // int32 | The minimum time required to process to ship listings with this shipping profile. (optional)
    maxProcessingTime := int32(56) // int32 | The maximum processing time the listing needs to ship. (optional)
    processingTimeUnit := "processingTimeUnit_example" // string | The unit used to represent how long a processing time is. A week is equivalent to 5 business days. If none is provided, the unit is set to \\\"business_days\\\". (optional) (default to "business_days")
    originPostalCode := "originPostalCode_example" // string | The postal code string (not necessarily a number) for the location from which the listing ships. Required if the `origin_country_iso` is `US` or `CA`. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.UpdateShopShippingProfile(context.Background(), shopId, shippingProfileId).Title(title).OriginCountryIso(originCountryIso).MinProcessingTime(minProcessingTime).MaxProcessingTime(maxProcessingTime).ProcessingTimeUnit(processingTimeUnit).OriginPostalCode(originPostalCode).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.UpdateShopShippingProfile``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateShopShippingProfile`: ShopShippingProfile
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.UpdateShopShippingProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateShopShippingProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **title** | **string** | The name string of this shipping profile. | 
 **originCountryIso** | **string** | The ISO code of the country from which the listing ships. | 
 **minProcessingTime** | **int32** | The minimum time required to process to ship listings with this shipping profile. | 
 **maxProcessingTime** | **int32** | The maximum processing time the listing needs to ship. | 
 **processingTimeUnit** | **string** | The unit used to represent how long a processing time is. A week is equivalent to 5 business days. If none is provided, the unit is set to \\\&quot;business_days\\\&quot;. | [default to &quot;business_days&quot;]
 **originPostalCode** | **string** | The postal code string (not necessarily a number) for the location from which the listing ships. Required if the &#x60;origin_country_iso&#x60; is &#x60;US&#x60; or &#x60;CA&#x60;. | 

### Return type

[**ShopShippingProfile**](ShopShippingProfile.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateShopShippingProfileDestination

> ShopShippingProfileDestination UpdateShopShippingProfileDestination(ctx, shopId, shippingProfileId, shippingProfileDestinationId).PrimaryCost(primaryCost).SecondaryCost(secondaryCost).DestinationCountryIso(destinationCountryIso).DestinationRegion(destinationRegion).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    shippingProfileDestinationId := int32(56) // int32 | The numeric ID of the shipping profile destination in the [shipping profile](/documentation/reference#tag/Shop-ShippingProfile) associated with the listing.
    primaryCost := float32(3.4) // float32 | The cost of shipping to this country/region alone, measured in the store's default currency. (optional)
    secondaryCost := float32(3.4) // float32 | The cost of shipping to this country/region with another item, measured in the store's default currency. (optional)
    destinationCountryIso := "destinationCountryIso_example" // string | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. (optional)
    destinationRegion := "destinationRegion_example" // string | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If `none`, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. (optional) (default to "none")
    shippingCarrierId := int32(56) // int32 | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with `mail_class`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    mailClass := "mailClass_example" // string | The unique ID string of a shipping carrier's mail class, which is used to calculate an estimated delivery date. **Required with `shipping_carrier_id`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    minDeliveryDays := int32(56) // int32 | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `max_delivery_days`** if `mail_class` is null. (optional)
    maxDeliveryDays := int32(56) // int32 | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `min_delivery_days`** if `mail_class` is null. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.UpdateShopShippingProfileDestination(context.Background(), shopId, shippingProfileId, shippingProfileDestinationId).PrimaryCost(primaryCost).SecondaryCost(secondaryCost).DestinationCountryIso(destinationCountryIso).DestinationRegion(destinationRegion).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.UpdateShopShippingProfileDestination``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateShopShippingProfileDestination`: ShopShippingProfileDestination
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.UpdateShopShippingProfileDestination`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 
**shippingProfileDestinationId** | **int32** | The numeric ID of the shipping profile destination in the [shipping profile](/documentation/reference#tag/Shop-ShippingProfile) associated with the listing. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateShopShippingProfileDestinationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **primaryCost** | **float32** | The cost of shipping to this country/region alone, measured in the store&#39;s default currency. | 
 **secondaryCost** | **float32** | The cost of shipping to this country/region with another item, measured in the store&#39;s default currency. | 
 **destinationCountryIso** | **string** | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. | 
 **destinationRegion** | **string** | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If &#x60;none&#x60;, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. | [default to &quot;none&quot;]
 **shippingCarrierId** | **int32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **mailClass** | **string** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **minDeliveryDays** | **int32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 
 **maxDeliveryDays** | **int32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 

### Return type

[**ShopShippingProfileDestination**](ShopShippingProfileDestination.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateShopShippingProfileUpgrade

> ShopShippingProfileUpgrade UpdateShopShippingProfileUpgrade(ctx, shopId, shippingProfileId, upgradeId).UpgradeName(upgradeName).Type_(type_).Price(price).SecondaryPrice(secondaryPrice).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()





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
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`.
    upgradeId := int32(56) // int32 | The numeric ID that is associated with a shipping upgrade
    upgradeName := "upgradeName_example" // string | Name for the shipping upgrade shown to shoppers at checkout, e.g. USPS Priority. (optional)
    type_ := "type__example" // string | The type of the shipping upgrade. Domestic (0) or international (1). (optional)
    price := float32(3.4) // float32 | Additional cost of adding the shipping upgrade. (optional)
    secondaryPrice := float32(3.4) // float32 | Additional cost of adding the shipping upgrade for each additional item. (optional)
    shippingCarrierId := int32(56) // int32 | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with `mail_class`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    mailClass := "mailClass_example" // string | The unique ID string of a shipping carrier's mail class, which is used to calculate an estimated delivery date. **Required with `shipping_carrier_id`** if `min_delivery_days` and `max_delivery_days` are null. (optional)
    minDeliveryDays := int32(56) // int32 | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `max_delivery_days`** if `mail_class` is null. (optional)
    maxDeliveryDays := int32(56) // int32 | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with `min_delivery_days`** if `mail_class` is null. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopShippingProfileApi.UpdateShopShippingProfileUpgrade(context.Background(), shopId, shippingProfileId, upgradeId).UpgradeName(upgradeName).Type_(type_).Price(price).SecondaryPrice(secondaryPrice).ShippingCarrierId(shippingCarrierId).MailClass(mailClass).MinDeliveryDays(minDeliveryDays).MaxDeliveryDays(maxDeliveryDays).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopShippingProfileApi.UpdateShopShippingProfileUpgrade``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateShopShippingProfileUpgrade`: ShopShippingProfileUpgrade
    fmt.Fprintf(os.Stdout, "Response from `ShopShippingProfileApi.UpdateShopShippingProfileUpgrade`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 
**upgradeId** | **int32** | The numeric ID that is associated with a shipping upgrade | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateShopShippingProfileUpgradeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **upgradeName** | **string** | Name for the shipping upgrade shown to shoppers at checkout, e.g. USPS Priority. | 
 **type_** | **string** | The type of the shipping upgrade. Domestic (0) or international (1). | 
 **price** | **float32** | Additional cost of adding the shipping upgrade. | 
 **secondaryPrice** | **float32** | Additional cost of adding the shipping upgrade for each additional item. | 
 **shippingCarrierId** | **int32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **mailClass** | **string** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | 
 **minDeliveryDays** | **int32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 
 **maxDeliveryDays** | **int32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | 

### Return type

[**ShopShippingProfileUpgrade**](ShopShippingProfileUpgrade.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

