# ShopListingWithAssociationsShippingProfile

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

### NewShopListingWithAssociationsShippingProfile

`func NewShopListingWithAssociationsShippingProfile() *ShopListingWithAssociationsShippingProfile`

NewShopListingWithAssociationsShippingProfile instantiates a new ShopListingWithAssociationsShippingProfile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingWithAssociationsShippingProfileWithDefaults

`func NewShopListingWithAssociationsShippingProfileWithDefaults() *ShopListingWithAssociationsShippingProfile`

NewShopListingWithAssociationsShippingProfileWithDefaults instantiates a new ShopListingWithAssociationsShippingProfile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShippingProfileId

`func (o *ShopListingWithAssociationsShippingProfile) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopListingWithAssociationsShippingProfile) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopListingWithAssociationsShippingProfile) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopListingWithAssociationsShippingProfile) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### GetTitle

`func (o *ShopListingWithAssociationsShippingProfile) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopListingWithAssociationsShippingProfile) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopListingWithAssociationsShippingProfile) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopListingWithAssociationsShippingProfile) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *ShopListingWithAssociationsShippingProfile) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *ShopListingWithAssociationsShippingProfile) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetUserId

`func (o *ShopListingWithAssociationsShippingProfile) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ShopListingWithAssociationsShippingProfile) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ShopListingWithAssociationsShippingProfile) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ShopListingWithAssociationsShippingProfile) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetMinProcessingDays

`func (o *ShopListingWithAssociationsShippingProfile) GetMinProcessingDays() int32`

GetMinProcessingDays returns the MinProcessingDays field if non-nil, zero value otherwise.

### GetMinProcessingDaysOk

`func (o *ShopListingWithAssociationsShippingProfile) GetMinProcessingDaysOk() (*int32, bool)`

GetMinProcessingDaysOk returns a tuple with the MinProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinProcessingDays

`func (o *ShopListingWithAssociationsShippingProfile) SetMinProcessingDays(v int32)`

SetMinProcessingDays sets MinProcessingDays field to given value.

### HasMinProcessingDays

`func (o *ShopListingWithAssociationsShippingProfile) HasMinProcessingDays() bool`

HasMinProcessingDays returns a boolean if a field has been set.

### SetMinProcessingDaysNil

`func (o *ShopListingWithAssociationsShippingProfile) SetMinProcessingDaysNil(b bool)`

 SetMinProcessingDaysNil sets the value for MinProcessingDays to be an explicit nil

### UnsetMinProcessingDays
`func (o *ShopListingWithAssociationsShippingProfile) UnsetMinProcessingDays()`

UnsetMinProcessingDays ensures that no value is present for MinProcessingDays, not even an explicit nil
### GetMaxProcessingDays

`func (o *ShopListingWithAssociationsShippingProfile) GetMaxProcessingDays() int32`

GetMaxProcessingDays returns the MaxProcessingDays field if non-nil, zero value otherwise.

### GetMaxProcessingDaysOk

`func (o *ShopListingWithAssociationsShippingProfile) GetMaxProcessingDaysOk() (*int32, bool)`

GetMaxProcessingDaysOk returns a tuple with the MaxProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxProcessingDays

`func (o *ShopListingWithAssociationsShippingProfile) SetMaxProcessingDays(v int32)`

SetMaxProcessingDays sets MaxProcessingDays field to given value.

### HasMaxProcessingDays

`func (o *ShopListingWithAssociationsShippingProfile) HasMaxProcessingDays() bool`

HasMaxProcessingDays returns a boolean if a field has been set.

### SetMaxProcessingDaysNil

`func (o *ShopListingWithAssociationsShippingProfile) SetMaxProcessingDaysNil(b bool)`

 SetMaxProcessingDaysNil sets the value for MaxProcessingDays to be an explicit nil

### UnsetMaxProcessingDays
`func (o *ShopListingWithAssociationsShippingProfile) UnsetMaxProcessingDays()`

UnsetMaxProcessingDays ensures that no value is present for MaxProcessingDays, not even an explicit nil
### GetProcessingDaysDisplayLabel

`func (o *ShopListingWithAssociationsShippingProfile) GetProcessingDaysDisplayLabel() string`

GetProcessingDaysDisplayLabel returns the ProcessingDaysDisplayLabel field if non-nil, zero value otherwise.

### GetProcessingDaysDisplayLabelOk

`func (o *ShopListingWithAssociationsShippingProfile) GetProcessingDaysDisplayLabelOk() (*string, bool)`

GetProcessingDaysDisplayLabelOk returns a tuple with the ProcessingDaysDisplayLabel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessingDaysDisplayLabel

`func (o *ShopListingWithAssociationsShippingProfile) SetProcessingDaysDisplayLabel(v string)`

SetProcessingDaysDisplayLabel sets ProcessingDaysDisplayLabel field to given value.

### HasProcessingDaysDisplayLabel

`func (o *ShopListingWithAssociationsShippingProfile) HasProcessingDaysDisplayLabel() bool`

HasProcessingDaysDisplayLabel returns a boolean if a field has been set.

### GetOriginCountryIso

`func (o *ShopListingWithAssociationsShippingProfile) GetOriginCountryIso() string`

GetOriginCountryIso returns the OriginCountryIso field if non-nil, zero value otherwise.

### GetOriginCountryIsoOk

`func (o *ShopListingWithAssociationsShippingProfile) GetOriginCountryIsoOk() (*string, bool)`

GetOriginCountryIsoOk returns a tuple with the OriginCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginCountryIso

`func (o *ShopListingWithAssociationsShippingProfile) SetOriginCountryIso(v string)`

SetOriginCountryIso sets OriginCountryIso field to given value.

### HasOriginCountryIso

`func (o *ShopListingWithAssociationsShippingProfile) HasOriginCountryIso() bool`

HasOriginCountryIso returns a boolean if a field has been set.

### GetIsDeleted

`func (o *ShopListingWithAssociationsShippingProfile) GetIsDeleted() bool`

GetIsDeleted returns the IsDeleted field if non-nil, zero value otherwise.

### GetIsDeletedOk

`func (o *ShopListingWithAssociationsShippingProfile) GetIsDeletedOk() (*bool, bool)`

GetIsDeletedOk returns a tuple with the IsDeleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDeleted

`func (o *ShopListingWithAssociationsShippingProfile) SetIsDeleted(v bool)`

SetIsDeleted sets IsDeleted field to given value.

### HasIsDeleted

`func (o *ShopListingWithAssociationsShippingProfile) HasIsDeleted() bool`

HasIsDeleted returns a boolean if a field has been set.

### GetShippingProfileDestinations

`func (o *ShopListingWithAssociationsShippingProfile) GetShippingProfileDestinations() []ShopShippingProfileShippingProfileDestinationsInner`

GetShippingProfileDestinations returns the ShippingProfileDestinations field if non-nil, zero value otherwise.

### GetShippingProfileDestinationsOk

`func (o *ShopListingWithAssociationsShippingProfile) GetShippingProfileDestinationsOk() (*[]ShopShippingProfileShippingProfileDestinationsInner, bool)`

GetShippingProfileDestinationsOk returns a tuple with the ShippingProfileDestinations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileDestinations

`func (o *ShopListingWithAssociationsShippingProfile) SetShippingProfileDestinations(v []ShopShippingProfileShippingProfileDestinationsInner)`

SetShippingProfileDestinations sets ShippingProfileDestinations field to given value.

### HasShippingProfileDestinations

`func (o *ShopListingWithAssociationsShippingProfile) HasShippingProfileDestinations() bool`

HasShippingProfileDestinations returns a boolean if a field has been set.

### GetShippingProfileUpgrades

`func (o *ShopListingWithAssociationsShippingProfile) GetShippingProfileUpgrades() []ShopShippingProfileShippingProfileUpgradesInner`

GetShippingProfileUpgrades returns the ShippingProfileUpgrades field if non-nil, zero value otherwise.

### GetShippingProfileUpgradesOk

`func (o *ShopListingWithAssociationsShippingProfile) GetShippingProfileUpgradesOk() (*[]ShopShippingProfileShippingProfileUpgradesInner, bool)`

GetShippingProfileUpgradesOk returns a tuple with the ShippingProfileUpgrades field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileUpgrades

`func (o *ShopListingWithAssociationsShippingProfile) SetShippingProfileUpgrades(v []ShopShippingProfileShippingProfileUpgradesInner)`

SetShippingProfileUpgrades sets ShippingProfileUpgrades field to given value.

### HasShippingProfileUpgrades

`func (o *ShopListingWithAssociationsShippingProfile) HasShippingProfileUpgrades() bool`

HasShippingProfileUpgrades returns a boolean if a field has been set.

### GetOriginPostalCode

`func (o *ShopListingWithAssociationsShippingProfile) GetOriginPostalCode() string`

GetOriginPostalCode returns the OriginPostalCode field if non-nil, zero value otherwise.

### GetOriginPostalCodeOk

`func (o *ShopListingWithAssociationsShippingProfile) GetOriginPostalCodeOk() (*string, bool)`

GetOriginPostalCodeOk returns a tuple with the OriginPostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginPostalCode

`func (o *ShopListingWithAssociationsShippingProfile) SetOriginPostalCode(v string)`

SetOriginPostalCode sets OriginPostalCode field to given value.

### HasOriginPostalCode

`func (o *ShopListingWithAssociationsShippingProfile) HasOriginPostalCode() bool`

HasOriginPostalCode returns a boolean if a field has been set.

### SetOriginPostalCodeNil

`func (o *ShopListingWithAssociationsShippingProfile) SetOriginPostalCodeNil(b bool)`

 SetOriginPostalCodeNil sets the value for OriginPostalCode to be an explicit nil

### UnsetOriginPostalCode
`func (o *ShopListingWithAssociationsShippingProfile) UnsetOriginPostalCode()`

UnsetOriginPostalCode ensures that no value is present for OriginPostalCode, not even an explicit nil
### GetProfileType

`func (o *ShopListingWithAssociationsShippingProfile) GetProfileType() string`

GetProfileType returns the ProfileType field if non-nil, zero value otherwise.

### GetProfileTypeOk

`func (o *ShopListingWithAssociationsShippingProfile) GetProfileTypeOk() (*string, bool)`

GetProfileTypeOk returns a tuple with the ProfileType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileType

`func (o *ShopListingWithAssociationsShippingProfile) SetProfileType(v string)`

SetProfileType sets ProfileType field to given value.

### HasProfileType

`func (o *ShopListingWithAssociationsShippingProfile) HasProfileType() bool`

HasProfileType returns a boolean if a field has been set.

### GetDomesticHandlingFee

`func (o *ShopListingWithAssociationsShippingProfile) GetDomesticHandlingFee() float32`

GetDomesticHandlingFee returns the DomesticHandlingFee field if non-nil, zero value otherwise.

### GetDomesticHandlingFeeOk

`func (o *ShopListingWithAssociationsShippingProfile) GetDomesticHandlingFeeOk() (*float32, bool)`

GetDomesticHandlingFeeOk returns a tuple with the DomesticHandlingFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomesticHandlingFee

`func (o *ShopListingWithAssociationsShippingProfile) SetDomesticHandlingFee(v float32)`

SetDomesticHandlingFee sets DomesticHandlingFee field to given value.

### HasDomesticHandlingFee

`func (o *ShopListingWithAssociationsShippingProfile) HasDomesticHandlingFee() bool`

HasDomesticHandlingFee returns a boolean if a field has been set.

### GetInternationalHandlingFee

`func (o *ShopListingWithAssociationsShippingProfile) GetInternationalHandlingFee() float32`

GetInternationalHandlingFee returns the InternationalHandlingFee field if non-nil, zero value otherwise.

### GetInternationalHandlingFeeOk

`func (o *ShopListingWithAssociationsShippingProfile) GetInternationalHandlingFeeOk() (*float32, bool)`

GetInternationalHandlingFeeOk returns a tuple with the InternationalHandlingFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInternationalHandlingFee

`func (o *ShopListingWithAssociationsShippingProfile) SetInternationalHandlingFee(v float32)`

SetInternationalHandlingFee sets InternationalHandlingFee field to given value.

### HasInternationalHandlingFee

`func (o *ShopListingWithAssociationsShippingProfile) HasInternationalHandlingFee() bool`

HasInternationalHandlingFee returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


