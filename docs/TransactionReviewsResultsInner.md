# TransactionReviewsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShopId** | Pointer to **int32** | The shop&#39;s numeric ID. | [optional] 
**ListingId** | Pointer to **int32** | The ID of the ShopListing that the TransactionReview belongs to. | [optional] 
**TransactionId** | Pointer to **int32** | The ID of the ShopReceipt Transaction that the TransactionReview belongs to. | [optional] 
**BuyerUserId** | Pointer to **NullableInt32** | The numeric ID of the user who was the buyer in this transaction. Note: This field may be absent, depending on the buyer&#39;s privacy settings. | [optional] 
**Rating** | Pointer to **int32** | Rating value on scale from 1 to 5 | [optional] 
**Review** | Pointer to **string** | A message left by the author, explaining the feedback, if provided. | [optional] [default to ""]
**Language** | Pointer to **string** | The language of the TransactionReview | [optional] 
**ImageUrlFullxfull** | Pointer to **NullableString** | The url to a photo provided with the feedback, dimensions fullxfull. Note: This field may be absent, depending on the buyer&#39;s privacy settings. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The date and time the TransactionReview was created in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The date and time the TransactionReview was created in epoch seconds. | [optional] 
**UpdateTimestamp** | Pointer to **int32** | The date and time the TransactionReview was updated in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The date and time the TransactionReview was updated in epoch seconds. | [optional] 

## Methods

### NewTransactionReviewsResultsInner

`func NewTransactionReviewsResultsInner() *TransactionReviewsResultsInner`

NewTransactionReviewsResultsInner instantiates a new TransactionReviewsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTransactionReviewsResultsInnerWithDefaults

`func NewTransactionReviewsResultsInnerWithDefaults() *TransactionReviewsResultsInner`

NewTransactionReviewsResultsInnerWithDefaults instantiates a new TransactionReviewsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShopId

`func (o *TransactionReviewsResultsInner) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *TransactionReviewsResultsInner) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *TransactionReviewsResultsInner) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *TransactionReviewsResultsInner) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetListingId

`func (o *TransactionReviewsResultsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *TransactionReviewsResultsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *TransactionReviewsResultsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *TransactionReviewsResultsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### GetTransactionId

`func (o *TransactionReviewsResultsInner) GetTransactionId() int32`

GetTransactionId returns the TransactionId field if non-nil, zero value otherwise.

### GetTransactionIdOk

`func (o *TransactionReviewsResultsInner) GetTransactionIdOk() (*int32, bool)`

GetTransactionIdOk returns a tuple with the TransactionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionId

`func (o *TransactionReviewsResultsInner) SetTransactionId(v int32)`

SetTransactionId sets TransactionId field to given value.

### HasTransactionId

`func (o *TransactionReviewsResultsInner) HasTransactionId() bool`

HasTransactionId returns a boolean if a field has been set.

### GetBuyerUserId

`func (o *TransactionReviewsResultsInner) GetBuyerUserId() int32`

GetBuyerUserId returns the BuyerUserId field if non-nil, zero value otherwise.

### GetBuyerUserIdOk

`func (o *TransactionReviewsResultsInner) GetBuyerUserIdOk() (*int32, bool)`

GetBuyerUserIdOk returns a tuple with the BuyerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerUserId

`func (o *TransactionReviewsResultsInner) SetBuyerUserId(v int32)`

SetBuyerUserId sets BuyerUserId field to given value.

### HasBuyerUserId

`func (o *TransactionReviewsResultsInner) HasBuyerUserId() bool`

HasBuyerUserId returns a boolean if a field has been set.

### SetBuyerUserIdNil

`func (o *TransactionReviewsResultsInner) SetBuyerUserIdNil(b bool)`

 SetBuyerUserIdNil sets the value for BuyerUserId to be an explicit nil

### UnsetBuyerUserId
`func (o *TransactionReviewsResultsInner) UnsetBuyerUserId()`

UnsetBuyerUserId ensures that no value is present for BuyerUserId, not even an explicit nil
### GetRating

`func (o *TransactionReviewsResultsInner) GetRating() int32`

GetRating returns the Rating field if non-nil, zero value otherwise.

### GetRatingOk

`func (o *TransactionReviewsResultsInner) GetRatingOk() (*int32, bool)`

GetRatingOk returns a tuple with the Rating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRating

`func (o *TransactionReviewsResultsInner) SetRating(v int32)`

SetRating sets Rating field to given value.

### HasRating

`func (o *TransactionReviewsResultsInner) HasRating() bool`

HasRating returns a boolean if a field has been set.

### GetReview

`func (o *TransactionReviewsResultsInner) GetReview() string`

GetReview returns the Review field if non-nil, zero value otherwise.

### GetReviewOk

`func (o *TransactionReviewsResultsInner) GetReviewOk() (*string, bool)`

GetReviewOk returns a tuple with the Review field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReview

`func (o *TransactionReviewsResultsInner) SetReview(v string)`

SetReview sets Review field to given value.

### HasReview

`func (o *TransactionReviewsResultsInner) HasReview() bool`

HasReview returns a boolean if a field has been set.

### GetLanguage

`func (o *TransactionReviewsResultsInner) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *TransactionReviewsResultsInner) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *TransactionReviewsResultsInner) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *TransactionReviewsResultsInner) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### GetImageUrlFullxfull

`func (o *TransactionReviewsResultsInner) GetImageUrlFullxfull() string`

GetImageUrlFullxfull returns the ImageUrlFullxfull field if non-nil, zero value otherwise.

### GetImageUrlFullxfullOk

`func (o *TransactionReviewsResultsInner) GetImageUrlFullxfullOk() (*string, bool)`

GetImageUrlFullxfullOk returns a tuple with the ImageUrlFullxfull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrlFullxfull

`func (o *TransactionReviewsResultsInner) SetImageUrlFullxfull(v string)`

SetImageUrlFullxfull sets ImageUrlFullxfull field to given value.

### HasImageUrlFullxfull

`func (o *TransactionReviewsResultsInner) HasImageUrlFullxfull() bool`

HasImageUrlFullxfull returns a boolean if a field has been set.

### SetImageUrlFullxfullNil

`func (o *TransactionReviewsResultsInner) SetImageUrlFullxfullNil(b bool)`

 SetImageUrlFullxfullNil sets the value for ImageUrlFullxfull to be an explicit nil

### UnsetImageUrlFullxfull
`func (o *TransactionReviewsResultsInner) UnsetImageUrlFullxfull()`

UnsetImageUrlFullxfull ensures that no value is present for ImageUrlFullxfull, not even an explicit nil
### GetCreateTimestamp

`func (o *TransactionReviewsResultsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *TransactionReviewsResultsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *TransactionReviewsResultsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *TransactionReviewsResultsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *TransactionReviewsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *TransactionReviewsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *TransactionReviewsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *TransactionReviewsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdateTimestamp

`func (o *TransactionReviewsResultsInner) GetUpdateTimestamp() int32`

GetUpdateTimestamp returns the UpdateTimestamp field if non-nil, zero value otherwise.

### GetUpdateTimestampOk

`func (o *TransactionReviewsResultsInner) GetUpdateTimestampOk() (*int32, bool)`

GetUpdateTimestampOk returns a tuple with the UpdateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateTimestamp

`func (o *TransactionReviewsResultsInner) SetUpdateTimestamp(v int32)`

SetUpdateTimestamp sets UpdateTimestamp field to given value.

### HasUpdateTimestamp

`func (o *TransactionReviewsResultsInner) HasUpdateTimestamp() bool`

HasUpdateTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *TransactionReviewsResultsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *TransactionReviewsResultsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *TransactionReviewsResultsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *TransactionReviewsResultsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


