# ShopListingsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListingId** | Pointer to **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | [optional] 
**UserId** | Pointer to **int32** | The numeric ID for the [user](/documentation/reference#tag/User) posting the listing. | [optional] 
**ShopId** | Pointer to **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | [optional] 
**Title** | Pointer to **string** | The listing&#39;s title string. When creating or updating a listing, valid title strings contain only letters, numbers, punctuation marks, mathematical symbols, whitespace characters, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{P}\\\\p{Sm}\\\\p{Zs}™©®]/u) You can only use the %, :, &amp; and + characters once each. | [optional] 
**Description** | Pointer to **string** | A description string of the product for sale in the listing. | [optional] 
**State** | Pointer to **string** | When _updating_ a listing, this value can be either &#x60;active&#x60; or &#x60;inactive&#x60;. Note: Setting a &#x60;draft&#x60; listing to &#x60;active&#x60; will also publish the listing on etsy.com and requires that the listing have an image set. Setting a &#x60;sold_out&#x60; listing to active will update the quantity to 1 and renew the listing on etsy.com. | [optional] 
**CreationTimestamp** | Pointer to **int32** | The listing\\&#39;s creation time, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The listing\\&#39;s creation time, in epoch seconds. | [optional] 
**EndingTimestamp** | Pointer to **int32** | The listing\\&#39;s expiration time, in epoch seconds. | [optional] 
**OriginalCreationTimestamp** | Pointer to **int32** | The listing\\&#39;s creation time, in epoch seconds. | [optional] 
**LastModifiedTimestamp** | Pointer to **int32** | The time of the last update to the listing, in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The time of the last update to the listing, in epoch seconds. | [optional] 
**StateTimestamp** | Pointer to **int32** | The date and time of the last state change of this listing. | [optional] 
**Quantity** | Pointer to **int32** | The positive non-zero number of products available for purchase in the listing. Note: The listing quantity is the sum of available offering quantities. You can request the quantities for individual offerings from the ListingInventory resource using the [getListingInventory](/documentation/reference#operation/getListingInventory) endpoint. | [optional] 
**ShopSectionId** | Pointer to **NullableInt32** | The numeric ID of a section in a specific Etsy shop. | [optional] 
**FeaturedRank** | Pointer to **int32** | The positive non-zero numeric position in the featured listings of the shop, with rank 1 listings appearing in the left-most position in featured listing on a shop’s home page. | [optional] 
**Url** | Pointer to **string** | The full URL to the listing&#39;s page on Etsy. | [optional] 
**NumFavorers** | Pointer to **int32** | The number of users who marked this Listing a favorite. | [optional] 
**NonTaxable** | Pointer to **bool** | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates do not apply to this listing at checkout. | [optional] 
**IsTaxable** | Pointer to **bool** | When true, applicable [shop](/documentation/reference#tag/Shop) tax rates apply to this listing at checkout. | [optional] 
**IsCustomizable** | Pointer to **bool** | When true, a buyer may contact the seller for a customized order. The default value is true when a shop accepts custom orders. Does not apply to shops that do not accept custom orders. | [optional] 
**IsPersonalizable** | Pointer to **bool** | When true, this listing is personalizable. The default value is null. | [optional] 
**PersonalizationIsRequired** | Pointer to **bool** | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is &#39;true&#39;. | [optional] 
**PersonalizationCharCountMax** | Pointer to **NullableInt32** | This is an integer value representing the maximum length for the personalization message entered by the buyer. Will only change if is_personalizable is &#39;true&#39;. | [optional] 
**PersonalizationInstructions** | Pointer to **NullableString** | When true, this listing requires personalization. The default value is null. Will only change if is_personalizable is &#39;true&#39;. | [optional] 
**ListingType** | Pointer to **string** | An enumerated type string that indicates whether the listing is physical or a digital download. | [optional] 
**Tags** | Pointer to **[]string** | A comma-separated list of tag strings for the listing. When creating or updating a listing, valid tag strings contain only letters, numbers, whitespace characters, -, &#39;, ™, ©, and ®. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}\\\\-&#39;™©®]/u) Default value is null. | [optional] 
**Materials** | Pointer to **[]string** | A list of material strings for materials used in the product. Valid materials strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. | [optional] 
**ShippingProfileId** | Pointer to **NullableInt32** | The numeric ID of the [shipping profile](/documentation/reference#operation/getShopShippingProfile) associated with the listing. Required when listing type is &#x60;physical&#x60;. | [optional] 
**ReturnPolicyId** | Pointer to **NullableInt32** | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). | [optional] 
**ProcessingMin** | Pointer to **NullableInt32** | The minimum number of days required to process this listing. Default value is null. | [optional] 
**ProcessingMax** | Pointer to **NullableInt32** | The maximum number of days required to process this listing. Default value is null. | [optional] 
**WhoMade** | Pointer to **NullableString** | An enumerated string indicating who made the product. Helps buyers locate the listing under the Handmade heading. Requires &#39;is_supply&#39; and &#39;when_made&#39;. | [optional] 
**WhenMade** | Pointer to **NullableString** | An enumerated string for the era in which the maker made the product in this listing. Helps buyers locate the listing under the Vintage heading. Requires &#39;is_supply&#39; and &#39;who_made&#39;. | [optional] 
**IsSupply** | Pointer to **NullableBool** | When true, tags the listing as a supply product, else indicates that it&#39;s a finished product. Helps buyers locate the listing under the Supplies heading. Requires &#39;who_made&#39; and &#39;when_made&#39;. | [optional] 
**ItemWeight** | Pointer to **NullableFloat32** | The numeric weight of the product measured in units set in \\&#39;item_weight_unit\\&#39;. Default value is null. If set, the value must be greater than 0. | [optional] 
**ItemWeightUnit** | Pointer to **NullableString** | A string defining the units used to measure the weight of the product. Default value is null. | [optional] 
**ItemLength** | Pointer to **NullableFloat32** | The numeric length of the product measured in units set in \\&#39;item_dimensions_unit\\&#39;. Default value is null. If set, the value must be greater than 0. | [optional] 
**ItemWidth** | Pointer to **NullableFloat32** | The numeric width of the product measured in units set in \\&#39;item_dimensions_unit\\&#39;. Default value is null. If set, the value must be greater than 0. | [optional] 
**ItemHeight** | Pointer to **NullableFloat32** | The numeric length of the product measured in units set in \\&#39;item_dimensions_unit\\&#39;. Default value is null. If set, the value must be greater than 0. | [optional] 
**ItemDimensionsUnit** | Pointer to **NullableString** | A string defining the units used to measure the dimensions of the product. Default value is null. | [optional] 
**IsPrivate** | Pointer to **bool** | When true, this is a private listing intended for a specific buyer and hidden from shop view. | [optional] 
**Style** | Pointer to **[]string** | An array of style strings for this listing, each of which is free-form text string such as \\\&quot;Formal\\\&quot;, or \\\&quot;Steampunk\\\&quot;. When creating or updating a listing, the listing may have up to two styles. Valid style strings contain only letters, numbers, and whitespace characters. (regex: /[^\\\\p{L}\\\\p{Nd}\\\\p{Zs}]/u) Default value is null. | [optional] 
**FileData** | Pointer to **string** | A string describing the files attached to a digital listing. | [optional] 
**HasVariations** | Pointer to **bool** | When true, the listing has variations. | [optional] 
**ShouldAutoRenew** | Pointer to **bool** | When true, renews a listing for four months upon expiration. | [optional] 
**Language** | Pointer to **NullableString** | The IETF language tag for the default language of the listing. Ex: &#x60;de&#x60;, &#x60;en&#x60;, &#x60;es&#x60;, &#x60;fr&#x60;, &#x60;it&#x60;, &#x60;ja&#x60;, &#x60;nl&#x60;, &#x60;pl&#x60;, &#x60;pt&#x60;, &#x60;ru&#x60;. | [optional] 
**Price** | Pointer to [**ShopListingPrice**](ShopListingPrice.md) |  | [optional] 
**TaxonomyId** | Pointer to **NullableInt32** | The numerical taxonomy ID of the listing. See [SellerTaxonomy](/documentation/reference#tag/SellerTaxonomy) and [BuyerTaxonomy](/documentation/reference#tag/BuyerTaxonomy) for more information. | [optional] 

## Methods

### NewShopListingsResultsInner

`func NewShopListingsResultsInner() *ShopListingsResultsInner`

NewShopListingsResultsInner instantiates a new ShopListingsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingsResultsInnerWithDefaults

`func NewShopListingsResultsInnerWithDefaults() *ShopListingsResultsInner`

NewShopListingsResultsInnerWithDefaults instantiates a new ShopListingsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListingId

`func (o *ShopListingsResultsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ShopListingsResultsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ShopListingsResultsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ShopListingsResultsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### GetUserId

`func (o *ShopListingsResultsInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ShopListingsResultsInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ShopListingsResultsInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ShopListingsResultsInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetShopId

`func (o *ShopListingsResultsInner) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *ShopListingsResultsInner) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *ShopListingsResultsInner) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *ShopListingsResultsInner) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetTitle

`func (o *ShopListingsResultsInner) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopListingsResultsInner) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopListingsResultsInner) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopListingsResultsInner) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetDescription

`func (o *ShopListingsResultsInner) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ShopListingsResultsInner) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ShopListingsResultsInner) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ShopListingsResultsInner) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetState

`func (o *ShopListingsResultsInner) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ShopListingsResultsInner) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ShopListingsResultsInner) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *ShopListingsResultsInner) HasState() bool`

HasState returns a boolean if a field has been set.

### GetCreationTimestamp

`func (o *ShopListingsResultsInner) GetCreationTimestamp() int32`

GetCreationTimestamp returns the CreationTimestamp field if non-nil, zero value otherwise.

### GetCreationTimestampOk

`func (o *ShopListingsResultsInner) GetCreationTimestampOk() (*int32, bool)`

GetCreationTimestampOk returns a tuple with the CreationTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreationTimestamp

`func (o *ShopListingsResultsInner) SetCreationTimestamp(v int32)`

SetCreationTimestamp sets CreationTimestamp field to given value.

### HasCreationTimestamp

`func (o *ShopListingsResultsInner) HasCreationTimestamp() bool`

HasCreationTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopListingsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopListingsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopListingsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopListingsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetEndingTimestamp

`func (o *ShopListingsResultsInner) GetEndingTimestamp() int32`

GetEndingTimestamp returns the EndingTimestamp field if non-nil, zero value otherwise.

### GetEndingTimestampOk

`func (o *ShopListingsResultsInner) GetEndingTimestampOk() (*int32, bool)`

GetEndingTimestampOk returns a tuple with the EndingTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndingTimestamp

`func (o *ShopListingsResultsInner) SetEndingTimestamp(v int32)`

SetEndingTimestamp sets EndingTimestamp field to given value.

### HasEndingTimestamp

`func (o *ShopListingsResultsInner) HasEndingTimestamp() bool`

HasEndingTimestamp returns a boolean if a field has been set.

### GetOriginalCreationTimestamp

`func (o *ShopListingsResultsInner) GetOriginalCreationTimestamp() int32`

GetOriginalCreationTimestamp returns the OriginalCreationTimestamp field if non-nil, zero value otherwise.

### GetOriginalCreationTimestampOk

`func (o *ShopListingsResultsInner) GetOriginalCreationTimestampOk() (*int32, bool)`

GetOriginalCreationTimestampOk returns a tuple with the OriginalCreationTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalCreationTimestamp

`func (o *ShopListingsResultsInner) SetOriginalCreationTimestamp(v int32)`

SetOriginalCreationTimestamp sets OriginalCreationTimestamp field to given value.

### HasOriginalCreationTimestamp

`func (o *ShopListingsResultsInner) HasOriginalCreationTimestamp() bool`

HasOriginalCreationTimestamp returns a boolean if a field has been set.

### GetLastModifiedTimestamp

`func (o *ShopListingsResultsInner) GetLastModifiedTimestamp() int32`

GetLastModifiedTimestamp returns the LastModifiedTimestamp field if non-nil, zero value otherwise.

### GetLastModifiedTimestampOk

`func (o *ShopListingsResultsInner) GetLastModifiedTimestampOk() (*int32, bool)`

GetLastModifiedTimestampOk returns a tuple with the LastModifiedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModifiedTimestamp

`func (o *ShopListingsResultsInner) SetLastModifiedTimestamp(v int32)`

SetLastModifiedTimestamp sets LastModifiedTimestamp field to given value.

### HasLastModifiedTimestamp

`func (o *ShopListingsResultsInner) HasLastModifiedTimestamp() bool`

HasLastModifiedTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *ShopListingsResultsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *ShopListingsResultsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *ShopListingsResultsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *ShopListingsResultsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetStateTimestamp

`func (o *ShopListingsResultsInner) GetStateTimestamp() int32`

GetStateTimestamp returns the StateTimestamp field if non-nil, zero value otherwise.

### GetStateTimestampOk

`func (o *ShopListingsResultsInner) GetStateTimestampOk() (*int32, bool)`

GetStateTimestampOk returns a tuple with the StateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStateTimestamp

`func (o *ShopListingsResultsInner) SetStateTimestamp(v int32)`

SetStateTimestamp sets StateTimestamp field to given value.

### HasStateTimestamp

`func (o *ShopListingsResultsInner) HasStateTimestamp() bool`

HasStateTimestamp returns a boolean if a field has been set.

### GetQuantity

`func (o *ShopListingsResultsInner) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *ShopListingsResultsInner) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *ShopListingsResultsInner) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.

### HasQuantity

`func (o *ShopListingsResultsInner) HasQuantity() bool`

HasQuantity returns a boolean if a field has been set.

### GetShopSectionId

`func (o *ShopListingsResultsInner) GetShopSectionId() int32`

GetShopSectionId returns the ShopSectionId field if non-nil, zero value otherwise.

### GetShopSectionIdOk

`func (o *ShopListingsResultsInner) GetShopSectionIdOk() (*int32, bool)`

GetShopSectionIdOk returns a tuple with the ShopSectionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopSectionId

`func (o *ShopListingsResultsInner) SetShopSectionId(v int32)`

SetShopSectionId sets ShopSectionId field to given value.

### HasShopSectionId

`func (o *ShopListingsResultsInner) HasShopSectionId() bool`

HasShopSectionId returns a boolean if a field has been set.

### SetShopSectionIdNil

`func (o *ShopListingsResultsInner) SetShopSectionIdNil(b bool)`

 SetShopSectionIdNil sets the value for ShopSectionId to be an explicit nil

### UnsetShopSectionId
`func (o *ShopListingsResultsInner) UnsetShopSectionId()`

UnsetShopSectionId ensures that no value is present for ShopSectionId, not even an explicit nil
### GetFeaturedRank

`func (o *ShopListingsResultsInner) GetFeaturedRank() int32`

GetFeaturedRank returns the FeaturedRank field if non-nil, zero value otherwise.

### GetFeaturedRankOk

`func (o *ShopListingsResultsInner) GetFeaturedRankOk() (*int32, bool)`

GetFeaturedRankOk returns a tuple with the FeaturedRank field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeaturedRank

`func (o *ShopListingsResultsInner) SetFeaturedRank(v int32)`

SetFeaturedRank sets FeaturedRank field to given value.

### HasFeaturedRank

`func (o *ShopListingsResultsInner) HasFeaturedRank() bool`

HasFeaturedRank returns a boolean if a field has been set.

### GetUrl

`func (o *ShopListingsResultsInner) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ShopListingsResultsInner) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ShopListingsResultsInner) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *ShopListingsResultsInner) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetNumFavorers

`func (o *ShopListingsResultsInner) GetNumFavorers() int32`

GetNumFavorers returns the NumFavorers field if non-nil, zero value otherwise.

### GetNumFavorersOk

`func (o *ShopListingsResultsInner) GetNumFavorersOk() (*int32, bool)`

GetNumFavorersOk returns a tuple with the NumFavorers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumFavorers

`func (o *ShopListingsResultsInner) SetNumFavorers(v int32)`

SetNumFavorers sets NumFavorers field to given value.

### HasNumFavorers

`func (o *ShopListingsResultsInner) HasNumFavorers() bool`

HasNumFavorers returns a boolean if a field has been set.

### GetNonTaxable

`func (o *ShopListingsResultsInner) GetNonTaxable() bool`

GetNonTaxable returns the NonTaxable field if non-nil, zero value otherwise.

### GetNonTaxableOk

`func (o *ShopListingsResultsInner) GetNonTaxableOk() (*bool, bool)`

GetNonTaxableOk returns a tuple with the NonTaxable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNonTaxable

`func (o *ShopListingsResultsInner) SetNonTaxable(v bool)`

SetNonTaxable sets NonTaxable field to given value.

### HasNonTaxable

`func (o *ShopListingsResultsInner) HasNonTaxable() bool`

HasNonTaxable returns a boolean if a field has been set.

### GetIsTaxable

`func (o *ShopListingsResultsInner) GetIsTaxable() bool`

GetIsTaxable returns the IsTaxable field if non-nil, zero value otherwise.

### GetIsTaxableOk

`func (o *ShopListingsResultsInner) GetIsTaxableOk() (*bool, bool)`

GetIsTaxableOk returns a tuple with the IsTaxable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTaxable

`func (o *ShopListingsResultsInner) SetIsTaxable(v bool)`

SetIsTaxable sets IsTaxable field to given value.

### HasIsTaxable

`func (o *ShopListingsResultsInner) HasIsTaxable() bool`

HasIsTaxable returns a boolean if a field has been set.

### GetIsCustomizable

`func (o *ShopListingsResultsInner) GetIsCustomizable() bool`

GetIsCustomizable returns the IsCustomizable field if non-nil, zero value otherwise.

### GetIsCustomizableOk

`func (o *ShopListingsResultsInner) GetIsCustomizableOk() (*bool, bool)`

GetIsCustomizableOk returns a tuple with the IsCustomizable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCustomizable

`func (o *ShopListingsResultsInner) SetIsCustomizable(v bool)`

SetIsCustomizable sets IsCustomizable field to given value.

### HasIsCustomizable

`func (o *ShopListingsResultsInner) HasIsCustomizable() bool`

HasIsCustomizable returns a boolean if a field has been set.

### GetIsPersonalizable

`func (o *ShopListingsResultsInner) GetIsPersonalizable() bool`

GetIsPersonalizable returns the IsPersonalizable field if non-nil, zero value otherwise.

### GetIsPersonalizableOk

`func (o *ShopListingsResultsInner) GetIsPersonalizableOk() (*bool, bool)`

GetIsPersonalizableOk returns a tuple with the IsPersonalizable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPersonalizable

`func (o *ShopListingsResultsInner) SetIsPersonalizable(v bool)`

SetIsPersonalizable sets IsPersonalizable field to given value.

### HasIsPersonalizable

`func (o *ShopListingsResultsInner) HasIsPersonalizable() bool`

HasIsPersonalizable returns a boolean if a field has been set.

### GetPersonalizationIsRequired

`func (o *ShopListingsResultsInner) GetPersonalizationIsRequired() bool`

GetPersonalizationIsRequired returns the PersonalizationIsRequired field if non-nil, zero value otherwise.

### GetPersonalizationIsRequiredOk

`func (o *ShopListingsResultsInner) GetPersonalizationIsRequiredOk() (*bool, bool)`

GetPersonalizationIsRequiredOk returns a tuple with the PersonalizationIsRequired field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPersonalizationIsRequired

`func (o *ShopListingsResultsInner) SetPersonalizationIsRequired(v bool)`

SetPersonalizationIsRequired sets PersonalizationIsRequired field to given value.

### HasPersonalizationIsRequired

`func (o *ShopListingsResultsInner) HasPersonalizationIsRequired() bool`

HasPersonalizationIsRequired returns a boolean if a field has been set.

### GetPersonalizationCharCountMax

`func (o *ShopListingsResultsInner) GetPersonalizationCharCountMax() int32`

GetPersonalizationCharCountMax returns the PersonalizationCharCountMax field if non-nil, zero value otherwise.

### GetPersonalizationCharCountMaxOk

`func (o *ShopListingsResultsInner) GetPersonalizationCharCountMaxOk() (*int32, bool)`

GetPersonalizationCharCountMaxOk returns a tuple with the PersonalizationCharCountMax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPersonalizationCharCountMax

`func (o *ShopListingsResultsInner) SetPersonalizationCharCountMax(v int32)`

SetPersonalizationCharCountMax sets PersonalizationCharCountMax field to given value.

### HasPersonalizationCharCountMax

`func (o *ShopListingsResultsInner) HasPersonalizationCharCountMax() bool`

HasPersonalizationCharCountMax returns a boolean if a field has been set.

### SetPersonalizationCharCountMaxNil

`func (o *ShopListingsResultsInner) SetPersonalizationCharCountMaxNil(b bool)`

 SetPersonalizationCharCountMaxNil sets the value for PersonalizationCharCountMax to be an explicit nil

### UnsetPersonalizationCharCountMax
`func (o *ShopListingsResultsInner) UnsetPersonalizationCharCountMax()`

UnsetPersonalizationCharCountMax ensures that no value is present for PersonalizationCharCountMax, not even an explicit nil
### GetPersonalizationInstructions

`func (o *ShopListingsResultsInner) GetPersonalizationInstructions() string`

GetPersonalizationInstructions returns the PersonalizationInstructions field if non-nil, zero value otherwise.

### GetPersonalizationInstructionsOk

`func (o *ShopListingsResultsInner) GetPersonalizationInstructionsOk() (*string, bool)`

GetPersonalizationInstructionsOk returns a tuple with the PersonalizationInstructions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPersonalizationInstructions

`func (o *ShopListingsResultsInner) SetPersonalizationInstructions(v string)`

SetPersonalizationInstructions sets PersonalizationInstructions field to given value.

### HasPersonalizationInstructions

`func (o *ShopListingsResultsInner) HasPersonalizationInstructions() bool`

HasPersonalizationInstructions returns a boolean if a field has been set.

### SetPersonalizationInstructionsNil

`func (o *ShopListingsResultsInner) SetPersonalizationInstructionsNil(b bool)`

 SetPersonalizationInstructionsNil sets the value for PersonalizationInstructions to be an explicit nil

### UnsetPersonalizationInstructions
`func (o *ShopListingsResultsInner) UnsetPersonalizationInstructions()`

UnsetPersonalizationInstructions ensures that no value is present for PersonalizationInstructions, not even an explicit nil
### GetListingType

`func (o *ShopListingsResultsInner) GetListingType() string`

GetListingType returns the ListingType field if non-nil, zero value otherwise.

### GetListingTypeOk

`func (o *ShopListingsResultsInner) GetListingTypeOk() (*string, bool)`

GetListingTypeOk returns a tuple with the ListingType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingType

`func (o *ShopListingsResultsInner) SetListingType(v string)`

SetListingType sets ListingType field to given value.

### HasListingType

`func (o *ShopListingsResultsInner) HasListingType() bool`

HasListingType returns a boolean if a field has been set.

### GetTags

`func (o *ShopListingsResultsInner) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *ShopListingsResultsInner) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *ShopListingsResultsInner) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *ShopListingsResultsInner) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetMaterials

`func (o *ShopListingsResultsInner) GetMaterials() []string`

GetMaterials returns the Materials field if non-nil, zero value otherwise.

### GetMaterialsOk

`func (o *ShopListingsResultsInner) GetMaterialsOk() (*[]string, bool)`

GetMaterialsOk returns a tuple with the Materials field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaterials

`func (o *ShopListingsResultsInner) SetMaterials(v []string)`

SetMaterials sets Materials field to given value.

### HasMaterials

`func (o *ShopListingsResultsInner) HasMaterials() bool`

HasMaterials returns a boolean if a field has been set.

### GetShippingProfileId

`func (o *ShopListingsResultsInner) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopListingsResultsInner) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopListingsResultsInner) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopListingsResultsInner) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### SetShippingProfileIdNil

`func (o *ShopListingsResultsInner) SetShippingProfileIdNil(b bool)`

 SetShippingProfileIdNil sets the value for ShippingProfileId to be an explicit nil

### UnsetShippingProfileId
`func (o *ShopListingsResultsInner) UnsetShippingProfileId()`

UnsetShippingProfileId ensures that no value is present for ShippingProfileId, not even an explicit nil
### GetReturnPolicyId

`func (o *ShopListingsResultsInner) GetReturnPolicyId() int32`

GetReturnPolicyId returns the ReturnPolicyId field if non-nil, zero value otherwise.

### GetReturnPolicyIdOk

`func (o *ShopListingsResultsInner) GetReturnPolicyIdOk() (*int32, bool)`

GetReturnPolicyIdOk returns a tuple with the ReturnPolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnPolicyId

`func (o *ShopListingsResultsInner) SetReturnPolicyId(v int32)`

SetReturnPolicyId sets ReturnPolicyId field to given value.

### HasReturnPolicyId

`func (o *ShopListingsResultsInner) HasReturnPolicyId() bool`

HasReturnPolicyId returns a boolean if a field has been set.

### SetReturnPolicyIdNil

`func (o *ShopListingsResultsInner) SetReturnPolicyIdNil(b bool)`

 SetReturnPolicyIdNil sets the value for ReturnPolicyId to be an explicit nil

### UnsetReturnPolicyId
`func (o *ShopListingsResultsInner) UnsetReturnPolicyId()`

UnsetReturnPolicyId ensures that no value is present for ReturnPolicyId, not even an explicit nil
### GetProcessingMin

`func (o *ShopListingsResultsInner) GetProcessingMin() int32`

GetProcessingMin returns the ProcessingMin field if non-nil, zero value otherwise.

### GetProcessingMinOk

`func (o *ShopListingsResultsInner) GetProcessingMinOk() (*int32, bool)`

GetProcessingMinOk returns a tuple with the ProcessingMin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessingMin

`func (o *ShopListingsResultsInner) SetProcessingMin(v int32)`

SetProcessingMin sets ProcessingMin field to given value.

### HasProcessingMin

`func (o *ShopListingsResultsInner) HasProcessingMin() bool`

HasProcessingMin returns a boolean if a field has been set.

### SetProcessingMinNil

`func (o *ShopListingsResultsInner) SetProcessingMinNil(b bool)`

 SetProcessingMinNil sets the value for ProcessingMin to be an explicit nil

### UnsetProcessingMin
`func (o *ShopListingsResultsInner) UnsetProcessingMin()`

UnsetProcessingMin ensures that no value is present for ProcessingMin, not even an explicit nil
### GetProcessingMax

`func (o *ShopListingsResultsInner) GetProcessingMax() int32`

GetProcessingMax returns the ProcessingMax field if non-nil, zero value otherwise.

### GetProcessingMaxOk

`func (o *ShopListingsResultsInner) GetProcessingMaxOk() (*int32, bool)`

GetProcessingMaxOk returns a tuple with the ProcessingMax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessingMax

`func (o *ShopListingsResultsInner) SetProcessingMax(v int32)`

SetProcessingMax sets ProcessingMax field to given value.

### HasProcessingMax

`func (o *ShopListingsResultsInner) HasProcessingMax() bool`

HasProcessingMax returns a boolean if a field has been set.

### SetProcessingMaxNil

`func (o *ShopListingsResultsInner) SetProcessingMaxNil(b bool)`

 SetProcessingMaxNil sets the value for ProcessingMax to be an explicit nil

### UnsetProcessingMax
`func (o *ShopListingsResultsInner) UnsetProcessingMax()`

UnsetProcessingMax ensures that no value is present for ProcessingMax, not even an explicit nil
### GetWhoMade

`func (o *ShopListingsResultsInner) GetWhoMade() string`

GetWhoMade returns the WhoMade field if non-nil, zero value otherwise.

### GetWhoMadeOk

`func (o *ShopListingsResultsInner) GetWhoMadeOk() (*string, bool)`

GetWhoMadeOk returns a tuple with the WhoMade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhoMade

`func (o *ShopListingsResultsInner) SetWhoMade(v string)`

SetWhoMade sets WhoMade field to given value.

### HasWhoMade

`func (o *ShopListingsResultsInner) HasWhoMade() bool`

HasWhoMade returns a boolean if a field has been set.

### SetWhoMadeNil

`func (o *ShopListingsResultsInner) SetWhoMadeNil(b bool)`

 SetWhoMadeNil sets the value for WhoMade to be an explicit nil

### UnsetWhoMade
`func (o *ShopListingsResultsInner) UnsetWhoMade()`

UnsetWhoMade ensures that no value is present for WhoMade, not even an explicit nil
### GetWhenMade

`func (o *ShopListingsResultsInner) GetWhenMade() string`

GetWhenMade returns the WhenMade field if non-nil, zero value otherwise.

### GetWhenMadeOk

`func (o *ShopListingsResultsInner) GetWhenMadeOk() (*string, bool)`

GetWhenMadeOk returns a tuple with the WhenMade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhenMade

`func (o *ShopListingsResultsInner) SetWhenMade(v string)`

SetWhenMade sets WhenMade field to given value.

### HasWhenMade

`func (o *ShopListingsResultsInner) HasWhenMade() bool`

HasWhenMade returns a boolean if a field has been set.

### SetWhenMadeNil

`func (o *ShopListingsResultsInner) SetWhenMadeNil(b bool)`

 SetWhenMadeNil sets the value for WhenMade to be an explicit nil

### UnsetWhenMade
`func (o *ShopListingsResultsInner) UnsetWhenMade()`

UnsetWhenMade ensures that no value is present for WhenMade, not even an explicit nil
### GetIsSupply

`func (o *ShopListingsResultsInner) GetIsSupply() bool`

GetIsSupply returns the IsSupply field if non-nil, zero value otherwise.

### GetIsSupplyOk

`func (o *ShopListingsResultsInner) GetIsSupplyOk() (*bool, bool)`

GetIsSupplyOk returns a tuple with the IsSupply field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSupply

`func (o *ShopListingsResultsInner) SetIsSupply(v bool)`

SetIsSupply sets IsSupply field to given value.

### HasIsSupply

`func (o *ShopListingsResultsInner) HasIsSupply() bool`

HasIsSupply returns a boolean if a field has been set.

### SetIsSupplyNil

`func (o *ShopListingsResultsInner) SetIsSupplyNil(b bool)`

 SetIsSupplyNil sets the value for IsSupply to be an explicit nil

### UnsetIsSupply
`func (o *ShopListingsResultsInner) UnsetIsSupply()`

UnsetIsSupply ensures that no value is present for IsSupply, not even an explicit nil
### GetItemWeight

`func (o *ShopListingsResultsInner) GetItemWeight() float32`

GetItemWeight returns the ItemWeight field if non-nil, zero value otherwise.

### GetItemWeightOk

`func (o *ShopListingsResultsInner) GetItemWeightOk() (*float32, bool)`

GetItemWeightOk returns a tuple with the ItemWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemWeight

`func (o *ShopListingsResultsInner) SetItemWeight(v float32)`

SetItemWeight sets ItemWeight field to given value.

### HasItemWeight

`func (o *ShopListingsResultsInner) HasItemWeight() bool`

HasItemWeight returns a boolean if a field has been set.

### SetItemWeightNil

`func (o *ShopListingsResultsInner) SetItemWeightNil(b bool)`

 SetItemWeightNil sets the value for ItemWeight to be an explicit nil

### UnsetItemWeight
`func (o *ShopListingsResultsInner) UnsetItemWeight()`

UnsetItemWeight ensures that no value is present for ItemWeight, not even an explicit nil
### GetItemWeightUnit

`func (o *ShopListingsResultsInner) GetItemWeightUnit() string`

GetItemWeightUnit returns the ItemWeightUnit field if non-nil, zero value otherwise.

### GetItemWeightUnitOk

`func (o *ShopListingsResultsInner) GetItemWeightUnitOk() (*string, bool)`

GetItemWeightUnitOk returns a tuple with the ItemWeightUnit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemWeightUnit

`func (o *ShopListingsResultsInner) SetItemWeightUnit(v string)`

SetItemWeightUnit sets ItemWeightUnit field to given value.

### HasItemWeightUnit

`func (o *ShopListingsResultsInner) HasItemWeightUnit() bool`

HasItemWeightUnit returns a boolean if a field has been set.

### SetItemWeightUnitNil

`func (o *ShopListingsResultsInner) SetItemWeightUnitNil(b bool)`

 SetItemWeightUnitNil sets the value for ItemWeightUnit to be an explicit nil

### UnsetItemWeightUnit
`func (o *ShopListingsResultsInner) UnsetItemWeightUnit()`

UnsetItemWeightUnit ensures that no value is present for ItemWeightUnit, not even an explicit nil
### GetItemLength

`func (o *ShopListingsResultsInner) GetItemLength() float32`

GetItemLength returns the ItemLength field if non-nil, zero value otherwise.

### GetItemLengthOk

`func (o *ShopListingsResultsInner) GetItemLengthOk() (*float32, bool)`

GetItemLengthOk returns a tuple with the ItemLength field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemLength

`func (o *ShopListingsResultsInner) SetItemLength(v float32)`

SetItemLength sets ItemLength field to given value.

### HasItemLength

`func (o *ShopListingsResultsInner) HasItemLength() bool`

HasItemLength returns a boolean if a field has been set.

### SetItemLengthNil

`func (o *ShopListingsResultsInner) SetItemLengthNil(b bool)`

 SetItemLengthNil sets the value for ItemLength to be an explicit nil

### UnsetItemLength
`func (o *ShopListingsResultsInner) UnsetItemLength()`

UnsetItemLength ensures that no value is present for ItemLength, not even an explicit nil
### GetItemWidth

`func (o *ShopListingsResultsInner) GetItemWidth() float32`

GetItemWidth returns the ItemWidth field if non-nil, zero value otherwise.

### GetItemWidthOk

`func (o *ShopListingsResultsInner) GetItemWidthOk() (*float32, bool)`

GetItemWidthOk returns a tuple with the ItemWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemWidth

`func (o *ShopListingsResultsInner) SetItemWidth(v float32)`

SetItemWidth sets ItemWidth field to given value.

### HasItemWidth

`func (o *ShopListingsResultsInner) HasItemWidth() bool`

HasItemWidth returns a boolean if a field has been set.

### SetItemWidthNil

`func (o *ShopListingsResultsInner) SetItemWidthNil(b bool)`

 SetItemWidthNil sets the value for ItemWidth to be an explicit nil

### UnsetItemWidth
`func (o *ShopListingsResultsInner) UnsetItemWidth()`

UnsetItemWidth ensures that no value is present for ItemWidth, not even an explicit nil
### GetItemHeight

`func (o *ShopListingsResultsInner) GetItemHeight() float32`

GetItemHeight returns the ItemHeight field if non-nil, zero value otherwise.

### GetItemHeightOk

`func (o *ShopListingsResultsInner) GetItemHeightOk() (*float32, bool)`

GetItemHeightOk returns a tuple with the ItemHeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemHeight

`func (o *ShopListingsResultsInner) SetItemHeight(v float32)`

SetItemHeight sets ItemHeight field to given value.

### HasItemHeight

`func (o *ShopListingsResultsInner) HasItemHeight() bool`

HasItemHeight returns a boolean if a field has been set.

### SetItemHeightNil

`func (o *ShopListingsResultsInner) SetItemHeightNil(b bool)`

 SetItemHeightNil sets the value for ItemHeight to be an explicit nil

### UnsetItemHeight
`func (o *ShopListingsResultsInner) UnsetItemHeight()`

UnsetItemHeight ensures that no value is present for ItemHeight, not even an explicit nil
### GetItemDimensionsUnit

`func (o *ShopListingsResultsInner) GetItemDimensionsUnit() string`

GetItemDimensionsUnit returns the ItemDimensionsUnit field if non-nil, zero value otherwise.

### GetItemDimensionsUnitOk

`func (o *ShopListingsResultsInner) GetItemDimensionsUnitOk() (*string, bool)`

GetItemDimensionsUnitOk returns a tuple with the ItemDimensionsUnit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemDimensionsUnit

`func (o *ShopListingsResultsInner) SetItemDimensionsUnit(v string)`

SetItemDimensionsUnit sets ItemDimensionsUnit field to given value.

### HasItemDimensionsUnit

`func (o *ShopListingsResultsInner) HasItemDimensionsUnit() bool`

HasItemDimensionsUnit returns a boolean if a field has been set.

### SetItemDimensionsUnitNil

`func (o *ShopListingsResultsInner) SetItemDimensionsUnitNil(b bool)`

 SetItemDimensionsUnitNil sets the value for ItemDimensionsUnit to be an explicit nil

### UnsetItemDimensionsUnit
`func (o *ShopListingsResultsInner) UnsetItemDimensionsUnit()`

UnsetItemDimensionsUnit ensures that no value is present for ItemDimensionsUnit, not even an explicit nil
### GetIsPrivate

`func (o *ShopListingsResultsInner) GetIsPrivate() bool`

GetIsPrivate returns the IsPrivate field if non-nil, zero value otherwise.

### GetIsPrivateOk

`func (o *ShopListingsResultsInner) GetIsPrivateOk() (*bool, bool)`

GetIsPrivateOk returns a tuple with the IsPrivate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPrivate

`func (o *ShopListingsResultsInner) SetIsPrivate(v bool)`

SetIsPrivate sets IsPrivate field to given value.

### HasIsPrivate

`func (o *ShopListingsResultsInner) HasIsPrivate() bool`

HasIsPrivate returns a boolean if a field has been set.

### GetStyle

`func (o *ShopListingsResultsInner) GetStyle() []string`

GetStyle returns the Style field if non-nil, zero value otherwise.

### GetStyleOk

`func (o *ShopListingsResultsInner) GetStyleOk() (*[]string, bool)`

GetStyleOk returns a tuple with the Style field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStyle

`func (o *ShopListingsResultsInner) SetStyle(v []string)`

SetStyle sets Style field to given value.

### HasStyle

`func (o *ShopListingsResultsInner) HasStyle() bool`

HasStyle returns a boolean if a field has been set.

### GetFileData

`func (o *ShopListingsResultsInner) GetFileData() string`

GetFileData returns the FileData field if non-nil, zero value otherwise.

### GetFileDataOk

`func (o *ShopListingsResultsInner) GetFileDataOk() (*string, bool)`

GetFileDataOk returns a tuple with the FileData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileData

`func (o *ShopListingsResultsInner) SetFileData(v string)`

SetFileData sets FileData field to given value.

### HasFileData

`func (o *ShopListingsResultsInner) HasFileData() bool`

HasFileData returns a boolean if a field has been set.

### GetHasVariations

`func (o *ShopListingsResultsInner) GetHasVariations() bool`

GetHasVariations returns the HasVariations field if non-nil, zero value otherwise.

### GetHasVariationsOk

`func (o *ShopListingsResultsInner) GetHasVariationsOk() (*bool, bool)`

GetHasVariationsOk returns a tuple with the HasVariations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasVariations

`func (o *ShopListingsResultsInner) SetHasVariations(v bool)`

SetHasVariations sets HasVariations field to given value.

### HasHasVariations

`func (o *ShopListingsResultsInner) HasHasVariations() bool`

HasHasVariations returns a boolean if a field has been set.

### GetShouldAutoRenew

`func (o *ShopListingsResultsInner) GetShouldAutoRenew() bool`

GetShouldAutoRenew returns the ShouldAutoRenew field if non-nil, zero value otherwise.

### GetShouldAutoRenewOk

`func (o *ShopListingsResultsInner) GetShouldAutoRenewOk() (*bool, bool)`

GetShouldAutoRenewOk returns a tuple with the ShouldAutoRenew field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShouldAutoRenew

`func (o *ShopListingsResultsInner) SetShouldAutoRenew(v bool)`

SetShouldAutoRenew sets ShouldAutoRenew field to given value.

### HasShouldAutoRenew

`func (o *ShopListingsResultsInner) HasShouldAutoRenew() bool`

HasShouldAutoRenew returns a boolean if a field has been set.

### GetLanguage

`func (o *ShopListingsResultsInner) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *ShopListingsResultsInner) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *ShopListingsResultsInner) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *ShopListingsResultsInner) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### SetLanguageNil

`func (o *ShopListingsResultsInner) SetLanguageNil(b bool)`

 SetLanguageNil sets the value for Language to be an explicit nil

### UnsetLanguage
`func (o *ShopListingsResultsInner) UnsetLanguage()`

UnsetLanguage ensures that no value is present for Language, not even an explicit nil
### GetPrice

`func (o *ShopListingsResultsInner) GetPrice() ShopListingPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ShopListingsResultsInner) GetPriceOk() (*ShopListingPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ShopListingsResultsInner) SetPrice(v ShopListingPrice)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ShopListingsResultsInner) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetTaxonomyId

`func (o *ShopListingsResultsInner) GetTaxonomyId() int32`

GetTaxonomyId returns the TaxonomyId field if non-nil, zero value otherwise.

### GetTaxonomyIdOk

`func (o *ShopListingsResultsInner) GetTaxonomyIdOk() (*int32, bool)`

GetTaxonomyIdOk returns a tuple with the TaxonomyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaxonomyId

`func (o *ShopListingsResultsInner) SetTaxonomyId(v int32)`

SetTaxonomyId sets TaxonomyId field to given value.

### HasTaxonomyId

`func (o *ShopListingsResultsInner) HasTaxonomyId() bool`

HasTaxonomyId returns a boolean if a field has been set.

### SetTaxonomyIdNil

`func (o *ShopListingsResultsInner) SetTaxonomyIdNil(b bool)`

 SetTaxonomyIdNil sets the value for TaxonomyId to be an explicit nil

### UnsetTaxonomyId
`func (o *ShopListingsResultsInner) UnsetTaxonomyId()`

UnsetTaxonomyId ensures that no value is present for TaxonomyId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


