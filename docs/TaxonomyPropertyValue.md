# TaxonomyPropertyValue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ValueId** | Pointer to **NullableInt32** | The numeric ID of this property value. | [optional] 
**Name** | Pointer to **string** | The name string of this property value. | [optional] 
**ScaleId** | Pointer to **NullableInt32** | The numeric scale ID of the scale to which this property value belongs. | [optional] 
**EqualTo** | Pointer to **[]int32** | A list of numeric property value IDs this property value is equal to (if any). | [optional] 

## Methods

### NewTaxonomyPropertyValue

`func NewTaxonomyPropertyValue() *TaxonomyPropertyValue`

NewTaxonomyPropertyValue instantiates a new TaxonomyPropertyValue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaxonomyPropertyValueWithDefaults

`func NewTaxonomyPropertyValueWithDefaults() *TaxonomyPropertyValue`

NewTaxonomyPropertyValueWithDefaults instantiates a new TaxonomyPropertyValue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValueId

`func (o *TaxonomyPropertyValue) GetValueId() int32`

GetValueId returns the ValueId field if non-nil, zero value otherwise.

### GetValueIdOk

`func (o *TaxonomyPropertyValue) GetValueIdOk() (*int32, bool)`

GetValueIdOk returns a tuple with the ValueId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueId

`func (o *TaxonomyPropertyValue) SetValueId(v int32)`

SetValueId sets ValueId field to given value.

### HasValueId

`func (o *TaxonomyPropertyValue) HasValueId() bool`

HasValueId returns a boolean if a field has been set.

### SetValueIdNil

`func (o *TaxonomyPropertyValue) SetValueIdNil(b bool)`

 SetValueIdNil sets the value for ValueId to be an explicit nil

### UnsetValueId
`func (o *TaxonomyPropertyValue) UnsetValueId()`

UnsetValueId ensures that no value is present for ValueId, not even an explicit nil
### GetName

`func (o *TaxonomyPropertyValue) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TaxonomyPropertyValue) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TaxonomyPropertyValue) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *TaxonomyPropertyValue) HasName() bool`

HasName returns a boolean if a field has been set.

### GetScaleId

`func (o *TaxonomyPropertyValue) GetScaleId() int32`

GetScaleId returns the ScaleId field if non-nil, zero value otherwise.

### GetScaleIdOk

`func (o *TaxonomyPropertyValue) GetScaleIdOk() (*int32, bool)`

GetScaleIdOk returns a tuple with the ScaleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleId

`func (o *TaxonomyPropertyValue) SetScaleId(v int32)`

SetScaleId sets ScaleId field to given value.

### HasScaleId

`func (o *TaxonomyPropertyValue) HasScaleId() bool`

HasScaleId returns a boolean if a field has been set.

### SetScaleIdNil

`func (o *TaxonomyPropertyValue) SetScaleIdNil(b bool)`

 SetScaleIdNil sets the value for ScaleId to be an explicit nil

### UnsetScaleId
`func (o *TaxonomyPropertyValue) UnsetScaleId()`

UnsetScaleId ensures that no value is present for ScaleId, not even an explicit nil
### GetEqualTo

`func (o *TaxonomyPropertyValue) GetEqualTo() []int32`

GetEqualTo returns the EqualTo field if non-nil, zero value otherwise.

### GetEqualToOk

`func (o *TaxonomyPropertyValue) GetEqualToOk() (*[]int32, bool)`

GetEqualToOk returns a tuple with the EqualTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEqualTo

`func (o *TaxonomyPropertyValue) SetEqualTo(v []int32)`

SetEqualTo sets EqualTo field to given value.

### HasEqualTo

`func (o *TaxonomyPropertyValue) HasEqualTo() bool`

HasEqualTo returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


