# ListingReviewsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShopId** | Pointer to **int32** | The shop&#39;s numeric ID. | [optional] 
**ListingId** | Pointer to **int32** | The ID of the ShopListing that the TransactionReview belongs to. | [optional] 
**Rating** | Pointer to **int32** | Rating value on scale from 1 to 5 | [optional] 
**Review** | Pointer to **NullableString** | A message left by the author, explaining the feedback, if provided. | [optional] 
**Language** | Pointer to **string** | The language of the TransactionReview | [optional] 
**ImageUrlFullxfull** | Pointer to **NullableString** | The url to a photo provided with the feedback, dimensions fullxfull. Note: This field may be absent, depending on the buyer&#39;s privacy settings. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The date and time the TransactionReview was created in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The date and time the TransactionReview was created in epoch seconds. | [optional] 
**UpdateTimestamp** | Pointer to **int32** | The date and time the TransactionReview was updated in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The date and time the TransactionReview was updated in epoch seconds. | [optional] 

## Methods

### NewListingReviewsResultsInner

`func NewListingReviewsResultsInner() *ListingReviewsResultsInner`

NewListingReviewsResultsInner instantiates a new ListingReviewsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListingReviewsResultsInnerWithDefaults

`func NewListingReviewsResultsInnerWithDefaults() *ListingReviewsResultsInner`

NewListingReviewsResultsInnerWithDefaults instantiates a new ListingReviewsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetShopId

`func (o *ListingReviewsResultsInner) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *ListingReviewsResultsInner) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *ListingReviewsResultsInner) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *ListingReviewsResultsInner) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetListingId

`func (o *ListingReviewsResultsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ListingReviewsResultsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ListingReviewsResultsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ListingReviewsResultsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### GetRating

`func (o *ListingReviewsResultsInner) GetRating() int32`

GetRating returns the Rating field if non-nil, zero value otherwise.

### GetRatingOk

`func (o *ListingReviewsResultsInner) GetRatingOk() (*int32, bool)`

GetRatingOk returns a tuple with the Rating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRating

`func (o *ListingReviewsResultsInner) SetRating(v int32)`

SetRating sets Rating field to given value.

### HasRating

`func (o *ListingReviewsResultsInner) HasRating() bool`

HasRating returns a boolean if a field has been set.

### GetReview

`func (o *ListingReviewsResultsInner) GetReview() string`

GetReview returns the Review field if non-nil, zero value otherwise.

### GetReviewOk

`func (o *ListingReviewsResultsInner) GetReviewOk() (*string, bool)`

GetReviewOk returns a tuple with the Review field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReview

`func (o *ListingReviewsResultsInner) SetReview(v string)`

SetReview sets Review field to given value.

### HasReview

`func (o *ListingReviewsResultsInner) HasReview() bool`

HasReview returns a boolean if a field has been set.

### SetReviewNil

`func (o *ListingReviewsResultsInner) SetReviewNil(b bool)`

 SetReviewNil sets the value for Review to be an explicit nil

### UnsetReview
`func (o *ListingReviewsResultsInner) UnsetReview()`

UnsetReview ensures that no value is present for Review, not even an explicit nil
### GetLanguage

`func (o *ListingReviewsResultsInner) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *ListingReviewsResultsInner) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *ListingReviewsResultsInner) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *ListingReviewsResultsInner) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### GetImageUrlFullxfull

`func (o *ListingReviewsResultsInner) GetImageUrlFullxfull() string`

GetImageUrlFullxfull returns the ImageUrlFullxfull field if non-nil, zero value otherwise.

### GetImageUrlFullxfullOk

`func (o *ListingReviewsResultsInner) GetImageUrlFullxfullOk() (*string, bool)`

GetImageUrlFullxfullOk returns a tuple with the ImageUrlFullxfull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrlFullxfull

`func (o *ListingReviewsResultsInner) SetImageUrlFullxfull(v string)`

SetImageUrlFullxfull sets ImageUrlFullxfull field to given value.

### HasImageUrlFullxfull

`func (o *ListingReviewsResultsInner) HasImageUrlFullxfull() bool`

HasImageUrlFullxfull returns a boolean if a field has been set.

### SetImageUrlFullxfullNil

`func (o *ListingReviewsResultsInner) SetImageUrlFullxfullNil(b bool)`

 SetImageUrlFullxfullNil sets the value for ImageUrlFullxfull to be an explicit nil

### UnsetImageUrlFullxfull
`func (o *ListingReviewsResultsInner) UnsetImageUrlFullxfull()`

UnsetImageUrlFullxfull ensures that no value is present for ImageUrlFullxfull, not even an explicit nil
### GetCreateTimestamp

`func (o *ListingReviewsResultsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *ListingReviewsResultsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *ListingReviewsResultsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *ListingReviewsResultsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ListingReviewsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ListingReviewsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ListingReviewsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ListingReviewsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdateTimestamp

`func (o *ListingReviewsResultsInner) GetUpdateTimestamp() int32`

GetUpdateTimestamp returns the UpdateTimestamp field if non-nil, zero value otherwise.

### GetUpdateTimestampOk

`func (o *ListingReviewsResultsInner) GetUpdateTimestampOk() (*int32, bool)`

GetUpdateTimestampOk returns a tuple with the UpdateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateTimestamp

`func (o *ListingReviewsResultsInner) SetUpdateTimestamp(v int32)`

SetUpdateTimestamp sets UpdateTimestamp field to given value.

### HasUpdateTimestamp

`func (o *ListingReviewsResultsInner) HasUpdateTimestamp() bool`

HasUpdateTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *ListingReviewsResultsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *ListingReviewsResultsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *ListingReviewsResultsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *ListingReviewsResultsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


