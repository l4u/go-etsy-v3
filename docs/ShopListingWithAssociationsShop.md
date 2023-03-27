# ShopListingWithAssociationsShop

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShopId** | Pointer to **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | [optional] 
**UserId** | Pointer to **int32** | The numeric user ID of the [user](/documentation/reference#tag/User) who owns this shop. | [optional] 
**ShopName** | Pointer to **string** | The shop&#39;s name string. | [optional] 
**CreateDate** | Pointer to **int32** | The date and time this shop was created, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The date and time this shop was created, in epoch seconds. | [optional] 
**Title** | Pointer to **NullableString** | A brief heading string for the shop\\&#39;s main page. | [optional] 
**Announcement** | Pointer to **NullableString** | An announcement string to buyers that displays on the shop&#39;s homepage. | [optional] 
**CurrencyCode** | Pointer to **string** | The ISO (alphabetic) code for the shop&#39;s currency. The shop displays all prices in this currency by default. | [optional] 
**IsVacation** | Pointer to **bool** | When true, this shop is not accepting purchases. | [optional] 
**VacationMessage** | Pointer to **NullableString** | The shop&#39;s message string displayed when &#x60;is_vacation&#x60; is true. | [optional] 
**SaleMessage** | Pointer to **NullableString** | A message string sent to users who complete a purchase from this shop. | [optional] 
**DigitalSaleMessage** | Pointer to **NullableString** | A message string sent to users who purchase a digital item from this shop. | [optional] 
**UpdateDate** | Pointer to **int32** | The date and time of the last update to the shop, in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The date and time of the last update to the shop, in epoch seconds. | [optional] 
**ListingActiveCount** | Pointer to **int32** | The number of active listings in the shop. | [optional] 
**DigitalListingCount** | Pointer to **int32** | The number of digital listings in the shop. | [optional] 
**LoginName** | Pointer to **string** | The shop owner\\&#39;s login name string. | [optional] 
**AcceptsCustomRequests** | Pointer to **bool** | When true, the shop accepts customization requests. | [optional] 
**PolicyWelcome** | Pointer to **NullableString** | The shop&#39;s policy welcome string (may be blank). | [optional] 
**PolicyPayment** | Pointer to **NullableString** | The shop&#39;s payment policy string (may be blank). | [optional] 
**PolicyShipping** | Pointer to **NullableString** | The shop&#39;s shipping policy string (may be blank). | [optional] 
**PolicyRefunds** | Pointer to **NullableString** | The shop&#39;s refund policy string (may be blank). | [optional] 
**PolicyAdditional** | Pointer to **NullableString** | The shop&#39;s additional policies string (may be blank). | [optional] 
**PolicySellerInfo** | Pointer to **NullableString** | The shop&#39;s seller information string (may be blank). | [optional] 
**PolicyUpdateDate** | Pointer to **int32** | The date and time of the last update to the shop&#39;s policies, in epoch seconds. | [optional] 
**PolicyHasPrivateReceiptInfo** | Pointer to **bool** | When true, EU receipts display private info. | [optional] 
**HasUnstructuredPolicies** | Pointer to **bool** | When true, the shop displays additional unstructured policy fields. | [optional] 
**PolicyPrivacy** | Pointer to **NullableString** | The shop&#39;s privacy policy string (may be blank). | [optional] 
**VacationAutoreply** | Pointer to **NullableString** | The shop&#39;s automatic reply string displayed in new conversations when &#x60;is_vacation&#x60; is true. | [optional] 
**Url** | Pointer to **string** | The URL string for this shop. | [optional] 
**ImageUrl760x100** | Pointer to **NullableString** | The URL string for this shop&#39;s banner image. | [optional] 
**NumFavorers** | Pointer to **int32** | The number of users who marked this shop a favorite. | [optional] 
**Languages** | Pointer to **[]string** | A list of language strings for the shop&#39;s enrolled languages where the default shop language is the first element in the array. | [optional] 
**IconUrlFullxfull** | Pointer to **NullableString** | The URL string for this shop&#39;s icon image. | [optional] 
**IsUsingStructuredPolicies** | Pointer to **bool** | When true, the shop accepted using structured policies. | [optional] 
**HasOnboardedStructuredPolicies** | Pointer to **bool** | When true, the shop accepted OR declined after viewing structured policies onboarding. | [optional] 
**IncludeDisputeFormLink** | Pointer to **bool** | When true, this shop\\&#39;s policies include a link to an EU online dispute form. | [optional] 
**IsDirectCheckoutOnboarded** | Pointer to **bool** | (**DEPRECATED: Replaced by _is_etsy_payments_onboarded_.) When true, the shop has onboarded onto Etsy Payments. | [optional] 
**IsEtsyPaymentsOnboarded** | Pointer to **bool** | When true, the shop has onboarded onto Etsy Payments. | [optional] 
**IsCalculatedEligible** | Pointer to **bool** | When true, the shop is eligible for calculated shipping profiles. (Only available in the US and Canada) | [optional] 
**IsOptedInToBuyerPromise** | Pointer to **bool** | When true, the shop opted in to buyer promise. | [optional] 
**IsShopUsBased** | Pointer to **bool** | When true, the shop is based in the US. | [optional] 
**TransactionSoldCount** | Pointer to **int32** | The total number of sales ([transactions](/documentation/reference#tag/Shop-Receipt-Transactions)) for this shop. | [optional] 
**ShippingFromCountryIso** | Pointer to **NullableString** | The country iso the shop is shipping from. | [optional] 
**ShopLocationCountryIso** | Pointer to **NullableString** | The country iso where the shop is located. | [optional] 
**ReviewCount** | Pointer to **NullableInt32** | Number of reviews of shop listings in the past year. | [optional] 
**ReviewAverage** | Pointer to **NullableFloat32** | Average rating based on reviews of shop listings in the past year. | [optional] 

## Methods

### NewShopListingWithAssociationsShop

`func NewShopListingWithAssociationsShop() *ShopListingWithAssociationsShop`

NewShopListingWithAssociationsShop instantiates a new ShopListingWithAssociationsShop object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingWithAssociationsShopWithDefaults

`func NewShopListingWithAssociationsShopWithDefaults() *ShopListingWithAssociationsShop`

NewShopListingWithAssociationsShopWithDefaults instantiates a new ShopListingWithAssociationsShop object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShopId

`func (o *ShopListingWithAssociationsShop) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *ShopListingWithAssociationsShop) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *ShopListingWithAssociationsShop) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *ShopListingWithAssociationsShop) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetUserId

`func (o *ShopListingWithAssociationsShop) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ShopListingWithAssociationsShop) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ShopListingWithAssociationsShop) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ShopListingWithAssociationsShop) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetShopName

`func (o *ShopListingWithAssociationsShop) GetShopName() string`

GetShopName returns the ShopName field if non-nil, zero value otherwise.

### GetShopNameOk

`func (o *ShopListingWithAssociationsShop) GetShopNameOk() (*string, bool)`

GetShopNameOk returns a tuple with the ShopName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopName

`func (o *ShopListingWithAssociationsShop) SetShopName(v string)`

SetShopName sets ShopName field to given value.

### HasShopName

`func (o *ShopListingWithAssociationsShop) HasShopName() bool`

HasShopName returns a boolean if a field has been set.

### GetCreateDate

`func (o *ShopListingWithAssociationsShop) GetCreateDate() int32`

GetCreateDate returns the CreateDate field if non-nil, zero value otherwise.

### GetCreateDateOk

`func (o *ShopListingWithAssociationsShop) GetCreateDateOk() (*int32, bool)`

GetCreateDateOk returns a tuple with the CreateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateDate

`func (o *ShopListingWithAssociationsShop) SetCreateDate(v int32)`

SetCreateDate sets CreateDate field to given value.

### HasCreateDate

`func (o *ShopListingWithAssociationsShop) HasCreateDate() bool`

HasCreateDate returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopListingWithAssociationsShop) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopListingWithAssociationsShop) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopListingWithAssociationsShop) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopListingWithAssociationsShop) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetTitle

`func (o *ShopListingWithAssociationsShop) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopListingWithAssociationsShop) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopListingWithAssociationsShop) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopListingWithAssociationsShop) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *ShopListingWithAssociationsShop) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *ShopListingWithAssociationsShop) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetAnnouncement

`func (o *ShopListingWithAssociationsShop) GetAnnouncement() string`

GetAnnouncement returns the Announcement field if non-nil, zero value otherwise.

### GetAnnouncementOk

`func (o *ShopListingWithAssociationsShop) GetAnnouncementOk() (*string, bool)`

GetAnnouncementOk returns a tuple with the Announcement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnnouncement

`func (o *ShopListingWithAssociationsShop) SetAnnouncement(v string)`

SetAnnouncement sets Announcement field to given value.

### HasAnnouncement

`func (o *ShopListingWithAssociationsShop) HasAnnouncement() bool`

HasAnnouncement returns a boolean if a field has been set.

### SetAnnouncementNil

`func (o *ShopListingWithAssociationsShop) SetAnnouncementNil(b bool)`

 SetAnnouncementNil sets the value for Announcement to be an explicit nil

### UnsetAnnouncement
`func (o *ShopListingWithAssociationsShop) UnsetAnnouncement()`

UnsetAnnouncement ensures that no value is present for Announcement, not even an explicit nil
### GetCurrencyCode

`func (o *ShopListingWithAssociationsShop) GetCurrencyCode() string`

GetCurrencyCode returns the CurrencyCode field if non-nil, zero value otherwise.

### GetCurrencyCodeOk

`func (o *ShopListingWithAssociationsShop) GetCurrencyCodeOk() (*string, bool)`

GetCurrencyCodeOk returns a tuple with the CurrencyCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyCode

`func (o *ShopListingWithAssociationsShop) SetCurrencyCode(v string)`

SetCurrencyCode sets CurrencyCode field to given value.

### HasCurrencyCode

`func (o *ShopListingWithAssociationsShop) HasCurrencyCode() bool`

HasCurrencyCode returns a boolean if a field has been set.

### GetIsVacation

`func (o *ShopListingWithAssociationsShop) GetIsVacation() bool`

GetIsVacation returns the IsVacation field if non-nil, zero value otherwise.

### GetIsVacationOk

`func (o *ShopListingWithAssociationsShop) GetIsVacationOk() (*bool, bool)`

GetIsVacationOk returns a tuple with the IsVacation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsVacation

`func (o *ShopListingWithAssociationsShop) SetIsVacation(v bool)`

SetIsVacation sets IsVacation field to given value.

### HasIsVacation

`func (o *ShopListingWithAssociationsShop) HasIsVacation() bool`

HasIsVacation returns a boolean if a field has been set.

### GetVacationMessage

`func (o *ShopListingWithAssociationsShop) GetVacationMessage() string`

GetVacationMessage returns the VacationMessage field if non-nil, zero value otherwise.

### GetVacationMessageOk

`func (o *ShopListingWithAssociationsShop) GetVacationMessageOk() (*string, bool)`

GetVacationMessageOk returns a tuple with the VacationMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVacationMessage

`func (o *ShopListingWithAssociationsShop) SetVacationMessage(v string)`

SetVacationMessage sets VacationMessage field to given value.

### HasVacationMessage

`func (o *ShopListingWithAssociationsShop) HasVacationMessage() bool`

HasVacationMessage returns a boolean if a field has been set.

### SetVacationMessageNil

`func (o *ShopListingWithAssociationsShop) SetVacationMessageNil(b bool)`

 SetVacationMessageNil sets the value for VacationMessage to be an explicit nil

### UnsetVacationMessage
`func (o *ShopListingWithAssociationsShop) UnsetVacationMessage()`

UnsetVacationMessage ensures that no value is present for VacationMessage, not even an explicit nil
### GetSaleMessage

`func (o *ShopListingWithAssociationsShop) GetSaleMessage() string`

GetSaleMessage returns the SaleMessage field if non-nil, zero value otherwise.

### GetSaleMessageOk

`func (o *ShopListingWithAssociationsShop) GetSaleMessageOk() (*string, bool)`

GetSaleMessageOk returns a tuple with the SaleMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSaleMessage

`func (o *ShopListingWithAssociationsShop) SetSaleMessage(v string)`

SetSaleMessage sets SaleMessage field to given value.

### HasSaleMessage

`func (o *ShopListingWithAssociationsShop) HasSaleMessage() bool`

HasSaleMessage returns a boolean if a field has been set.

### SetSaleMessageNil

`func (o *ShopListingWithAssociationsShop) SetSaleMessageNil(b bool)`

 SetSaleMessageNil sets the value for SaleMessage to be an explicit nil

### UnsetSaleMessage
`func (o *ShopListingWithAssociationsShop) UnsetSaleMessage()`

UnsetSaleMessage ensures that no value is present for SaleMessage, not even an explicit nil
### GetDigitalSaleMessage

`func (o *ShopListingWithAssociationsShop) GetDigitalSaleMessage() string`

GetDigitalSaleMessage returns the DigitalSaleMessage field if non-nil, zero value otherwise.

### GetDigitalSaleMessageOk

`func (o *ShopListingWithAssociationsShop) GetDigitalSaleMessageOk() (*string, bool)`

GetDigitalSaleMessageOk returns a tuple with the DigitalSaleMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigitalSaleMessage

`func (o *ShopListingWithAssociationsShop) SetDigitalSaleMessage(v string)`

SetDigitalSaleMessage sets DigitalSaleMessage field to given value.

### HasDigitalSaleMessage

`func (o *ShopListingWithAssociationsShop) HasDigitalSaleMessage() bool`

HasDigitalSaleMessage returns a boolean if a field has been set.

### SetDigitalSaleMessageNil

`func (o *ShopListingWithAssociationsShop) SetDigitalSaleMessageNil(b bool)`

 SetDigitalSaleMessageNil sets the value for DigitalSaleMessage to be an explicit nil

### UnsetDigitalSaleMessage
`func (o *ShopListingWithAssociationsShop) UnsetDigitalSaleMessage()`

UnsetDigitalSaleMessage ensures that no value is present for DigitalSaleMessage, not even an explicit nil
### GetUpdateDate

`func (o *ShopListingWithAssociationsShop) GetUpdateDate() int32`

GetUpdateDate returns the UpdateDate field if non-nil, zero value otherwise.

### GetUpdateDateOk

`func (o *ShopListingWithAssociationsShop) GetUpdateDateOk() (*int32, bool)`

GetUpdateDateOk returns a tuple with the UpdateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateDate

`func (o *ShopListingWithAssociationsShop) SetUpdateDate(v int32)`

SetUpdateDate sets UpdateDate field to given value.

### HasUpdateDate

`func (o *ShopListingWithAssociationsShop) HasUpdateDate() bool`

HasUpdateDate returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *ShopListingWithAssociationsShop) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *ShopListingWithAssociationsShop) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *ShopListingWithAssociationsShop) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *ShopListingWithAssociationsShop) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetListingActiveCount

`func (o *ShopListingWithAssociationsShop) GetListingActiveCount() int32`

GetListingActiveCount returns the ListingActiveCount field if non-nil, zero value otherwise.

### GetListingActiveCountOk

`func (o *ShopListingWithAssociationsShop) GetListingActiveCountOk() (*int32, bool)`

GetListingActiveCountOk returns a tuple with the ListingActiveCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingActiveCount

`func (o *ShopListingWithAssociationsShop) SetListingActiveCount(v int32)`

SetListingActiveCount sets ListingActiveCount field to given value.

### HasListingActiveCount

`func (o *ShopListingWithAssociationsShop) HasListingActiveCount() bool`

HasListingActiveCount returns a boolean if a field has been set.

### GetDigitalListingCount

`func (o *ShopListingWithAssociationsShop) GetDigitalListingCount() int32`

GetDigitalListingCount returns the DigitalListingCount field if non-nil, zero value otherwise.

### GetDigitalListingCountOk

`func (o *ShopListingWithAssociationsShop) GetDigitalListingCountOk() (*int32, bool)`

GetDigitalListingCountOk returns a tuple with the DigitalListingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigitalListingCount

`func (o *ShopListingWithAssociationsShop) SetDigitalListingCount(v int32)`

SetDigitalListingCount sets DigitalListingCount field to given value.

### HasDigitalListingCount

`func (o *ShopListingWithAssociationsShop) HasDigitalListingCount() bool`

HasDigitalListingCount returns a boolean if a field has been set.

### GetLoginName

`func (o *ShopListingWithAssociationsShop) GetLoginName() string`

GetLoginName returns the LoginName field if non-nil, zero value otherwise.

### GetLoginNameOk

`func (o *ShopListingWithAssociationsShop) GetLoginNameOk() (*string, bool)`

GetLoginNameOk returns a tuple with the LoginName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoginName

`func (o *ShopListingWithAssociationsShop) SetLoginName(v string)`

SetLoginName sets LoginName field to given value.

### HasLoginName

`func (o *ShopListingWithAssociationsShop) HasLoginName() bool`

HasLoginName returns a boolean if a field has been set.

### GetAcceptsCustomRequests

`func (o *ShopListingWithAssociationsShop) GetAcceptsCustomRequests() bool`

GetAcceptsCustomRequests returns the AcceptsCustomRequests field if non-nil, zero value otherwise.

### GetAcceptsCustomRequestsOk

`func (o *ShopListingWithAssociationsShop) GetAcceptsCustomRequestsOk() (*bool, bool)`

GetAcceptsCustomRequestsOk returns a tuple with the AcceptsCustomRequests field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAcceptsCustomRequests

`func (o *ShopListingWithAssociationsShop) SetAcceptsCustomRequests(v bool)`

SetAcceptsCustomRequests sets AcceptsCustomRequests field to given value.

### HasAcceptsCustomRequests

`func (o *ShopListingWithAssociationsShop) HasAcceptsCustomRequests() bool`

HasAcceptsCustomRequests returns a boolean if a field has been set.

### GetPolicyWelcome

`func (o *ShopListingWithAssociationsShop) GetPolicyWelcome() string`

GetPolicyWelcome returns the PolicyWelcome field if non-nil, zero value otherwise.

### GetPolicyWelcomeOk

`func (o *ShopListingWithAssociationsShop) GetPolicyWelcomeOk() (*string, bool)`

GetPolicyWelcomeOk returns a tuple with the PolicyWelcome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyWelcome

`func (o *ShopListingWithAssociationsShop) SetPolicyWelcome(v string)`

SetPolicyWelcome sets PolicyWelcome field to given value.

### HasPolicyWelcome

`func (o *ShopListingWithAssociationsShop) HasPolicyWelcome() bool`

HasPolicyWelcome returns a boolean if a field has been set.

### SetPolicyWelcomeNil

`func (o *ShopListingWithAssociationsShop) SetPolicyWelcomeNil(b bool)`

 SetPolicyWelcomeNil sets the value for PolicyWelcome to be an explicit nil

### UnsetPolicyWelcome
`func (o *ShopListingWithAssociationsShop) UnsetPolicyWelcome()`

UnsetPolicyWelcome ensures that no value is present for PolicyWelcome, not even an explicit nil
### GetPolicyPayment

`func (o *ShopListingWithAssociationsShop) GetPolicyPayment() string`

GetPolicyPayment returns the PolicyPayment field if non-nil, zero value otherwise.

### GetPolicyPaymentOk

`func (o *ShopListingWithAssociationsShop) GetPolicyPaymentOk() (*string, bool)`

GetPolicyPaymentOk returns a tuple with the PolicyPayment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyPayment

`func (o *ShopListingWithAssociationsShop) SetPolicyPayment(v string)`

SetPolicyPayment sets PolicyPayment field to given value.

### HasPolicyPayment

`func (o *ShopListingWithAssociationsShop) HasPolicyPayment() bool`

HasPolicyPayment returns a boolean if a field has been set.

### SetPolicyPaymentNil

`func (o *ShopListingWithAssociationsShop) SetPolicyPaymentNil(b bool)`

 SetPolicyPaymentNil sets the value for PolicyPayment to be an explicit nil

### UnsetPolicyPayment
`func (o *ShopListingWithAssociationsShop) UnsetPolicyPayment()`

UnsetPolicyPayment ensures that no value is present for PolicyPayment, not even an explicit nil
### GetPolicyShipping

`func (o *ShopListingWithAssociationsShop) GetPolicyShipping() string`

GetPolicyShipping returns the PolicyShipping field if non-nil, zero value otherwise.

### GetPolicyShippingOk

`func (o *ShopListingWithAssociationsShop) GetPolicyShippingOk() (*string, bool)`

GetPolicyShippingOk returns a tuple with the PolicyShipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyShipping

`func (o *ShopListingWithAssociationsShop) SetPolicyShipping(v string)`

SetPolicyShipping sets PolicyShipping field to given value.

### HasPolicyShipping

`func (o *ShopListingWithAssociationsShop) HasPolicyShipping() bool`

HasPolicyShipping returns a boolean if a field has been set.

### SetPolicyShippingNil

`func (o *ShopListingWithAssociationsShop) SetPolicyShippingNil(b bool)`

 SetPolicyShippingNil sets the value for PolicyShipping to be an explicit nil

### UnsetPolicyShipping
`func (o *ShopListingWithAssociationsShop) UnsetPolicyShipping()`

UnsetPolicyShipping ensures that no value is present for PolicyShipping, not even an explicit nil
### GetPolicyRefunds

`func (o *ShopListingWithAssociationsShop) GetPolicyRefunds() string`

GetPolicyRefunds returns the PolicyRefunds field if non-nil, zero value otherwise.

### GetPolicyRefundsOk

`func (o *ShopListingWithAssociationsShop) GetPolicyRefundsOk() (*string, bool)`

GetPolicyRefundsOk returns a tuple with the PolicyRefunds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyRefunds

`func (o *ShopListingWithAssociationsShop) SetPolicyRefunds(v string)`

SetPolicyRefunds sets PolicyRefunds field to given value.

### HasPolicyRefunds

`func (o *ShopListingWithAssociationsShop) HasPolicyRefunds() bool`

HasPolicyRefunds returns a boolean if a field has been set.

### SetPolicyRefundsNil

`func (o *ShopListingWithAssociationsShop) SetPolicyRefundsNil(b bool)`

 SetPolicyRefundsNil sets the value for PolicyRefunds to be an explicit nil

### UnsetPolicyRefunds
`func (o *ShopListingWithAssociationsShop) UnsetPolicyRefunds()`

UnsetPolicyRefunds ensures that no value is present for PolicyRefunds, not even an explicit nil
### GetPolicyAdditional

`func (o *ShopListingWithAssociationsShop) GetPolicyAdditional() string`

GetPolicyAdditional returns the PolicyAdditional field if non-nil, zero value otherwise.

### GetPolicyAdditionalOk

`func (o *ShopListingWithAssociationsShop) GetPolicyAdditionalOk() (*string, bool)`

GetPolicyAdditionalOk returns a tuple with the PolicyAdditional field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyAdditional

`func (o *ShopListingWithAssociationsShop) SetPolicyAdditional(v string)`

SetPolicyAdditional sets PolicyAdditional field to given value.

### HasPolicyAdditional

`func (o *ShopListingWithAssociationsShop) HasPolicyAdditional() bool`

HasPolicyAdditional returns a boolean if a field has been set.

### SetPolicyAdditionalNil

`func (o *ShopListingWithAssociationsShop) SetPolicyAdditionalNil(b bool)`

 SetPolicyAdditionalNil sets the value for PolicyAdditional to be an explicit nil

### UnsetPolicyAdditional
`func (o *ShopListingWithAssociationsShop) UnsetPolicyAdditional()`

UnsetPolicyAdditional ensures that no value is present for PolicyAdditional, not even an explicit nil
### GetPolicySellerInfo

`func (o *ShopListingWithAssociationsShop) GetPolicySellerInfo() string`

GetPolicySellerInfo returns the PolicySellerInfo field if non-nil, zero value otherwise.

### GetPolicySellerInfoOk

`func (o *ShopListingWithAssociationsShop) GetPolicySellerInfoOk() (*string, bool)`

GetPolicySellerInfoOk returns a tuple with the PolicySellerInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicySellerInfo

`func (o *ShopListingWithAssociationsShop) SetPolicySellerInfo(v string)`

SetPolicySellerInfo sets PolicySellerInfo field to given value.

### HasPolicySellerInfo

`func (o *ShopListingWithAssociationsShop) HasPolicySellerInfo() bool`

HasPolicySellerInfo returns a boolean if a field has been set.

### SetPolicySellerInfoNil

`func (o *ShopListingWithAssociationsShop) SetPolicySellerInfoNil(b bool)`

 SetPolicySellerInfoNil sets the value for PolicySellerInfo to be an explicit nil

### UnsetPolicySellerInfo
`func (o *ShopListingWithAssociationsShop) UnsetPolicySellerInfo()`

UnsetPolicySellerInfo ensures that no value is present for PolicySellerInfo, not even an explicit nil
### GetPolicyUpdateDate

`func (o *ShopListingWithAssociationsShop) GetPolicyUpdateDate() int32`

GetPolicyUpdateDate returns the PolicyUpdateDate field if non-nil, zero value otherwise.

### GetPolicyUpdateDateOk

`func (o *ShopListingWithAssociationsShop) GetPolicyUpdateDateOk() (*int32, bool)`

GetPolicyUpdateDateOk returns a tuple with the PolicyUpdateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyUpdateDate

`func (o *ShopListingWithAssociationsShop) SetPolicyUpdateDate(v int32)`

SetPolicyUpdateDate sets PolicyUpdateDate field to given value.

### HasPolicyUpdateDate

`func (o *ShopListingWithAssociationsShop) HasPolicyUpdateDate() bool`

HasPolicyUpdateDate returns a boolean if a field has been set.

### GetPolicyHasPrivateReceiptInfo

`func (o *ShopListingWithAssociationsShop) GetPolicyHasPrivateReceiptInfo() bool`

GetPolicyHasPrivateReceiptInfo returns the PolicyHasPrivateReceiptInfo field if non-nil, zero value otherwise.

### GetPolicyHasPrivateReceiptInfoOk

`func (o *ShopListingWithAssociationsShop) GetPolicyHasPrivateReceiptInfoOk() (*bool, bool)`

GetPolicyHasPrivateReceiptInfoOk returns a tuple with the PolicyHasPrivateReceiptInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyHasPrivateReceiptInfo

`func (o *ShopListingWithAssociationsShop) SetPolicyHasPrivateReceiptInfo(v bool)`

SetPolicyHasPrivateReceiptInfo sets PolicyHasPrivateReceiptInfo field to given value.

### HasPolicyHasPrivateReceiptInfo

`func (o *ShopListingWithAssociationsShop) HasPolicyHasPrivateReceiptInfo() bool`

HasPolicyHasPrivateReceiptInfo returns a boolean if a field has been set.

### GetHasUnstructuredPolicies

`func (o *ShopListingWithAssociationsShop) GetHasUnstructuredPolicies() bool`

GetHasUnstructuredPolicies returns the HasUnstructuredPolicies field if non-nil, zero value otherwise.

### GetHasUnstructuredPoliciesOk

`func (o *ShopListingWithAssociationsShop) GetHasUnstructuredPoliciesOk() (*bool, bool)`

GetHasUnstructuredPoliciesOk returns a tuple with the HasUnstructuredPolicies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasUnstructuredPolicies

`func (o *ShopListingWithAssociationsShop) SetHasUnstructuredPolicies(v bool)`

SetHasUnstructuredPolicies sets HasUnstructuredPolicies field to given value.

### HasHasUnstructuredPolicies

`func (o *ShopListingWithAssociationsShop) HasHasUnstructuredPolicies() bool`

HasHasUnstructuredPolicies returns a boolean if a field has been set.

### GetPolicyPrivacy

`func (o *ShopListingWithAssociationsShop) GetPolicyPrivacy() string`

GetPolicyPrivacy returns the PolicyPrivacy field if non-nil, zero value otherwise.

### GetPolicyPrivacyOk

`func (o *ShopListingWithAssociationsShop) GetPolicyPrivacyOk() (*string, bool)`

GetPolicyPrivacyOk returns a tuple with the PolicyPrivacy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyPrivacy

`func (o *ShopListingWithAssociationsShop) SetPolicyPrivacy(v string)`

SetPolicyPrivacy sets PolicyPrivacy field to given value.

### HasPolicyPrivacy

`func (o *ShopListingWithAssociationsShop) HasPolicyPrivacy() bool`

HasPolicyPrivacy returns a boolean if a field has been set.

### SetPolicyPrivacyNil

`func (o *ShopListingWithAssociationsShop) SetPolicyPrivacyNil(b bool)`

 SetPolicyPrivacyNil sets the value for PolicyPrivacy to be an explicit nil

### UnsetPolicyPrivacy
`func (o *ShopListingWithAssociationsShop) UnsetPolicyPrivacy()`

UnsetPolicyPrivacy ensures that no value is present for PolicyPrivacy, not even an explicit nil
### GetVacationAutoreply

`func (o *ShopListingWithAssociationsShop) GetVacationAutoreply() string`

GetVacationAutoreply returns the VacationAutoreply field if non-nil, zero value otherwise.

### GetVacationAutoreplyOk

`func (o *ShopListingWithAssociationsShop) GetVacationAutoreplyOk() (*string, bool)`

GetVacationAutoreplyOk returns a tuple with the VacationAutoreply field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVacationAutoreply

`func (o *ShopListingWithAssociationsShop) SetVacationAutoreply(v string)`

SetVacationAutoreply sets VacationAutoreply field to given value.

### HasVacationAutoreply

`func (o *ShopListingWithAssociationsShop) HasVacationAutoreply() bool`

HasVacationAutoreply returns a boolean if a field has been set.

### SetVacationAutoreplyNil

`func (o *ShopListingWithAssociationsShop) SetVacationAutoreplyNil(b bool)`

 SetVacationAutoreplyNil sets the value for VacationAutoreply to be an explicit nil

### UnsetVacationAutoreply
`func (o *ShopListingWithAssociationsShop) UnsetVacationAutoreply()`

UnsetVacationAutoreply ensures that no value is present for VacationAutoreply, not even an explicit nil
### GetUrl

`func (o *ShopListingWithAssociationsShop) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ShopListingWithAssociationsShop) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ShopListingWithAssociationsShop) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *ShopListingWithAssociationsShop) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetImageUrl760x100

`func (o *ShopListingWithAssociationsShop) GetImageUrl760x100() string`

GetImageUrl760x100 returns the ImageUrl760x100 field if non-nil, zero value otherwise.

### GetImageUrl760x100Ok

`func (o *ShopListingWithAssociationsShop) GetImageUrl760x100Ok() (*string, bool)`

GetImageUrl760x100Ok returns a tuple with the ImageUrl760x100 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrl760x100

`func (o *ShopListingWithAssociationsShop) SetImageUrl760x100(v string)`

SetImageUrl760x100 sets ImageUrl760x100 field to given value.

### HasImageUrl760x100

`func (o *ShopListingWithAssociationsShop) HasImageUrl760x100() bool`

HasImageUrl760x100 returns a boolean if a field has been set.

### SetImageUrl760x100Nil

`func (o *ShopListingWithAssociationsShop) SetImageUrl760x100Nil(b bool)`

 SetImageUrl760x100Nil sets the value for ImageUrl760x100 to be an explicit nil

### UnsetImageUrl760x100
`func (o *ShopListingWithAssociationsShop) UnsetImageUrl760x100()`

UnsetImageUrl760x100 ensures that no value is present for ImageUrl760x100, not even an explicit nil
### GetNumFavorers

`func (o *ShopListingWithAssociationsShop) GetNumFavorers() int32`

GetNumFavorers returns the NumFavorers field if non-nil, zero value otherwise.

### GetNumFavorersOk

`func (o *ShopListingWithAssociationsShop) GetNumFavorersOk() (*int32, bool)`

GetNumFavorersOk returns a tuple with the NumFavorers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumFavorers

`func (o *ShopListingWithAssociationsShop) SetNumFavorers(v int32)`

SetNumFavorers sets NumFavorers field to given value.

### HasNumFavorers

`func (o *ShopListingWithAssociationsShop) HasNumFavorers() bool`

HasNumFavorers returns a boolean if a field has been set.

### GetLanguages

`func (o *ShopListingWithAssociationsShop) GetLanguages() []string`

GetLanguages returns the Languages field if non-nil, zero value otherwise.

### GetLanguagesOk

`func (o *ShopListingWithAssociationsShop) GetLanguagesOk() (*[]string, bool)`

GetLanguagesOk returns a tuple with the Languages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguages

`func (o *ShopListingWithAssociationsShop) SetLanguages(v []string)`

SetLanguages sets Languages field to given value.

### HasLanguages

`func (o *ShopListingWithAssociationsShop) HasLanguages() bool`

HasLanguages returns a boolean if a field has been set.

### GetIconUrlFullxfull

`func (o *ShopListingWithAssociationsShop) GetIconUrlFullxfull() string`

GetIconUrlFullxfull returns the IconUrlFullxfull field if non-nil, zero value otherwise.

### GetIconUrlFullxfullOk

`func (o *ShopListingWithAssociationsShop) GetIconUrlFullxfullOk() (*string, bool)`

GetIconUrlFullxfullOk returns a tuple with the IconUrlFullxfull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIconUrlFullxfull

`func (o *ShopListingWithAssociationsShop) SetIconUrlFullxfull(v string)`

SetIconUrlFullxfull sets IconUrlFullxfull field to given value.

### HasIconUrlFullxfull

`func (o *ShopListingWithAssociationsShop) HasIconUrlFullxfull() bool`

HasIconUrlFullxfull returns a boolean if a field has been set.

### SetIconUrlFullxfullNil

`func (o *ShopListingWithAssociationsShop) SetIconUrlFullxfullNil(b bool)`

 SetIconUrlFullxfullNil sets the value for IconUrlFullxfull to be an explicit nil

### UnsetIconUrlFullxfull
`func (o *ShopListingWithAssociationsShop) UnsetIconUrlFullxfull()`

UnsetIconUrlFullxfull ensures that no value is present for IconUrlFullxfull, not even an explicit nil
### GetIsUsingStructuredPolicies

`func (o *ShopListingWithAssociationsShop) GetIsUsingStructuredPolicies() bool`

GetIsUsingStructuredPolicies returns the IsUsingStructuredPolicies field if non-nil, zero value otherwise.

### GetIsUsingStructuredPoliciesOk

`func (o *ShopListingWithAssociationsShop) GetIsUsingStructuredPoliciesOk() (*bool, bool)`

GetIsUsingStructuredPoliciesOk returns a tuple with the IsUsingStructuredPolicies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsUsingStructuredPolicies

`func (o *ShopListingWithAssociationsShop) SetIsUsingStructuredPolicies(v bool)`

SetIsUsingStructuredPolicies sets IsUsingStructuredPolicies field to given value.

### HasIsUsingStructuredPolicies

`func (o *ShopListingWithAssociationsShop) HasIsUsingStructuredPolicies() bool`

HasIsUsingStructuredPolicies returns a boolean if a field has been set.

### GetHasOnboardedStructuredPolicies

`func (o *ShopListingWithAssociationsShop) GetHasOnboardedStructuredPolicies() bool`

GetHasOnboardedStructuredPolicies returns the HasOnboardedStructuredPolicies field if non-nil, zero value otherwise.

### GetHasOnboardedStructuredPoliciesOk

`func (o *ShopListingWithAssociationsShop) GetHasOnboardedStructuredPoliciesOk() (*bool, bool)`

GetHasOnboardedStructuredPoliciesOk returns a tuple with the HasOnboardedStructuredPolicies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasOnboardedStructuredPolicies

`func (o *ShopListingWithAssociationsShop) SetHasOnboardedStructuredPolicies(v bool)`

SetHasOnboardedStructuredPolicies sets HasOnboardedStructuredPolicies field to given value.

### HasHasOnboardedStructuredPolicies

`func (o *ShopListingWithAssociationsShop) HasHasOnboardedStructuredPolicies() bool`

HasHasOnboardedStructuredPolicies returns a boolean if a field has been set.

### GetIncludeDisputeFormLink

`func (o *ShopListingWithAssociationsShop) GetIncludeDisputeFormLink() bool`

GetIncludeDisputeFormLink returns the IncludeDisputeFormLink field if non-nil, zero value otherwise.

### GetIncludeDisputeFormLinkOk

`func (o *ShopListingWithAssociationsShop) GetIncludeDisputeFormLinkOk() (*bool, bool)`

GetIncludeDisputeFormLinkOk returns a tuple with the IncludeDisputeFormLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeDisputeFormLink

`func (o *ShopListingWithAssociationsShop) SetIncludeDisputeFormLink(v bool)`

SetIncludeDisputeFormLink sets IncludeDisputeFormLink field to given value.

### HasIncludeDisputeFormLink

`func (o *ShopListingWithAssociationsShop) HasIncludeDisputeFormLink() bool`

HasIncludeDisputeFormLink returns a boolean if a field has been set.

### GetIsDirectCheckoutOnboarded

`func (o *ShopListingWithAssociationsShop) GetIsDirectCheckoutOnboarded() bool`

GetIsDirectCheckoutOnboarded returns the IsDirectCheckoutOnboarded field if non-nil, zero value otherwise.

### GetIsDirectCheckoutOnboardedOk

`func (o *ShopListingWithAssociationsShop) GetIsDirectCheckoutOnboardedOk() (*bool, bool)`

GetIsDirectCheckoutOnboardedOk returns a tuple with the IsDirectCheckoutOnboarded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDirectCheckoutOnboarded

`func (o *ShopListingWithAssociationsShop) SetIsDirectCheckoutOnboarded(v bool)`

SetIsDirectCheckoutOnboarded sets IsDirectCheckoutOnboarded field to given value.

### HasIsDirectCheckoutOnboarded

`func (o *ShopListingWithAssociationsShop) HasIsDirectCheckoutOnboarded() bool`

HasIsDirectCheckoutOnboarded returns a boolean if a field has been set.

### GetIsEtsyPaymentsOnboarded

`func (o *ShopListingWithAssociationsShop) GetIsEtsyPaymentsOnboarded() bool`

GetIsEtsyPaymentsOnboarded returns the IsEtsyPaymentsOnboarded field if non-nil, zero value otherwise.

### GetIsEtsyPaymentsOnboardedOk

`func (o *ShopListingWithAssociationsShop) GetIsEtsyPaymentsOnboardedOk() (*bool, bool)`

GetIsEtsyPaymentsOnboardedOk returns a tuple with the IsEtsyPaymentsOnboarded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEtsyPaymentsOnboarded

`func (o *ShopListingWithAssociationsShop) SetIsEtsyPaymentsOnboarded(v bool)`

SetIsEtsyPaymentsOnboarded sets IsEtsyPaymentsOnboarded field to given value.

### HasIsEtsyPaymentsOnboarded

`func (o *ShopListingWithAssociationsShop) HasIsEtsyPaymentsOnboarded() bool`

HasIsEtsyPaymentsOnboarded returns a boolean if a field has been set.

### GetIsCalculatedEligible

`func (o *ShopListingWithAssociationsShop) GetIsCalculatedEligible() bool`

GetIsCalculatedEligible returns the IsCalculatedEligible field if non-nil, zero value otherwise.

### GetIsCalculatedEligibleOk

`func (o *ShopListingWithAssociationsShop) GetIsCalculatedEligibleOk() (*bool, bool)`

GetIsCalculatedEligibleOk returns a tuple with the IsCalculatedEligible field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCalculatedEligible

`func (o *ShopListingWithAssociationsShop) SetIsCalculatedEligible(v bool)`

SetIsCalculatedEligible sets IsCalculatedEligible field to given value.

### HasIsCalculatedEligible

`func (o *ShopListingWithAssociationsShop) HasIsCalculatedEligible() bool`

HasIsCalculatedEligible returns a boolean if a field has been set.

### GetIsOptedInToBuyerPromise

`func (o *ShopListingWithAssociationsShop) GetIsOptedInToBuyerPromise() bool`

GetIsOptedInToBuyerPromise returns the IsOptedInToBuyerPromise field if non-nil, zero value otherwise.

### GetIsOptedInToBuyerPromiseOk

`func (o *ShopListingWithAssociationsShop) GetIsOptedInToBuyerPromiseOk() (*bool, bool)`

GetIsOptedInToBuyerPromiseOk returns a tuple with the IsOptedInToBuyerPromise field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOptedInToBuyerPromise

`func (o *ShopListingWithAssociationsShop) SetIsOptedInToBuyerPromise(v bool)`

SetIsOptedInToBuyerPromise sets IsOptedInToBuyerPromise field to given value.

### HasIsOptedInToBuyerPromise

`func (o *ShopListingWithAssociationsShop) HasIsOptedInToBuyerPromise() bool`

HasIsOptedInToBuyerPromise returns a boolean if a field has been set.

### GetIsShopUsBased

`func (o *ShopListingWithAssociationsShop) GetIsShopUsBased() bool`

GetIsShopUsBased returns the IsShopUsBased field if non-nil, zero value otherwise.

### GetIsShopUsBasedOk

`func (o *ShopListingWithAssociationsShop) GetIsShopUsBasedOk() (*bool, bool)`

GetIsShopUsBasedOk returns a tuple with the IsShopUsBased field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsShopUsBased

`func (o *ShopListingWithAssociationsShop) SetIsShopUsBased(v bool)`

SetIsShopUsBased sets IsShopUsBased field to given value.

### HasIsShopUsBased

`func (o *ShopListingWithAssociationsShop) HasIsShopUsBased() bool`

HasIsShopUsBased returns a boolean if a field has been set.

### GetTransactionSoldCount

`func (o *ShopListingWithAssociationsShop) GetTransactionSoldCount() int32`

GetTransactionSoldCount returns the TransactionSoldCount field if non-nil, zero value otherwise.

### GetTransactionSoldCountOk

`func (o *ShopListingWithAssociationsShop) GetTransactionSoldCountOk() (*int32, bool)`

GetTransactionSoldCountOk returns a tuple with the TransactionSoldCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionSoldCount

`func (o *ShopListingWithAssociationsShop) SetTransactionSoldCount(v int32)`

SetTransactionSoldCount sets TransactionSoldCount field to given value.

### HasTransactionSoldCount

`func (o *ShopListingWithAssociationsShop) HasTransactionSoldCount() bool`

HasTransactionSoldCount returns a boolean if a field has been set.

### GetShippingFromCountryIso

`func (o *ShopListingWithAssociationsShop) GetShippingFromCountryIso() string`

GetShippingFromCountryIso returns the ShippingFromCountryIso field if non-nil, zero value otherwise.

### GetShippingFromCountryIsoOk

`func (o *ShopListingWithAssociationsShop) GetShippingFromCountryIsoOk() (*string, bool)`

GetShippingFromCountryIsoOk returns a tuple with the ShippingFromCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingFromCountryIso

`func (o *ShopListingWithAssociationsShop) SetShippingFromCountryIso(v string)`

SetShippingFromCountryIso sets ShippingFromCountryIso field to given value.

### HasShippingFromCountryIso

`func (o *ShopListingWithAssociationsShop) HasShippingFromCountryIso() bool`

HasShippingFromCountryIso returns a boolean if a field has been set.

### SetShippingFromCountryIsoNil

`func (o *ShopListingWithAssociationsShop) SetShippingFromCountryIsoNil(b bool)`

 SetShippingFromCountryIsoNil sets the value for ShippingFromCountryIso to be an explicit nil

### UnsetShippingFromCountryIso
`func (o *ShopListingWithAssociationsShop) UnsetShippingFromCountryIso()`

UnsetShippingFromCountryIso ensures that no value is present for ShippingFromCountryIso, not even an explicit nil
### GetShopLocationCountryIso

`func (o *ShopListingWithAssociationsShop) GetShopLocationCountryIso() string`

GetShopLocationCountryIso returns the ShopLocationCountryIso field if non-nil, zero value otherwise.

### GetShopLocationCountryIsoOk

`func (o *ShopListingWithAssociationsShop) GetShopLocationCountryIsoOk() (*string, bool)`

GetShopLocationCountryIsoOk returns a tuple with the ShopLocationCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopLocationCountryIso

`func (o *ShopListingWithAssociationsShop) SetShopLocationCountryIso(v string)`

SetShopLocationCountryIso sets ShopLocationCountryIso field to given value.

### HasShopLocationCountryIso

`func (o *ShopListingWithAssociationsShop) HasShopLocationCountryIso() bool`

HasShopLocationCountryIso returns a boolean if a field has been set.

### SetShopLocationCountryIsoNil

`func (o *ShopListingWithAssociationsShop) SetShopLocationCountryIsoNil(b bool)`

 SetShopLocationCountryIsoNil sets the value for ShopLocationCountryIso to be an explicit nil

### UnsetShopLocationCountryIso
`func (o *ShopListingWithAssociationsShop) UnsetShopLocationCountryIso()`

UnsetShopLocationCountryIso ensures that no value is present for ShopLocationCountryIso, not even an explicit nil
### GetReviewCount

`func (o *ShopListingWithAssociationsShop) GetReviewCount() int32`

GetReviewCount returns the ReviewCount field if non-nil, zero value otherwise.

### GetReviewCountOk

`func (o *ShopListingWithAssociationsShop) GetReviewCountOk() (*int32, bool)`

GetReviewCountOk returns a tuple with the ReviewCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReviewCount

`func (o *ShopListingWithAssociationsShop) SetReviewCount(v int32)`

SetReviewCount sets ReviewCount field to given value.

### HasReviewCount

`func (o *ShopListingWithAssociationsShop) HasReviewCount() bool`

HasReviewCount returns a boolean if a field has been set.

### SetReviewCountNil

`func (o *ShopListingWithAssociationsShop) SetReviewCountNil(b bool)`

 SetReviewCountNil sets the value for ReviewCount to be an explicit nil

### UnsetReviewCount
`func (o *ShopListingWithAssociationsShop) UnsetReviewCount()`

UnsetReviewCount ensures that no value is present for ReviewCount, not even an explicit nil
### GetReviewAverage

`func (o *ShopListingWithAssociationsShop) GetReviewAverage() float32`

GetReviewAverage returns the ReviewAverage field if non-nil, zero value otherwise.

### GetReviewAverageOk

`func (o *ShopListingWithAssociationsShop) GetReviewAverageOk() (*float32, bool)`

GetReviewAverageOk returns a tuple with the ReviewAverage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReviewAverage

`func (o *ShopListingWithAssociationsShop) SetReviewAverage(v float32)`

SetReviewAverage sets ReviewAverage field to given value.

### HasReviewAverage

`func (o *ShopListingWithAssociationsShop) HasReviewAverage() bool`

HasReviewAverage returns a boolean if a field has been set.

### SetReviewAverageNil

`func (o *ShopListingWithAssociationsShop) SetReviewAverageNil(b bool)`

 SetReviewAverageNil sets the value for ReviewAverage to be an explicit nil

### UnsetReviewAverage
`func (o *ShopListingWithAssociationsShop) UnsetReviewAverage()`

UnsetReviewAverage ensures that no value is present for ReviewAverage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


