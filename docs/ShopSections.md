# ShopSections

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Count** | Pointer to **int32** | The number of results. | [optional] 
**Results** | Pointer to [**[]ShopSectionsResultsInner**](ShopSectionsResultsInner.md) | The list of requested resources. | [optional] 

## Methods

### NewShopSections

`func NewShopSections() *ShopSections`

NewShopSections instantiates a new ShopSections object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopSectionsWithDefaults

`func NewShopSectionsWithDefaults() *ShopSections`

NewShopSectionsWithDefaults instantiates a new ShopSections object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCount

`func (o *ShopSections) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ShopSections) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ShopSections) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *ShopSections) HasCount() bool`

HasCount returns a boolean if a field has been set.

### GetResults

`func (o *ShopSections) GetResults() []ShopSectionsResultsInner`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *ShopSections) GetResultsOk() (*[]ShopSectionsResultsInner, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *ShopSections) SetResults(v []ShopSectionsResultsInner)`

SetResults sets Results field to given value.

### HasResults

`func (o *ShopSections) HasResults() bool`

HasResults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


