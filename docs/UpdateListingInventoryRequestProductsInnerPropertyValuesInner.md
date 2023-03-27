# UpdateListingInventoryRequestProductsInnerPropertyValuesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PropertyId** | **int32** | The unique ID of an Etsy [listing property](/documentation/reference#operation/getListingProperties). | 
**ValueIds** | **[]int32** | An array of unique IDs of multiple Etsy [listing property](/documentation/reference#operation/getListingProperties) values. For example, if your listing offers different sizes of a product, then the value ID list contains value IDs for each size. | 
**ScaleId** | Pointer to **NullableInt32** | The numeric ID of a single Etsy.com measurement scale. For example, for shoe size, there are three &#x60;scale_id&#x60;s available - &#x60;UK&#x60;, &#x60;US/Canada&#x60;, and &#x60;EU&#x60;, where &#x60;US/Canada&#x60; has &#x60;scale_id&#x60; 19. | [optional] 
**PropertyName** | Pointer to **string** | The name of the property, in the requested locale language. | [optional] 
**Values** | **[]string** | A list of property value entries for this product. Note: parenthesis characters (&#x60;(&#x60; and &#x60;)&#x60;) are not allowed. | 

## Methods

### NewUpdateListingInventoryRequestProductsInnerPropertyValuesInner

`func NewUpdateListingInventoryRequestProductsInnerPropertyValuesInner(propertyId int32, valueIds []int32, values []string, ) *UpdateListingInventoryRequestProductsInnerPropertyValuesInner`

NewUpdateListingInventoryRequestProductsInnerPropertyValuesInner instantiates a new UpdateListingInventoryRequestProductsInnerPropertyValuesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateListingInventoryRequestProductsInnerPropertyValuesInnerWithDefaults

`func NewUpdateListingInventoryRequestProductsInnerPropertyValuesInnerWithDefaults() *UpdateListingInventoryRequestProductsInnerPropertyValuesInner`

NewUpdateListingInventoryRequestProductsInnerPropertyValuesInnerWithDefaults instantiates a new UpdateListingInventoryRequestProductsInnerPropertyValuesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPropertyId

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetPropertyId() int32`

GetPropertyId returns the PropertyId field if non-nil, zero value otherwise.

### GetPropertyIdOk

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetPropertyIdOk() (*int32, bool)`

GetPropertyIdOk returns a tuple with the PropertyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyId

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) SetPropertyId(v int32)`

SetPropertyId sets PropertyId field to given value.


### GetValueIds

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetValueIds() []int32`

GetValueIds returns the ValueIds field if non-nil, zero value otherwise.

### GetValueIdsOk

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetValueIdsOk() (*[]int32, bool)`

GetValueIdsOk returns a tuple with the ValueIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValueIds

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) SetValueIds(v []int32)`

SetValueIds sets ValueIds field to given value.


### GetScaleId

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetScaleId() int32`

GetScaleId returns the ScaleId field if non-nil, zero value otherwise.

### GetScaleIdOk

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetScaleIdOk() (*int32, bool)`

GetScaleIdOk returns a tuple with the ScaleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScaleId

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) SetScaleId(v int32)`

SetScaleId sets ScaleId field to given value.

### HasScaleId

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) HasScaleId() bool`

HasScaleId returns a boolean if a field has been set.

### SetScaleIdNil

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) SetScaleIdNil(b bool)`

 SetScaleIdNil sets the value for ScaleId to be an explicit nil

### UnsetScaleId
`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) UnsetScaleId()`

UnsetScaleId ensures that no value is present for ScaleId, not even an explicit nil
### GetPropertyName

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetPropertyName() string`

GetPropertyName returns the PropertyName field if non-nil, zero value otherwise.

### GetPropertyNameOk

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetPropertyNameOk() (*string, bool)`

GetPropertyNameOk returns a tuple with the PropertyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyName

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) SetPropertyName(v string)`

SetPropertyName sets PropertyName field to given value.

### HasPropertyName

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) HasPropertyName() bool`

HasPropertyName returns a boolean if a field has been set.

### GetValues

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetValues() []string`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) GetValuesOk() (*[]string, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *UpdateListingInventoryRequestProductsInnerPropertyValuesInner) SetValues(v []string)`

SetValues sets Values field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


