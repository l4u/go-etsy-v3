# BuyerTaxonomyNodePropertiesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PropertyId** | Pointer to **int32** | The unique numeric ID of this product property. | [optional] 
**Name** | Pointer to **string** | The name string for this taxonomy node. | [optional] 
**DisplayName** | Pointer to **string** | The human-readable product property name string. | [optional] 
**Scales** | Pointer to [**[]BuyerTaxonomyNodePropertyScalesInner**](BuyerTaxonomyNodePropertyScalesInner.md) | A list of available scales. | [optional] 
**IsRequired** | Pointer to **bool** | When true, listings assigned eligible taxonomy IDs require this property. | [optional] 
**SupportsAttributes** | Pointer to **bool** | When true, you can use this property in listing attributes. | [optional] 
**SupportsVariations** | Pointer to **bool** | When true, you can use this property in listing variations. | [optional] 
**IsMultivalued** | Pointer to **bool** | When true, you can assign multiple property values to this property | [optional] 
**MaxValuesAllowed** | Pointer to **NullableInt32** | When true, you can assign multiple property values to this property | [optional] 
**PossibleValues** | Pointer to [**[]BuyerTaxonomyNodePropertyPossibleValuesInner**](BuyerTaxonomyNodePropertyPossibleValuesInner.md) | A list of supported property value strings for this property. | [optional] 
**SelectedValues** | Pointer to [**[]BuyerTaxonomyNodePropertySelectedValuesInner**](BuyerTaxonomyNodePropertySelectedValuesInner.md) | A list of property value strings automatically and always selected for the given property. | [optional] 

## Methods

### NewBuyerTaxonomyNodePropertiesResultsInner

`func NewBuyerTaxonomyNodePropertiesResultsInner() *BuyerTaxonomyNodePropertiesResultsInner`

NewBuyerTaxonomyNodePropertiesResultsInner instantiates a new BuyerTaxonomyNodePropertiesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBuyerTaxonomyNodePropertiesResultsInnerWithDefaults

`func NewBuyerTaxonomyNodePropertiesResultsInnerWithDefaults() *BuyerTaxonomyNodePropertiesResultsInner`

NewBuyerTaxonomyNodePropertiesResultsInnerWithDefaults instantiates a new BuyerTaxonomyNodePropertiesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPropertyId

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetPropertyId() int32`

GetPropertyId returns the PropertyId field if non-nil, zero value otherwise.

### GetPropertyIdOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetPropertyIdOk() (*int32, bool)`

GetPropertyIdOk returns a tuple with the PropertyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyId

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetPropertyId(v int32)`

SetPropertyId sets PropertyId field to given value.

### HasPropertyId

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasPropertyId() bool`

HasPropertyId returns a boolean if a field has been set.

### GetName

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDisplayName

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### GetScales

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetScales() []BuyerTaxonomyNodePropertyScalesInner`

GetScales returns the Scales field if non-nil, zero value otherwise.

### GetScalesOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetScalesOk() (*[]BuyerTaxonomyNodePropertyScalesInner, bool)`

GetScalesOk returns a tuple with the Scales field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScales

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetScales(v []BuyerTaxonomyNodePropertyScalesInner)`

SetScales sets Scales field to given value.

### HasScales

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasScales() bool`

HasScales returns a boolean if a field has been set.

### GetIsRequired

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetIsRequired() bool`

GetIsRequired returns the IsRequired field if non-nil, zero value otherwise.

### GetIsRequiredOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetIsRequiredOk() (*bool, bool)`

GetIsRequiredOk returns a tuple with the IsRequired field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRequired

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetIsRequired(v bool)`

SetIsRequired sets IsRequired field to given value.

### HasIsRequired

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasIsRequired() bool`

HasIsRequired returns a boolean if a field has been set.

### GetSupportsAttributes

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetSupportsAttributes() bool`

GetSupportsAttributes returns the SupportsAttributes field if non-nil, zero value otherwise.

### GetSupportsAttributesOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetSupportsAttributesOk() (*bool, bool)`

GetSupportsAttributesOk returns a tuple with the SupportsAttributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportsAttributes

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetSupportsAttributes(v bool)`

SetSupportsAttributes sets SupportsAttributes field to given value.

### HasSupportsAttributes

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasSupportsAttributes() bool`

HasSupportsAttributes returns a boolean if a field has been set.

### GetSupportsVariations

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetSupportsVariations() bool`

GetSupportsVariations returns the SupportsVariations field if non-nil, zero value otherwise.

### GetSupportsVariationsOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetSupportsVariationsOk() (*bool, bool)`

GetSupportsVariationsOk returns a tuple with the SupportsVariations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportsVariations

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetSupportsVariations(v bool)`

SetSupportsVariations sets SupportsVariations field to given value.

### HasSupportsVariations

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasSupportsVariations() bool`

HasSupportsVariations returns a boolean if a field has been set.

### GetIsMultivalued

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetIsMultivalued() bool`

GetIsMultivalued returns the IsMultivalued field if non-nil, zero value otherwise.

### GetIsMultivaluedOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetIsMultivaluedOk() (*bool, bool)`

GetIsMultivaluedOk returns a tuple with the IsMultivalued field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMultivalued

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetIsMultivalued(v bool)`

SetIsMultivalued sets IsMultivalued field to given value.

### HasIsMultivalued

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasIsMultivalued() bool`

HasIsMultivalued returns a boolean if a field has been set.

### GetMaxValuesAllowed

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetMaxValuesAllowed() int32`

GetMaxValuesAllowed returns the MaxValuesAllowed field if non-nil, zero value otherwise.

### GetMaxValuesAllowedOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetMaxValuesAllowedOk() (*int32, bool)`

GetMaxValuesAllowedOk returns a tuple with the MaxValuesAllowed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxValuesAllowed

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetMaxValuesAllowed(v int32)`

SetMaxValuesAllowed sets MaxValuesAllowed field to given value.

### HasMaxValuesAllowed

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasMaxValuesAllowed() bool`

HasMaxValuesAllowed returns a boolean if a field has been set.

### SetMaxValuesAllowedNil

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetMaxValuesAllowedNil(b bool)`

 SetMaxValuesAllowedNil sets the value for MaxValuesAllowed to be an explicit nil

### UnsetMaxValuesAllowed
`func (o *BuyerTaxonomyNodePropertiesResultsInner) UnsetMaxValuesAllowed()`

UnsetMaxValuesAllowed ensures that no value is present for MaxValuesAllowed, not even an explicit nil
### GetPossibleValues

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetPossibleValues() []BuyerTaxonomyNodePropertyPossibleValuesInner`

GetPossibleValues returns the PossibleValues field if non-nil, zero value otherwise.

### GetPossibleValuesOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetPossibleValuesOk() (*[]BuyerTaxonomyNodePropertyPossibleValuesInner, bool)`

GetPossibleValuesOk returns a tuple with the PossibleValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossibleValues

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetPossibleValues(v []BuyerTaxonomyNodePropertyPossibleValuesInner)`

SetPossibleValues sets PossibleValues field to given value.

### HasPossibleValues

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasPossibleValues() bool`

HasPossibleValues returns a boolean if a field has been set.

### GetSelectedValues

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetSelectedValues() []BuyerTaxonomyNodePropertySelectedValuesInner`

GetSelectedValues returns the SelectedValues field if non-nil, zero value otherwise.

### GetSelectedValuesOk

`func (o *BuyerTaxonomyNodePropertiesResultsInner) GetSelectedValuesOk() (*[]BuyerTaxonomyNodePropertySelectedValuesInner, bool)`

GetSelectedValuesOk returns a tuple with the SelectedValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelectedValues

`func (o *BuyerTaxonomyNodePropertiesResultsInner) SetSelectedValues(v []BuyerTaxonomyNodePropertySelectedValuesInner)`

SetSelectedValues sets SelectedValues field to given value.

### HasSelectedValues

`func (o *BuyerTaxonomyNodePropertiesResultsInner) HasSelectedValues() bool`

HasSelectedValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


