# ShopListingFilesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListingFileId** | Pointer to **int32** | The unique numeric ID of a file associated with a digital listing. | [optional] 
**ListingId** | Pointer to **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | [optional] 
**Rank** | Pointer to **int32** | The numeric index of the display order position of this file in the listing, starting at 1. | [optional] 
**Filename** | Pointer to **string** | The file name string for a file associated with a digital listing. | [optional] 
**Filesize** | Pointer to **string** | A human-readable format size string for the size of a file. | [optional] 
**SizeBytes** | Pointer to **int32** | A number indicating the size of a file, measured in bytes. | [optional] 
**Filetype** | Pointer to **string** | A type string indicating a file&#39;s MIME type. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The unique numeric ID of a file associated with a digital listing. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The unique numeric ID of a file associated with a digital listing. | [optional] 

## Methods

### NewShopListingFilesResultsInner

`func NewShopListingFilesResultsInner() *ShopListingFilesResultsInner`

NewShopListingFilesResultsInner instantiates a new ShopListingFilesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingFilesResultsInnerWithDefaults

`func NewShopListingFilesResultsInnerWithDefaults() *ShopListingFilesResultsInner`

NewShopListingFilesResultsInnerWithDefaults instantiates a new ShopListingFilesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListingFileId

`func (o *ShopListingFilesResultsInner) GetListingFileId() int32`

GetListingFileId returns the ListingFileId field if non-nil, zero value otherwise.

### GetListingFileIdOk

`func (o *ShopListingFilesResultsInner) GetListingFileIdOk() (*int32, bool)`

GetListingFileIdOk returns a tuple with the ListingFileId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingFileId

`func (o *ShopListingFilesResultsInner) SetListingFileId(v int32)`

SetListingFileId sets ListingFileId field to given value.

### HasListingFileId

`func (o *ShopListingFilesResultsInner) HasListingFileId() bool`

HasListingFileId returns a boolean if a field has been set.

### GetListingId

`func (o *ShopListingFilesResultsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ShopListingFilesResultsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ShopListingFilesResultsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ShopListingFilesResultsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### GetRank

`func (o *ShopListingFilesResultsInner) GetRank() int32`

GetRank returns the Rank field if non-nil, zero value otherwise.

### GetRankOk

`func (o *ShopListingFilesResultsInner) GetRankOk() (*int32, bool)`

GetRankOk returns a tuple with the Rank field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRank

`func (o *ShopListingFilesResultsInner) SetRank(v int32)`

SetRank sets Rank field to given value.

### HasRank

`func (o *ShopListingFilesResultsInner) HasRank() bool`

HasRank returns a boolean if a field has been set.

### GetFilename

`func (o *ShopListingFilesResultsInner) GetFilename() string`

GetFilename returns the Filename field if non-nil, zero value otherwise.

### GetFilenameOk

`func (o *ShopListingFilesResultsInner) GetFilenameOk() (*string, bool)`

GetFilenameOk returns a tuple with the Filename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilename

`func (o *ShopListingFilesResultsInner) SetFilename(v string)`

SetFilename sets Filename field to given value.

### HasFilename

`func (o *ShopListingFilesResultsInner) HasFilename() bool`

HasFilename returns a boolean if a field has been set.

### GetFilesize

`func (o *ShopListingFilesResultsInner) GetFilesize() string`

GetFilesize returns the Filesize field if non-nil, zero value otherwise.

### GetFilesizeOk

`func (o *ShopListingFilesResultsInner) GetFilesizeOk() (*string, bool)`

GetFilesizeOk returns a tuple with the Filesize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilesize

`func (o *ShopListingFilesResultsInner) SetFilesize(v string)`

SetFilesize sets Filesize field to given value.

### HasFilesize

`func (o *ShopListingFilesResultsInner) HasFilesize() bool`

HasFilesize returns a boolean if a field has been set.

### GetSizeBytes

`func (o *ShopListingFilesResultsInner) GetSizeBytes() int32`

GetSizeBytes returns the SizeBytes field if non-nil, zero value otherwise.

### GetSizeBytesOk

`func (o *ShopListingFilesResultsInner) GetSizeBytesOk() (*int32, bool)`

GetSizeBytesOk returns a tuple with the SizeBytes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeBytes

`func (o *ShopListingFilesResultsInner) SetSizeBytes(v int32)`

SetSizeBytes sets SizeBytes field to given value.

### HasSizeBytes

`func (o *ShopListingFilesResultsInner) HasSizeBytes() bool`

HasSizeBytes returns a boolean if a field has been set.

### GetFiletype

`func (o *ShopListingFilesResultsInner) GetFiletype() string`

GetFiletype returns the Filetype field if non-nil, zero value otherwise.

### GetFiletypeOk

`func (o *ShopListingFilesResultsInner) GetFiletypeOk() (*string, bool)`

GetFiletypeOk returns a tuple with the Filetype field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiletype

`func (o *ShopListingFilesResultsInner) SetFiletype(v string)`

SetFiletype sets Filetype field to given value.

### HasFiletype

`func (o *ShopListingFilesResultsInner) HasFiletype() bool`

HasFiletype returns a boolean if a field has been set.

### GetCreateTimestamp

`func (o *ShopListingFilesResultsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *ShopListingFilesResultsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *ShopListingFilesResultsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *ShopListingFilesResultsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopListingFilesResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopListingFilesResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopListingFilesResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopListingFilesResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


