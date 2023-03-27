# TaxonomyNodePropertiesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PropertyId** | Pointer to **int32** | The unique numeric ID of this product property. | [optional] 
**Name** | Pointer to **string** | The name string for this taxonomy node. | [optional] 
**DisplayName** | Pointer to **string** | The human-readable product property name string. | [optional] 
**Scales** | Pointer to [**[]TaxonomyNodePropertyScalesInner**](TaxonomyNodePropertyScalesInner.md) | A list of available scales. | [optional] 
**IsRequired** | Pointer to **bool** | When true, listings assigned eligible taxonomy IDs require this property. | [optional] 
**SupportsAttributes** | Pointer to **bool** | When true, you can use this property in listing attributes. | [optional] 
**SupportsVariations** | Pointer to **bool** | When true, you can use this property in listing variations. | [optional] 
**IsMultivalued** | Pointer to **bool** | When true, you can assign multiple property values to this property | [optional] 
**MaxValuesAllowed** | Pointer to **NullableInt32** | When true, you can assign multiple property values to this property | [optional] 
**PossibleValues** | Pointer to [**[]TaxonomyNodePropertyPossibleValuesInner**](TaxonomyNodePropertyPossibleValuesInner.md) | A list of supported property value strings for this property. | [optional] 
**SelectedValues** | Pointer to [**[]TaxonomyNodePropertySelectedValuesInner**](TaxonomyNodePropertySelectedValuesInner.md) | A list of property value strings automatically and always selected for the given property. | [optional] 

## Methods

### NewTaxonomyNodePropertiesResultsInner

`func NewTaxonomyNodePropertiesResultsInner() *TaxonomyNodePropertiesResultsInner`

NewTaxonomyNodePropertiesResultsInner instantiates a new TaxonomyNodePropertiesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaxonomyNodePropertiesResultsInnerWithDefaults

`func NewTaxonomyNodePropertiesResultsInnerWithDefaults() *TaxonomyNodePropertiesResultsInner`

NewTaxonomyNodePropertiesResultsInnerWithDefaults instantiates a new TaxonomyNodePropertiesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPropertyId

`func (o *TaxonomyNodePropertiesResultsInner) GetPropertyId() int32`

GetPropertyId returns the PropertyId field if non-nil, zero value otherwise.

### GetPropertyIdOk

`func (o *TaxonomyNodePropertiesResultsInner) GetPropertyIdOk() (*int32, bool)`

GetPropertyIdOk returns a tuple with the PropertyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPropertyId

`func (o *TaxonomyNodePropertiesResultsInner) SetPropertyId(v int32)`

SetPropertyId sets PropertyId field to given value.

### HasPropertyId

`func (o *TaxonomyNodePropertiesResultsInner) HasPropertyId() bool`

HasPropertyId returns a boolean if a field has been set.

### GetName

`func (o *TaxonomyNodePropertiesResultsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TaxonomyNodePropertiesResultsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TaxonomyNodePropertiesResultsInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *TaxonomyNodePropertiesResultsInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDisplayName

`func (o *TaxonomyNodePropertiesResultsInner) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *TaxonomyNodePropertiesResultsInner) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *TaxonomyNodePropertiesResultsInner) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *TaxonomyNodePropertiesResultsInner) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### GetScales

`func (o *TaxonomyNodePropertiesResultsInner) GetScales() []TaxonomyNodePropertyScalesInner`

GetScales returns the Scales field if non-nil, zero value otherwise.

### GetScalesOk

`func (o *TaxonomyNodePropertiesResultsInner) GetScalesOk() (*[]TaxonomyNodePropertyScalesInner, bool)`

GetScalesOk returns a tuple with the Scales field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScales

`func (o *TaxonomyNodePropertiesResultsInner) SetScales(v []TaxonomyNodePropertyScalesInner)`

SetScales sets Scales field to given value.

### HasScales

`func (o *TaxonomyNodePropertiesResultsInner) HasScales() bool`

HasScales returns a boolean if a field has been set.

### GetIsRequired

`func (o *TaxonomyNodePropertiesResultsInner) GetIsRequired() bool`

GetIsRequired returns the IsRequired field if non-nil, zero value otherwise.

### GetIsRequiredOk

`func (o *TaxonomyNodePropertiesResultsInner) GetIsRequiredOk() (*bool, bool)`

GetIsRequiredOk returns a tuple with the IsRequired field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRequired

`func (o *TaxonomyNodePropertiesResultsInner) SetIsRequired(v bool)`

SetIsRequired sets IsRequired field to given value.

### HasIsRequired

`func (o *TaxonomyNodePropertiesResultsInner) HasIsRequired() bool`

HasIsRequired returns a boolean if a field has been set.

### GetSupportsAttributes

`func (o *TaxonomyNodePropertiesResultsInner) GetSupportsAttributes() bool`

GetSupportsAttributes returns the SupportsAttributes field if non-nil, zero value otherwise.

### GetSupportsAttributesOk

`func (o *TaxonomyNodePropertiesResultsInner) GetSupportsAttributesOk() (*bool, bool)`

GetSupportsAttributesOk returns a tuple with the SupportsAttributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportsAttributes

`func (o *TaxonomyNodePropertiesResultsInner) SetSupportsAttributes(v bool)`

SetSupportsAttributes sets SupportsAttributes field to given value.

### HasSupportsAttributes

`func (o *TaxonomyNodePropertiesResultsInner) HasSupportsAttributes() bool`

HasSupportsAttributes returns a boolean if a field has been set.

### GetSupportsVariations

`func (o *TaxonomyNodePropertiesResultsInner) GetSupportsVariations() bool`

GetSupportsVariations returns the SupportsVariations field if non-nil, zero value otherwise.

### GetSupportsVariationsOk

`func (o *TaxonomyNodePropertiesResultsInner) GetSupportsVariationsOk() (*bool, bool)`

GetSupportsVariationsOk returns a tuple with the SupportsVariations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportsVariations

`func (o *TaxonomyNodePropertiesResultsInner) SetSupportsVariations(v bool)`

SetSupportsVariations sets SupportsVariations field to given value.

### HasSupportsVariations

`func (o *TaxonomyNodePropertiesResultsInner) HasSupportsVariations() bool`

HasSupportsVariations returns a boolean if a field has been set.

### GetIsMultivalued

`func (o *TaxonomyNodePropertiesResultsInner) GetIsMultivalued() bool`

GetIsMultivalued returns the IsMultivalued field if non-nil, zero value otherwise.

### GetIsMultivaluedOk

`func (o *TaxonomyNodePropertiesResultsInner) GetIsMultivaluedOk() (*bool, bool)`

GetIsMultivaluedOk returns a tuple with the IsMultivalued field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMultivalued

`func (o *TaxonomyNodePropertiesResultsInner) SetIsMultivalued(v bool)`

SetIsMultivalued sets IsMultivalued field to given value.

### HasIsMultivalued

`func (o *TaxonomyNodePropertiesResultsInner) HasIsMultivalued() bool`

HasIsMultivalued returns a boolean if a field has been set.

### GetMaxValuesAllowed

`func (o *TaxonomyNodePropertiesResultsInner) GetMaxValuesAllowed() int32`

GetMaxValuesAllowed returns the MaxValuesAllowed field if non-nil, zero value otherwise.

### GetMaxValuesAllowedOk

`func (o *TaxonomyNodePropertiesResultsInner) GetMaxValuesAllowedOk() (*int32, bool)`

GetMaxValuesAllowedOk returns a tuple with the MaxValuesAllowed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxValuesAllowed

`func (o *TaxonomyNodePropertiesResultsInner) SetMaxValuesAllowed(v int32)`

SetMaxValuesAllowed sets MaxValuesAllowed field to given value.

### HasMaxValuesAllowed

`func (o *TaxonomyNodePropertiesResultsInner) HasMaxValuesAllowed() bool`

HasMaxValuesAllowed returns a boolean if a field has been set.

### SetMaxValuesAllowedNil

`func (o *TaxonomyNodePropertiesResultsInner) SetMaxValuesAllowedNil(b bool)`

 SetMaxValuesAllowedNil sets the value for MaxValuesAllowed to be an explicit nil

### UnsetMaxValuesAllowed
`func (o *TaxonomyNodePropertiesResultsInner) UnsetMaxValuesAllowed()`

UnsetMaxValuesAllowed ensures that no value is present for MaxValuesAllowed, not even an explicit nil
### GetPossibleValues

`func (o *TaxonomyNodePropertiesResultsInner) GetPossibleValues() []TaxonomyNodePropertyPossibleValuesInner`

GetPossibleValues returns the PossibleValues field if non-nil, zero value otherwise.

### GetPossibleValuesOk

`func (o *TaxonomyNodePropertiesResultsInner) GetPossibleValuesOk() (*[]TaxonomyNodePropertyPossibleValuesInner, bool)`

GetPossibleValuesOk returns a tuple with the PossibleValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossibleValues

`func (o *TaxonomyNodePropertiesResultsInner) SetPossibleValues(v []TaxonomyNodePropertyPossibleValuesInner)`

SetPossibleValues sets PossibleValues field to given value.

### HasPossibleValues

`func (o *TaxonomyNodePropertiesResultsInner) HasPossibleValues() bool`

HasPossibleValues returns a boolean if a field has been set.

### GetSelectedValues

`func (o *TaxonomyNodePropertiesResultsInner) GetSelectedValues() []TaxonomyNodePropertySelectedValuesInner`

GetSelectedValues returns the SelectedValues field if non-nil, zero value otherwise.

### GetSelectedValuesOk

`func (o *TaxonomyNodePropertiesResultsInner) GetSelectedValuesOk() (*[]TaxonomyNodePropertySelectedValuesInner, bool)`

GetSelectedValuesOk returns a tuple with the SelectedValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelectedValues

`func (o *TaxonomyNodePropertiesResultsInner) SetSelectedValues(v []TaxonomyNodePropertySelectedValuesInner)`

SetSelectedValues sets SelectedValues field to given value.

### HasSelectedValues

`func (o *TaxonomyNodePropertiesResultsInner) HasSelectedValues() bool`

HasSelectedValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


