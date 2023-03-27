# ShopListingFiles

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Count** | Pointer to **int32** | The number of ShopListingFiles being returned.. | [optional] 
**Results** | Pointer to [**[]ShopListingFilesResultsInner**](ShopListingFilesResultsInner.md) | An array of ShopListingFile resources. | [optional] 

## Methods

### NewShopListingFiles

`func NewShopListingFiles() *ShopListingFiles`

NewShopListingFiles instantiates a new ShopListingFiles object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingFilesWithDefaults

`func NewShopListingFilesWithDefaults() *ShopListingFiles`

NewShopListingFilesWithDefaults instantiates a new ShopListingFiles object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCount

`func (o *ShopListingFiles) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ShopListingFiles) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ShopListingFiles) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *ShopListingFiles) HasCount() bool`

HasCount returns a boolean if a field has been set.

### GetResults

`func (o *ShopListingFiles) GetResults() []ShopListingFilesResultsInner`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *ShopListingFiles) GetResultsOk() (*[]ShopListingFilesResultsInner, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *ShopListingFiles) SetResults(v []ShopListingFilesResultsInner)`

SetResults sets Results field to given value.

### HasResults

`func (o *ShopListingFiles) HasResults() bool`

HasResults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

