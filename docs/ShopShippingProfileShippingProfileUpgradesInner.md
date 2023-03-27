# ShopShippingProfileShippingProfileUpgradesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShippingProfileId** | Pointer to **int32** | The numeric ID of the base shipping profile. | [optional] 
**UpgradeId** | Pointer to **int32** | The numeric ID that is associated with a shipping upgrade | [optional] 
**UpgradeName** | Pointer to **string** | Name for the shipping upgrade shown to shoppers at checkout, e.g. USPS Priority. | [optional] 
**Type** | Pointer to **string** | The type of the shipping upgrade. Domestic (0) or international (1). | [optional] 
**Rank** | Pointer to **int32** | The positive non-zero numeric position in the images displayed in a listing, with rank 1 images appearing in the left-most position in a listing. | [optional] 
**Language** | Pointer to **string** | The IETF language tag for the language of the shipping profile. Ex: &#x60;de&#x60;, &#x60;en&#x60;, &#x60;es&#x60;, &#x60;fr&#x60;, &#x60;it&#x60;, &#x60;ja&#x60;, &#x60;nl&#x60;, &#x60;pl&#x60;, &#x60;pt&#x60; | [optional] 
**Price** | Pointer to [**ShopShippingProfileUpgradePrice**](ShopShippingProfileUpgradePrice.md) |  | [optional] 
**SecondaryPrice** | Pointer to [**ShopShippingProfileUpgradeSecondaryPrice**](ShopShippingProfileUpgradeSecondaryPrice.md) |  | [optional] 
**ShippingCarrierId** | Pointer to **NullableInt32** | The unique ID of a supported shipping carrier, which is used to calculate an Estimated Delivery Date. **Required with &#x60;mail_class&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [optional] 
**MailClass** | Pointer to **NullableString** | The unique ID string of a shipping carrier&#39;s mail class, which is used to calculate an estimated delivery date. **Required with &#x60;shipping_carrier_id&#x60;** if &#x60;min_delivery_days&#x60; and &#x60;max_delivery_days&#x60; are null. | [optional] 
**MinDeliveryDays** | Pointer to **NullableInt32** | The minimum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;max_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | [optional] 
**MaxDeliveryDays** | Pointer to **NullableInt32** | The maximum number of business days a buyer can expect to wait to receive their purchased item once it has shipped. **Required with &#x60;min_delivery_days&#x60;** if &#x60;mail_class&#x60; is null. | [optional] 

## Methods

### NewShopShippingProfileShippingProfileUpgradesInner

`func NewShopShippingProfileShippingProfileUpgradesInner() *ShopShippingProfileShippingProfileUpgradesInner`

NewShopShippingProfileShippingProfileUpgradesInner instantiates a new ShopShippingProfileShippingProfileUpgradesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopShippingProfileShippingProfileUpgradesInnerWithDefaults

`func NewShopShippingProfileShippingProfileUpgradesInnerWithDefaults() *ShopShippingProfileShippingProfileUpgradesInner`

NewShopShippingProfileShippingProfileUpgradesInnerWithDefaults instantiates a new ShopShippingProfileShippingProfileUpgradesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShippingProfileId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### GetUpgradeId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetUpgradeId() int32`

GetUpgradeId returns the UpgradeId field if non-nil, zero value otherwise.

### GetUpgradeIdOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetUpgradeIdOk() (*int32, bool)`

GetUpgradeIdOk returns a tuple with the UpgradeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpgradeId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetUpgradeId(v int32)`

SetUpgradeId sets UpgradeId field to given value.

### HasUpgradeId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasUpgradeId() bool`

HasUpgradeId returns a boolean if a field has been set.

### GetUpgradeName

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetUpgradeName() string`

GetUpgradeName returns the UpgradeName field if non-nil, zero value otherwise.

### GetUpgradeNameOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetUpgradeNameOk() (*string, bool)`

GetUpgradeNameOk returns a tuple with the UpgradeName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpgradeName

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetUpgradeName(v string)`

SetUpgradeName sets UpgradeName field to given value.

### HasUpgradeName

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasUpgradeName() bool`

HasUpgradeName returns a boolean if a field has been set.

### GetType

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasType() bool`

HasType returns a boolean if a field has been set.

### GetRank

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetRank() int32`

GetRank returns the Rank field if non-nil, zero value otherwise.

### GetRankOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetRankOk() (*int32, bool)`

GetRankOk returns a tuple with the Rank field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRank

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetRank(v int32)`

SetRank sets Rank field to given value.

### HasRank

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasRank() bool`

HasRank returns a boolean if a field has been set.

### GetLanguage

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### GetPrice

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetPrice() ShopShippingProfileUpgradePrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetPriceOk() (*ShopShippingProfileUpgradePrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetPrice(v ShopShippingProfileUpgradePrice)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetSecondaryPrice

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetSecondaryPrice() ShopShippingProfileUpgradeSecondaryPrice`

GetSecondaryPrice returns the SecondaryPrice field if non-nil, zero value otherwise.

### GetSecondaryPriceOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetSecondaryPriceOk() (*ShopShippingProfileUpgradeSecondaryPrice, bool)`

GetSecondaryPriceOk returns a tuple with the SecondaryPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryPrice

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetSecondaryPrice(v ShopShippingProfileUpgradeSecondaryPrice)`

SetSecondaryPrice sets SecondaryPrice field to given value.

### HasSecondaryPrice

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasSecondaryPrice() bool`

HasSecondaryPrice returns a boolean if a field has been set.

### GetShippingCarrierId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetShippingCarrierId() int32`

GetShippingCarrierId returns the ShippingCarrierId field if non-nil, zero value otherwise.

### GetShippingCarrierIdOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetShippingCarrierIdOk() (*int32, bool)`

GetShippingCarrierIdOk returns a tuple with the ShippingCarrierId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingCarrierId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetShippingCarrierId(v int32)`

SetShippingCarrierId sets ShippingCarrierId field to given value.

### HasShippingCarrierId

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasShippingCarrierId() bool`

HasShippingCarrierId returns a boolean if a field has been set.

### SetShippingCarrierIdNil

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetShippingCarrierIdNil(b bool)`

 SetShippingCarrierIdNil sets the value for ShippingCarrierId to be an explicit nil

### UnsetShippingCarrierId
`func (o *ShopShippingProfileShippingProfileUpgradesInner) UnsetShippingCarrierId()`

UnsetShippingCarrierId ensures that no value is present for ShippingCarrierId, not even an explicit nil
### GetMailClass

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetMailClass() string`

GetMailClass returns the MailClass field if non-nil, zero value otherwise.

### GetMailClassOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetMailClassOk() (*string, bool)`

GetMailClassOk returns a tuple with the MailClass field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMailClass

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetMailClass(v string)`

SetMailClass sets MailClass field to given value.

### HasMailClass

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasMailClass() bool`

HasMailClass returns a boolean if a field has been set.

### SetMailClassNil

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetMailClassNil(b bool)`

 SetMailClassNil sets the value for MailClass to be an explicit nil

### UnsetMailClass
`func (o *ShopShippingProfileShippingProfileUpgradesInner) UnsetMailClass()`

UnsetMailClass ensures that no value is present for MailClass, not even an explicit nil
### GetMinDeliveryDays

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetMinDeliveryDays() int32`

GetMinDeliveryDays returns the MinDeliveryDays field if non-nil, zero value otherwise.

### GetMinDeliveryDaysOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetMinDeliveryDaysOk() (*int32, bool)`

GetMinDeliveryDaysOk returns a tuple with the MinDeliveryDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinDeliveryDays

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetMinDeliveryDays(v int32)`

SetMinDeliveryDays sets MinDeliveryDays field to given value.

### HasMinDeliveryDays

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasMinDeliveryDays() bool`

HasMinDeliveryDays returns a boolean if a field has been set.

### SetMinDeliveryDaysNil

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetMinDeliveryDaysNil(b bool)`

 SetMinDeliveryDaysNil sets the value for MinDeliveryDays to be an explicit nil

### UnsetMinDeliveryDays
`func (o *ShopShippingProfileShippingProfileUpgradesInner) UnsetMinDeliveryDays()`

UnsetMinDeliveryDays ensures that no value is present for MinDeliveryDays, not even an explicit nil
### GetMaxDeliveryDays

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetMaxDeliveryDays() int32`

GetMaxDeliveryDays returns the MaxDeliveryDays field if non-nil, zero value otherwise.

### GetMaxDeliveryDaysOk

`func (o *ShopShippingProfileShippingProfileUpgradesInner) GetMaxDeliveryDaysOk() (*int32, bool)`

GetMaxDeliveryDaysOk returns a tuple with the MaxDeliveryDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxDeliveryDays

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetMaxDeliveryDays(v int32)`

SetMaxDeliveryDays sets MaxDeliveryDays field to given value.

### HasMaxDeliveryDays

`func (o *ShopShippingProfileShippingProfileUpgradesInner) HasMaxDeliveryDays() bool`

HasMaxDeliveryDays returns a boolean if a field has been set.

### SetMaxDeliveryDaysNil

`func (o *ShopShippingProfileShippingProfileUpgradesInner) SetMaxDeliveryDaysNil(b bool)`

 SetMaxDeliveryDaysNil sets the value for MaxDeliveryDays to be an explicit nil

### UnsetMaxDeliveryDays
`func (o *ShopShippingProfileShippingProfileUpgradesInner) UnsetMaxDeliveryDays()`

UnsetMaxDeliveryDays ensures that no value is present for MaxDeliveryDays, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


