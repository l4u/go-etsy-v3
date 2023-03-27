# ShopReceiptTransactionsInner

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

### NewShopReceiptTransactionsInner

`func NewShopReceiptTransactionsInner() *ShopReceiptTransactionsInner`

NewShopReceiptTransactionsInner instantiates a new ShopReceiptTransactionsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReceiptTransactionsInnerWithDefaults

`func NewShopReceiptTransactionsInnerWithDefaults() *ShopReceiptTransactionsInner`

NewShopReceiptTransactionsInnerWithDefaults instantiates a new ShopReceiptTransactionsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTransactionId

`func (o *ShopReceiptTransactionsInner) GetTransactionId() int32`

GetTransactionId returns the TransactionId field if non-nil, zero value otherwise.

### GetTransactionIdOk

`func (o *ShopReceiptTransactionsInner) GetTransactionIdOk() (*int32, bool)`

GetTransactionIdOk returns a tuple with the TransactionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionId

`func (o *ShopReceiptTransactionsInner) SetTransactionId(v int32)`

SetTransactionId sets TransactionId field to given value.

### HasTransactionId

`func (o *ShopReceiptTransactionsInner) HasTransactionId() bool`

HasTransactionId returns a boolean if a field has been set.

### GetTitle

`func (o *ShopReceiptTransactionsInner) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ShopReceiptTransactionsInner) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ShopReceiptTransactionsInner) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ShopReceiptTransactionsInner) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *ShopReceiptTransactionsInner) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *ShopReceiptTransactionsInner) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetDescription

`func (o *ShopReceiptTransactionsInner) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ShopReceiptTransactionsInner) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ShopReceiptTransactionsInner) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ShopReceiptTransactionsInner) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *ShopReceiptTransactionsInner) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *ShopReceiptTransactionsInner) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetSellerUserId

`func (o *ShopReceiptTransactionsInner) GetSellerUserId() int32`

GetSellerUserId returns the SellerUserId field if non-nil, zero value otherwise.

### GetSellerUserIdOk

`func (o *ShopReceiptTransactionsInner) GetSellerUserIdOk() (*int32, bool)`

GetSellerUserIdOk returns a tuple with the SellerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerUserId

`func (o *ShopReceiptTransactionsInner) SetSellerUserId(v int32)`

SetSellerUserId sets SellerUserId field to given value.

### HasSellerUserId

`func (o *ShopReceiptTransactionsInner) HasSellerUserId() bool`

HasSellerUserId returns a boolean if a field has been set.

### GetBuyerUserId

`func (o *ShopReceiptTransactionsInner) GetBuyerUserId() int32`

GetBuyerUserId returns the BuyerUserId field if non-nil, zero value otherwise.

### GetBuyerUserIdOk

`func (o *ShopReceiptTransactionsInner) GetBuyerUserIdOk() (*int32, bool)`

GetBuyerUserIdOk returns a tuple with the BuyerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerUserId

`func (o *ShopReceiptTransactionsInner) SetBuyerUserId(v int32)`

SetBuyerUserId sets BuyerUserId field to given value.

### HasBuyerUserId

`func (o *ShopReceiptTransactionsInner) HasBuyerUserId() bool`

HasBuyerUserId returns a boolean if a field has been set.

### GetCreateTimestamp

`func (o *ShopReceiptTransactionsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *ShopReceiptTransactionsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *ShopReceiptTransactionsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *ShopReceiptTransactionsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopReceiptTransactionsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopReceiptTransactionsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopReceiptTransactionsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopReceiptTransactionsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetPaidTimestamp

`func (o *ShopReceiptTransactionsInner) GetPaidTimestamp() int32`

GetPaidTimestamp returns the PaidTimestamp field if non-nil, zero value otherwise.

### GetPaidTimestampOk

`func (o *ShopReceiptTransactionsInner) GetPaidTimestampOk() (*int32, bool)`

GetPaidTimestampOk returns a tuple with the PaidTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaidTimestamp

`func (o *ShopReceiptTransactionsInner) SetPaidTimestamp(v int32)`

SetPaidTimestamp sets PaidTimestamp field to given value.

### HasPaidTimestamp

`func (o *ShopReceiptTransactionsInner) HasPaidTimestamp() bool`

HasPaidTimestamp returns a boolean if a field has been set.

### SetPaidTimestampNil

`func (o *ShopReceiptTransactionsInner) SetPaidTimestampNil(b bool)`

 SetPaidTimestampNil sets the value for PaidTimestamp to be an explicit nil

### UnsetPaidTimestamp
`func (o *ShopReceiptTransactionsInner) UnsetPaidTimestamp()`

UnsetPaidTimestamp ensures that no value is present for PaidTimestamp, not even an explicit nil
### GetShippedTimestamp

`func (o *ShopReceiptTransactionsInner) GetShippedTimestamp() int32`

GetShippedTimestamp returns the ShippedTimestamp field if non-nil, zero value otherwise.

### GetShippedTimestampOk

`func (o *ShopReceiptTransactionsInner) GetShippedTimestampOk() (*int32, bool)`

GetShippedTimestampOk returns a tuple with the ShippedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippedTimestamp

`func (o *ShopReceiptTransactionsInner) SetShippedTimestamp(v int32)`

SetShippedTimestamp sets ShippedTimestamp field to given value.

### HasShippedTimestamp

`func (o *ShopReceiptTransactionsInner) HasShippedTimestamp() bool`

HasShippedTimestamp returns a boolean if a field has been set.

### SetShippedTimestampNil

`func (o *ShopReceiptTransactionsInner) SetShippedTimestampNil(b bool)`

 SetShippedTimestampNil sets the value for ShippedTimestamp to be an explicit nil

### UnsetShippedTimestamp
`func (o *ShopReceiptTransactionsInner) UnsetShippedTimestamp()`

UnsetShippedTimestamp ensures that no value is present for ShippedTimestamp, not even an explicit nil
### GetQuantity

`func (o *ShopReceiptTransactionsInner) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *ShopReceiptTransactionsInner) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *ShopReceiptTransactionsInner) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.

### HasQuantity

`func (o *ShopReceiptTransactionsInner) HasQuantity() bool`

HasQuantity returns a boolean if a field has been set.

### GetListingImageId

`func (o *ShopReceiptTransactionsInner) GetListingImageId() int32`

GetListingImageId returns the ListingImageId field if non-nil, zero value otherwise.

### GetListingImageIdOk

`func (o *ShopReceiptTransactionsInner) GetListingImageIdOk() (*int32, bool)`

GetListingImageIdOk returns a tuple with the ListingImageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingImageId

`func (o *ShopReceiptTransactionsInner) SetListingImageId(v int32)`

SetListingImageId sets ListingImageId field to given value.

### HasListingImageId

`func (o *ShopReceiptTransactionsInner) HasListingImageId() bool`

HasListingImageId returns a boolean if a field has been set.

### SetListingImageIdNil

`func (o *ShopReceiptTransactionsInner) SetListingImageIdNil(b bool)`

 SetListingImageIdNil sets the value for ListingImageId to be an explicit nil

### UnsetListingImageId
`func (o *ShopReceiptTransactionsInner) UnsetListingImageId()`

UnsetListingImageId ensures that no value is present for ListingImageId, not even an explicit nil
### GetReceiptId

`func (o *ShopReceiptTransactionsInner) GetReceiptId() int32`

GetReceiptId returns the ReceiptId field if non-nil, zero value otherwise.

### GetReceiptIdOk

`func (o *ShopReceiptTransactionsInner) GetReceiptIdOk() (*int32, bool)`

GetReceiptIdOk returns a tuple with the ReceiptId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptId

`func (o *ShopReceiptTransactionsInner) SetReceiptId(v int32)`

SetReceiptId sets ReceiptId field to given value.

### HasReceiptId

`func (o *ShopReceiptTransactionsInner) HasReceiptId() bool`

HasReceiptId returns a boolean if a field has been set.

### GetIsDigital

`func (o *ShopReceiptTransactionsInner) GetIsDigital() bool`

GetIsDigital returns the IsDigital field if non-nil, zero value otherwise.

### GetIsDigitalOk

`func (o *ShopReceiptTransactionsInner) GetIsDigitalOk() (*bool, bool)`

GetIsDigitalOk returns a tuple with the IsDigital field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDigital

`func (o *ShopReceiptTransactionsInner) SetIsDigital(v bool)`

SetIsDigital sets IsDigital field to given value.

### HasIsDigital

`func (o *ShopReceiptTransactionsInner) HasIsDigital() bool`

HasIsDigital returns a boolean if a field has been set.

### GetFileData

`func (o *ShopReceiptTransactionsInner) GetFileData() string`

GetFileData returns the FileData field if non-nil, zero value otherwise.

### GetFileDataOk

`func (o *ShopReceiptTransactionsInner) GetFileDataOk() (*string, bool)`

GetFileDataOk returns a tuple with the FileData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileData

`func (o *ShopReceiptTransactionsInner) SetFileData(v string)`

SetFileData sets FileData field to given value.

### HasFileData

`func (o *ShopReceiptTransactionsInner) HasFileData() bool`

HasFileData returns a boolean if a field has been set.

### GetListingId

`func (o *ShopReceiptTransactionsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ShopReceiptTransactionsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ShopReceiptTransactionsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ShopReceiptTransactionsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### SetListingIdNil

`func (o *ShopReceiptTransactionsInner) SetListingIdNil(b bool)`

 SetListingIdNil sets the value for ListingId to be an explicit nil

### UnsetListingId
`func (o *ShopReceiptTransactionsInner) UnsetListingId()`

UnsetListingId ensures that no value is present for ListingId, not even an explicit nil
### GetTransactionType

`func (o *ShopReceiptTransactionsInner) GetTransactionType() string`

GetTransactionType returns the TransactionType field if non-nil, zero value otherwise.

### GetTransactionTypeOk

`func (o *ShopReceiptTransactionsInner) GetTransactionTypeOk() (*string, bool)`

GetTransactionTypeOk returns a tuple with the TransactionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionType

`func (o *ShopReceiptTransactionsInner) SetTransactionType(v string)`

SetTransactionType sets TransactionType field to given value.

### HasTransactionType

`func (o *ShopReceiptTransactionsInner) HasTransactionType() bool`

HasTransactionType returns a boolean if a field has been set.

### GetProductId

`func (o *ShopReceiptTransactionsInner) GetProductId() int32`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *ShopReceiptTransactionsInner) GetProductIdOk() (*int32, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *ShopReceiptTransactionsInner) SetProductId(v int32)`

SetProductId sets ProductId field to given value.

### HasProductId

`func (o *ShopReceiptTransactionsInner) HasProductId() bool`

HasProductId returns a boolean if a field has been set.

### SetProductIdNil

`func (o *ShopReceiptTransactionsInner) SetProductIdNil(b bool)`

 SetProductIdNil sets the value for ProductId to be an explicit nil

### UnsetProductId
`func (o *ShopReceiptTransactionsInner) UnsetProductId()`

UnsetProductId ensures that no value is present for ProductId, not even an explicit nil
### GetSku

`func (o *ShopReceiptTransactionsInner) GetSku() string`

GetSku returns the Sku field if non-nil, zero value otherwise.

### GetSkuOk

`func (o *ShopReceiptTransactionsInner) GetSkuOk() (*string, bool)`

GetSkuOk returns a tuple with the Sku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSku

`func (o *ShopReceiptTransactionsInner) SetSku(v string)`

SetSku sets Sku field to given value.

### HasSku

`func (o *ShopReceiptTransactionsInner) HasSku() bool`

HasSku returns a boolean if a field has been set.

### SetSkuNil

`func (o *ShopReceiptTransactionsInner) SetSkuNil(b bool)`

 SetSkuNil sets the value for Sku to be an explicit nil

### UnsetSku
`func (o *ShopReceiptTransactionsInner) UnsetSku()`

UnsetSku ensures that no value is present for Sku, not even an explicit nil
### GetPrice

`func (o *ShopReceiptTransactionsInner) GetPrice() ShopReceiptTransactionPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ShopReceiptTransactionsInner) GetPriceOk() (*ShopReceiptTransactionPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ShopReceiptTransactionsInner) SetPrice(v ShopReceiptTransactionPrice)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ShopReceiptTransactionsInner) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetShippingCost

`func (o *ShopReceiptTransactionsInner) GetShippingCost() ShopReceiptTransactionShippingCost`

GetShippingCost returns the ShippingCost field if non-nil, zero value otherwise.

### GetShippingCostOk

`func (o *ShopReceiptTransactionsInner) GetShippingCostOk() (*ShopReceiptTransactionShippingCost, bool)`

GetShippingCostOk returns a tuple with the ShippingCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingCost

`func (o *ShopReceiptTransactionsInner) SetShippingCost(v ShopReceiptTransactionShippingCost)`

SetShippingCost sets ShippingCost field to given value.

### HasShippingCost

`func (o *ShopReceiptTransactionsInner) HasShippingCost() bool`

HasShippingCost returns a boolean if a field has been set.

### GetVariations

`func (o *ShopReceiptTransactionsInner) GetVariations() []ShopReceiptTransactionVariationsInner`

GetVariations returns the Variations field if non-nil, zero value otherwise.

### GetVariationsOk

`func (o *ShopReceiptTransactionsInner) GetVariationsOk() (*[]ShopReceiptTransactionVariationsInner, bool)`

GetVariationsOk returns a tuple with the Variations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariations

`func (o *ShopReceiptTransactionsInner) SetVariations(v []ShopReceiptTransactionVariationsInner)`

SetVariations sets Variations field to given value.

### HasVariations

`func (o *ShopReceiptTransactionsInner) HasVariations() bool`

HasVariations returns a boolean if a field has been set.

### GetProductData

`func (o *ShopReceiptTransactionsInner) GetProductData() []ListingInventoryProductPropertyValuesInner`

GetProductData returns the ProductData field if non-nil, zero value otherwise.

### GetProductDataOk

`func (o *ShopReceiptTransactionsInner) GetProductDataOk() (*[]ListingInventoryProductPropertyValuesInner, bool)`

GetProductDataOk returns a tuple with the ProductData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductData

`func (o *ShopReceiptTransactionsInner) SetProductData(v []ListingInventoryProductPropertyValuesInner)`

SetProductData sets ProductData field to given value.

### HasProductData

`func (o *ShopReceiptTransactionsInner) HasProductData() bool`

HasProductData returns a boolean if a field has been set.

### GetShippingProfileId

`func (o *ShopReceiptTransactionsInner) GetShippingProfileId() int32`

GetShippingProfileId returns the ShippingProfileId field if non-nil, zero value otherwise.

### GetShippingProfileIdOk

`func (o *ShopReceiptTransactionsInner) GetShippingProfileIdOk() (*int32, bool)`

GetShippingProfileIdOk returns a tuple with the ShippingProfileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingProfileId

`func (o *ShopReceiptTransactionsInner) SetShippingProfileId(v int32)`

SetShippingProfileId sets ShippingProfileId field to given value.

### HasShippingProfileId

`func (o *ShopReceiptTransactionsInner) HasShippingProfileId() bool`

HasShippingProfileId returns a boolean if a field has been set.

### SetShippingProfileIdNil

`func (o *ShopReceiptTransactionsInner) SetShippingProfileIdNil(b bool)`

 SetShippingProfileIdNil sets the value for ShippingProfileId to be an explicit nil

### UnsetShippingProfileId
`func (o *ShopReceiptTransactionsInner) UnsetShippingProfileId()`

UnsetShippingProfileId ensures that no value is present for ShippingProfileId, not even an explicit nil
### GetMinProcessingDays

`func (o *ShopReceiptTransactionsInner) GetMinProcessingDays() int32`

GetMinProcessingDays returns the MinProcessingDays field if non-nil, zero value otherwise.

### GetMinProcessingDaysOk

`func (o *ShopReceiptTransactionsInner) GetMinProcessingDaysOk() (*int32, bool)`

GetMinProcessingDaysOk returns a tuple with the MinProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinProcessingDays

`func (o *ShopReceiptTransactionsInner) SetMinProcessingDays(v int32)`

SetMinProcessingDays sets MinProcessingDays field to given value.

### HasMinProcessingDays

`func (o *ShopReceiptTransactionsInner) HasMinProcessingDays() bool`

HasMinProcessingDays returns a boolean if a field has been set.

### SetMinProcessingDaysNil

`func (o *ShopReceiptTransactionsInner) SetMinProcessingDaysNil(b bool)`

 SetMinProcessingDaysNil sets the value for MinProcessingDays to be an explicit nil

### UnsetMinProcessingDays
`func (o *ShopReceiptTransactionsInner) UnsetMinProcessingDays()`

UnsetMinProcessingDays ensures that no value is present for MinProcessingDays, not even an explicit nil
### GetMaxProcessingDays

`func (o *ShopReceiptTransactionsInner) GetMaxProcessingDays() int32`

GetMaxProcessingDays returns the MaxProcessingDays field if non-nil, zero value otherwise.

### GetMaxProcessingDaysOk

`func (o *ShopReceiptTransactionsInner) GetMaxProcessingDaysOk() (*int32, bool)`

GetMaxProcessingDaysOk returns a tuple with the MaxProcessingDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxProcessingDays

`func (o *ShopReceiptTransactionsInner) SetMaxProcessingDays(v int32)`

SetMaxProcessingDays sets MaxProcessingDays field to given value.

### HasMaxProcessingDays

`func (o *ShopReceiptTransactionsInner) HasMaxProcessingDays() bool`

HasMaxProcessingDays returns a boolean if a field has been set.

### SetMaxProcessingDaysNil

`func (o *ShopReceiptTransactionsInner) SetMaxProcessingDaysNil(b bool)`

 SetMaxProcessingDaysNil sets the value for MaxProcessingDays to be an explicit nil

### UnsetMaxProcessingDays
`func (o *ShopReceiptTransactionsInner) UnsetMaxProcessingDays()`

UnsetMaxProcessingDays ensures that no value is present for MaxProcessingDays, not even an explicit nil
### GetShippingMethod

`func (o *ShopReceiptTransactionsInner) GetShippingMethod() string`

GetShippingMethod returns the ShippingMethod field if non-nil, zero value otherwise.

### GetShippingMethodOk

`func (o *ShopReceiptTransactionsInner) GetShippingMethodOk() (*string, bool)`

GetShippingMethodOk returns a tuple with the ShippingMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingMethod

`func (o *ShopReceiptTransactionsInner) SetShippingMethod(v string)`

SetShippingMethod sets ShippingMethod field to given value.

### HasShippingMethod

`func (o *ShopReceiptTransactionsInner) HasShippingMethod() bool`

HasShippingMethod returns a boolean if a field has been set.

### SetShippingMethodNil

`func (o *ShopReceiptTransactionsInner) SetShippingMethodNil(b bool)`

 SetShippingMethodNil sets the value for ShippingMethod to be an explicit nil

### UnsetShippingMethod
`func (o *ShopReceiptTransactionsInner) UnsetShippingMethod()`

UnsetShippingMethod ensures that no value is present for ShippingMethod, not even an explicit nil
### GetShippingUpgrade

`func (o *ShopReceiptTransactionsInner) GetShippingUpgrade() string`

GetShippingUpgrade returns the ShippingUpgrade field if non-nil, zero value otherwise.

### GetShippingUpgradeOk

`func (o *ShopReceiptTransactionsInner) GetShippingUpgradeOk() (*string, bool)`

GetShippingUpgradeOk returns a tuple with the ShippingUpgrade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingUpgrade

`func (o *ShopReceiptTransactionsInner) SetShippingUpgrade(v string)`

SetShippingUpgrade sets ShippingUpgrade field to given value.

### HasShippingUpgrade

`func (o *ShopReceiptTransactionsInner) HasShippingUpgrade() bool`

HasShippingUpgrade returns a boolean if a field has been set.

### SetShippingUpgradeNil

`func (o *ShopReceiptTransactionsInner) SetShippingUpgradeNil(b bool)`

 SetShippingUpgradeNil sets the value for ShippingUpgrade to be an explicit nil

### UnsetShippingUpgrade
`func (o *ShopReceiptTransactionsInner) UnsetShippingUpgrade()`

UnsetShippingUpgrade ensures that no value is present for ShippingUpgrade, not even an explicit nil
### GetExpectedShipDate

`func (o *ShopReceiptTransactionsInner) GetExpectedShipDate() int32`

GetExpectedShipDate returns the ExpectedShipDate field if non-nil, zero value otherwise.

### GetExpectedShipDateOk

`func (o *ShopReceiptTransactionsInner) GetExpectedShipDateOk() (*int32, bool)`

GetExpectedShipDateOk returns a tuple with the ExpectedShipDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpectedShipDate

`func (o *ShopReceiptTransactionsInner) SetExpectedShipDate(v int32)`

SetExpectedShipDate sets ExpectedShipDate field to given value.

### HasExpectedShipDate

`func (o *ShopReceiptTransactionsInner) HasExpectedShipDate() bool`

HasExpectedShipDate returns a boolean if a field has been set.

### SetExpectedShipDateNil

`func (o *ShopReceiptTransactionsInner) SetExpectedShipDateNil(b bool)`

 SetExpectedShipDateNil sets the value for ExpectedShipDate to be an explicit nil

### UnsetExpectedShipDate
`func (o *ShopReceiptTransactionsInner) UnsetExpectedShipDate()`

UnsetExpectedShipDate ensures that no value is present for ExpectedShipDate, not even an explicit nil
### GetBuyerCoupon

`func (o *ShopReceiptTransactionsInner) GetBuyerCoupon() float32`

GetBuyerCoupon returns the BuyerCoupon field if non-nil, zero value otherwise.

### GetBuyerCouponOk

`func (o *ShopReceiptTransactionsInner) GetBuyerCouponOk() (*float32, bool)`

GetBuyerCouponOk returns a tuple with the BuyerCoupon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerCoupon

`func (o *ShopReceiptTransactionsInner) SetBuyerCoupon(v float32)`

SetBuyerCoupon sets BuyerCoupon field to given value.

### HasBuyerCoupon

`func (o *ShopReceiptTransactionsInner) HasBuyerCoupon() bool`

HasBuyerCoupon returns a boolean if a field has been set.

### GetShopCoupon

`func (o *ShopReceiptTransactionsInner) GetShopCoupon() float32`

GetShopCoupon returns the ShopCoupon field if non-nil, zero value otherwise.

### GetShopCouponOk

`func (o *ShopReceiptTransactionsInner) GetShopCouponOk() (*float32, bool)`

GetShopCouponOk returns a tuple with the ShopCoupon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopCoupon

`func (o *ShopReceiptTransactionsInner) SetShopCoupon(v float32)`

SetShopCoupon sets ShopCoupon field to given value.

### HasShopCoupon

`func (o *ShopReceiptTransactionsInner) HasShopCoupon() bool`

HasShopCoupon returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


