# ListingInventoryProductOfferingsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OfferingId** | Pointer to **int32** | The ID for the ProductOffering | [optional] 
**Quantity** | Pointer to **int32** | The quantity the ProductOffering | [optional] 
**IsEnabled** | Pointer to **bool** | Whether or not the offering can be shown to buyers. | [optional] 
**IsDeleted** | Pointer to **bool** | Whether or not the offering has been deleted. | [optional] 
**Price** | Pointer to [**ListingInventoryProductOfferingPrice**](ListingInventoryProductOfferingPrice.md) |  | [optional] 

## Methods

### NewListingInventoryProductOfferingsInner

`func NewListingInventoryProductOfferingsInner() *ListingInventoryProductOfferingsInner`

NewListingInventoryProductOfferingsInner instantiates a new ListingInventoryProductOfferingsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListingInventoryProductOfferingsInnerWithDefaults

`func NewListingInventoryProductOfferingsInnerWithDefaults() *ListingInventoryProductOfferingsInner`

NewListingInventoryProductOfferingsInnerWithDefaults instantiates a new ListingInventoryProductOfferingsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOfferingId

`func (o *ListingInventoryProductOfferingsInner) GetOfferingId() int32`

GetOfferingId returns the OfferingId field if non-nil, zero value otherwise.

### GetOfferingIdOk

`func (o *ListingInventoryProductOfferingsInner) GetOfferingIdOk() (*int32, bool)`

GetOfferingIdOk returns a tuple with the OfferingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOfferingId

`func (o *ListingInventoryProductOfferingsInner) SetOfferingId(v int32)`

SetOfferingId sets OfferingId field to given value.

### HasOfferingId

`func (o *ListingInventoryProductOfferingsInner) HasOfferingId() bool`

HasOfferingId returns a boolean if a field has been set.

### GetQuantity

`func (o *ListingInventoryProductOfferingsInner) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *ListingInventoryProductOfferingsInner) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *ListingInventoryProductOfferingsInner) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.

### HasQuantity

`func (o *ListingInventoryProductOfferingsInner) HasQuantity() bool`

HasQuantity returns a boolean if a field has been set.

### GetIsEnabled

`func (o *ListingInventoryProductOfferingsInner) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *ListingInventoryProductOfferingsInner) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *ListingInventoryProductOfferingsInner) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.

### HasIsEnabled

`func (o *ListingInventoryProductOfferingsInner) HasIsEnabled() bool`

HasIsEnabled returns a boolean if a field has been set.

### GetIsDeleted

`func (o *ListingInventoryProductOfferingsInner) GetIsDeleted() bool`

GetIsDeleted returns the IsDeleted field if non-nil, zero value otherwise.

### GetIsDeletedOk

`func (o *ListingInventoryProductOfferingsInner) GetIsDeletedOk() (*bool, bool)`

GetIsDeletedOk returns a tuple with the IsDeleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDeleted

`func (o *ListingInventoryProductOfferingsInner) SetIsDeleted(v bool)`

SetIsDeleted sets IsDeleted field to given value.

### HasIsDeleted

`func (o *ListingInventoryProductOfferingsInner) HasIsDeleted() bool`

HasIsDeleted returns a boolean if a field has been set.

### GetPrice

`func (o *ListingInventoryProductOfferingsInner) GetPrice() ListingInventoryProductOfferingPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ListingInventoryProductOfferingsInner) GetPriceOk() (*ListingInventoryProductOfferingPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ListingInventoryProductOfferingsInner) SetPrice(v ListingInventoryProductOfferingPrice)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ListingInventoryProductOfferingsInner) HasPrice() bool`

HasPrice returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


