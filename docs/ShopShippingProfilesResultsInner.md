# ShopShippingProfilesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShippingProfileId** | Pointer to **int32** | The numeric ID of the shipping profile. | [optional] 
**Title** | Pointer to **NullableString** | The name string of this shipping profile. | [optional] 
**UserId** | Pointer to **int32** | The numeric ID for the [user](/documentation/reference#tag/User) who owns the shipping profile. | [optional] 
**MinProcessingDays** | Pointer to **NullableInt32** | The minimum number of days for processing the listing. | [optional] 
**MaxProcessingDays** | Pointer to **NullableInt32** | The maximum number of days for processing the listing. | [optional] 
**ProcessingDaysDisplayLabel** | Pointer to **string** | Translated display label string for processing days. | [optional] 
**OriginCountryIso** | Pointer to **string** | The ISO code of the country from which the listing ships. | [optional] 
**IsDeleted** | Pointer to **bool** | When true, someone deleted this shipping profile. | [optional] 
**ShippingProfileDestinations** | Pointer to [**[]ShopShippingProfileShippingProfileDestinationsInner**](ShopShippingProfileShippingProfileDestinationsInner.md) | A list of [shipping profile destinations](/documentation/reference/#operation/createShopShippingProfileDestination) available for this shipping profile. | [optional] 
**ShippingProfileUpgrades** | Pointer to [**[]ShopShippingProfileShippingProfileUpgradesInner**](ShopShippingProfileShippingProfileUpgradesInner.md) | A list of [shipping profile upgrades](/documentation/reference/#operation/createShopShippingProfileUpgrade) available for this shipping profile. | [optional] 
**OriginPostalCode** | Pointer to **NullableString** | The postal code string (not necessarily a number) for the location from which the listing ships. Required if the &#x60;origin_country_iso&#x60; is &#x60;US&#x60; or &#x60;CA&#x60;. | [optional] 
**ProfileType** | Pointer to **string** |  | [optional] 
**DomesticHandlingFee** | Pointer to **float32** | The domestic handling fee added to buyer&#39;s shipping total - only available for calculated shipping profiles. | [optional] [default to 0]
**InternationalHandlingFee** | Pointer to **float32** | The international handling fee added to buyer&#39;s shipping total - only available for calculated shipping profiles. | [optional] [default to 0]

## Methods

### NewShopShippingProfilesResultsInner

`func NewShopShippingProfilesResultsInner() *ShopShippingProfilesResultsInner`

NewShopShippingProfilesResultsInner instantiates a new ShopShippingProfilesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopShippingProfilesResultsInnerWithDefaults

`func NewShopShippingProfilesResultsInnerWithDefaults() *ShopShippingProfilesResultsInner`

NewShopShippingProfilesResultsInnerWithDefaults instantiates a new ShopShippingProfilesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShippingProfileId

`func (o *ShopShippingProfilesResultsInner) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopShippingProfilesResultsInner) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopShippingProfilesResultsInner) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopShippingProfilesResultsInner) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### GetTitle

`func (o *ShopShippingProfilesResultsInner) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopShippingProfilesResultsInner) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopShippingProfilesResultsInner) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopShippingProfilesResultsInner) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *ShopShippingProfilesResultsInner) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *ShopShippingProfilesResultsInner) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetUserId

`func (o *ShopShippingProfilesResultsInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ShopShippingProfilesResultsInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ShopShippingProfilesResultsInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ShopShippingProfilesResultsInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetMinProcessingDays

`func (o *ShopShippingProfilesResultsInner) GetMinProcessingDays() int32`

GetMinProcessingDays returns the MinProcessingDays field if non-nil, zero value otherwise.

### GetMinProcessingDaysOk

`func (o *ShopShippingProfilesResultsInner) GetMinProcessingDaysOk() (*int32, bool)`

GetMinProcessingDaysOk returns a tuple with the MinProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinProcessingDays

`func (o *ShopShippingProfilesResultsInner) SetMinProcessingDays(v int32)`

SetMinProcessingDays sets MinProcessingDays field to given value.

### HasMinProcessingDays

`func (o *ShopShippingProfilesResultsInner) HasMinProcessingDays() bool`

HasMinProcessingDays returns a boolean if a field has been set.

### SetMinProcessingDaysNil

`func (o *ShopShippingProfilesResultsInner) SetMinProcessingDaysNil(b bool)`

 SetMinProcessingDaysNil sets the value for MinProcessingDays to be an explicit nil

### UnsetMinProcessingDays
`func (o *ShopShippingProfilesResultsInner) UnsetMinProcessingDays()`

UnsetMinProcessingDays ensures that no value is present for MinProcessingDays, not even an explicit nil
### GetMaxProcessingDays

`func (o *ShopShippingProfilesResultsInner) GetMaxProcessingDays() int32`

GetMaxProcessingDays returns the MaxProcessingDays field if non-nil, zero value otherwise.

### GetMaxProcessingDaysOk

`func (o *ShopShippingProfilesResultsInner) GetMaxProcessingDaysOk() (*int32, bool)`

GetMaxProcessingDaysOk returns a tuple with the MaxProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxProcessingDays

`func (o *ShopShippingProfilesResultsInner) SetMaxProcessingDays(v int32)`

SetMaxProcessingDays sets MaxProcessingDays field to given value.

### HasMaxProcessingDays

`func (o *ShopShippingProfilesResultsInner) HasMaxProcessingDays() bool`

HasMaxProcessingDays returns a boolean if a field has been set.

### SetMaxProcessingDaysNil

`func (o *ShopShippingProfilesResultsInner) SetMaxProcessingDaysNil(b bool)`

 SetMaxProcessingDaysNil sets the value for MaxProcessingDays to be an explicit nil

### UnsetMaxProcessingDays
`func (o *ShopShippingProfilesResultsInner) UnsetMaxProcessingDays()`

UnsetMaxProcessingDays ensures that no value is present for MaxProcessingDays, not even an explicit nil
### GetProcessingDaysDisplayLabel

`func (o *ShopShippingProfilesResultsInner) GetProcessingDaysDisplayLabel() string`

GetProcessingDaysDisplayLabel returns the ProcessingDaysDisplayLabel field if non-nil, zero value otherwise.

### GetProcessingDaysDisplayLabelOk

`func (o *ShopShippingProfilesResultsInner) GetProcessingDaysDisplayLabelOk() (*string, bool)`

GetProcessingDaysDisplayLabelOk returns a tuple with the ProcessingDaysDisplayLabel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessingDaysDisplayLabel

`func (o *ShopShippingProfilesResultsInner) SetProcessingDaysDisplayLabel(v string)`

SetProcessingDaysDisplayLabel sets ProcessingDaysDisplayLabel field to given value.

### HasProcessingDaysDisplayLabel

`func (o *ShopShippingProfilesResultsInner) HasProcessingDaysDisplayLabel() bool`

HasProcessingDaysDisplayLabel returns a boolean if a field has been set.

### GetOriginCountryIso

`func (o *ShopShippingProfilesResultsInner) GetOriginCountryIso() string`

GetOriginCountryIso returns the OriginCountryIso field if non-nil, zero value otherwise.

### GetOriginCountryIsoOk

`func (o *ShopShippingProfilesResultsInner) GetOriginCountryIsoOk() (*string, bool)`

GetOriginCountryIsoOk returns a tuple with the OriginCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginCountryIso

`func (o *ShopShippingProfilesResultsInner) SetOriginCountryIso(v string)`

SetOriginCountryIso sets OriginCountryIso field to given value.

### HasOriginCountryIso

`func (o *ShopShippingProfilesResultsInner) HasOriginCountryIso() bool`

HasOriginCountryIso returns a boolean if a field has been set.

### GetIsDeleted

`func (o *ShopShippingProfilesResultsInner) GetIsDeleted() bool`

GetIsDeleted returns the IsDeleted field if non-nil, zero value otherwise.

### GetIsDeletedOk

`func (o *ShopShippingProfilesResultsInner) GetIsDeletedOk() (*bool, bool)`

GetIsDeletedOk returns a tuple with the IsDeleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDeleted

`func (o *ShopShippingProfilesResultsInner) SetIsDeleted(v bool)`

SetIsDeleted sets IsDeleted field to given value.

### HasIsDeleted

`func (o *ShopShippingProfilesResultsInner) HasIsDeleted() bool`

HasIsDeleted returns a boolean if a field has been set.

### GetShippingProfileDestinations

`func (o *ShopShippingProfilesResultsInner) GetShippingProfileDestinations() []ShopShippingProfileShippingProfileDestinationsInner`

GetShippingProfileDestinations returns the ShippingProfileDestinations field if non-nil, zero value otherwise.

### GetShippingProfileDestinationsOk

`func (o *ShopShippingProfilesResultsInner) GetShippingProfileDestinationsOk() (*[]ShopShippingProfileShippingProfileDestinationsInner, bool)`

GetShippingProfileDestinationsOk returns a tuple with the ShippingProfileDestinations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileDestinations

`func (o *ShopShippingProfilesResultsInner) SetShippingProfileDestinations(v []ShopShippingProfileShippingProfileDestinationsInner)`

SetShippingProfileDestinations sets ShippingProfileDestinations field to given value.

### HasShippingProfileDestinations

`func (o *ShopShippingProfilesResultsInner) HasShippingProfileDestinations() bool`

HasShippingProfileDestinations returns a boolean if a field has been set.

### GetShippingProfileUpgrades

`func (o *ShopShippingProfilesResultsInner) GetShippingProfileUpgrades() []ShopShippingProfileShippingProfileUpgradesInner`

GetShippingProfileUpgrades returns the ShippingProfileUpgrades field if non-nil, zero value otherwise.

### GetShippingProfileUpgradesOk

`func (o *ShopShippingProfilesResultsInner) GetShippingProfileUpgradesOk() (*[]ShopShippingProfileShippingProfileUpgradesInner, bool)`

GetShippingProfileUpgradesOk returns a tuple with the ShippingProfileUpgrades field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileUpgrades

`func (o *ShopShippingProfilesResultsInner) SetShippingProfileUpgrades(v []ShopShippingProfileShippingProfileUpgradesInner)`

SetShippingProfileUpgrades sets ShippingProfileUpgrades field to given value.

### HasShippingProfileUpgrades

`func (o *ShopShippingProfilesResultsInner) HasShippingProfileUpgrades() bool`

HasShippingProfileUpgrades returns a boolean if a field has been set.

### GetOriginPostalCode

`func (o *ShopShippingProfilesResultsInner) GetOriginPostalCode() string`

GetOriginPostalCode returns the OriginPostalCode field if non-nil, zero value otherwise.

### GetOriginPostalCodeOk

`func (o *ShopShippingProfilesResultsInner) GetOriginPostalCodeOk() (*string, bool)`

GetOriginPostalCodeOk returns a tuple with the OriginPostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginPostalCode

`func (o *ShopShippingProfilesResultsInner) SetOriginPostalCode(v string)`

SetOriginPostalCode sets OriginPostalCode field to given value.

### HasOriginPostalCode

`func (o *ShopShippingProfilesResultsInner) HasOriginPostalCode() bool`

HasOriginPostalCode returns a boolean if a field has been set.

### SetOriginPostalCodeNil

`func (o *ShopShippingProfilesResultsInner) SetOriginPostalCodeNil(b bool)`

 SetOriginPostalCodeNil sets the value for OriginPostalCode to be an explicit nil

### UnsetOriginPostalCode
`func (o *ShopShippingProfilesResultsInner) UnsetOriginPostalCode()`

UnsetOriginPostalCode ensures that no value is present for OriginPostalCode, not even an explicit nil
### GetProfileType

`func (o *ShopShippingProfilesResultsInner) GetProfileType() string`

GetProfileType returns the ProfileType field if non-nil, zero value otherwise.

### GetProfileTypeOk

`func (o *ShopShippingProfilesResultsInner) GetProfileTypeOk() (*string, bool)`

GetProfileTypeOk returns a tuple with the ProfileType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileType

`func (o *ShopShippingProfilesResultsInner) SetProfileType(v string)`

SetProfileType sets ProfileType field to given value.

### HasProfileType

`func (o *ShopShippingProfilesResultsInner) HasProfileType() bool`

HasProfileType returns a boolean if a field has been set.

### GetDomesticHandlingFee

`func (o *ShopShippingProfilesResultsInner) GetDomesticHandlingFee() float32`

GetDomesticHandlingFee returns the DomesticHandlingFee field if non-nil, zero value otherwise.

### GetDomesticHandlingFeeOk

`func (o *ShopShippingProfilesResultsInner) GetDomesticHandlingFeeOk() (*float32, bool)`

GetDomesticHandlingFeeOk returns a tuple with the DomesticHandlingFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomesticHandlingFee

`func (o *ShopShippingProfilesResultsInner) SetDomesticHandlingFee(v float32)`

SetDomesticHandlingFee sets DomesticHandlingFee field to given value.

### HasDomesticHandlingFee

`func (o *ShopShippingProfilesResultsInner) HasDomesticHandlingFee() bool`

HasDomesticHandlingFee returns a boolean if a field has been set.

### GetInternationalHandlingFee

`func (o *ShopShippingProfilesResultsInner) GetInternationalHandlingFee() float32`

GetInternationalHandlingFee returns the InternationalHandlingFee field if non-nil, zero value otherwise.

### GetInternationalHandlingFeeOk

`func (o *ShopShippingProfilesResultsInner) GetInternationalHandlingFeeOk() (*float32, bool)`

GetInternationalHandlingFeeOk returns a tuple with the InternationalHandlingFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInternationalHandlingFee

`func (o *ShopShippingProfilesResultsInner) SetInternationalHandlingFee(v float32)`

SetInternationalHandlingFee sets InternationalHandlingFee field to given value.

### HasInternationalHandlingFee

`func (o *ShopShippingProfilesResultsInner) HasInternationalHandlingFee() bool`

HasInternationalHandlingFee returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


