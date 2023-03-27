# ShopReceiptTransactionsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TransactionId** | Pointer to **int32** | The unique numeric ID for a transaction. | [optional] 
**Title** | Pointer to **NullableString** | The title string of the [listing](/documentation/reference#tag/ShopListing) purchased in this transaction. | [optional] 
**Description** | Pointer to **NullableString** | The description string of the [listing](/documentation/reference#tag/ShopListing) purchased in this transaction. | [optional] 
**SellerUserId** | Pointer to **int32** | The numeric user ID for the seller in this transaction. | [optional] 
**BuyerUserId** | Pointer to **int32** | The numeric user ID for the buyer in this transaction. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The transaction\\&#39;s creation date and time, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The transaction\\&#39;s creation date and time, in epoch seconds. | [optional] 
**PaidTimestamp** | Pointer to **NullableInt32** | The transaction\\&#39;s paid date and time, in epoch seconds. | [optional] 
**ShippedTimestamp** | Pointer to **NullableInt32** | The transaction\\&#39;s shipping date and time, in epoch seconds. | [optional] 
**Quantity** | Pointer to **int32** | The numeric quantity of products purchased in this transaction. | [optional] 
**ListingImageId** | Pointer to **NullableInt32** | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. | [optional] 
**ReceiptId** | Pointer to **int32** | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction. | [optional] 
**IsDigital** | Pointer to **bool** | When true, the transaction recorded the purchase of a digital listing. | [optional] 
**FileData** | Pointer to **string** | A string describing the files purchased in this transaction. | [optional] 
**ListingId** | Pointer to **NullableInt32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | [optional] 
**TransactionType** | Pointer to **string** | The type string for the transaction, usually \&quot;listing\&quot;. | [optional] 
**ProductId** | Pointer to **NullableInt32** | The numeric ID for a specific [product](/documentation/reference#tag/ShopListing-Product) purchased from a listing. | [optional] 
**Sku** | Pointer to **NullableString** | The SKU string for the product | [optional] 
**Price** | Pointer to [**ShopReceiptTransactionPrice**](ShopReceiptTransactionPrice.md) |  | [optional] 
**ShippingCost** | Pointer to [**ShopReceiptTransactionShippingCost**](ShopReceiptTransactionShippingCost.md) |  | [optional] 
**Variations** | Pointer to [**[]ShopReceiptTransactionVariationsInner**](ShopReceiptTransactionVariationsInner.md) | Array of variations and personalizations the buyer chose. | [optional] 
**ProductData** | Pointer to [**[]ListingInventoryProductPropertyValuesInner**](ListingInventoryProductPropertyValuesInner.md) | A list of property value entries for this product. Note: parenthesis characters (&#x60;(&#x60; and &#x60;)&#x60;) are not allowed. | [optional] 
**ShippingProfileId** | Pointer to **NullableInt32** | The ID of the shipping profile selected for this listing. | [optional] 
**MinProcessingDays** | Pointer to **NullableInt32** | The minimum number of days for processing the listing. | [optional] 
**MaxProcessingDays** | Pointer to **NullableInt32** | The maximum number of days for processing the listing. | [optional] 
**ShippingMethod** | Pointer to **NullableString** | Name of the selected shipping method. | [optional] 
**ShippingUpgrade** | Pointer to **NullableString** | The name of the shipping upgrade selected for this listing. Default value is null. | [optional] 
**ExpectedShipDate** | Pointer to **NullableInt32** | The date &amp; time of the expected ship date, in epoch seconds. | [optional] 
**BuyerCoupon** | Pointer to **float32** | The amount of the buyer coupon that was discounted in the shop&#39;s currency. | [optional] [default to 0]
**ShopCoupon** | Pointer to **float32** | The amount of the shop coupon that was discounted in the shop&#39;s currency. | [optional] [default to 0]

## Methods

### NewShopReceiptTransactionsResultsInner

`func NewShopReceiptTransactionsResultsInner() *ShopReceiptTransactionsResultsInner`

NewShopReceiptTransactionsResultsInner instantiates a new ShopReceiptTransactionsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReceiptTransactionsResultsInnerWithDefaults

`func NewShopReceiptTransactionsResultsInnerWithDefaults() *ShopReceiptTransactionsResultsInner`

NewShopReceiptTransactionsResultsInnerWithDefaults instantiates a new ShopReceiptTransactionsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTransactionId

`func (o *ShopReceiptTransactionsResultsInner) GetTransactionId() int32`

GetTransactionId returns the TransactionId field if non-nil, zero value otherwise.

### GetTransactionIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetTransactionIdOk() (*int32, bool)`

GetTransactionIdOk returns a tuple with the TransactionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionId

`func (o *ShopReceiptTransactionsResultsInner) SetTransactionId(v int32)`

SetTransactionId sets TransactionId field to given value.

### HasTransactionId

`func (o *ShopReceiptTransactionsResultsInner) HasTransactionId() bool`

HasTransactionId returns a boolean if a field has been set.

### GetTitle

`func (o *ShopReceiptTransactionsResultsInner) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopReceiptTransactionsResultsInner) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopReceiptTransactionsResultsInner) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopReceiptTransactionsResultsInner) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *ShopReceiptTransactionsResultsInner) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *ShopReceiptTransactionsResultsInner) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetDescription

`func (o *ShopReceiptTransactionsResultsInner) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ShopReceiptTransactionsResultsInner) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ShopReceiptTransactionsResultsInner) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ShopReceiptTransactionsResultsInner) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *ShopReceiptTransactionsResultsInner) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *ShopReceiptTransactionsResultsInner) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetSellerUserId

`func (o *ShopReceiptTransactionsResultsInner) GetSellerUserId() int32`

GetSellerUserId returns the SellerUserId field if non-nil, zero value otherwise.

### GetSellerUserIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetSellerUserIdOk() (*int32, bool)`

GetSellerUserIdOk returns a tuple with the SellerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerUserId

`func (o *ShopReceiptTransactionsResultsInner) SetSellerUserId(v int32)`

SetSellerUserId sets SellerUserId field to given value.

### HasSellerUserId

`func (o *ShopReceiptTransactionsResultsInner) HasSellerUserId() bool`

HasSellerUserId returns a boolean if a field has been set.

### GetBuyerUserId

`func (o *ShopReceiptTransactionsResultsInner) GetBuyerUserId() int32`

GetBuyerUserId returns the BuyerUserId field if non-nil, zero value otherwise.

### GetBuyerUserIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetBuyerUserIdOk() (*int32, bool)`

GetBuyerUserIdOk returns a tuple with the BuyerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerUserId

`func (o *ShopReceiptTransactionsResultsInner) SetBuyerUserId(v int32)`

SetBuyerUserId sets BuyerUserId field to given value.

### HasBuyerUserId

`func (o *ShopReceiptTransactionsResultsInner) HasBuyerUserId() bool`

HasBuyerUserId returns a boolean if a field has been set.

### GetCreateTimestamp

`func (o *ShopReceiptTransactionsResultsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *ShopReceiptTransactionsResultsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *ShopReceiptTransactionsResultsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *ShopReceiptTransactionsResultsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopReceiptTransactionsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopReceiptTransactionsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopReceiptTransactionsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopReceiptTransactionsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetPaidTimestamp

`func (o *ShopReceiptTransactionsResultsInner) GetPaidTimestamp() int32`

GetPaidTimestamp returns the PaidTimestamp field if non-nil, zero value otherwise.

### GetPaidTimestampOk

`func (o *ShopReceiptTransactionsResultsInner) GetPaidTimestampOk() (*int32, bool)`

GetPaidTimestampOk returns a tuple with the PaidTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaidTimestamp

`func (o *ShopReceiptTransactionsResultsInner) SetPaidTimestamp(v int32)`

SetPaidTimestamp sets PaidTimestamp field to given value.

### HasPaidTimestamp

`func (o *ShopReceiptTransactionsResultsInner) HasPaidTimestamp() bool`

HasPaidTimestamp returns a boolean if a field has been set.

### SetPaidTimestampNil

`func (o *ShopReceiptTransactionsResultsInner) SetPaidTimestampNil(b bool)`

 SetPaidTimestampNil sets the value for PaidTimestamp to be an explicit nil

### UnsetPaidTimestamp
`func (o *ShopReceiptTransactionsResultsInner) UnsetPaidTimestamp()`

UnsetPaidTimestamp ensures that no value is present for PaidTimestamp, not even an explicit nil
### GetShippedTimestamp

`func (o *ShopReceiptTransactionsResultsInner) GetShippedTimestamp() int32`

GetShippedTimestamp returns the ShippedTimestamp field if non-nil, zero value otherwise.

### GetShippedTimestampOk

`func (o *ShopReceiptTransactionsResultsInner) GetShippedTimestampOk() (*int32, bool)`

GetShippedTimestampOk returns a tuple with the ShippedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippedTimestamp

`func (o *ShopReceiptTransactionsResultsInner) SetShippedTimestamp(v int32)`

SetShippedTimestamp sets ShippedTimestamp field to given value.

### HasShippedTimestamp

`func (o *ShopReceiptTransactionsResultsInner) HasShippedTimestamp() bool`

HasShippedTimestamp returns a boolean if a field has been set.

### SetShippedTimestampNil

`func (o *ShopReceiptTransactionsResultsInner) SetShippedTimestampNil(b bool)`

 SetShippedTimestampNil sets the value for ShippedTimestamp to be an explicit nil

### UnsetShippedTimestamp
`func (o *ShopReceiptTransactionsResultsInner) UnsetShippedTimestamp()`

UnsetShippedTimestamp ensures that no value is present for ShippedTimestamp, not even an explicit nil
### GetQuantity

`func (o *ShopReceiptTransactionsResultsInner) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *ShopReceiptTransactionsResultsInner) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *ShopReceiptTransactionsResultsInner) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.

### HasQuantity

`func (o *ShopReceiptTransactionsResultsInner) HasQuantity() bool`

HasQuantity returns a boolean if a field has been set.

### GetListingImageId

`func (o *ShopReceiptTransactionsResultsInner) GetListingImageId() int32`

GetListingImageId returns the ListingImageId field if non-nil, zero value otherwise.

### GetListingImageIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetListingImageIdOk() (*int32, bool)`

GetListingImageIdOk returns a tuple with the ListingImageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingImageId

`func (o *ShopReceiptTransactionsResultsInner) SetListingImageId(v int32)`

SetListingImageId sets ListingImageId field to given value.

### HasListingImageId

`func (o *ShopReceiptTransactionsResultsInner) HasListingImageId() bool`

HasListingImageId returns a boolean if a field has been set.

### SetListingImageIdNil

`func (o *ShopReceiptTransactionsResultsInner) SetListingImageIdNil(b bool)`

 SetListingImageIdNil sets the value for ListingImageId to be an explicit nil

### UnsetListingImageId
`func (o *ShopReceiptTransactionsResultsInner) UnsetListingImageId()`

UnsetListingImageId ensures that no value is present for ListingImageId, not even an explicit nil
### GetReceiptId

`func (o *ShopReceiptTransactionsResultsInner) GetReceiptId() int32`

GetReceiptId returns the ReceiptId field if non-nil, zero value otherwise.

### GetReceiptIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetReceiptIdOk() (*int32, bool)`

GetReceiptIdOk returns a tuple with the ReceiptId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptId

`func (o *ShopReceiptTransactionsResultsInner) SetReceiptId(v int32)`

SetReceiptId sets ReceiptId field to given value.

### HasReceiptId

`func (o *ShopReceiptTransactionsResultsInner) HasReceiptId() bool`

HasReceiptId returns a boolean if a field has been set.

### GetIsDigital

`func (o *ShopReceiptTransactionsResultsInner) GetIsDigital() bool`

GetIsDigital returns the IsDigital field if non-nil, zero value otherwise.

### GetIsDigitalOk

`func (o *ShopReceiptTransactionsResultsInner) GetIsDigitalOk() (*bool, bool)`

GetIsDigitalOk returns a tuple with the IsDigital field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDigital

`func (o *ShopReceiptTransactionsResultsInner) SetIsDigital(v bool)`

SetIsDigital sets IsDigital field to given value.

### HasIsDigital

`func (o *ShopReceiptTransactionsResultsInner) HasIsDigital() bool`

HasIsDigital returns a boolean if a field has been set.

### GetFileData

`func (o *ShopReceiptTransactionsResultsInner) GetFileData() string`

GetFileData returns the FileData field if non-nil, zero value otherwise.

### GetFileDataOk

`func (o *ShopReceiptTransactionsResultsInner) GetFileDataOk() (*string, bool)`

GetFileDataOk returns a tuple with the FileData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileData

`func (o *ShopReceiptTransactionsResultsInner) SetFileData(v string)`

SetFileData sets FileData field to given value.

### HasFileData

`func (o *ShopReceiptTransactionsResultsInner) HasFileData() bool`

HasFileData returns a boolean if a field has been set.

### GetListingId

`func (o *ShopReceiptTransactionsResultsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ShopReceiptTransactionsResultsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ShopReceiptTransactionsResultsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### SetListingIdNil

`func (o *ShopReceiptTransactionsResultsInner) SetListingIdNil(b bool)`

 SetListingIdNil sets the value for ListingId to be an explicit nil

### UnsetListingId
`func (o *ShopReceiptTransactionsResultsInner) UnsetListingId()`

UnsetListingId ensures that no value is present for ListingId, not even an explicit nil
### GetTransactionType

`func (o *ShopReceiptTransactionsResultsInner) GetTransactionType() string`

GetTransactionType returns the TransactionType field if non-nil, zero value otherwise.

### GetTransactionTypeOk

`func (o *ShopReceiptTransactionsResultsInner) GetTransactionTypeOk() (*string, bool)`

GetTransactionTypeOk returns a tuple with the TransactionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionType

`func (o *ShopReceiptTransactionsResultsInner) SetTransactionType(v string)`

SetTransactionType sets TransactionType field to given value.

### HasTransactionType

`func (o *ShopReceiptTransactionsResultsInner) HasTransactionType() bool`

HasTransactionType returns a boolean if a field has been set.

### GetProductId

`func (o *ShopReceiptTransactionsResultsInner) GetProductId() int32`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetProductIdOk() (*int32, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *ShopReceiptTransactionsResultsInner) SetProductId(v int32)`

SetProductId sets ProductId field to given value.

### HasProductId

`func (o *ShopReceiptTransactionsResultsInner) HasProductId() bool`

HasProductId returns a boolean if a field has been set.

### SetProductIdNil

`func (o *ShopReceiptTransactionsResultsInner) SetProductIdNil(b bool)`

 SetProductIdNil sets the value for ProductId to be an explicit nil

### UnsetProductId
`func (o *ShopReceiptTransactionsResultsInner) UnsetProductId()`

UnsetProductId ensures that no value is present for ProductId, not even an explicit nil
### GetSku

`func (o *ShopReceiptTransactionsResultsInner) GetSku() string`

GetSku returns the Sku field if non-nil, zero value otherwise.

### GetSkuOk

`func (o *ShopReceiptTransactionsResultsInner) GetSkuOk() (*string, bool)`

GetSkuOk returns a tuple with the Sku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSku

`func (o *ShopReceiptTransactionsResultsInner) SetSku(v string)`

SetSku sets Sku field to given value.

### HasSku

`func (o *ShopReceiptTransactionsResultsInner) HasSku() bool`

HasSku returns a boolean if a field has been set.

### SetSkuNil

`func (o *ShopReceiptTransactionsResultsInner) SetSkuNil(b bool)`

 SetSkuNil sets the value for Sku to be an explicit nil

### UnsetSku
`func (o *ShopReceiptTransactionsResultsInner) UnsetSku()`

UnsetSku ensures that no value is present for Sku, not even an explicit nil
### GetPrice

`func (o *ShopReceiptTransactionsResultsInner) GetPrice() ShopReceiptTransactionPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ShopReceiptTransactionsResultsInner) GetPriceOk() (*ShopReceiptTransactionPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ShopReceiptTransactionsResultsInner) SetPrice(v ShopReceiptTransactionPrice)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ShopReceiptTransactionsResultsInner) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetShippingCost

`func (o *ShopReceiptTransactionsResultsInner) GetShippingCost() ShopReceiptTransactionShippingCost`

GetShippingCost returns the ShippingCost field if non-nil, zero value otherwise.

### GetShippingCostOk

`func (o *ShopReceiptTransactionsResultsInner) GetShippingCostOk() (*ShopReceiptTransactionShippingCost, bool)`

GetShippingCostOk returns a tuple with the ShippingCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingCost

`func (o *ShopReceiptTransactionsResultsInner) SetShippingCost(v ShopReceiptTransactionShippingCost)`

SetShippingCost sets ShippingCost field to given value.

### HasShippingCost

`func (o *ShopReceiptTransactionsResultsInner) HasShippingCost() bool`

HasShippingCost returns a boolean if a field has been set.

### GetVariations

`func (o *ShopReceiptTransactionsResultsInner) GetVariations() []ShopReceiptTransactionVariationsInner`

GetVariations returns the Variations field if non-nil, zero value otherwise.

### GetVariationsOk

`func (o *ShopReceiptTransactionsResultsInner) GetVariationsOk() (*[]ShopReceiptTransactionVariationsInner, bool)`

GetVariationsOk returns a tuple with the Variations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariations

`func (o *ShopReceiptTransactionsResultsInner) SetVariations(v []ShopReceiptTransactionVariationsInner)`

SetVariations sets Variations field to given value.

### HasVariations

`func (o *ShopReceiptTransactionsResultsInner) HasVariations() bool`

HasVariations returns a boolean if a field has been set.

### GetProductData

`func (o *ShopReceiptTransactionsResultsInner) GetProductData() []ListingInventoryProductPropertyValuesInner`

GetProductData returns the ProductData field if non-nil, zero value otherwise.

### GetProductDataOk

`func (o *ShopReceiptTransactionsResultsInner) GetProductDataOk() (*[]ListingInventoryProductPropertyValuesInner, bool)`

GetProductDataOk returns a tuple with the ProductData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductData

`func (o *ShopReceiptTransactionsResultsInner) SetProductData(v []ListingInventoryProductPropertyValuesInner)`

SetProductData sets ProductData field to given value.

### HasProductData

`func (o *ShopReceiptTransactionsResultsInner) HasProductData() bool`

HasProductData returns a boolean if a field has been set.

### GetShippingProfileId

`func (o *ShopReceiptTransactionsResultsInner) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopReceiptTransactionsResultsInner) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopReceiptTransactionsResultsInner) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopReceiptTransactionsResultsInner) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### SetShippingProfileIdNil

`func (o *ShopReceiptTransactionsResultsInner) SetShippingProfileIdNil(b bool)`

 SetShippingProfileIdNil sets the value for ShippingProfileId to be an explicit nil

### UnsetShippingProfileId
`func (o *ShopReceiptTransactionsResultsInner) UnsetShippingProfileId()`

UnsetShippingProfileId ensures that no value is present for ShippingProfileId, not even an explicit nil
### GetMinProcessingDays

`func (o *ShopReceiptTransactionsResultsInner) GetMinProcessingDays() int32`

GetMinProcessingDays returns the MinProcessingDays field if non-nil, zero value otherwise.

### GetMinProcessingDaysOk

`func (o *ShopReceiptTransactionsResultsInner) GetMinProcessingDaysOk() (*int32, bool)`

GetMinProcessingDaysOk returns a tuple with the MinProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinProcessingDays

`func (o *ShopReceiptTransactionsResultsInner) SetMinProcessingDays(v int32)`

SetMinProcessingDays sets MinProcessingDays field to given value.

### HasMinProcessingDays

`func (o *ShopReceiptTransactionsResultsInner) HasMinProcessingDays() bool`

HasMinProcessingDays returns a boolean if a field has been set.

### SetMinProcessingDaysNil

`func (o *ShopReceiptTransactionsResultsInner) SetMinProcessingDaysNil(b bool)`

 SetMinProcessingDaysNil sets the value for MinProcessingDays to be an explicit nil

### UnsetMinProcessingDays
`func (o *ShopReceiptTransactionsResultsInner) UnsetMinProcessingDays()`

UnsetMinProcessingDays ensures that no value is present for MinProcessingDays, not even an explicit nil
### GetMaxProcessingDays

`func (o *ShopReceiptTransactionsResultsInner) GetMaxProcessingDays() int32`

GetMaxProcessingDays returns the MaxProcessingDays field if non-nil, zero value otherwise.

### GetMaxProcessingDaysOk

`func (o *ShopReceiptTransactionsResultsInner) GetMaxProcessingDaysOk() (*int32, bool)`

GetMaxProcessingDaysOk returns a tuple with the MaxProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxProcessingDays

`func (o *ShopReceiptTransactionsResultsInner) SetMaxProcessingDays(v int32)`

SetMaxProcessingDays sets MaxProcessingDays field to given value.

### HasMaxProcessingDays

`func (o *ShopReceiptTransactionsResultsInner) HasMaxProcessingDays() bool`

HasMaxProcessingDays returns a boolean if a field has been set.

### SetMaxProcessingDaysNil

`func (o *ShopReceiptTransactionsResultsInner) SetMaxProcessingDaysNil(b bool)`

 SetMaxProcessingDaysNil sets the value for MaxProcessingDays to be an explicit nil

### UnsetMaxProcessingDays
`func (o *ShopReceiptTransactionsResultsInner) UnsetMaxProcessingDays()`

UnsetMaxProcessingDays ensures that no value is present for MaxProcessingDays, not even an explicit nil
### GetShippingMethod

`func (o *ShopReceiptTransactionsResultsInner) GetShippingMethod() string`

GetShippingMethod returns the ShippingMethod field if non-nil, zero value otherwise.

### GetShippingMethodOk

`func (o *ShopReceiptTransactionsResultsInner) GetShippingMethodOk() (*string, bool)`

GetShippingMethodOk returns a tuple with the ShippingMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingMethod

`func (o *ShopReceiptTransactionsResultsInner) SetShippingMethod(v string)`

SetShippingMethod sets ShippingMethod field to given value.

### HasShippingMethod

`func (o *ShopReceiptTransactionsResultsInner) HasShippingMethod() bool`

HasShippingMethod returns a boolean if a field has been set.

### SetShippingMethodNil

`func (o *ShopReceiptTransactionsResultsInner) SetShippingMethodNil(b bool)`

 SetShippingMethodNil sets the value for ShippingMethod to be an explicit nil

### UnsetShippingMethod
`func (o *ShopReceiptTransactionsResultsInner) UnsetShippingMethod()`

UnsetShippingMethod ensures that no value is present for ShippingMethod, not even an explicit nil
### GetShippingUpgrade

`func (o *ShopReceiptTransactionsResultsInner) GetShippingUpgrade() string`

GetShippingUpgrade returns the ShippingUpgrade field if non-nil, zero value otherwise.

### GetShippingUpgradeOk

`func (o *ShopReceiptTransactionsResultsInner) GetShippingUpgradeOk() (*string, bool)`

GetShippingUpgradeOk returns a tuple with the ShippingUpgrade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingUpgrade

`func (o *ShopReceiptTransactionsResultsInner) SetShippingUpgrade(v string)`

SetShippingUpgrade sets ShippingUpgrade field to given value.

### HasShippingUpgrade

`func (o *ShopReceiptTransactionsResultsInner) HasShippingUpgrade() bool`

HasShippingUpgrade returns a boolean if a field has been set.

### SetShippingUpgradeNil

`func (o *ShopReceiptTransactionsResultsInner) SetShippingUpgradeNil(b bool)`

 SetShippingUpgradeNil sets the value for ShippingUpgrade to be an explicit nil

### UnsetShippingUpgrade
`func (o *ShopReceiptTransactionsResultsInner) UnsetShippingUpgrade()`

UnsetShippingUpgrade ensures that no value is present for ShippingUpgrade, not even an explicit nil
### GetExpectedShipDate

`func (o *ShopReceiptTransactionsResultsInner) GetExpectedShipDate() int32`

GetExpectedShipDate returns the ExpectedShipDate field if non-nil, zero value otherwise.

### GetExpectedShipDateOk

`func (o *ShopReceiptTransactionsResultsInner) GetExpectedShipDateOk() (*int32, bool)`

GetExpectedShipDateOk returns a tuple with the ExpectedShipDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpectedShipDate

`func (o *ShopReceiptTransactionsResultsInner) SetExpectedShipDate(v int32)`

SetExpectedShipDate sets ExpectedShipDate field to given value.

### HasExpectedShipDate

`func (o *ShopReceiptTransactionsResultsInner) HasExpectedShipDate() bool`

HasExpectedShipDate returns a boolean if a field has been set.

### SetExpectedShipDateNil

`func (o *ShopReceiptTransactionsResultsInner) SetExpectedShipDateNil(b bool)`

 SetExpectedShipDateNil sets the value for ExpectedShipDate to be an explicit nil

### UnsetExpectedShipDate
`func (o *ShopReceiptTransactionsResultsInner) UnsetExpectedShipDate()`

UnsetExpectedShipDate ensures that no value is present for ExpectedShipDate, not even an explicit nil
### GetBuyerCoupon

`func (o *ShopReceiptTransactionsResultsInner) GetBuyerCoupon() float32`

GetBuyerCoupon returns the BuyerCoupon field if non-nil, zero value otherwise.

### GetBuyerCouponOk

`func (o *ShopReceiptTransactionsResultsInner) GetBuyerCouponOk() (*float32, bool)`

GetBuyerCouponOk returns a tuple with the BuyerCoupon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerCoupon

`func (o *ShopReceiptTransactionsResultsInner) SetBuyerCoupon(v float32)`

SetBuyerCoupon sets BuyerCoupon field to given value.

### HasBuyerCoupon

`func (o *ShopReceiptTransactionsResultsInner) HasBuyerCoupon() bool`

HasBuyerCoupon returns a boolean if a field has been set.

### GetShopCoupon

`func (o *ShopReceiptTransactionsResultsInner) GetShopCoupon() float32`

GetShopCoupon returns the ShopCoupon field if non-nil, zero value otherwise.

### GetShopCouponOk

`func (o *ShopReceiptTransactionsResultsInner) GetShopCouponOk() (*float32, bool)`

GetShopCouponOk returns a tuple with the ShopCoupon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopCoupon

`func (o *ShopReceiptTransactionsResultsInner) SetShopCoupon(v float32)`

SetShopCoupon sets ShopCoupon field to given value.

### HasShopCoupon

`func (o *ShopReceiptTransactionsResultsInner) HasShopCoupon() bool`

HasShopCoupon returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


