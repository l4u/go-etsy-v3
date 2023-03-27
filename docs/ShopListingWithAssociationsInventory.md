# ShopListingWithAssociationsInventory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Products** | Pointer to [**[]ListingInventoryProductsInner**](ListingInventoryProductsInner.md) | A JSON array of products available in a listing, even if only one product. All field names in the JSON blobs are lowercase. | [optional] 
**PriceOnProperty** | Pointer to **[]int32** | An array of unique [listing property](/documentation/reference#operation/getListingProperties) ID integers for the properties that change product prices, if any. For example, if you charge specific prices for different sized products in the same listing, then this array contains the property ID for size. | [optional] 
**QuantityOnProperty** | Pointer to **[]int32** | An array of unique [listing property](/documentation/reference#operation/getListingProperties) ID integers for the properties that change the quantity of the products, if any. For example, if you stock specific quantities of different colored products in the same listing, then this array contains the property ID for color. | [optional] 
**SkuOnProperty** | Pointer to **[]int32** | An array of unique [listing property](/documentation/reference#operation/getListingProperties) ID integers for the properties that change the product SKU, if any. For example, if you use specific skus for different colored products in the same listing, then this array contains the property ID for color. | [optional] 

## Methods

### NewShopListingWithAssociationsInventory

`func NewShopListingWithAssociationsInventory() *ShopListingWithAssociationsInventory`

NewShopListingWithAssociationsInventory instantiates a new ShopListingWithAssociationsInventory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingWithAssociationsInventoryWithDefaults

`func NewShopListingWithAssociationsInventoryWithDefaults() *ShopListingWithAssociationsInventory`

NewShopListingWithAssociationsInventoryWithDefaults instantiates a new ShopListingWithAssociationsInventory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProducts

`func (o *ShopListingWithAssociationsInventory) GetProducts() []ListingInventoryProductsInner`

GetProducts returns the Products field if non-nil, zero value otherwise.

### GetProductsOk

`func (o *ShopListingWithAssociationsInventory) GetProductsOk() (*[]ListingInventoryProductsInner, bool)`

GetProductsOk returns a tuple with the Products field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProducts

`func (o *ShopListingWithAssociationsInventory) SetProducts(v []ListingInventoryProductsInner)`

SetProducts sets Products field to given value.

### HasProducts

`func (o *ShopListingWithAssociationsInventory) HasProducts() bool`

HasProducts returns a boolean if a field has been set.

### GetPriceOnProperty

`func (o *ShopListingWithAssociationsInventory) GetPriceOnProperty() []int32`

GetPriceOnProperty returns the PriceOnProperty field if non-nil, zero value otherwise.

### GetPriceOnPropertyOk

`func (o *ShopListingWithAssociationsInventory) GetPriceOnPropertyOk() (*[]int32, bool)`

GetPriceOnPropertyOk returns a tuple with the PriceOnProperty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceOnProperty

`func (o *ShopListingWithAssociationsInventory) SetPriceOnProperty(v []int32)`

SetPriceOnProperty sets PriceOnProperty field to given value.

### HasPriceOnProperty

`func (o *ShopListingWithAssociationsInventory) HasPriceOnProperty() bool`

HasPriceOnProperty returns a boolean if a field has been set.

### GetQuantityOnProperty

`func (o *ShopListingWithAssociationsInventory) GetQuantityOnProperty() []int32`

GetQuantityOnProperty returns the QuantityOnProperty field if non-nil, zero value otherwise.

### GetQuantityOnPropertyOk

`func (o *ShopListingWithAssociationsInventory) GetQuantityOnPropertyOk() (*[]int32, bool)`

GetQuantityOnPropertyOk returns a tuple with the QuantityOnProperty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantityOnProperty

`func (o *ShopListingWithAssociationsInventory) SetQuantityOnProperty(v []int32)`

SetQuantityOnProperty sets QuantityOnProperty field to given value.

### HasQuantityOnProperty

`func (o *ShopListingWithAssociationsInventory) HasQuantityOnProperty() bool`

HasQuantityOnProperty returns a boolean if a field has been set.

### GetSkuOnProperty

`func (o *ShopListingWithAssociationsInventory) GetSkuOnProperty() []int32`

GetSkuOnProperty returns the SkuOnProperty field if non-nil, zero value otherwise.

### GetSkuOnPropertyOk

`func (o *ShopListingWithAssociationsInventory) GetSkuOnPropertyOk() (*[]int32, bool)`

GetSkuOnPropertyOk returns a tuple with the SkuOnProperty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkuOnProperty

`func (o *ShopListingWithAssociationsInventory) SetSkuOnProperty(v []int32)`

SetSkuOnProperty sets SkuOnProperty field to given value.

### HasSkuOnProperty

`func (o *ShopListingWithAssociationsInventory) HasSkuOnProperty() bool`

HasSkuOnProperty returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


