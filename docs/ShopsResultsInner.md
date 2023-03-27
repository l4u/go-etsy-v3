# ShopsResultsInner

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

### NewShopsResultsInner

`func NewShopsResultsInner() *ShopsResultsInner`

NewShopsResultsInner instantiates a new ShopsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopsResultsInnerWithDefaults

`func NewShopsResultsInnerWithDefaults() *ShopsResultsInner`

NewShopsResultsInnerWithDefaults instantiates a new ShopsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShopId

`func (o *ShopsResultsInner) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *ShopsResultsInner) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *ShopsResultsInner) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *ShopsResultsInner) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetUserId

`func (o *ShopsResultsInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ShopsResultsInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ShopsResultsInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ShopsResultsInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetShopName

`func (o *ShopsResultsInner) GetShopName() string`

GetShopName returns the ShopName field if non-nil, zero value otherwise.

### GetShopNameOk

`func (o *ShopsResultsInner) GetShopNameOk() (*string, bool)`

GetShopNameOk returns a tuple with the ShopName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopName

`func (o *ShopsResultsInner) SetShopName(v string)`

SetShopName sets ShopName field to given value.

### HasShopName

`func (o *ShopsResultsInner) HasShopName() bool`

HasShopName returns a boolean if a field has been set.

### GetCreateDate

`func (o *ShopsResultsInner) GetCreateDate() int32`

GetCreateDate returns the CreateDate field if non-nil, zero value otherwise.

### GetCreateDateOk

`func (o *ShopsResultsInner) GetCreateDateOk() (*int32, bool)`

GetCreateDateOk returns a tuple with the CreateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateDate

`func (o *ShopsResultsInner) SetCreateDate(v int32)`

SetCreateDate sets CreateDate field to given value.

### HasCreateDate

`func (o *ShopsResultsInner) HasCreateDate() bool`

HasCreateDate returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetTitle

`func (o *ShopsResultsInner) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopsResultsInner) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopsResultsInner) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopsResultsInner) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *ShopsResultsInner) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *ShopsResultsInner) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetAnnouncement

`func (o *ShopsResultsInner) GetAnnouncement() string`

GetAnnouncement returns the Announcement field if non-nil, zero value otherwise.

### GetAnnouncementOk

`func (o *ShopsResultsInner) GetAnnouncementOk() (*string, bool)`

GetAnnouncementOk returns a tuple with the Announcement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnnouncement

`func (o *ShopsResultsInner) SetAnnouncement(v string)`

SetAnnouncement sets Announcement field to given value.

### HasAnnouncement

`func (o *ShopsResultsInner) HasAnnouncement() bool`

HasAnnouncement returns a boolean if a field has been set.

### SetAnnouncementNil

`func (o *ShopsResultsInner) SetAnnouncementNil(b bool)`

 SetAnnouncementNil sets the value for Announcement to be an explicit nil

### UnsetAnnouncement
`func (o *ShopsResultsInner) UnsetAnnouncement()`

UnsetAnnouncement ensures that no value is present for Announcement, not even an explicit nil
### GetCurrencyCode

`func (o *ShopsResultsInner) GetCurrencyCode() string`

GetCurrencyCode returns the CurrencyCode field if non-nil, zero value otherwise.

### GetCurrencyCodeOk

`func (o *ShopsResultsInner) GetCurrencyCodeOk() (*string, bool)`

GetCurrencyCodeOk returns a tuple with the CurrencyCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyCode

`func (o *ShopsResultsInner) SetCurrencyCode(v string)`

SetCurrencyCode sets CurrencyCode field to given value.

### HasCurrencyCode

`func (o *ShopsResultsInner) HasCurrencyCode() bool`

HasCurrencyCode returns a boolean if a field has been set.

### GetIsVacation

`func (o *ShopsResultsInner) GetIsVacation() bool`

GetIsVacation returns the IsVacation field if non-nil, zero value otherwise.

### GetIsVacationOk

`func (o *ShopsResultsInner) GetIsVacationOk() (*bool, bool)`

GetIsVacationOk returns a tuple with the IsVacation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsVacation

`func (o *ShopsResultsInner) SetIsVacation(v bool)`

SetIsVacation sets IsVacation field to given value.

### HasIsVacation

`func (o *ShopsResultsInner) HasIsVacation() bool`

HasIsVacation returns a boolean if a field has been set.

### GetVacationMessage

`func (o *ShopsResultsInner) GetVacationMessage() string`

GetVacationMessage returns the VacationMessage field if non-nil, zero value otherwise.

### GetVacationMessageOk

`func (o *ShopsResultsInner) GetVacationMessageOk() (*string, bool)`

GetVacationMessageOk returns a tuple with the VacationMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVacationMessage

`func (o *ShopsResultsInner) SetVacationMessage(v string)`

SetVacationMessage sets VacationMessage field to given value.

### HasVacationMessage

`func (o *ShopsResultsInner) HasVacationMessage() bool`

HasVacationMessage returns a boolean if a field has been set.

### SetVacationMessageNil

`func (o *ShopsResultsInner) SetVacationMessageNil(b bool)`

 SetVacationMessageNil sets the value for VacationMessage to be an explicit nil

### UnsetVacationMessage
`func (o *ShopsResultsInner) UnsetVacationMessage()`

UnsetVacationMessage ensures that no value is present for VacationMessage, not even an explicit nil
### GetSaleMessage

`func (o *ShopsResultsInner) GetSaleMessage() string`

GetSaleMessage returns the SaleMessage field if non-nil, zero value otherwise.

### GetSaleMessageOk

`func (o *ShopsResultsInner) GetSaleMessageOk() (*string, bool)`

GetSaleMessageOk returns a tuple with the SaleMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSaleMessage

`func (o *ShopsResultsInner) SetSaleMessage(v string)`

SetSaleMessage sets SaleMessage field to given value.

### HasSaleMessage

`func (o *ShopsResultsInner) HasSaleMessage() bool`

HasSaleMessage returns a boolean if a field has been set.

### SetSaleMessageNil

`func (o *ShopsResultsInner) SetSaleMessageNil(b bool)`

 SetSaleMessageNil sets the value for SaleMessage to be an explicit nil

### UnsetSaleMessage
`func (o *ShopsResultsInner) UnsetSaleMessage()`

UnsetSaleMessage ensures that no value is present for SaleMessage, not even an explicit nil
### GetDigitalSaleMessage

`func (o *ShopsResultsInner) GetDigitalSaleMessage() string`

GetDigitalSaleMessage returns the DigitalSaleMessage field if non-nil, zero value otherwise.

### GetDigitalSaleMessageOk

`func (o *ShopsResultsInner) GetDigitalSaleMessageOk() (*string, bool)`

GetDigitalSaleMessageOk returns a tuple with the DigitalSaleMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigitalSaleMessage

`func (o *ShopsResultsInner) SetDigitalSaleMessage(v string)`

SetDigitalSaleMessage sets DigitalSaleMessage field to given value.

### HasDigitalSaleMessage

`func (o *ShopsResultsInner) HasDigitalSaleMessage() bool`

HasDigitalSaleMessage returns a boolean if a field has been set.

### SetDigitalSaleMessageNil

`func (o *ShopsResultsInner) SetDigitalSaleMessageNil(b bool)`

 SetDigitalSaleMessageNil sets the value for DigitalSaleMessage to be an explicit nil

### UnsetDigitalSaleMessage
`func (o *ShopsResultsInner) UnsetDigitalSaleMessage()`

UnsetDigitalSaleMessage ensures that no value is present for DigitalSaleMessage, not even an explicit nil
### GetUpdateDate

`func (o *ShopsResultsInner) GetUpdateDate() int32`

GetUpdateDate returns the UpdateDate field if non-nil, zero value otherwise.

### GetUpdateDateOk

`func (o *ShopsResultsInner) GetUpdateDateOk() (*int32, bool)`

GetUpdateDateOk returns a tuple with the UpdateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateDate

`func (o *ShopsResultsInner) SetUpdateDate(v int32)`

SetUpdateDate sets UpdateDate field to given value.

### HasUpdateDate

`func (o *ShopsResultsInner) HasUpdateDate() bool`

HasUpdateDate returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *ShopsResultsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *ShopsResultsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *ShopsResultsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *ShopsResultsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetListingActiveCount

`func (o *ShopsResultsInner) GetListingActiveCount() int32`

GetListingActiveCount returns the ListingActiveCount field if non-nil, zero value otherwise.

### GetListingActiveCountOk

`func (o *ShopsResultsInner) GetListingActiveCountOk() (*int32, bool)`

GetListingActiveCountOk returns a tuple with the ListingActiveCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingActiveCount

`func (o *ShopsResultsInner) SetListingActiveCount(v int32)`

SetListingActiveCount sets ListingActiveCount field to given value.

### HasListingActiveCount

`func (o *ShopsResultsInner) HasListingActiveCount() bool`

HasListingActiveCount returns a boolean if a field has been set.

### GetDigitalListingCount

`func (o *ShopsResultsInner) GetDigitalListingCount() int32`

GetDigitalListingCount returns the DigitalListingCount field if non-nil, zero value otherwise.

### GetDigitalListingCountOk

`func (o *ShopsResultsInner) GetDigitalListingCountOk() (*int32, bool)`

GetDigitalListingCountOk returns a tuple with the DigitalListingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigitalListingCount

`func (o *ShopsResultsInner) SetDigitalListingCount(v int32)`

SetDigitalListingCount sets DigitalListingCount field to given value.

### HasDigitalListingCount

`func (o *ShopsResultsInner) HasDigitalListingCount() bool`

HasDigitalListingCount returns a boolean if a field has been set.

### GetLoginName

`func (o *ShopsResultsInner) GetLoginName() string`

GetLoginName returns the LoginName field if non-nil, zero value otherwise.

### GetLoginNameOk

`func (o *ShopsResultsInner) GetLoginNameOk() (*string, bool)`

GetLoginNameOk returns a tuple with the LoginName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoginName

`func (o *ShopsResultsInner) SetLoginName(v string)`

SetLoginName sets LoginName field to given value.

### HasLoginName

`func (o *ShopsResultsInner) HasLoginName() bool`

HasLoginName returns a boolean if a field has been set.

### GetAcceptsCustomRequests

`func (o *ShopsResultsInner) GetAcceptsCustomRequests() bool`

GetAcceptsCustomRequests returns the AcceptsCustomRequests field if non-nil, zero value otherwise.

### GetAcceptsCustomRequestsOk

`func (o *ShopsResultsInner) GetAcceptsCustomRequestsOk() (*bool, bool)`

GetAcceptsCustomRequestsOk returns a tuple with the AcceptsCustomRequests field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAcceptsCustomRequests

`func (o *ShopsResultsInner) SetAcceptsCustomRequests(v bool)`

SetAcceptsCustomRequests sets AcceptsCustomRequests field to given value.

### HasAcceptsCustomRequests

`func (o *ShopsResultsInner) HasAcceptsCustomRequests() bool`

HasAcceptsCustomRequests returns a boolean if a field has been set.

### GetPolicyWelcome

`func (o *ShopsResultsInner) GetPolicyWelcome() string`

GetPolicyWelcome returns the PolicyWelcome field if non-nil, zero value otherwise.

### GetPolicyWelcomeOk

`func (o *ShopsResultsInner) GetPolicyWelcomeOk() (*string, bool)`

GetPolicyWelcomeOk returns a tuple with the PolicyWelcome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyWelcome

`func (o *ShopsResultsInner) SetPolicyWelcome(v string)`

SetPolicyWelcome sets PolicyWelcome field to given value.

### HasPolicyWelcome

`func (o *ShopsResultsInner) HasPolicyWelcome() bool`

HasPolicyWelcome returns a boolean if a field has been set.

### SetPolicyWelcomeNil

`func (o *ShopsResultsInner) SetPolicyWelcomeNil(b bool)`

 SetPolicyWelcomeNil sets the value for PolicyWelcome to be an explicit nil

### UnsetPolicyWelcome
`func (o *ShopsResultsInner) UnsetPolicyWelcome()`

UnsetPolicyWelcome ensures that no value is present for PolicyWelcome, not even an explicit nil
### GetPolicyPayment

`func (o *ShopsResultsInner) GetPolicyPayment() string`

GetPolicyPayment returns the PolicyPayment field if non-nil, zero value otherwise.

### GetPolicyPaymentOk

`func (o *ShopsResultsInner) GetPolicyPaymentOk() (*string, bool)`

GetPolicyPaymentOk returns a tuple with the PolicyPayment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyPayment

`func (o *ShopsResultsInner) SetPolicyPayment(v string)`

SetPolicyPayment sets PolicyPayment field to given value.

### HasPolicyPayment

`func (o *ShopsResultsInner) HasPolicyPayment() bool`

HasPolicyPayment returns a boolean if a field has been set.

### SetPolicyPaymentNil

`func (o *ShopsResultsInner) SetPolicyPaymentNil(b bool)`

 SetPolicyPaymentNil sets the value for PolicyPayment to be an explicit nil

### UnsetPolicyPayment
`func (o *ShopsResultsInner) UnsetPolicyPayment()`

UnsetPolicyPayment ensures that no value is present for PolicyPayment, not even an explicit nil
### GetPolicyShipping

`func (o *ShopsResultsInner) GetPolicyShipping() string`

GetPolicyShipping returns the PolicyShipping field if non-nil, zero value otherwise.

### GetPolicyShippingOk

`func (o *ShopsResultsInner) GetPolicyShippingOk() (*string, bool)`

GetPolicyShippingOk returns a tuple with the PolicyShipping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyShipping

`func (o *ShopsResultsInner) SetPolicyShipping(v string)`

SetPolicyShipping sets PolicyShipping field to given value.

### HasPolicyShipping

`func (o *ShopsResultsInner) HasPolicyShipping() bool`

HasPolicyShipping returns a boolean if a field has been set.

### SetPolicyShippingNil

`func (o *ShopsResultsInner) SetPolicyShippingNil(b bool)`

 SetPolicyShippingNil sets the value for PolicyShipping to be an explicit nil

### UnsetPolicyShipping
`func (o *ShopsResultsInner) UnsetPolicyShipping()`

UnsetPolicyShipping ensures that no value is present for PolicyShipping, not even an explicit nil
### GetPolicyRefunds

`func (o *ShopsResultsInner) GetPolicyRefunds() string`

GetPolicyRefunds returns the PolicyRefunds field if non-nil, zero value otherwise.

### GetPolicyRefundsOk

`func (o *ShopsResultsInner) GetPolicyRefundsOk() (*string, bool)`

GetPolicyRefundsOk returns a tuple with the PolicyRefunds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyRefunds

`func (o *ShopsResultsInner) SetPolicyRefunds(v string)`

SetPolicyRefunds sets PolicyRefunds field to given value.

### HasPolicyRefunds

`func (o *ShopsResultsInner) HasPolicyRefunds() bool`

HasPolicyRefunds returns a boolean if a field has been set.

### SetPolicyRefundsNil

`func (o *ShopsResultsInner) SetPolicyRefundsNil(b bool)`

 SetPolicyRefundsNil sets the value for PolicyRefunds to be an explicit nil

### UnsetPolicyRefunds
`func (o *ShopsResultsInner) UnsetPolicyRefunds()`

UnsetPolicyRefunds ensures that no value is present for PolicyRefunds, not even an explicit nil
### GetPolicyAdditional

`func (o *ShopsResultsInner) GetPolicyAdditional() string`

GetPolicyAdditional returns the PolicyAdditional field if non-nil, zero value otherwise.

### GetPolicyAdditionalOk

`func (o *ShopsResultsInner) GetPolicyAdditionalOk() (*string, bool)`

GetPolicyAdditionalOk returns a tuple with the PolicyAdditional field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyAdditional

`func (o *ShopsResultsInner) SetPolicyAdditional(v string)`

SetPolicyAdditional sets PolicyAdditional field to given value.

### HasPolicyAdditional

`func (o *ShopsResultsInner) HasPolicyAdditional() bool`

HasPolicyAdditional returns a boolean if a field has been set.

### SetPolicyAdditionalNil

`func (o *ShopsResultsInner) SetPolicyAdditionalNil(b bool)`

 SetPolicyAdditionalNil sets the value for PolicyAdditional to be an explicit nil

### UnsetPolicyAdditional
`func (o *ShopsResultsInner) UnsetPolicyAdditional()`

UnsetPolicyAdditional ensures that no value is present for PolicyAdditional, not even an explicit nil
### GetPolicySellerInfo

`func (o *ShopsResultsInner) GetPolicySellerInfo() string`

GetPolicySellerInfo returns the PolicySellerInfo field if non-nil, zero value otherwise.

### GetPolicySellerInfoOk

`func (o *ShopsResultsInner) GetPolicySellerInfoOk() (*string, bool)`

GetPolicySellerInfoOk returns a tuple with the PolicySellerInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicySellerInfo

`func (o *ShopsResultsInner) SetPolicySellerInfo(v string)`

SetPolicySellerInfo sets PolicySellerInfo field to given value.

### HasPolicySellerInfo

`func (o *ShopsResultsInner) HasPolicySellerInfo() bool`

HasPolicySellerInfo returns a boolean if a field has been set.

### SetPolicySellerInfoNil

`func (o *ShopsResultsInner) SetPolicySellerInfoNil(b bool)`

 SetPolicySellerInfoNil sets the value for PolicySellerInfo to be an explicit nil

### UnsetPolicySellerInfo
`func (o *ShopsResultsInner) UnsetPolicySellerInfo()`

UnsetPolicySellerInfo ensures that no value is present for PolicySellerInfo, not even an explicit nil
### GetPolicyUpdateDate

`func (o *ShopsResultsInner) GetPolicyUpdateDate() int32`

GetPolicyUpdateDate returns the PolicyUpdateDate field if non-nil, zero value otherwise.

### GetPolicyUpdateDateOk

`func (o *ShopsResultsInner) GetPolicyUpdateDateOk() (*int32, bool)`

GetPolicyUpdateDateOk returns a tuple with the PolicyUpdateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyUpdateDate

`func (o *ShopsResultsInner) SetPolicyUpdateDate(v int32)`

SetPolicyUpdateDate sets PolicyUpdateDate field to given value.

### HasPolicyUpdateDate

`func (o *ShopsResultsInner) HasPolicyUpdateDate() bool`

HasPolicyUpdateDate returns a boolean if a field has been set.

### GetPolicyHasPrivateReceiptInfo

`func (o *ShopsResultsInner) GetPolicyHasPrivateReceiptInfo() bool`

GetPolicyHasPrivateReceiptInfo returns the PolicyHasPrivateReceiptInfo field if non-nil, zero value otherwise.

### GetPolicyHasPrivateReceiptInfoOk

`func (o *ShopsResultsInner) GetPolicyHasPrivateReceiptInfoOk() (*bool, bool)`

GetPolicyHasPrivateReceiptInfoOk returns a tuple with the PolicyHasPrivateReceiptInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyHasPrivateReceiptInfo

`func (o *ShopsResultsInner) SetPolicyHasPrivateReceiptInfo(v bool)`

SetPolicyHasPrivateReceiptInfo sets PolicyHasPrivateReceiptInfo field to given value.

### HasPolicyHasPrivateReceiptInfo

`func (o *ShopsResultsInner) HasPolicyHasPrivateReceiptInfo() bool`

HasPolicyHasPrivateReceiptInfo returns a boolean if a field has been set.

### GetHasUnstructuredPolicies

`func (o *ShopsResultsInner) GetHasUnstructuredPolicies() bool`

GetHasUnstructuredPolicies returns the HasUnstructuredPolicies field if non-nil, zero value otherwise.

### GetHasUnstructuredPoliciesOk

`func (o *ShopsResultsInner) GetHasUnstructuredPoliciesOk() (*bool, bool)`

GetHasUnstructuredPoliciesOk returns a tuple with the HasUnstructuredPolicies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasUnstructuredPolicies

`func (o *ShopsResultsInner) SetHasUnstructuredPolicies(v bool)`

SetHasUnstructuredPolicies sets HasUnstructuredPolicies field to given value.

### HasHasUnstructuredPolicies

`func (o *ShopsResultsInner) HasHasUnstructuredPolicies() bool`

HasHasUnstructuredPolicies returns a boolean if a field has been set.

### GetPolicyPrivacy

`func (o *ShopsResultsInner) GetPolicyPrivacy() string`

GetPolicyPrivacy returns the PolicyPrivacy field if non-nil, zero value otherwise.

### GetPolicyPrivacyOk

`func (o *ShopsResultsInner) GetPolicyPrivacyOk() (*string, bool)`

GetPolicyPrivacyOk returns a tuple with the PolicyPrivacy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyPrivacy

`func (o *ShopsResultsInner) SetPolicyPrivacy(v string)`

SetPolicyPrivacy sets PolicyPrivacy field to given value.

### HasPolicyPrivacy

`func (o *ShopsResultsInner) HasPolicyPrivacy() bool`

HasPolicyPrivacy returns a boolean if a field has been set.

### SetPolicyPrivacyNil

`func (o *ShopsResultsInner) SetPolicyPrivacyNil(b bool)`

 SetPolicyPrivacyNil sets the value for PolicyPrivacy to be an explicit nil

### UnsetPolicyPrivacy
`func (o *ShopsResultsInner) UnsetPolicyPrivacy()`

UnsetPolicyPrivacy ensures that no value is present for PolicyPrivacy, not even an explicit nil
### GetVacationAutoreply

`func (o *ShopsResultsInner) GetVacationAutoreply() string`

GetVacationAutoreply returns the VacationAutoreply field if non-nil, zero value otherwise.

### GetVacationAutoreplyOk

`func (o *ShopsResultsInner) GetVacationAutoreplyOk() (*string, bool)`

GetVacationAutoreplyOk returns a tuple with the VacationAutoreply field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVacationAutoreply

`func (o *ShopsResultsInner) SetVacationAutoreply(v string)`

SetVacationAutoreply sets VacationAutoreply field to given value.

### HasVacationAutoreply

`func (o *ShopsResultsInner) HasVacationAutoreply() bool`

HasVacationAutoreply returns a boolean if a field has been set.

### SetVacationAutoreplyNil

`func (o *ShopsResultsInner) SetVacationAutoreplyNil(b bool)`

 SetVacationAutoreplyNil sets the value for VacationAutoreply to be an explicit nil

### UnsetVacationAutoreply
`func (o *ShopsResultsInner) UnsetVacationAutoreply()`

UnsetVacationAutoreply ensures that no value is present for VacationAutoreply, not even an explicit nil
### GetUrl

`func (o *ShopsResultsInner) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ShopsResultsInner) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ShopsResultsInner) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *ShopsResultsInner) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetImageUrl760x100

`func (o *ShopsResultsInner) GetImageUrl760x100() string`

GetImageUrl760x100 returns the ImageUrl760x100 field if non-nil, zero value otherwise.

### GetImageUrl760x100Ok

`func (o *ShopsResultsInner) GetImageUrl760x100Ok() (*string, bool)`

GetImageUrl760x100Ok returns a tuple with the ImageUrl760x100 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrl760x100

`func (o *ShopsResultsInner) SetImageUrl760x100(v string)`

SetImageUrl760x100 sets ImageUrl760x100 field to given value.

### HasImageUrl760x100

`func (o *ShopsResultsInner) HasImageUrl760x100() bool`

HasImageUrl760x100 returns a boolean if a field has been set.

### SetImageUrl760x100Nil

`func (o *ShopsResultsInner) SetImageUrl760x100Nil(b bool)`

 SetImageUrl760x100Nil sets the value for ImageUrl760x100 to be an explicit nil

### UnsetImageUrl760x100
`func (o *ShopsResultsInner) UnsetImageUrl760x100()`

UnsetImageUrl760x100 ensures that no value is present for ImageUrl760x100, not even an explicit nil
### GetNumFavorers

`func (o *ShopsResultsInner) GetNumFavorers() int32`

GetNumFavorers returns the NumFavorers field if non-nil, zero value otherwise.

### GetNumFavorersOk

`func (o *ShopsResultsInner) GetNumFavorersOk() (*int32, bool)`

GetNumFavorersOk returns a tuple with the NumFavorers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumFavorers

`func (o *ShopsResultsInner) SetNumFavorers(v int32)`

SetNumFavorers sets NumFavorers field to given value.

### HasNumFavorers

`func (o *ShopsResultsInner) HasNumFavorers() bool`

HasNumFavorers returns a boolean if a field has been set.

### GetLanguages

`func (o *ShopsResultsInner) GetLanguages() []string`

GetLanguages returns the Languages field if non-nil, zero value otherwise.

### GetLanguagesOk

`func (o *ShopsResultsInner) GetLanguagesOk() (*[]string, bool)`

GetLanguagesOk returns a tuple with the Languages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguages

`func (o *ShopsResultsInner) SetLanguages(v []string)`

SetLanguages sets Languages field to given value.

### HasLanguages

`func (o *ShopsResultsInner) HasLanguages() bool`

HasLanguages returns a boolean if a field has been set.

### GetIconUrlFullxfull

`func (o *ShopsResultsInner) GetIconUrlFullxfull() string`

GetIconUrlFullxfull returns the IconUrlFullxfull field if non-nil, zero value otherwise.

### GetIconUrlFullxfullOk

`func (o *ShopsResultsInner) GetIconUrlFullxfullOk() (*string, bool)`

GetIconUrlFullxfullOk returns a tuple with the IconUrlFullxfull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIconUrlFullxfull

`func (o *ShopsResultsInner) SetIconUrlFullxfull(v string)`

SetIconUrlFullxfull sets IconUrlFullxfull field to given value.

### HasIconUrlFullxfull

`func (o *ShopsResultsInner) HasIconUrlFullxfull() bool`

HasIconUrlFullxfull returns a boolean if a field has been set.

### SetIconUrlFullxfullNil

`func (o *ShopsResultsInner) SetIconUrlFullxfullNil(b bool)`

 SetIconUrlFullxfullNil sets the value for IconUrlFullxfull to be an explicit nil

### UnsetIconUrlFullxfull
`func (o *ShopsResultsInner) UnsetIconUrlFullxfull()`

UnsetIconUrlFullxfull ensures that no value is present for IconUrlFullxfull, not even an explicit nil
### GetIsUsingStructuredPolicies

`func (o *ShopsResultsInner) GetIsUsingStructuredPolicies() bool`

GetIsUsingStructuredPolicies returns the IsUsingStructuredPolicies field if non-nil, zero value otherwise.

### GetIsUsingStructuredPoliciesOk

`func (o *ShopsResultsInner) GetIsUsingStructuredPoliciesOk() (*bool, bool)`

GetIsUsingStructuredPoliciesOk returns a tuple with the IsUsingStructuredPolicies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsUsingStructuredPolicies

`func (o *ShopsResultsInner) SetIsUsingStructuredPolicies(v bool)`

SetIsUsingStructuredPolicies sets IsUsingStructuredPolicies field to given value.

### HasIsUsingStructuredPolicies

`func (o *ShopsResultsInner) HasIsUsingStructuredPolicies() bool`

HasIsUsingStructuredPolicies returns a boolean if a field has been set.

### GetHasOnboardedStructuredPolicies

`func (o *ShopsResultsInner) GetHasOnboardedStructuredPolicies() bool`

GetHasOnboardedStructuredPolicies returns the HasOnboardedStructuredPolicies field if non-nil, zero value otherwise.

### GetHasOnboardedStructuredPoliciesOk

`func (o *ShopsResultsInner) GetHasOnboardedStructuredPoliciesOk() (*bool, bool)`

GetHasOnboardedStructuredPoliciesOk returns a tuple with the HasOnboardedStructuredPolicies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasOnboardedStructuredPolicies

`func (o *ShopsResultsInner) SetHasOnboardedStructuredPolicies(v bool)`

SetHasOnboardedStructuredPolicies sets HasOnboardedStructuredPolicies field to given value.

### HasHasOnboardedStructuredPolicies

`func (o *ShopsResultsInner) HasHasOnboardedStructuredPolicies() bool`

HasHasOnboardedStructuredPolicies returns a boolean if a field has been set.

### GetIncludeDisputeFormLink

`func (o *ShopsResultsInner) GetIncludeDisputeFormLink() bool`

GetIncludeDisputeFormLink returns the IncludeDisputeFormLink field if non-nil, zero value otherwise.

### GetIncludeDisputeFormLinkOk

`func (o *ShopsResultsInner) GetIncludeDisputeFormLinkOk() (*bool, bool)`

GetIncludeDisputeFormLinkOk returns a tuple with the IncludeDisputeFormLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeDisputeFormLink

`func (o *ShopsResultsInner) SetIncludeDisputeFormLink(v bool)`

SetIncludeDisputeFormLink sets IncludeDisputeFormLink field to given value.

### HasIncludeDisputeFormLink

`func (o *ShopsResultsInner) HasIncludeDisputeFormLink() bool`

HasIncludeDisputeFormLink returns a boolean if a field has been set.

### GetIsDirectCheckoutOnboarded

`func (o *ShopsResultsInner) GetIsDirectCheckoutOnboarded() bool`

GetIsDirectCheckoutOnboarded returns the IsDirectCheckoutOnboarded field if non-nil, zero value otherwise.

### GetIsDirectCheckoutOnboardedOk

`func (o *ShopsResultsInner) GetIsDirectCheckoutOnboardedOk() (*bool, bool)`

GetIsDirectCheckoutOnboardedOk returns a tuple with the IsDirectCheckoutOnboarded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDirectCheckoutOnboarded

`func (o *ShopsResultsInner) SetIsDirectCheckoutOnboarded(v bool)`

SetIsDirectCheckoutOnboarded sets IsDirectCheckoutOnboarded field to given value.

### HasIsDirectCheckoutOnboarded

`func (o *ShopsResultsInner) HasIsDirectCheckoutOnboarded() bool`

HasIsDirectCheckoutOnboarded returns a boolean if a field has been set.

### GetIsEtsyPaymentsOnboarded

`func (o *ShopsResultsInner) GetIsEtsyPaymentsOnboarded() bool`

GetIsEtsyPaymentsOnboarded returns the IsEtsyPaymentsOnboarded field if non-nil, zero value otherwise.

### GetIsEtsyPaymentsOnboardedOk

`func (o *ShopsResultsInner) GetIsEtsyPaymentsOnboardedOk() (*bool, bool)`

GetIsEtsyPaymentsOnboardedOk returns a tuple with the IsEtsyPaymentsOnboarded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEtsyPaymentsOnboarded

`func (o *ShopsResultsInner) SetIsEtsyPaymentsOnboarded(v bool)`

SetIsEtsyPaymentsOnboarded sets IsEtsyPaymentsOnboarded field to given value.

### HasIsEtsyPaymentsOnboarded

`func (o *ShopsResultsInner) HasIsEtsyPaymentsOnboarded() bool`

HasIsEtsyPaymentsOnboarded returns a boolean if a field has been set.

### GetIsCalculatedEligible

`func (o *ShopsResultsInner) GetIsCalculatedEligible() bool`

GetIsCalculatedEligible returns the IsCalculatedEligible field if non-nil, zero value otherwise.

### GetIsCalculatedEligibleOk

`func (o *ShopsResultsInner) GetIsCalculatedEligibleOk() (*bool, bool)`

GetIsCalculatedEligibleOk returns a tuple with the IsCalculatedEligible field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCalculatedEligible

`func (o *ShopsResultsInner) SetIsCalculatedEligible(v bool)`

SetIsCalculatedEligible sets IsCalculatedEligible field to given value.

### HasIsCalculatedEligible

`func (o *ShopsResultsInner) HasIsCalculatedEligible() bool`

HasIsCalculatedEligible returns a boolean if a field has been set.

### GetIsOptedInToBuyerPromise

`func (o *ShopsResultsInner) GetIsOptedInToBuyerPromise() bool`

GetIsOptedInToBuyerPromise returns the IsOptedInToBuyerPromise field if non-nil, zero value otherwise.

### GetIsOptedInToBuyerPromiseOk

`func (o *ShopsResultsInner) GetIsOptedInToBuyerPromiseOk() (*bool, bool)`

GetIsOptedInToBuyerPromiseOk returns a tuple with the IsOptedInToBuyerPromise field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOptedInToBuyerPromise

`func (o *ShopsResultsInner) SetIsOptedInToBuyerPromise(v bool)`

SetIsOptedInToBuyerPromise sets IsOptedInToBuyerPromise field to given value.

### HasIsOptedInToBuyerPromise

`func (o *ShopsResultsInner) HasIsOptedInToBuyerPromise() bool`

HasIsOptedInToBuyerPromise returns a boolean if a field has been set.

### GetIsShopUsBased

`func (o *ShopsResultsInner) GetIsShopUsBased() bool`

GetIsShopUsBased returns the IsShopUsBased field if non-nil, zero value otherwise.

### GetIsShopUsBasedOk

`func (o *ShopsResultsInner) GetIsShopUsBasedOk() (*bool, bool)`

GetIsShopUsBasedOk returns a tuple with the IsShopUsBased field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsShopUsBased

`func (o *ShopsResultsInner) SetIsShopUsBased(v bool)`

SetIsShopUsBased sets IsShopUsBased field to given value.

### HasIsShopUsBased

`func (o *ShopsResultsInner) HasIsShopUsBased() bool`

HasIsShopUsBased returns a boolean if a field has been set.

### GetTransactionSoldCount

`func (o *ShopsResultsInner) GetTransactionSoldCount() int32`

GetTransactionSoldCount returns the TransactionSoldCount field if non-nil, zero value otherwise.

### GetTransactionSoldCountOk

`func (o *ShopsResultsInner) GetTransactionSoldCountOk() (*int32, bool)`

GetTransactionSoldCountOk returns a tuple with the TransactionSoldCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionSoldCount

`func (o *ShopsResultsInner) SetTransactionSoldCount(v int32)`

SetTransactionSoldCount sets TransactionSoldCount field to given value.

### HasTransactionSoldCount

`func (o *ShopsResultsInner) HasTransactionSoldCount() bool`

HasTransactionSoldCount returns a boolean if a field has been set.

### GetShippingFromCountryIso

`func (o *ShopsResultsInner) GetShippingFromCountryIso() string`

GetShippingFromCountryIso returns the ShippingFromCountryIso field if non-nil, zero value otherwise.

### GetShippingFromCountryIsoOk

`func (o *ShopsResultsInner) GetShippingFromCountryIsoOk() (*string, bool)`

GetShippingFromCountryIsoOk returns a tuple with the ShippingFromCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingFromCountryIso

`func (o *ShopsResultsInner) SetShippingFromCountryIso(v string)`

SetShippingFromCountryIso sets ShippingFromCountryIso field to given value.

### HasShippingFromCountryIso

`func (o *ShopsResultsInner) HasShippingFromCountryIso() bool`

HasShippingFromCountryIso returns a boolean if a field has been set.

### SetShippingFromCountryIsoNil

`func (o *ShopsResultsInner) SetShippingFromCountryIsoNil(b bool)`

 SetShippingFromCountryIsoNil sets the value for ShippingFromCountryIso to be an explicit nil

### UnsetShippingFromCountryIso
`func (o *ShopsResultsInner) UnsetShippingFromCountryIso()`

UnsetShippingFromCountryIso ensures that no value is present for ShippingFromCountryIso, not even an explicit nil
### GetShopLocationCountryIso

`func (o *ShopsResultsInner) GetShopLocationCountryIso() string`

GetShopLocationCountryIso returns the ShopLocationCountryIso field if non-nil, zero value otherwise.

### GetShopLocationCountryIsoOk

`func (o *ShopsResultsInner) GetShopLocationCountryIsoOk() (*string, bool)`

GetShopLocationCountryIsoOk returns a tuple with the ShopLocationCountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopLocationCountryIso

`func (o *ShopsResultsInner) SetShopLocationCountryIso(v string)`

SetShopLocationCountryIso sets ShopLocationCountryIso field to given value.

### HasShopLocationCountryIso

`func (o *ShopsResultsInner) HasShopLocationCountryIso() bool`

HasShopLocationCountryIso returns a boolean if a field has been set.

### SetShopLocationCountryIsoNil

`func (o *ShopsResultsInner) SetShopLocationCountryIsoNil(b bool)`

 SetShopLocationCountryIsoNil sets the value for ShopLocationCountryIso to be an explicit nil

### UnsetShopLocationCountryIso
`func (o *ShopsResultsInner) UnsetShopLocationCountryIso()`

UnsetShopLocationCountryIso ensures that no value is present for ShopLocationCountryIso, not even an explicit nil
### GetReviewCount

`func (o *ShopsResultsInner) GetReviewCount() int32`

GetReviewCount returns the ReviewCount field if non-nil, zero value otherwise.

### GetReviewCountOk

`func (o *ShopsResultsInner) GetReviewCountOk() (*int32, bool)`

GetReviewCountOk returns a tuple with the ReviewCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReviewCount

`func (o *ShopsResultsInner) SetReviewCount(v int32)`

SetReviewCount sets ReviewCount field to given value.

### HasReviewCount

`func (o *ShopsResultsInner) HasReviewCount() bool`

HasReviewCount returns a boolean if a field has been set.

### SetReviewCountNil

`func (o *ShopsResultsInner) SetReviewCountNil(b bool)`

 SetReviewCountNil sets the value for ReviewCount to be an explicit nil

### UnsetReviewCount
`func (o *ShopsResultsInner) UnsetReviewCount()`

UnsetReviewCount ensures that no value is present for ReviewCount, not even an explicit nil
### GetReviewAverage

`func (o *ShopsResultsInner) GetReviewAverage() float32`

GetReviewAverage returns the ReviewAverage field if non-nil, zero value otherwise.

### GetReviewAverageOk

`func (o *ShopsResultsInner) GetReviewAverageOk() (*float32, bool)`

GetReviewAverageOk returns a tuple with the ReviewAverage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReviewAverage

`func (o *ShopsResultsInner) SetReviewAverage(v float32)`

SetReviewAverage sets ReviewAverage field to given value.

### HasReviewAverage

`func (o *ShopsResultsInner) HasReviewAverage() bool`

HasReviewAverage returns a boolean if a field has been set.

### SetReviewAverageNil

`func (o *ShopsResultsInner) SetReviewAverageNil(b bool)`

 SetReviewAverageNil sets the value for ReviewAverage to be an explicit nil

### UnsetReviewAverage
`func (o *ShopsResultsInner) UnsetReviewAverage()`

UnsetReviewAverage ensures that no value is present for ReviewAverage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


