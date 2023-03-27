# TaxonomyNodePropertyPossibleValuesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ValueId** | Pointer to **NullableInt32** | The numeric ID of this property value. | [optional] 
**Name** | Pointer to **string** | The name string of this property value. | [optional] 
**ScaleId** | Pointer to **NullableInt32** | The numeric scale ID of the scale to which this property value belongs. | [optional] 
**EqualTo** | Pointer to **[]int32** | A list of numeric property value IDs this property value is equal to (if any). | [optional] 

## Methods

### NewTaxonomyNodePropertyPossibleValuesInner

`func NewTaxonomyNodePropertyPossibleValuesInner() *TaxonomyNodePropertyPossibleValuesInner`

NewTaxonomyNodePropertyPossibleValuesInner instantiates a new TaxonomyNodePropertyPossibleValuesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaxonomyNodePropertyPossibleValuesInnerWithDefaults

`func NewTaxonomyNodePropertyPossibleValuesInnerWithDefaults() *TaxonomyNodePropertyPossibleValuesInner`

NewTaxonomyNodePropertyPossibleValuesInnerWithDefaults instantiates a new TaxonomyNodePropertyPossibleValuesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValueId

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetValueId() int32`

GetValueId returns the ValueId field if non-nil, zero value otherwise.

### GetValueIdOk

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetValueIdOk() (*int32, bool)`

GetValueIdOk returns a tuple with the ValueId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueId

`func (o *TaxonomyNodePropertyPossibleValuesInner) SetValueId(v int32)`

SetValueId sets ValueId field to given value.

### HasValueId

`func (o *TaxonomyNodePropertyPossibleValuesInner) HasValueId() bool`

HasValueId returns a boolean if a field has been set.

### SetValueIdNil

`func (o *TaxonomyNodePropertyPossibleValuesInner) SetValueIdNil(b bool)`

 SetValueIdNil sets the value for ValueId to be an explicit nil

### UnsetValueId
`func (o *TaxonomyNodePropertyPossibleValuesInner) UnsetValueId()`

UnsetValueId ensures that no value is present for ValueId, not even an explicit nil
### GetName

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TaxonomyNodePropertyPossibleValuesInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *TaxonomyNodePropertyPossibleValuesInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetScaleId

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetScaleId() int32`

GetScaleId returns the ScaleId field if non-nil, zero value otherwise.

### GetScaleIdOk

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetScaleIdOk() (*int32, bool)`

GetScaleIdOk returns a tuple with the ScaleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleId

`func (o *TaxonomyNodePropertyPossibleValuesInner) SetScaleId(v int32)`

SetScaleId sets ScaleId field to given value.

### HasScaleId

`func (o *TaxonomyNodePropertyPossibleValuesInner) HasScaleId() bool`

HasScaleId returns a boolean if a field has been set.

### SetScaleIdNil

`func (o *TaxonomyNodePropertyPossibleValuesInner) SetScaleIdNil(b bool)`

 SetScaleIdNil sets the value for ScaleId to be an explicit nil

### UnsetScaleId
`func (o *TaxonomyNodePropertyPossibleValuesInner) UnsetScaleId()`

UnsetScaleId ensures that no value is present for ScaleId, not even an explicit nil
### GetEqualTo

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetEqualTo() []int32`

GetEqualTo returns the EqualTo field if non-nil, zero value otherwise.

### GetEqualToOk

`func (o *TaxonomyNodePropertyPossibleValuesInner) GetEqualToOk() (*[]int32, bool)`

GetEqualToOk returns a tuple with the EqualTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEqualTo

`func (o *TaxonomyNodePropertyPossibleValuesInner) SetEqualTo(v []int32)`

SetEqualTo sets EqualTo field to given value.

### HasEqualTo

`func (o *TaxonomyNodePropertyPossibleValuesInner) HasEqualTo() bool`

HasEqualTo returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


