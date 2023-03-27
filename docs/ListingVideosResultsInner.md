# ListingVideosResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VideoId** | Pointer to **int32** | The unique ID of a video associated with a listing. | [optional] 
**Height** | Pointer to **int32** | The video height dimension in pixels. | [optional] 
**Width** | Pointer to **int32** | The video width dimension in pixels. | [optional] 
**ThumbnailUrl** | Pointer to **string** | The url of the video thumbnail. | [optional] 
**VideoUrl** | Pointer to **string** | The url of the video file. | [optional] 
**VideoState** | Pointer to **string** | The current state of a given video. Value is one of &#x60;active&#x60;, &#x60;inactive&#x60;, &#x60;deleted&#x60; or &#x60;flagged&#x60;. | [optional] 

## Methods

### NewListingVideosResultsInner

`func NewListingVideosResultsInner() *ListingVideosResultsInner`

NewListingVideosResultsInner instantiates a new ListingVideosResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListingVideosResultsInnerWithDefaults

`func NewListingVideosResultsInnerWithDefaults() *ListingVideosResultsInner`

NewListingVideosResultsInnerWithDefaults instantiates a new ListingVideosResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVideoId

`func (o *ListingVideosResultsInner) GetVideoId() int32`

GetVideoId returns the VideoId field if non-nil, zero value otherwise.

### GetVideoIdOk

`func (o *ListingVideosResultsInner) GetVideoIdOk() (*int32, bool)`

GetVideoIdOk returns a tuple with the VideoId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVideoId

`func (o *ListingVideosResultsInner) SetVideoId(v int32)`

SetVideoId sets VideoId field to given value.

### HasVideoId

`func (o *ListingVideosResultsInner) HasVideoId() bool`

HasVideoId returns a boolean if a field has been set.

### GetHeight

`func (o *ListingVideosResultsInner) GetHeight() int32`

GetHeight returns the Height field if non-nil, zero value otherwise.

### GetHeightOk

`func (o *ListingVideosResultsInner) GetHeightOk() (*int32, bool)`

GetHeightOk returns a tuple with the Height field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeight

`func (o *ListingVideosResultsInner) SetHeight(v int32)`

SetHeight sets Height field to given value.

### HasHeight

`func (o *ListingVideosResultsInner) HasHeight() bool`

HasHeight returns a boolean if a field has been set.

### GetWidth

`func (o *ListingVideosResultsInner) GetWidth() int32`

GetWidth returns the Width field if non-nil, zero value otherwise.

### GetWidthOk

`func (o *ListingVideosResultsInner) GetWidthOk() (*int32, bool)`

GetWidthOk returns a tuple with the Width field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidth

`func (o *ListingVideosResultsInner) SetWidth(v int32)`

SetWidth sets Width field to given value.

### HasWidth

`func (o *ListingVideosResultsInner) HasWidth() bool`

HasWidth returns a boolean if a field has been set.

### GetThumbnailUrl

`func (o *ListingVideosResultsInner) GetThumbnailUrl() string`

GetThumbnailUrl returns the ThumbnailUrl field if non-nil, zero value otherwise.

### GetThumbnailUrlOk

`func (o *ListingVideosResultsInner) GetThumbnailUrlOk() (*string, bool)`

GetThumbnailUrlOk returns a tuple with the ThumbnailUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThumbnailUrl

`func (o *ListingVideosResultsInner) SetThumbnailUrl(v string)`

SetThumbnailUrl sets ThumbnailUrl field to given value.

### HasThumbnailUrl

`func (o *ListingVideosResultsInner) HasThumbnailUrl() bool`

HasThumbnailUrl returns a boolean if a field has been set.

### GetVideoUrl

`func (o *ListingVideosResultsInner) GetVideoUrl() string`

GetVideoUrl returns the VideoUrl field if non-nil, zero value otherwise.

### GetVideoUrlOk

`func (o *ListingVideosResultsInner) GetVideoUrlOk() (*string, bool)`

GetVideoUrlOk returns a tuple with the VideoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVideoUrl

`func (o *ListingVideosResultsInner) SetVideoUrl(v string)`

SetVideoUrl sets VideoUrl field to given value.

### HasVideoUrl

`func (o *ListingVideosResultsInner) HasVideoUrl() bool`

HasVideoUrl returns a boolean if a field has been set.

### GetVideoState

`func (o *ListingVideosResultsInner) GetVideoState() string`

GetVideoState returns the VideoState field if non-nil, zero value otherwise.

### GetVideoStateOk

`func (o *ListingVideosResultsInner) GetVideoStateOk() (*string, bool)`

GetVideoStateOk returns a tuple with the VideoState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVideoState

`func (o *ListingVideosResultsInner) SetVideoState(v string)`

SetVideoState sets VideoState field to given value.

### HasVideoState

`func (o *ListingVideosResultsInner) HasVideoState() bool`

HasVideoState returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


