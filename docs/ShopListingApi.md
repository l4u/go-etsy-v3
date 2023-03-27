# \ShopListingApi

All URIs are relative to *https://openapi.etsy.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDraftListing**](ShopListingApi.md#CreateDraftListing) | **Post** /v3/application/shops/{shop_id}/listings | 
[**DeleteListing**](ShopListingApi.md#DeleteListing) | **Delete** /v3/application/listings/{listing_id} | 
[**DeleteListingProperty**](ShopListingApi.md#DeleteListingProperty) | **Delete** /v3/application/shops/{shop_id}/listings/{listing_id}/properties/{property_id} | 
[**FindAllActiveListingsByShop**](ShopListingApi.md#FindAllActiveListingsByShop) | **Get** /v3/application/shops/{shop_id}/listings/active | 
[**FindAllListingsActive**](ShopListingApi.md#FindAllListingsActive) | **Get** /v3/application/listings/active | 
[**GetFeaturedListingsByShop**](ShopListingApi.md#GetFeaturedListingsByShop) | **Get** /v3/application/shops/{shop_id}/listings/featured | 
[**GetListing**](ShopListingApi.md#GetListing) | **Get** /v3/application/listings/{listing_id} | 
[**GetListingProperties**](ShopListingApi.md#GetListingProperties) | **Get** /v3/application/shops/{shop_id}/listings/{listing_id}/properties | 
[**GetListingProperty**](ShopListingApi.md#GetListingProperty) | **Get** /v3/application/listings/{listing_id}/properties/{property_id} | 
[**GetListingsByListingIds**](ShopListingApi.md#GetListingsByListingIds) | **Get** /v3/application/listings/batch | 
[**GetListingsByShop**](ShopListingApi.md#GetListingsByShop) | **Get** /v3/application/shops/{shop_id}/listings | 
[**GetListingsByShopReceipt**](ShopListingApi.md#GetListingsByShopReceipt) | **Get** /v3/application/shops/{shop_id}/receipts/{receipt_id}/listings | 
[**GetListingsByShopReturnPolicy**](ShopListingApi.md#GetListingsByShopReturnPolicy) | **Get** /v3/application/shops/{shop_id}/policies/return/{return_policy_id}/listings | 
[**GetListingsByShopSectionId**](ShopListingApi.md#GetListingsByShopSectionId) | **Get** /v3/application/shops/{shop_id}/shop-sections/listings | 
[**UpdateListing**](ShopListingApi.md#UpdateListing) | **Patch** /v3/application/shops/{shop_id}/listings/{listing_id} | 
[**UpdateListingDeprecated**](ShopListingApi.md#UpdateListingDeprecated) | **Put** /v3/application/shops/{shop_id}/listings/{listing_id} | 
[**UpdateListingProperty**](ShopListingApi.md#UpdateListingProperty) | **Put** /v3/application/shops/{shop_id}/listings/{listing_id}/properties/{property_id} | 



## CreateDraftListing

> ShopListing CreateDraftListing(ctx, shopId).Quantity(quantity).Title(title).Description(description).Price(price).WhoMade(whoMade).WhenMade(whenMade).TaxonomyId(taxonomyId).ShippingProfileId(shippingProfileId).ReturnPolicyId(returnPolicyId).Materials(materials).ShopSectionId(shopSectionId).ProcessingMin(processingMin).ProcessingMax(processingMax).Tags(tags).Styles(styles).ItemWeight(itemWeight).ItemLength(itemLength).ItemWidth(itemWidth).ItemHeight(itemHeight).ItemWeightUnit(itemWeightUnit).ItemDimensionsUnit(itemDimensionsUnit).IsPersonalizable(isPersonalizable).PersonalizationIsRequired(personalizationIsRequired).PersonalizationCharCountMax(personalizationCharCountMax).PersonalizationInstructions(personalizationInstructions).ProductionPartnerIds(productionPartnerIds).ImageIds(imageIds).IsSupply(isSupply).IsCustomizable(isCustomizable).ShouldAutoRenew(shouldAutoRenew).IsTaxable(isTaxable).Type_(type_).Execute()





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
    quantity := int32(56) // int32 | The positive non-zero number of products available for purchase in the listing. Note: The listing quantity is the sum of available offering quantities. You can request the quantities for individual offerings from the ListingInventory resource using the [getListingInventory](/documentation/reference#operation/getListingInventory) endpoint.
    title := "title_example" // string | The listing's title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, & and + characters once each.
    description := "description_example" // string | A description string of the product for sale in the listing.
    price := float32(3.4) // float32 | The positive non-zero price of the product. (Sold product listings are private) Note: The price is the minimum possible price. The [`getListingInventory`](/documentation/reference/#operation/getListingInventory) method requests exact prices for available offerings.
    whoMade := "whoMade_example" // string | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires 'is_supply' and 'when_made'.
    whenMade := "whenMade_example" // string | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires 'is_supply' and 'who_made'.
    taxonomyId := int32(56) // int32 | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information.
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`. (optional)
    returnPolicyId := int32(56) // int32 | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). (optional)
    materials := []string{"Inner_example"} // []string | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. (optional)
    shopSectionId := int32(56) // int32 | The numeric ID of the [shop section](/documentation/reference#tag/Shop-Section) for this listing. Default value is null. (optional)
    processingMin := int32(56) // int32 | The minimum number of days required to process this listing. Default value is null. (optional)
    processingMax := int32(56) // int32 | The maximum number of days required to process this listing. Default value is null. (optional)
    tags := []string{"Inner_example"} // []string | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, ', ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-'™©®]/u) Default value is null. (optional)
    styles := []string{"Inner_example"} // []string | An array of style strings for this listing, each of which is free-form text string such as \\\"Formal\\\", or \\\"Steampunk\\\". When creating or updating a listing, the listing may have up to two styles. Valid style strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. (optional)
    itemWeight := float32(3.4) // float32 | The numeric weight of the product measured in units set in 'item_weight_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemLength := float32(3.4) // float32 | The numeric length of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemWidth := float32(3.4) // float32 | The numeric width of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemHeight := float32(3.4) // float32 | The numeric height of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemWeightUnit := "itemWeightUnit_example" // string | A string defining the units used to measure the weight of the product. Default value is null. (optional)
    itemDimensionsUnit := "itemDimensionsUnit_example" // string | A string defining the units used to measure the dimensions of the product. Default value is null. (optional)
    isPersonalizable := true // bool | When true, this listing is personalizable. The default value is null. (optional)
    personalizationIsRequired := true // bool | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is 'true'. (optional)
    personalizationCharCountMax := int32(56) // int32 | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is 'true'. (optional)
    personalizationInstructions := "personalizationInstructions_example" // string | A string representing instructions for the buyer to enter the personalization. Will only change if is_personalizable is 'true'. (optional)
    productionPartnerIds := []int32{int32(123)} // []int32 | An array of unique IDs of production partner ids. (optional)
    imageIds := []int32{int32(123)} // []int32 | An array of numeric image IDs of the images in a listing, which can include up to 10 images. (optional)
    isSupply := true // bool | When true, tags the listing as a supply product, else indicates that it's a finished product. Helps buyers locate the listing under the Supplies heading. Requires 'who_made' and 'when_made'. (optional)
    isCustomizable := true // bool | When true, a buyer may contact the seller for a customized order. The default value is true when a shop accepts custom orders. Does not apply to shops that do not accept custom orders. (optional)
    shouldAutoRenew := true // bool | When true, renews a listing for four months upon expiration. (optional)
    isTaxable := true // bool | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. (optional)
    type_ := "type__example" // string | An enumerated type string that indicates whether the listing is physical or a digital download. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.CreateDraftListing(context.Background(), shopId).Quantity(quantity).Title(title).Description(description).Price(price).WhoMade(whoMade).WhenMade(whenMade).TaxonomyId(taxonomyId).ShippingProfileId(shippingProfileId).ReturnPolicyId(returnPolicyId).Materials(materials).ShopSectionId(shopSectionId).ProcessingMin(processingMin).ProcessingMax(processingMax).Tags(tags).Styles(styles).ItemWeight(itemWeight).ItemLength(itemLength).ItemWidth(itemWidth).ItemHeight(itemHeight).ItemWeightUnit(itemWeightUnit).ItemDimensionsUnit(itemDimensionsUnit).IsPersonalizable(isPersonalizable).PersonalizationIsRequired(personalizationIsRequired).PersonalizationCharCountMax(personalizationCharCountMax).PersonalizationInstructions(personalizationInstructions).ProductionPartnerIds(productionPartnerIds).ImageIds(imageIds).IsSupply(isSupply).IsCustomizable(isCustomizable).ShouldAutoRenew(shouldAutoRenew).IsTaxable(isTaxable).Type_(type_).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.CreateDraftListing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `CreateDraftListing`: ShopListing
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.CreateDraftListing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateDraftListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **quantity** | **int32** | The positive non-zero number of products available for purchase in the listing. Note: The listing quantity is the sum of available offering quantities. You can request the quantities for individual offerings from the ListingInventory resource using the [getListingInventory](/documentation/reference#operation/getListingInventory) endpoint. | 
 **title** | **string** | The listing&#39;s title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, &amp; and + characters once each. | 
 **description** | **string** | A description string of the product for sale in the listing. | 
 **price** | **float32** | The positive non-zero price of the product. (Sold product listings are private) Note: The price is the minimum possible price. The [&#x60;getListingInventory&#x60;](/documentation/reference/#operation/getListingInventory) method requests exact prices for available offerings. | 
 **whoMade** | **string** | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires &#39;is_supply&#39; and &#39;when_made&#39;. | 
 **whenMade** | **string** | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires &#39;is_supply&#39; and &#39;who_made&#39;. | 
 **taxonomyId** | **int32** | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. | 
 **shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 
 **returnPolicyId** | **int32** | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). | 
 **materials** | **[]string** | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. | 
 **shopSectionId** | **int32** | The numeric ID of the [shop section](/documentation/reference#tag/Shop-Section) for this listing. Default value is null. | 
 **processingMin** | **int32** | The minimum number of days required to process this listing. Default value is null. | 
 **processingMax** | **int32** | The maximum number of days required to process this listing. Default value is null. | 
 **tags** | **[]string** | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, &#39;, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-&#39;™©®]/u) Default value is null. | 
 **styles** | **[]string** | An array of style strings for this listing, each of which is free-form text string such as \\\&quot;Formal\\\&quot;, or \\\&quot;Steampunk\\\&quot;. When creating or updating a listing, the listing may have up to two styles. Valid style strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. | 
 **itemWeight** | **float32** | The numeric weight of the product measured in units set in &#39;item_weight_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemLength** | **float32** | The numeric length of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemWidth** | **float32** | The numeric width of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemHeight** | **float32** | The numeric height of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemWeightUnit** | **string** | A string defining the units used to measure the weight of the product. Default value is null. | 
 **itemDimensionsUnit** | **string** | A string defining the units used to measure the dimensions of the product. Default value is null. | 
 **isPersonalizable** | **bool** | When true, this listing is personalizable. The default value is null. | 
 **personalizationIsRequired** | **bool** | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is &#39;true&#39;. | 
 **personalizationCharCountMax** | **int32** | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is &#39;true&#39;. | 
 **personalizationInstructions** | **string** | A string representing instructions for the buyer to enter the personalization. Will only change if is_personalizable is &#39;true&#39;. | 
 **productionPartnerIds** | **[]int32** | An array of unique IDs of production partner ids. | 
 **imageIds** | **[]int32** | An array of numeric image IDs of the images in a listing, which can include up to 10 images. | 
 **isSupply** | **bool** | When true, tags the listing as a supply product, else indicates that it&#39;s a finished product. Helps buyers locate the listing under the Supplies heading. Requires &#39;who_made&#39; and &#39;when_made&#39;. | 
 **isCustomizable** | **bool** | When true, a buyer may contact the seller for a customized order. The default value is true when a shop accepts custom orders. Does not apply to shops that do not accept custom orders. | 
 **shouldAutoRenew** | **bool** | When true, renews a listing for four months upon expiration. | 
 **isTaxable** | **bool** | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. | 
 **type_** | **string** | An enumerated type string that indicates whether the listing is physical or a digital download. | 

### Return type

[**ShopListing**](ShopListing.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteListing

> DeleteListing(ctx, listingId).Execute()





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

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopListingApi.DeleteListing(context.Background(), listingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.DeleteListing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteListingRequest struct via the builder pattern


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


## DeleteListingProperty

> DeleteListingProperty(ctx, shopId, listingId, propertyId).Execute()





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
    propertyId := int32(56) // int32 | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties).

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    r, err := apiClient.ShopListingApi.DeleteListingProperty(context.Background(), shopId, listingId, propertyId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.DeleteListingProperty``: %v\n", err)
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
**propertyId** | **int32** | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties). | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteListingPropertyRequest struct via the builder pattern


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


## FindAllActiveListingsByShop

> ShopListings FindAllActiveListingsByShop(ctx, shopId).Limit(limit).SortOn(sortOn).SortOrder(sortOrder).Offset(offset).Keywords(keywords).Execute()





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
    sortOn := "sortOn_example" // string | The value to sort a search result of listings on. NOTES: a) `sort_on` only works when combined with one of the search options (keywords, region, etc.). b) when using `score` the returned results will always be in _descending_ order, regardless of the `sort_order` parameter. (optional) (default to "created")
    sortOrder := "sortOrder_example" // string | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). (optional) (default to "desc")
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)
    keywords := "keywords_example" // string | Search term or phrase that must appear in all results. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.FindAllActiveListingsByShop(context.Background(), shopId).Limit(limit).SortOn(sortOn).SortOrder(sortOrder).Offset(offset).Keywords(keywords).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.FindAllActiveListingsByShop``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `FindAllActiveListingsByShop`: ShopListings
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.FindAllActiveListingsByShop`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiFindAllActiveListingsByShopRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **sortOn** | **string** | The value to sort a search result of listings on. NOTES: a) &#x60;sort_on&#x60; only works when combined with one of the search options (keywords, region, etc.). b) when using &#x60;score&#x60; the returned results will always be in _descending_ order, regardless of the &#x60;sort_order&#x60; parameter. | [default to &quot;created&quot;]
 **sortOrder** | **string** | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). | [default to &quot;desc&quot;]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]
 **keywords** | **string** | Search term or phrase that must appear in all results. | 

### Return type

[**ShopListings**](ShopListings.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FindAllListingsActive

> ShopListings FindAllListingsActive(ctx).Limit(limit).Offset(offset).Keywords(keywords).SortOn(sortOn).SortOrder(sortOrder).MinPrice(minPrice).MaxPrice(maxPrice).TaxonomyId(taxonomyId).ShopLocation(shopLocation).Execute()





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
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)
    keywords := "keywords_example" // string | Search term or phrase that must appear in all results. (optional)
    sortOn := "sortOn_example" // string | The value to sort a search result of listings on. NOTES: a) `sort_on` only works when combined with one of the search options (keywords, region, etc.). b) when using `score` the returned results will always be in _descending_ order, regardless of the `sort_order` parameter. (optional) (default to "created")
    sortOrder := "sortOrder_example" // string | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). (optional) (default to "desc")
    minPrice := float32(3.4) // float32 | The minimum price of listings to be returned by a search result. (optional)
    maxPrice := float32(3.4) // float32 | The maximum price of listings to be returned by a search result. (optional)
    taxonomyId := int32(56) // int32 | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. (optional)
    shopLocation := "shopLocation_example" // string | Filters by shop location. If location cannot be parsed, Etsy responds with an error. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.FindAllListingsActive(context.Background()).Limit(limit).Offset(offset).Keywords(keywords).SortOn(sortOn).SortOrder(sortOrder).MinPrice(minPrice).MaxPrice(maxPrice).TaxonomyId(taxonomyId).ShopLocation(shopLocation).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.FindAllListingsActive``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `FindAllListingsActive`: ShopListings
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.FindAllListingsActive`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFindAllListingsActiveRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]
 **keywords** | **string** | Search term or phrase that must appear in all results. | 
 **sortOn** | **string** | The value to sort a search result of listings on. NOTES: a) &#x60;sort_on&#x60; only works when combined with one of the search options (keywords, region, etc.). b) when using &#x60;score&#x60; the returned results will always be in _descending_ order, regardless of the &#x60;sort_order&#x60; parameter. | [default to &quot;created&quot;]
 **sortOrder** | **string** | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). | [default to &quot;desc&quot;]
 **minPrice** | **float32** | The minimum price of listings to be returned by a search result. | 
 **maxPrice** | **float32** | The maximum price of listings to be returned by a search result. | 
 **taxonomyId** | **int32** | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. | 
 **shopLocation** | **string** | Filters by shop location. If location cannot be parsed, Etsy responds with an error. | 

### Return type

[**ShopListings**](ShopListings.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetFeaturedListingsByShop

> ShopListings GetFeaturedListingsByShop(ctx, shopId).Limit(limit).Offset(offset).Execute()





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
    resp, r, err := apiClient.ShopListingApi.GetFeaturedListingsByShop(context.Background(), shopId).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetFeaturedListingsByShop``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetFeaturedListingsByShop`: ShopListings
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetFeaturedListingsByShop`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetFeaturedListingsByShopRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**ShopListings**](ShopListings.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListing

> ShopListingWithAssociations GetListing(ctx, listingId).Includes(includes).Language(language).Execute()





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
    includes := []string{"Includes_example"} // []string | An enumerated string that attaches a valid association. Acceptable inputs are 'Shipping', 'Shop', 'Images', 'User', 'Translations' and 'Inventory'. (optional)
    language := "language_example" // string | The IETF language tag for the language of this translation. Ex: `de`, `en`, `es`, `fr`, `it`, `ja`, `nl`, `pl`, `pt`. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListing(context.Background(), listingId).Includes(includes).Language(language).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListing`: ShopListingWithAssociations
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **includes** | **[]string** | An enumerated string that attaches a valid association. Acceptable inputs are &#39;Shipping&#39;, &#39;Shop&#39;, &#39;Images&#39;, &#39;User&#39;, &#39;Translations&#39; and &#39;Inventory&#39;. | 
 **language** | **string** | The IETF language tag for the language of this translation. Ex: &#x60;de&#x60;, &#x60;en&#x60;, &#x60;es&#x60;, &#x60;fr&#x60;, &#x60;it&#x60;, &#x60;ja&#x60;, &#x60;nl&#x60;, &#x60;pl&#x60;, &#x60;pt&#x60;. | 

### Return type

[**ShopListingWithAssociations**](ShopListingWithAssociations.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingProperties

> ListingPropertyValues GetListingProperties(ctx, shopId, listingId).Execute()





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

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingProperties(context.Background(), shopId, listingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingProperties``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingProperties`: ListingPropertyValues
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingProperties`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingPropertiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListingPropertyValues**](ListingPropertyValues.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingProperty

> ListingPropertyValue GetListingProperty(ctx, listingId, propertyId).Execute()





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
    propertyId := int32(56) // int32 | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties).

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingProperty(context.Background(), listingId, propertyId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingProperty``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingProperty`: ListingPropertyValue
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingProperty`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**propertyId** | **int32** | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties). | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingPropertyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListingPropertyValue**](ListingPropertyValue.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingsByListingIds

> ShopListingsWithAssociations GetListingsByListingIds(ctx).ListingIds(listingIds).Includes(includes).Execute()





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
    listingIds := []int32{int32(123)} // []int32 | The list of numeric IDS for the listings in a specific Etsy shop.
    includes := []string{"Includes_example"} // []string | An enumerated string that attaches a valid association. Acceptable inputs are 'Shipping', 'Shop', 'Images', 'User', 'Translations' and 'Inventory'. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingsByListingIds(context.Background()).ListingIds(listingIds).Includes(includes).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingsByListingIds``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingsByListingIds`: ShopListingsWithAssociations
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingsByListingIds`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetListingsByListingIdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **listingIds** | **[]int32** | The list of numeric IDS for the listings in a specific Etsy shop. | 
 **includes** | **[]string** | An enumerated string that attaches a valid association. Acceptable inputs are &#39;Shipping&#39;, &#39;Shop&#39;, &#39;Images&#39;, &#39;User&#39;, &#39;Translations&#39; and &#39;Inventory&#39;. | 

### Return type

[**ShopListingsWithAssociations**](ShopListingsWithAssociations.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingsByShop

> ShopListingsWithAssociations GetListingsByShop(ctx, shopId).State(state).Limit(limit).Offset(offset).SortOn(sortOn).SortOrder(sortOrder).Includes(includes).Execute()





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
    state := "state_example" // string | When _updating_ a listing, this value can be either `active` or `inactive`. Note: Setting a `draft` listing to `active` will also publish the listing on etsy.com and requires that the listing have an image set. Setting a `sold_out` listing to active will update the quantity to 1 and renew the listing on etsy.com. (optional) (default to "active")
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)
    sortOn := "sortOn_example" // string | The value to sort a search result of listings on. NOTES: a) `sort_on` only works when combined with one of the search options (keywords, region, etc.). b) when using `score` the returned results will always be in _descending_ order, regardless of the `sort_order` parameter. (optional) (default to "created")
    sortOrder := "sortOrder_example" // string | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). (optional) (default to "desc")
    includes := []string{"Includes_example"} // []string | An enumerated string that attaches a valid association. Acceptable inputs are 'Shipping', 'Shop', 'Images', 'User', 'Translations' and 'Inventory'. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingsByShop(context.Background(), shopId).State(state).Limit(limit).Offset(offset).SortOn(sortOn).SortOrder(sortOrder).Includes(includes).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingsByShop``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingsByShop`: ShopListingsWithAssociations
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingsByShop`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingsByShopRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **state** | **string** | When _updating_ a listing, this value can be either &#x60;active&#x60; or &#x60;inactive&#x60;. Note: Setting a &#x60;draft&#x60; listing to &#x60;active&#x60; will also publish the listing on etsy.com and requires that the listing have an image set. Setting a &#x60;sold_out&#x60; listing to active will update the quantity to 1 and renew the listing on etsy.com. | [default to &quot;active&quot;]
 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]
 **sortOn** | **string** | The value to sort a search result of listings on. NOTES: a) &#x60;sort_on&#x60; only works when combined with one of the search options (keywords, region, etc.). b) when using &#x60;score&#x60; the returned results will always be in _descending_ order, regardless of the &#x60;sort_order&#x60; parameter. | [default to &quot;created&quot;]
 **sortOrder** | **string** | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). | [default to &quot;desc&quot;]
 **includes** | **[]string** | An enumerated string that attaches a valid association. Acceptable inputs are &#39;Shipping&#39;, &#39;Shop&#39;, &#39;Images&#39;, &#39;User&#39;, &#39;Translations&#39; and &#39;Inventory&#39;. | 

### Return type

[**ShopListingsWithAssociations**](ShopListingsWithAssociations.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingsByShopReceipt

> ShopListings GetListingsByShopReceipt(ctx, receiptId, shopId).Limit(limit).Offset(offset).Execute()





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
    receiptId := int32(56) // int32 | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction.
    shopId := int32(56) // int32 | The unique positive non-zero numeric ID for an Etsy Shop.
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingsByShopReceipt(context.Background(), receiptId, shopId).Limit(limit).Offset(offset).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingsByShopReceipt``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingsByShopReceipt`: ShopListings
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingsByShopReceipt`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptId** | **int32** | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction. | 
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingsByShopReceiptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]

### Return type

[**ShopListings**](ShopListings.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingsByShopReturnPolicy

> ShopListings GetListingsByShopReturnPolicy(ctx, returnPolicyId, shopId).Execute()





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
    returnPolicyId := int32(56) // int32 | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies).
    shopId := int32(56) // int32 | The unique positive non-zero numeric ID for an Etsy Shop.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingsByShopReturnPolicy(context.Background(), returnPolicyId, shopId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingsByShopReturnPolicy``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingsByShopReturnPolicy`: ShopListings
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingsByShopReturnPolicy`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**returnPolicyId** | **int32** | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). | 
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingsByShopReturnPolicyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ShopListings**](ShopListings.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListingsByShopSectionId

> ShopListings GetListingsByShopSectionId(ctx, shopId).ShopSectionIds(shopSectionIds).Limit(limit).Offset(offset).SortOn(sortOn).SortOrder(sortOrder).Execute()





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
    shopSectionIds := []int32{int32(123)} // []int32 | A list of numeric IDS for all sections in a specific Etsy shop.
    limit := int32(56) // int32 | The maximum number of results to return. (optional) (default to 25)
    offset := int32(56) // int32 | The number of records to skip before selecting the first result. (optional) (default to 0)
    sortOn := "sortOn_example" // string | The value to sort a search result of listings on. NOTES: a) `sort_on` only works when combined with one of the search options (keywords, region, etc.). b) when using `score` the returned results will always be in _descending_ order, regardless of the `sort_order` parameter. (optional) (default to "created")
    sortOrder := "sortOrder_example" // string | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). (optional) (default to "desc")

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.GetListingsByShopSectionId(context.Background(), shopId).ShopSectionIds(shopSectionIds).Limit(limit).Offset(offset).SortOn(sortOn).SortOrder(sortOrder).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.GetListingsByShopSectionId``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetListingsByShopSectionId`: ShopListings
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.GetListingsByShopSectionId`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListingsByShopSectionIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **shopSectionIds** | **[]int32** | A list of numeric IDS for all sections in a specific Etsy shop. | 
 **limit** | **int32** | The maximum number of results to return. | [default to 25]
 **offset** | **int32** | The number of records to skip before selecting the first result. | [default to 0]
 **sortOn** | **string** | The value to sort a search result of listings on. NOTES: a) &#x60;sort_on&#x60; only works when combined with one of the search options (keywords, region, etc.). b) when using &#x60;score&#x60; the returned results will always be in _descending_ order, regardless of the &#x60;sort_order&#x60; parameter. | [default to &quot;created&quot;]
 **sortOrder** | **string** | The ascending(up) or descending(down) order to sort listings by. NOTE: sort_order only works when combined with one of the search options (keywords, region, etc.). | [default to &quot;desc&quot;]

### Return type

[**ShopListings**](ShopListings.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateListing

> ShopListing UpdateListing(ctx, shopId, listingId).ImageIds(imageIds).Title(title).Description(description).Materials(materials).ShouldAutoRenew(shouldAutoRenew).ShippingProfileId(shippingProfileId).ReturnPolicyId(returnPolicyId).ShopSectionId(shopSectionId).ItemWeight(itemWeight).ItemLength(itemLength).ItemWidth(itemWidth).ItemHeight(itemHeight).ItemWeightUnit(itemWeightUnit).ItemDimensionsUnit(itemDimensionsUnit).IsTaxable(isTaxable).TaxonomyId(taxonomyId).Tags(tags).WhoMade(whoMade).WhenMade(whenMade).FeaturedRank(featuredRank).IsPersonalizable(isPersonalizable).PersonalizationIsRequired(personalizationIsRequired).PersonalizationCharCountMax(personalizationCharCountMax).PersonalizationInstructions(personalizationInstructions).State(state).IsSupply(isSupply).ProductionPartnerIds(productionPartnerIds).Type_(type_).Execute()





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
    imageIds := []int32{int32(123)} // []int32 | An array of numeric image IDs of the images in a listing, which can include up to 10 images. (optional)
    title := "title_example" // string | The listing's title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, & and + characters once each. (optional)
    description := "description_example" // string | A description string of the product for sale in the listing. (optional)
    materials := []string{"Inner_example"} // []string | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. (optional)
    shouldAutoRenew := true // bool | When true, renews a listing for four months upon expiration. (optional)
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`. (optional)
    returnPolicyId := int32(56) // int32 | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). Required for active physical listings. This requirement does not apply to listings of EU-based shops. (optional)
    shopSectionId := int32(56) // int32 | The numeric ID of the [shop section](/documentation/reference#tag/Shop-Section) for this listing. Default value is null. (optional)
    itemWeight := float32(3.4) // float32 | The numeric weight of the product measured in units set in 'item_weight_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemLength := float32(3.4) // float32 | The numeric length of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemWidth := float32(3.4) // float32 | The numeric width of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemHeight := float32(3.4) // float32 | The numeric height of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemWeightUnit := "itemWeightUnit_example" // string | A string defining the units used to measure the weight of the product. Default value is null. (optional)
    itemDimensionsUnit := "itemDimensionsUnit_example" // string | A string defining the units used to measure the dimensions of the product. Default value is null. (optional)
    isTaxable := true // bool | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. (optional)
    taxonomyId := int32(56) // int32 | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. (optional)
    tags := []string{"Inner_example"} // []string | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, ', ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-'™©®]/u) Default value is null. (optional)
    whoMade := "whoMade_example" // string | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires 'is_supply' and 'when_made'. (optional)
    whenMade := "whenMade_example" // string | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires 'is_supply' and 'who_made'. (optional)
    featuredRank := int32(56) // int32 | The positive non-zero numeric position in the featured listings of the shop, with rank 1 listings appearing in the left-most position in featured listing on a shop’s home page. (optional)
    isPersonalizable := true // bool | When true, this listing is personalizable. The default value is null. (optional)
    personalizationIsRequired := true // bool | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is 'true'. (optional)
    personalizationCharCountMax := int32(56) // int32 | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is 'true'. (optional)
    personalizationInstructions := "personalizationInstructions_example" // string | A string representing instructions for the buyer to enter the personalization. Will only change if is_personalizable is 'true'. (optional)
    state := "state_example" // string | When _updating_ a listing, this value can be either `active` or `inactive`. Note: Setting a `draft` listing to `active` will also publish the listing on etsy.com and requires that the listing have an image set. Setting a `sold_out` listing to active will update the quantity to 1 and renew the listing on etsy.com. (optional)
    isSupply := true // bool | When true, tags the listing as a supply product, else indicates that it's a finished product. Helps buyers locate the listing under the Supplies heading. Requires 'who_made' and 'when_made'. (optional)
    productionPartnerIds := []int32{int32(123)} // []int32 | An array of unique IDs of production partner ids. (optional)
    type_ := "type__example" // string | An enumerated type string that indicates whether the listing is physical or a digital download. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.UpdateListing(context.Background(), shopId, listingId).ImageIds(imageIds).Title(title).Description(description).Materials(materials).ShouldAutoRenew(shouldAutoRenew).ShippingProfileId(shippingProfileId).ReturnPolicyId(returnPolicyId).ShopSectionId(shopSectionId).ItemWeight(itemWeight).ItemLength(itemLength).ItemWidth(itemWidth).ItemHeight(itemHeight).ItemWeightUnit(itemWeightUnit).ItemDimensionsUnit(itemDimensionsUnit).IsTaxable(isTaxable).TaxonomyId(taxonomyId).Tags(tags).WhoMade(whoMade).WhenMade(whenMade).FeaturedRank(featuredRank).IsPersonalizable(isPersonalizable).PersonalizationIsRequired(personalizationIsRequired).PersonalizationCharCountMax(personalizationCharCountMax).PersonalizationInstructions(personalizationInstructions).State(state).IsSupply(isSupply).ProductionPartnerIds(productionPartnerIds).Type_(type_).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.UpdateListing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateListing`: ShopListing
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.UpdateListing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **imageIds** | **[]int32** | An array of numeric image IDs of the images in a listing, which can include up to 10 images. | 
 **title** | **string** | The listing&#39;s title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, &amp; and + characters once each. | 
 **description** | **string** | A description string of the product for sale in the listing. | 
 **materials** | **[]string** | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. | 
 **shouldAutoRenew** | **bool** | When true, renews a listing for four months upon expiration. | 
 **shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 
 **returnPolicyId** | **int32** | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). Required for active physical listings. This requirement does not apply to listings of EU-based shops. | 
 **shopSectionId** | **int32** | The numeric ID of the [shop section](/documentation/reference#tag/Shop-Section) for this listing. Default value is null. | 
 **itemWeight** | **float32** | The numeric weight of the product measured in units set in &#39;item_weight_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemLength** | **float32** | The numeric length of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemWidth** | **float32** | The numeric width of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemHeight** | **float32** | The numeric height of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemWeightUnit** | **string** | A string defining the units used to measure the weight of the product. Default value is null. | 
 **itemDimensionsUnit** | **string** | A string defining the units used to measure the dimensions of the product. Default value is null. | 
 **isTaxable** | **bool** | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. | 
 **taxonomyId** | **int32** | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. | 
 **tags** | **[]string** | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, &#39;, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-&#39;™©®]/u) Default value is null. | 
 **whoMade** | **string** | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires &#39;is_supply&#39; and &#39;when_made&#39;. | 
 **whenMade** | **string** | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires &#39;is_supply&#39; and &#39;who_made&#39;. | 
 **featuredRank** | **int32** | The positive non-zero numeric position in the featured listings of the shop, with rank 1 listings appearing in the left-most position in featured listing on a shop’s home page. | 
 **isPersonalizable** | **bool** | When true, this listing is personalizable. The default value is null. | 
 **personalizationIsRequired** | **bool** | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is &#39;true&#39;. | 
 **personalizationCharCountMax** | **int32** | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is &#39;true&#39;. | 
 **personalizationInstructions** | **string** | A string representing instructions for the buyer to enter the personalization. Will only change if is_personalizable is &#39;true&#39;. | 
 **state** | **string** | When _updating_ a listing, this value can be either &#x60;active&#x60; or &#x60;inactive&#x60;. Note: Setting a &#x60;draft&#x60; listing to &#x60;active&#x60; will also publish the listing on etsy.com and requires that the listing have an image set. Setting a &#x60;sold_out&#x60; listing to active will update the quantity to 1 and renew the listing on etsy.com. | 
 **isSupply** | **bool** | When true, tags the listing as a supply product, else indicates that it&#39;s a finished product. Helps buyers locate the listing under the Supplies heading. Requires &#39;who_made&#39; and &#39;when_made&#39;. | 
 **productionPartnerIds** | **[]int32** | An array of unique IDs of production partner ids. | 
 **type_** | **string** | An enumerated type string that indicates whether the listing is physical or a digital download. | 

### Return type

[**ShopListing**](ShopListing.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateListingDeprecated

> ShopListing UpdateListingDeprecated(ctx, shopId, listingId).ImageIds(imageIds).Title(title).Description(description).Materials(materials).ShouldAutoRenew(shouldAutoRenew).ShippingProfileId(shippingProfileId).ShopSectionId(shopSectionId).ItemWeight(itemWeight).ItemLength(itemLength).ItemWidth(itemWidth).ItemHeight(itemHeight).ItemWeightUnit(itemWeightUnit).ItemDimensionsUnit(itemDimensionsUnit).IsTaxable(isTaxable).TaxonomyId(taxonomyId).Tags(tags).WhoMade(whoMade).WhenMade(whenMade).FeaturedRank(featuredRank).IsPersonalizable(isPersonalizable).PersonalizationIsRequired(personalizationIsRequired).PersonalizationCharCountMax(personalizationCharCountMax).PersonalizationInstructions(personalizationInstructions).State(state).IsSupply(isSupply).ProductionPartnerIds(productionPartnerIds).Type_(type_).Execute()





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
    imageIds := []int32{int32(123)} // []int32 | An array of numeric image IDs of the images in a listing, which can include up to 10 images. (optional)
    title := "title_example" // string | The listing's title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, & and + characters once each. (optional)
    description := "description_example" // string | A description string of the product for sale in the listing. (optional)
    materials := []string{"Inner_example"} // []string | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. (optional)
    shouldAutoRenew := true // bool | When true, renews a listing for four months upon expiration. (optional)
    shippingProfileId := int32(56) // int32 | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is `physical`. (optional)
    shopSectionId := int32(56) // int32 | The numeric ID of the [shop section](/documentation/reference#tag/Shop-Section) for this listing. Default value is null. (optional)
    itemWeight := float32(3.4) // float32 | The numeric weight of the product measured in units set in 'item_weight_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemLength := float32(3.4) // float32 | The numeric length of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemWidth := float32(3.4) // float32 | The numeric width of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemHeight := float32(3.4) // float32 | The numeric height of the product measured in units set in 'item_dimensions_unit'. Default value is null. If set, the value must be greater than 0. (optional)
    itemWeightUnit := "itemWeightUnit_example" // string | A string defining the units used to measure the weight of the product. Default value is null. (optional)
    itemDimensionsUnit := "itemDimensionsUnit_example" // string | A string defining the units used to measure the dimensions of the product. Default value is null. (optional)
    isTaxable := true // bool | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. (optional)
    taxonomyId := int32(56) // int32 | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. (optional)
    tags := []string{"Inner_example"} // []string | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, ', ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-'™©®]/u) Default value is null. (optional)
    whoMade := "whoMade_example" // string | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires 'is_supply' and 'when_made'. (optional)
    whenMade := "whenMade_example" // string | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires 'is_supply' and 'who_made'. (optional)
    featuredRank := int32(56) // int32 | The positive non-zero numeric position in the featured listings of the shop, with rank 1 listings appearing in the left-most position in featured listing on a shop’s home page. (optional)
    isPersonalizable := true // bool | When true, this listing is personalizable. The default value is null. (optional)
    personalizationIsRequired := true // bool | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is 'true'. (optional)
    personalizationCharCountMax := int32(56) // int32 | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is 'true'. (optional)
    personalizationInstructions := "personalizationInstructions_example" // string | A string representing instructions for the buyer to enter the personalization. Will only change if is_personalizable is 'true'. (optional)
    state := "state_example" // string | When _updating_ a listing, this value can be either `active` or `inactive`. Note: Setting a `draft` listing to `active` will also publish the listing on etsy.com and requires that the listing have an image set. Setting a `sold_out` listing to active will update the quantity to 1 and renew the listing on etsy.com. (optional)
    isSupply := true // bool | When true, tags the listing as a supply product, else indicates that it's a finished product. Helps buyers locate the listing under the Supplies heading. Requires 'who_made' and 'when_made'. (optional)
    productionPartnerIds := []int32{int32(123)} // []int32 | An array of unique IDs of production partner ids. (optional)
    type_ := "type__example" // string | An enumerated type string that indicates whether the listing is physical or a digital download. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.UpdateListingDeprecated(context.Background(), shopId, listingId).ImageIds(imageIds).Title(title).Description(description).Materials(materials).ShouldAutoRenew(shouldAutoRenew).ShippingProfileId(shippingProfileId).ShopSectionId(shopSectionId).ItemWeight(itemWeight).ItemLength(itemLength).ItemWidth(itemWidth).ItemHeight(itemHeight).ItemWeightUnit(itemWeightUnit).ItemDimensionsUnit(itemDimensionsUnit).IsTaxable(isTaxable).TaxonomyId(taxonomyId).Tags(tags).WhoMade(whoMade).WhenMade(whenMade).FeaturedRank(featuredRank).IsPersonalizable(isPersonalizable).PersonalizationIsRequired(personalizationIsRequired).PersonalizationCharCountMax(personalizationCharCountMax).PersonalizationInstructions(personalizationInstructions).State(state).IsSupply(isSupply).ProductionPartnerIds(productionPartnerIds).Type_(type_).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.UpdateListingDeprecated``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateListingDeprecated`: ShopListing
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.UpdateListingDeprecated`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateListingDeprecatedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **imageIds** | **[]int32** | An array of numeric image IDs of the images in a listing, which can include up to 10 images. | 
 **title** | **string** | The listing&#39;s title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, &amp; and + characters once each. | 
 **description** | **string** | A description string of the product for sale in the listing. | 
 **materials** | **[]string** | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. | 
 **shouldAutoRenew** | **bool** | When true, renews a listing for four months upon expiration. | 
 **shippingProfileId** | **int32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | 
 **shopSectionId** | **int32** | The numeric ID of the [shop section](/documentation/reference#tag/Shop-Section) for this listing. Default value is null. | 
 **itemWeight** | **float32** | The numeric weight of the product measured in units set in &#39;item_weight_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemLength** | **float32** | The numeric length of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemWidth** | **float32** | The numeric width of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemHeight** | **float32** | The numeric height of the product measured in units set in &#39;item_dimensions_unit&#39;. Default value is null. If set, the value must be greater than 0. | 
 **itemWeightUnit** | **string** | A string defining the units used to measure the weight of the product. Default value is null. | 
 **itemDimensionsUnit** | **string** | A string defining the units used to measure the dimensions of the product. Default value is null. | 
 **isTaxable** | **bool** | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. | 
 **taxonomyId** | **int32** | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. | 
 **tags** | **[]string** | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, &#39;, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-&#39;™©®]/u) Default value is null. | 
 **whoMade** | **string** | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires &#39;is_supply&#39; and &#39;when_made&#39;. | 
 **whenMade** | **string** | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires &#39;is_supply&#39; and &#39;who_made&#39;. | 
 **featuredRank** | **int32** | The positive non-zero numeric position in the featured listings of the shop, with rank 1 listings appearing in the left-most position in featured listing on a shop’s home page. | 
 **isPersonalizable** | **bool** | When true, this listing is personalizable. The default value is null. | 
 **personalizationIsRequired** | **bool** | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is &#39;true&#39;. | 
 **personalizationCharCountMax** | **int32** | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is &#39;true&#39;. | 
 **personalizationInstructions** | **string** | A string representing instructions for the buyer to enter the personalization. Will only change if is_personalizable is &#39;true&#39;. | 
 **state** | **string** | When _updating_ a listing, this value can be either &#x60;active&#x60; or &#x60;inactive&#x60;. Note: Setting a &#x60;draft&#x60; listing to &#x60;active&#x60; will also publish the listing on etsy.com and requires that the listing have an image set. Setting a &#x60;sold_out&#x60; listing to active will update the quantity to 1 and renew the listing on etsy.com. | 
 **isSupply** | **bool** | When true, tags the listing as a supply product, else indicates that it&#39;s a finished product. Helps buyers locate the listing under the Supplies heading. Requires &#39;who_made&#39; and &#39;when_made&#39;. | 
 **productionPartnerIds** | **[]int32** | An array of unique IDs of production partner ids. | 
 **type_** | **string** | An enumerated type string that indicates whether the listing is physical or a digital download. | 

### Return type

[**ShopListing**](ShopListing.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateListingProperty

> ListingPropertyValue UpdateListingProperty(ctx, shopId, listingId, propertyId).ValueIds(valueIds).Values(values).ScaleId(scaleId).Execute()





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
    propertyId := int32(56) // int32 | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties).
    valueIds := []int32{int32(123)} // []int32 | An array of unique IDs of multiple Etsy [listing property](/documentation/reference#operation/getListingProperties) values. For example, if your listing offers different sizes of a product, then the value ID list contains value IDs for each size.
    values := []string{"Inner_example"} // []string | An array of value strings for multiple Etsy [listing property](/documentation/reference#operation/getListingProperties) values. For example, if your listing offers different colored products, then the values array contains the color strings for each color. Note: parenthesis characters (`(` and `)`) are not allowed.
    scaleId := int32(56) // int32 | The numeric ID of a single Etsy.com measurement scale. For example, for shoe size, there are three `scale_id`s available - `UK`, `US/Canada`, and `EU`, where `US/Canada` has `scale_id` 19. (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.ShopListingApi.UpdateListingProperty(context.Background(), shopId, listingId, propertyId).ValueIds(valueIds).Values(values).ScaleId(scaleId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `ShopListingApi.UpdateListingProperty``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateListingProperty`: ListingPropertyValue
    fmt.Fprintf(os.Stdout, "Response from `ShopListingApi.UpdateListingProperty`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopId** | **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | 
**listingId** | **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | 
**propertyId** | **int32** | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties). | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateListingPropertyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **valueIds** | **[]int32** | An array of unique IDs of multiple Etsy [listing property](/documentation/reference#operation/getListingProperties) values. For example, if your listing offers different sizes of a product, then the value ID list contains value IDs for each size. | 
 **values** | **[]string** | An array of value strings for multiple Etsy [listing property](/documentation/reference#operation/getListingProperties) values. For example, if your listing offers different colored products, then the values array contains the color strings for each color. Note: parenthesis characters (&#x60;(&#x60; and &#x60;)&#x60;) are not allowed. | 
 **scaleId** | **int32** | The numeric ID of a single Etsy.com measurement scale. For example, for shoe size, there are three &#x60;scale_id&#x60;s available - &#x60;UK&#x60;, &#x60;US/Canada&#x60;, and &#x60;EU&#x60;, where &#x60;US/Canada&#x60; has &#x60;scale_id&#x60; 19. | 

### Return type

[**ListingPropertyValue**](ListingPropertyValue.md)

### Authorization

[api_key](../README.md#api_key), [oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

