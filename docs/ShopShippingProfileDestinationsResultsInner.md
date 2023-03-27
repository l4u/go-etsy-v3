# ShopShippingProfileDestinationsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShippingProfileDestinationId** | Pointer to **int32** | The numeric ID of the shipping profile destination in the [shipping profile](/documentation/reference#tag/Shop-ShippingProfile) associated with the listing. | [optional] 
**ShippingProfileId** | Pointer to **int32** | The numeric ID of the shipping profile. | [optional] 
**OriginCountryIso** | Pointer to **string** | The ISO code of the country from which the listing ships. | [optional] 
**DestinationCountryIso** | Pointer to **string** | The ISO code of the country to which the listing ships. If null, request sets destination to destination_region. Required if destination_region is null or not provided. | [optional] 
**DestinationRegion** | Pointer to **string** | The code of the region to which the listing ships. A region represents a set of countries. Supported regions are Europe Union and Non-Europe Union (countries in Europe not in EU). If \\&#x60;none\\&#x60;, request sets destination to destination_country_iso. Required if destination_country_iso is null or not provided. | [optional] 
**PrimaryCost** | Pointer to [**ShopShippingProfileDestinationPrimaryCost**](ShopShippingProfileDestinationPrimaryCost.md) |  | [optional] 
**SecondaryCost** | Pointer to [**ShopShippingProfileDestinationSecondaryCost**](ShopShippingProfileDestinationSecondaryCost.md) |  | [optional] 
**ShippingCarrierId** | Pointer to **NullableInt32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [optional] 
**MailClass** | Pointer to **NullableString** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [optional] 
**MinDeliveryDays** | Pointer to **NullableInt32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | [optional] 
**MaxDeliveryDays** | Pointer to **NullableInt32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | [optional] 

## Methods

### NewShopShippingProfileDestinationsResultsInner

`func NewShopShippingProfileDestinationsResultsInner() *ShopShippingProfileDestinationsResultsInner`

NewShopShippingProfileDestinationsResultsInner instantiates a new ShopShippingProfileDestinationsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopShippingProfileDestinationsResultsInnerWithDefaults

`func NewShopShippingProfileDestinationsResultsInnerWithDefaults() *ShopShippingProfileDestinationsResultsInner`

NewShopShippingProfileDestinationsResultsInnerWithDefaults instantiates a new ShopShippingProfileDestinationsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShippingProfileDestinationId

`func (o *ShopShippingProfileDestinationsResultsInner) GetShippingProfileDestinationId() int32`

GetShippingProfileDestinationId returns the ShippingProfileDestinationId field if non-nil, zero value otherwise.

### GetShippingProfileDestinationIdOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetShippingProfileDestinationIdOk() (*int32, bool)`

GetShippingProfileDestinationIdOk returns a tuple with the ShippingProfileDestinationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileDestinationId

`func (o *ShopShippingProfileDestinationsResultsInner) SetShippingProfileDestinationId(v int32)`

SetShippingProfileDestinationId sets ShippingProfileDestinationId field to given value.

### HasShippingProfileDestinationId

`func (o *ShopShippingProfileDestinationsResultsInner) HasShippingProfileDestinationId() bool`

HasShippingProfileDestinationId returns a boolean if a field has been set.

### GetShippingProfileId

`func (o *ShopShippingProfileDestinationsResultsInner) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopShippingProfileDestinationsResultsInner) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopShippingProfileDestinationsResultsInner) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### GetOriginCountryIso

`func (o *ShopShippingProfileDestinationsResultsInner) GetOriginCountryIso() string`

GetOriginCountryIso returns the OriginCountryIso field if non-nil, zero value otherwise.

### GetOriginCountryIsoOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetOriginCountryIsoOk() (*string, bool)`

GetOriginCountryIsoOk returns a tuple with the OriginCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginCountryIso

`func (o *ShopShippingProfileDestinationsResultsInner) SetOriginCountryIso(v string)`

SetOriginCountryIso sets OriginCountryIso field to given value.

### HasOriginCountryIso

`func (o *ShopShippingProfileDestinationsResultsInner) HasOriginCountryIso() bool`

HasOriginCountryIso returns a boolean if a field has been set.

### GetDestinationCountryIso

`func (o *ShopShippingProfileDestinationsResultsInner) GetDestinationCountryIso() string`

GetDestinationCountryIso returns the DestinationCountryIso field if non-nil, zero value otherwise.

### GetDestinationCountryIsoOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetDestinationCountryIsoOk() (*string, bool)`

GetDestinationCountryIsoOk returns a tuple with the DestinationCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDestinationCountryIso

`func (o *ShopShippingProfileDestinationsResultsInner) SetDestinationCountryIso(v string)`

SetDestinationCountryIso sets DestinationCountryIso field to given value.

### HasDestinationCountryIso

`func (o *ShopShippingProfileDestinationsResultsInner) HasDestinationCountryIso() bool`

HasDestinationCountryIso returns a boolean if a field has been set.

### GetDestinationRegion

`func (o *ShopShippingProfileDestinationsResultsInner) GetDestinationRegion() string`

GetDestinationRegion returns the DestinationRegion field if non-nil, zero value otherwise.

### GetDestinationRegionOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetDestinationRegionOk() (*string, bool)`

GetDestinationRegionOk returns a tuple with the DestinationRegion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDestinationRegion

`func (o *ShopShippingProfileDestinationsResultsInner) SetDestinationRegion(v string)`

SetDestinationRegion sets DestinationRegion field to given value.

### HasDestinationRegion

`func (o *ShopShippingProfileDestinationsResultsInner) HasDestinationRegion() bool`

HasDestinationRegion returns a boolean if a field has been set.

### GetPrimaryCost

`func (o *ShopShippingProfileDestinationsResultsInner) GetPrimaryCost() ShopShippingProfileDestinationPrimaryCost`

GetPrimaryCost returns the PrimaryCost field if non-nil, zero value otherwise.

### GetPrimaryCostOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetPrimaryCostOk() (*ShopShippingProfileDestinationPrimaryCost, bool)`

GetPrimaryCostOk returns a tuple with the PrimaryCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryCost

`func (o *ShopShippingProfileDestinationsResultsInner) SetPrimaryCost(v ShopShippingProfileDestinationPrimaryCost)`

SetPrimaryCost sets PrimaryCost field to given value.

### HasPrimaryCost

`func (o *ShopShippingProfileDestinationsResultsInner) HasPrimaryCost() bool`

HasPrimaryCost returns a boolean if a field has been set.

### GetSecondaryCost

`func (o *ShopShippingProfileDestinationsResultsInner) GetSecondaryCost() ShopShippingProfileDestinationSecondaryCost`

GetSecondaryCost returns the SecondaryCost field if non-nil, zero value otherwise.

### GetSecondaryCostOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetSecondaryCostOk() (*ShopShippingProfileDestinationSecondaryCost, bool)`

GetSecondaryCostOk returns a tuple with the SecondaryCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryCost

`func (o *ShopShippingProfileDestinationsResultsInner) SetSecondaryCost(v ShopShippingProfileDestinationSecondaryCost)`

SetSecondaryCost sets SecondaryCost field to given value.

### HasSecondaryCost

`func (o *ShopShippingProfileDestinationsResultsInner) HasSecondaryCost() bool`

HasSecondaryCost returns a boolean if a field has been set.

### GetShippingCarrierId

`func (o *ShopShippingProfileDestinationsResultsInner) GetShippingCarrierId() int32`

GetShippingCarrierId returns the ShippingCarrierId field if non-nil, zero value otherwise.

### GetShippingCarrierIdOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetShippingCarrierIdOk() (*int32, bool)`

GetShippingCarrierIdOk returns a tuple with the ShippingCarrierId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingCarrierId

`func (o *ShopShippingProfileDestinationsResultsInner) SetShippingCarrierId(v int32)`

SetShippingCarrierId sets ShippingCarrierId field to given value.

### HasShippingCarrierId

`func (o *ShopShippingProfileDestinationsResultsInner) HasShippingCarrierId() bool`

HasShippingCarrierId returns a boolean if a field has been set.

### SetShippingCarrierIdNil

`func (o *ShopShippingProfileDestinationsResultsInner) SetShippingCarrierIdNil(b bool)`

 SetShippingCarrierIdNil sets the value for ShippingCarrierId to be an explicit nil

### UnsetShippingCarrierId
`func (o *ShopShippingProfileDestinationsResultsInner) UnsetShippingCarrierId()`

UnsetShippingCarrierId ensures that no value is present for ShippingCarrierId, not even an explicit nil
### GetMailClass

`func (o *ShopShippingProfileDestinationsResultsInner) GetMailClass() string`

GetMailClass returns the MailClass field if non-nil, zero value otherwise.

### GetMailClassOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetMailClassOk() (*string, bool)`

GetMailClassOk returns a tuple with the MailClass field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMailClass

`func (o *ShopShippingProfileDestinationsResultsInner) SetMailClass(v string)`

SetMailClass sets MailClass field to given value.

### HasMailClass

`func (o *ShopShippingProfileDestinationsResultsInner) HasMailClass() bool`

HasMailClass returns a boolean if a field has been set.

### SetMailClassNil

`func (o *ShopShippingProfileDestinationsResultsInner) SetMailClassNil(b bool)`

 SetMailClassNil sets the value for MailClass to be an explicit nil

### UnsetMailClass
`func (o *ShopShippingProfileDestinationsResultsInner) UnsetMailClass()`

UnsetMailClass ensures that no value is present for MailClass, not even an explicit nil
### GetMinDeliveryDays

`func (o *ShopShippingProfileDestinationsResultsInner) GetMinDeliveryDays() int32`

GetMinDeliveryDays returns the MinDeliveryDays field if non-nil, zero value otherwise.

### GetMinDeliveryDaysOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetMinDeliveryDaysOk() (*int32, bool)`

GetMinDeliveryDaysOk returns a tuple with the MinDeliveryDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinDeliveryDays

`func (o *ShopShippingProfileDestinationsResultsInner) SetMinDeliveryDays(v int32)`

SetMinDeliveryDays sets MinDeliveryDays field to given value.

### HasMinDeliveryDays

`func (o *ShopShippingProfileDestinationsResultsInner) HasMinDeliveryDays() bool`

HasMinDeliveryDays returns a boolean if a field has been set.

### SetMinDeliveryDaysNil

`func (o *ShopShippingProfileDestinationsResultsInner) SetMinDeliveryDaysNil(b bool)`

 SetMinDeliveryDaysNil sets the value for MinDeliveryDays to be an explicit nil

### UnsetMinDeliveryDays
`func (o *ShopShippingProfileDestinationsResultsInner) UnsetMinDeliveryDays()`

UnsetMinDeliveryDays ensures that no value is present for MinDeliveryDays, not even an explicit nil
### GetMaxDeliveryDays

`func (o *ShopShippingProfileDestinationsResultsInner) GetMaxDeliveryDays() int32`

GetMaxDeliveryDays returns the MaxDeliveryDays field if non-nil, zero value otherwise.

### GetMaxDeliveryDaysOk

`func (o *ShopShippingProfileDestinationsResultsInner) GetMaxDeliveryDaysOk() (*int32, bool)`

GetMaxDeliveryDaysOk returns a tuple with the MaxDeliveryDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxDeliveryDays

`func (o *ShopShippingProfileDestinationsResultsInner) SetMaxDeliveryDays(v int32)`

SetMaxDeliveryDays sets MaxDeliveryDays field to given value.

### HasMaxDeliveryDays

`func (o *ShopShippingProfileDestinationsResultsInner) HasMaxDeliveryDays() bool`

HasMaxDeliveryDays returns a boolean if a field has been set.

### SetMaxDeliveryDaysNil

`func (o *ShopShippingProfileDestinationsResultsInner) SetMaxDeliveryDaysNil(b bool)`

 SetMaxDeliveryDaysNil sets the value for MaxDeliveryDays to be an explicit nil

### UnsetMaxDeliveryDays
`func (o *ShopShippingProfileDestinationsResultsInner) UnsetMaxDeliveryDays()`

UnsetMaxDeliveryDays ensures that no value is present for MaxDeliveryDays, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


