# ShopListings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Count** | Pointer to **int32** | The number of ShopListing resources found. | [optional] 
**Results** | Pointer to [**[]ShopListingsResultsInner**](ShopListingsResultsInner.md) | The ShopListing resources found. | [optional] 

## Methods

### NewShopListings

`func NewShopListings() *ShopListings`

NewShopListings instantiates a new ShopListings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingsWithDefaults

`func NewShopListingsWithDefaults() *ShopListings`

NewShopListingsWithDefaults instantiates a new ShopListings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCount

`func (o *ShopListings) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ShopListings) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ShopListings) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *ShopListings) HasCount() bool`

HasCount returns a boolean if a field has been set.

### GetResults

`func (o *ShopListings) GetResults() []ShopListingsResultsInner`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *ShopListings) GetResultsOk() (*[]ShopListingsResultsInner, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *ShopListings) SetResults(v []ShopListingsResultsInner)`

SetResults sets Results field to given value.

### HasResults

`func (o *ShopListings) HasResults() bool`

HasResults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


