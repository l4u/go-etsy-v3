# ListingInventoryProductPropertyValuesInner

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

### NewListingInventoryProductPropertyValuesInner

`func NewListingInventoryProductPropertyValuesInner() *ListingInventoryProductPropertyValuesInner`

NewListingInventoryProductPropertyValuesInner instantiates a new ListingInventoryProductPropertyValuesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListingInventoryProductPropertyValuesInnerWithDefaults

`func NewListingInventoryProductPropertyValuesInnerWithDefaults() *ListingInventoryProductPropertyValuesInner`

NewListingInventoryProductPropertyValuesInnerWithDefaults instantiates a new ListingInventoryProductPropertyValuesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPropertyId

`func (o *ListingInventoryProductPropertyValuesInner) GetPropertyId() int32`

GetPropertyId returns the PropertyId field if non-nil, zero value otherwise.

### GetPropertyIdOk

`func (o *ListingInventoryProductPropertyValuesInner) GetPropertyIdOk() (*int32, bool)`

GetPropertyIdOk returns a tuple with the PropertyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyId

`func (o *ListingInventoryProductPropertyValuesInner) SetPropertyId(v int32)`

SetPropertyId sets PropertyId field to given value.

### HasPropertyId

`func (o *ListingInventoryProductPropertyValuesInner) HasPropertyId() bool`

HasPropertyId returns a boolean if a field has been set.

### GetPropertyName

`func (o *ListingInventoryProductPropertyValuesInner) GetPropertyName() string`

GetPropertyName returns the PropertyName field if non-nil, zero value otherwise.

### GetPropertyNameOk

`func (o *ListingInventoryProductPropertyValuesInner) GetPropertyNameOk() (*string, bool)`

GetPropertyNameOk returns a tuple with the PropertyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyName

`func (o *ListingInventoryProductPropertyValuesInner) SetPropertyName(v string)`

SetPropertyName sets PropertyName field to given value.

### HasPropertyName

`func (o *ListingInventoryProductPropertyValuesInner) HasPropertyName() bool`

HasPropertyName returns a boolean if a field has been set.

### SetPropertyNameNil

`func (o *ListingInventoryProductPropertyValuesInner) SetPropertyNameNil(b bool)`

 SetPropertyNameNil sets the value for PropertyName to be an explicit nil

### UnsetPropertyName
`func (o *ListingInventoryProductPropertyValuesInner) UnsetPropertyName()`

UnsetPropertyName ensures that no value is present for PropertyName, not even an explicit nil
### GetScaleId

`func (o *ListingInventoryProductPropertyValuesInner) GetScaleId() int32`

GetScaleId returns the ScaleId field if non-nil, zero value otherwise.

### GetScaleIdOk

`func (o *ListingInventoryProductPropertyValuesInner) GetScaleIdOk() (*int32, bool)`

GetScaleIdOk returns a tuple with the ScaleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleId

`func (o *ListingInventoryProductPropertyValuesInner) SetScaleId(v int32)`

SetScaleId sets ScaleId field to given value.

### HasScaleId

`func (o *ListingInventoryProductPropertyValuesInner) HasScaleId() bool`

HasScaleId returns a boolean if a field has been set.

### SetScaleIdNil

`func (o *ListingInventoryProductPropertyValuesInner) SetScaleIdNil(b bool)`

 SetScaleIdNil sets the value for ScaleId to be an explicit nil

### UnsetScaleId
`func (o *ListingInventoryProductPropertyValuesInner) UnsetScaleId()`

UnsetScaleId ensures that no value is present for ScaleId, not even an explicit nil
### GetScaleName

`func (o *ListingInventoryProductPropertyValuesInner) GetScaleName() string`

GetScaleName returns the ScaleName field if non-nil, zero value otherwise.

### GetScaleNameOk

`func (o *ListingInventoryProductPropertyValuesInner) GetScaleNameOk() (*string, bool)`

GetScaleNameOk returns a tuple with the ScaleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleName

`func (o *ListingInventoryProductPropertyValuesInner) SetScaleName(v string)`

SetScaleName sets ScaleName field to given value.

### HasScaleName

`func (o *ListingInventoryProductPropertyValuesInner) HasScaleName() bool`

HasScaleName returns a boolean if a field has been set.

### SetScaleNameNil

`func (o *ListingInventoryProductPropertyValuesInner) SetScaleNameNil(b bool)`

 SetScaleNameNil sets the value for ScaleName to be an explicit nil

### UnsetScaleName
`func (o *ListingInventoryProductPropertyValuesInner) UnsetScaleName()`

UnsetScaleName ensures that no value is present for ScaleName, not even an explicit nil
### GetValueIds

`func (o *ListingInventoryProductPropertyValuesInner) GetValueIds() []int32`

GetValueIds returns the ValueIds field if non-nil, zero value otherwise.

### GetValueIdsOk

`func (o *ListingInventoryProductPropertyValuesInner) GetValueIdsOk() (*[]int32, bool)`

GetValueIdsOk returns a tuple with the ValueIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueIds

`func (o *ListingInventoryProductPropertyValuesInner) SetValueIds(v []int32)`

SetValueIds sets ValueIds field to given value.

### HasValueIds

`func (o *ListingInventoryProductPropertyValuesInner) HasValueIds() bool`

HasValueIds returns a boolean if a field has been set.

### GetValues

`func (o *ListingInventoryProductPropertyValuesInner) GetValues() []string`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *ListingInventoryProductPropertyValuesInner) GetValuesOk() (*[]string, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *ListingInventoryProductPropertyValuesInner) SetValues(v []string)`

SetValues sets Values field to given value.

### HasValues

`func (o *ListingInventoryProductPropertyValuesInner) HasValues() bool`

HasValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


