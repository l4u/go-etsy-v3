# ListingPropertyValuesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PropertyId** | Pointer to **int32** | The numeric ID of the Property. | [optional] 
**PropertyName** | Pointer to **NullableString** | The name of the Property. | [optional] 
**ScaleId** | Pointer to **NullableInt32** | The numeric ID of the scale (if any). | [optional] 
**ScaleName** | Pointer to **NullableString** | The label used to describe the chosen scale (if any). | [optional] 
**ValueIds** | Pointer to **[]int32** | The numeric IDs of the Property values | [optional] 
**Values** | Pointer to **[]string** | The Property values | [optional] 

## Methods

### NewListingPropertyValuesResultsInner

`func NewListingPropertyValuesResultsInner() *ListingPropertyValuesResultsInner`

NewListingPropertyValuesResultsInner instantiates a new ListingPropertyValuesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListingPropertyValuesResultsInnerWithDefaults

`func NewListingPropertyValuesResultsInnerWithDefaults() *ListingPropertyValuesResultsInner`

NewListingPropertyValuesResultsInnerWithDefaults instantiates a new ListingPropertyValuesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPropertyId

`func (o *ListingPropertyValuesResultsInner) GetPropertyId() int32`

GetPropertyId returns the PropertyId field if non-nil, zero value otherwise.

### GetPropertyIdOk

`func (o *ListingPropertyValuesResultsInner) GetPropertyIdOk() (*int32, bool)`

GetPropertyIdOk returns a tuple with the PropertyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyId

`func (o *ListingPropertyValuesResultsInner) SetPropertyId(v int32)`

SetPropertyId sets PropertyId field to given value.

### HasPropertyId

`func (o *ListingPropertyValuesResultsInner) HasPropertyId() bool`

HasPropertyId returns a boolean if a field has been set.

### GetPropertyName

`func (o *ListingPropertyValuesResultsInner) GetPropertyName() string`

GetPropertyName returns the PropertyName field if non-nil, zero value otherwise.

### GetPropertyNameOk

`func (o *ListingPropertyValuesResultsInner) GetPropertyNameOk() (*string, bool)`

GetPropertyNameOk returns a tuple with the PropertyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyName

`func (o *ListingPropertyValuesResultsInner) SetPropertyName(v string)`

SetPropertyName sets PropertyName field to given value.

### HasPropertyName

`func (o *ListingPropertyValuesResultsInner) HasPropertyName() bool`

HasPropertyName returns a boolean if a field has been set.

### SetPropertyNameNil

`func (o *ListingPropertyValuesResultsInner) SetPropertyNameNil(b bool)`

 SetPropertyNameNil sets the value for PropertyName to be an explicit nil

### UnsetPropertyName
`func (o *ListingPropertyValuesResultsInner) UnsetPropertyName()`

UnsetPropertyName ensures that no value is present for PropertyName, not even an explicit nil
### GetScaleId

`func (o *ListingPropertyValuesResultsInner) GetScaleId() int32`

GetScaleId returns the ScaleId field if non-nil, zero value otherwise.

### GetScaleIdOk

`func (o *ListingPropertyValuesResultsInner) GetScaleIdOk() (*int32, bool)`

GetScaleIdOk returns a tuple with the ScaleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleId

`func (o *ListingPropertyValuesResultsInner) SetScaleId(v int32)`

SetScaleId sets ScaleId field to given value.

### HasScaleId

`func (o *ListingPropertyValuesResultsInner) HasScaleId() bool`

HasScaleId returns a boolean if a field has been set.

### SetScaleIdNil

`func (o *ListingPropertyValuesResultsInner) SetScaleIdNil(b bool)`

 SetScaleIdNil sets the value for ScaleId to be an explicit nil

### UnsetScaleId
`func (o *ListingPropertyValuesResultsInner) UnsetScaleId()`

UnsetScaleId ensures that no value is present for ScaleId, not even an explicit nil
### GetScaleName

`func (o *ListingPropertyValuesResultsInner) GetScaleName() string`

GetScaleName returns the ScaleName field if non-nil, zero value otherwise.

### GetScaleNameOk

`func (o *ListingPropertyValuesResultsInner) GetScaleNameOk() (*string, bool)`

GetScaleNameOk returns a tuple with the ScaleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleName

`func (o *ListingPropertyValuesResultsInner) SetScaleName(v string)`

SetScaleName sets ScaleName field to given value.

### HasScaleName

`func (o *ListingPropertyValuesResultsInner) HasScaleName() bool`

HasScaleName returns a boolean if a field has been set.

### SetScaleNameNil

`func (o *ListingPropertyValuesResultsInner) SetScaleNameNil(b bool)`

 SetScaleNameNil sets the value for ScaleName to be an explicit nil

### UnsetScaleName
`func (o *ListingPropertyValuesResultsInner) UnsetScaleName()`

UnsetScaleName ensures that no value is present for ScaleName, not even an explicit nil
### GetValueIds

`func (o *ListingPropertyValuesResultsInner) GetValueIds() []int32`

GetValueIds returns the ValueIds field if non-nil, zero value otherwise.

### GetValueIdsOk

`func (o *ListingPropertyValuesResultsInner) GetValueIdsOk() (*[]int32, bool)`

GetValueIdsOk returns a tuple with the ValueIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueIds

`func (o *ListingPropertyValuesResultsInner) SetValueIds(v []int32)`

SetValueIds sets ValueIds field to given value.

### HasValueIds

`func (o *ListingPropertyValuesResultsInner) HasValueIds() bool`

HasValueIds returns a boolean if a field has been set.

### GetValues

`func (o *ListingPropertyValuesResultsInner) GetValues() []string`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *ListingPropertyValuesResultsInner) GetValuesOk() (*[]string, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *ListingPropertyValuesResultsInner) SetValues(v []string)`

SetValues sets Values field to given value.

### HasValues

`func (o *ListingPropertyValuesResultsInner) HasValues() bool`

HasValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


