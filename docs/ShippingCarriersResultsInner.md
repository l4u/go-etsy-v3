# ShippingCarriersResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShippingCarrierId** | Pointer to **int32** | The numeric ID of this shipping carrier. | [optional] 
**Name** | Pointer to **string** | The name of this shipping carrier. | [optional] 
**DomesticClasses** | Pointer to [**[]ShippingCarrierDomesticClassesInner**](ShippingCarrierDomesticClassesInner.md) | Set of domestic mail classes of this shipping carrier. | [optional] 
**InternationalClasses** | Pointer to [**[]ShippingCarrierInternationalClassesInner**](ShippingCarrierInternationalClassesInner.md) | Set of international mail classes of this shipping carrier. | [optional] 

## Methods

### NewShippingCarriersResultsInner

`func NewShippingCarriersResultsInner() *ShippingCarriersResultsInner`

NewShippingCarriersResultsInner instantiates a new ShippingCarriersResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShippingCarriersResultsInnerWithDefaults

`func NewShippingCarriersResultsInnerWithDefaults() *ShippingCarriersResultsInner`

NewShippingCarriersResultsInnerWithDefaults instantiates a new ShippingCarriersResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShippingCarrierId

`func (o *ShippingCarriersResultsInner) GetShippingCarrierId() int32`

GetShippingCarrierId returns the ShippingCarrierId field if non-nil, zero value otherwise.

### GetShippingCarrierIdOk

`func (o *ShippingCarriersResultsInner) GetShippingCarrierIdOk() (*int32, bool)`

GetShippingCarrierIdOk returns a tuple with the ShippingCarrierId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingCarrierId

`func (o *ShippingCarriersResultsInner) SetShippingCarrierId(v int32)`

SetShippingCarrierId sets ShippingCarrierId field to given value.

### HasShippingCarrierId

`func (o *ShippingCarriersResultsInner) HasShippingCarrierId() bool`

HasShippingCarrierId returns a boolean if a field has been set.

### GetName

`func (o *ShippingCarriersResultsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ShippingCarriersResultsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ShippingCarriersResultsInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ShippingCarriersResultsInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDomesticClasses

`func (o *ShippingCarriersResultsInner) GetDomesticClasses() []ShippingCarrierDomesticClassesInner`

GetDomesticClasses returns the DomesticClasses field if non-nil, zero value otherwise.

### GetDomesticClassesOk

`func (o *ShippingCarriersResultsInner) GetDomesticClassesOk() (*[]ShippingCarrierDomesticClassesInner, bool)`

GetDomesticClassesOk returns a tuple with the DomesticClasses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomesticClasses

`func (o *ShippingCarriersResultsInner) SetDomesticClasses(v []ShippingCarrierDomesticClassesInner)`

SetDomesticClasses sets DomesticClasses field to given value.

### HasDomesticClasses

`func (o *ShippingCarriersResultsInner) HasDomesticClasses() bool`

HasDomesticClasses returns a boolean if a field has been set.

### GetInternationalClasses

`func (o *ShippingCarriersResultsInner) GetInternationalClasses() []ShippingCarrierInternationalClassesInner`

GetInternationalClasses returns the InternationalClasses field if non-nil, zero value otherwise.

### GetInternationalClassesOk

`func (o *ShippingCarriersResultsInner) GetInternationalClassesOk() (*[]ShippingCarrierInternationalClassesInner, bool)`

GetInternationalClassesOk returns a tuple with the InternationalClasses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInternationalClasses

`func (o *ShippingCarriersResultsInner) SetInternationalClasses(v []ShippingCarrierInternationalClassesInner)`

SetInternationalClasses sets InternationalClasses field to given value.

### HasInternationalClasses

`func (o *ShippingCarriersResultsInner) HasInternationalClasses() bool`

HasInternationalClasses returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


