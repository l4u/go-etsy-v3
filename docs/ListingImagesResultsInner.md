# ListingImagesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListingId** | Pointer to **int32** | The numeric ID for the [listing](/documentation/reference#tag/ShopListing) associated to this transaction. | [optional] 
**ListingImageId** | Pointer to **int32** | The numeric ID of the primary [listing image](/documentation/reference#tag/ShopListing-Image) for this transaction. | [optional] 
**HexCode** | Pointer to **NullableString** | The webhex string for the image&#39;s average color, in webhex notation. | [optional] 
**Red** | Pointer to **NullableInt32** | The numeric red value equal to the image&#39;s average red value, from 0-255 (RGB color). | [optional] 
**Green** | Pointer to **NullableInt32** | The numeric red value equal to the image&#39;s average red value, from 0-255 (RGB color). | [optional] 
**Blue** | Pointer to **NullableInt32** | The numeric red value equal to the image&#39;s average red value, from 0-255 (RGB color). | [optional] 
**Hue** | Pointer to **NullableInt32** | The numeric hue equal to the image&#39;s average hue, from 0-360 (HSV color). | [optional] 
**Saturation** | Pointer to **NullableInt32** | The numeric saturation equal to the image&#39;s average saturation, from 0-100 (HSV color). | [optional] 
**Brightness** | Pointer to **NullableInt32** | The numeric brightness equal to the image&#39;s average brightness, from 0-100 (HSV color). | [optional] 
**IsBlackAndWhite** | Pointer to **NullableBool** | When true, the image is in black &amp; white. | [optional] 
**CreationTsz** | Pointer to **int32** | The listing image\\&#39;s creation time, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The listing image\\&#39;s creation time, in epoch seconds. | [optional] 
**Rank** | Pointer to **int32** | The positive non-zero numeric position in the images displayed in a listing, with rank 1 images appearing in the left-most position in a listing. | [optional] 
**Url75x75** | Pointer to **string** | The url string for a 75x75 pixel thumbnail of the image. | [optional] 
**Url170x135** | Pointer to **string** | The url string for a 170x135 pixel thumbnail of the image. | [optional] 
**Url570xN** | Pointer to **string** | The url string for a thumbnail of the image, no more than 570 pixels wide with variable height. | [optional] 
**UrlFullxfull** | Pointer to **string** | The url string for the full-size image, up to 3000 pixels in each dimension. | [optional] 
**FullHeight** | Pointer to **NullableInt32** | The numeric height, measured in pixels, of the full-sized image referenced in url_fullxfull. | [optional] 
**FullWidth** | Pointer to **NullableInt32** | The numeric width, measured in pixels, of the full-sized image referenced in url_fullxfull. | [optional] 
**AltText** | Pointer to **NullableString** | Alt text for the listing image. | [optional] 

## Methods

### NewListingImagesResultsInner

`func NewListingImagesResultsInner() *ListingImagesResultsInner`

NewListingImagesResultsInner instantiates a new ListingImagesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListingImagesResultsInnerWithDefaults

`func NewListingImagesResultsInnerWithDefaults() *ListingImagesResultsInner`

NewListingImagesResultsInnerWithDefaults instantiates a new ListingImagesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListingId

`func (o *ListingImagesResultsInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ListingImagesResultsInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ListingImagesResultsInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ListingImagesResultsInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### GetListingImageId

`func (o *ListingImagesResultsInner) GetListingImageId() int32`

GetListingImageId returns the ListingImageId field if non-nil, zero value otherwise.

### GetListingImageIdOk

`func (o *ListingImagesResultsInner) GetListingImageIdOk() (*int32, bool)`

GetListingImageIdOk returns a tuple with the ListingImageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingImageId

`func (o *ListingImagesResultsInner) SetListingImageId(v int32)`

SetListingImageId sets ListingImageId field to given value.

### HasListingImageId

`func (o *ListingImagesResultsInner) HasListingImageId() bool`

HasListingImageId returns a boolean if a field has been set.

### GetHexCode

`func (o *ListingImagesResultsInner) GetHexCode() string`

GetHexCode returns the HexCode field if non-nil, zero value otherwise.

### GetHexCodeOk

`func (o *ListingImagesResultsInner) GetHexCodeOk() (*string, bool)`

GetHexCodeOk returns a tuple with the HexCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHexCode

`func (o *ListingImagesResultsInner) SetHexCode(v string)`

SetHexCode sets HexCode field to given value.

### HasHexCode

`func (o *ListingImagesResultsInner) HasHexCode() bool`

HasHexCode returns a boolean if a field has been set.

### SetHexCodeNil

`func (o *ListingImagesResultsInner) SetHexCodeNil(b bool)`

 SetHexCodeNil sets the value for HexCode to be an explicit nil

### UnsetHexCode
`func (o *ListingImagesResultsInner) UnsetHexCode()`

UnsetHexCode ensures that no value is present for HexCode, not even an explicit nil
### GetRed

`func (o *ListingImagesResultsInner) GetRed() int32`

GetRed returns the Red field if non-nil, zero value otherwise.

### GetRedOk

`func (o *ListingImagesResultsInner) GetRedOk() (*int32, bool)`

GetRedOk returns a tuple with the Red field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRed

`func (o *ListingImagesResultsInner) SetRed(v int32)`

SetRed sets Red field to given value.

### HasRed

`func (o *ListingImagesResultsInner) HasRed() bool`

HasRed returns a boolean if a field has been set.

### SetRedNil

`func (o *ListingImagesResultsInner) SetRedNil(b bool)`

 SetRedNil sets the value for Red to be an explicit nil

### UnsetRed
`func (o *ListingImagesResultsInner) UnsetRed()`

UnsetRed ensures that no value is present for Red, not even an explicit nil
### GetGreen

`func (o *ListingImagesResultsInner) GetGreen() int32`

GetGreen returns the Green field if non-nil, zero value otherwise.

### GetGreenOk

`func (o *ListingImagesResultsInner) GetGreenOk() (*int32, bool)`

GetGreenOk returns a tuple with the Green field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGreen

`func (o *ListingImagesResultsInner) SetGreen(v int32)`

SetGreen sets Green field to given value.

### HasGreen

`func (o *ListingImagesResultsInner) HasGreen() bool`

HasGreen returns a boolean if a field has been set.

### SetGreenNil

`func (o *ListingImagesResultsInner) SetGreenNil(b bool)`

 SetGreenNil sets the value for Green to be an explicit nil

### UnsetGreen
`func (o *ListingImagesResultsInner) UnsetGreen()`

UnsetGreen ensures that no value is present for Green, not even an explicit nil
### GetBlue

`func (o *ListingImagesResultsInner) GetBlue() int32`

GetBlue returns the Blue field if non-nil, zero value otherwise.

### GetBlueOk

`func (o *ListingImagesResultsInner) GetBlueOk() (*int32, bool)`

GetBlueOk returns a tuple with the Blue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlue

`func (o *ListingImagesResultsInner) SetBlue(v int32)`

SetBlue sets Blue field to given value.

### HasBlue

`func (o *ListingImagesResultsInner) HasBlue() bool`

HasBlue returns a boolean if a field has been set.

### SetBlueNil

`func (o *ListingImagesResultsInner) SetBlueNil(b bool)`

 SetBlueNil sets the value for Blue to be an explicit nil

### UnsetBlue
`func (o *ListingImagesResultsInner) UnsetBlue()`

UnsetBlue ensures that no value is present for Blue, not even an explicit nil
### GetHue

`func (o *ListingImagesResultsInner) GetHue() int32`

GetHue returns the Hue field if non-nil, zero value otherwise.

### GetHueOk

`func (o *ListingImagesResultsInner) GetHueOk() (*int32, bool)`

GetHueOk returns a tuple with the Hue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHue

`func (o *ListingImagesResultsInner) SetHue(v int32)`

SetHue sets Hue field to given value.

### HasHue

`func (o *ListingImagesResultsInner) HasHue() bool`

HasHue returns a boolean if a field has been set.

### SetHueNil

`func (o *ListingImagesResultsInner) SetHueNil(b bool)`

 SetHueNil sets the value for Hue to be an explicit nil

### UnsetHue
`func (o *ListingImagesResultsInner) UnsetHue()`

UnsetHue ensures that no value is present for Hue, not even an explicit nil
### GetSaturation

`func (o *ListingImagesResultsInner) GetSaturation() int32`

GetSaturation returns the Saturation field if non-nil, zero value otherwise.

### GetSaturationOk

`func (o *ListingImagesResultsInner) GetSaturationOk() (*int32, bool)`

GetSaturationOk returns a tuple with the Saturation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSaturation

`func (o *ListingImagesResultsInner) SetSaturation(v int32)`

SetSaturation sets Saturation field to given value.

### HasSaturation

`func (o *ListingImagesResultsInner) HasSaturation() bool`

HasSaturation returns a boolean if a field has been set.

### SetSaturationNil

`func (o *ListingImagesResultsInner) SetSaturationNil(b bool)`

 SetSaturationNil sets the value for Saturation to be an explicit nil

### UnsetSaturation
`func (o *ListingImagesResultsInner) UnsetSaturation()`

UnsetSaturation ensures that no value is present for Saturation, not even an explicit nil
### GetBrightness

`func (o *ListingImagesResultsInner) GetBrightness() int32`

GetBrightness returns the Brightness field if non-nil, zero value otherwise.

### GetBrightnessOk

`func (o *ListingImagesResultsInner) GetBrightnessOk() (*int32, bool)`

GetBrightnessOk returns a tuple with the Brightness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrightness

`func (o *ListingImagesResultsInner) SetBrightness(v int32)`

SetBrightness sets Brightness field to given value.

### HasBrightness

`func (o *ListingImagesResultsInner) HasBrightness() bool`

HasBrightness returns a boolean if a field has been set.

### SetBrightnessNil

`func (o *ListingImagesResultsInner) SetBrightnessNil(b bool)`

 SetBrightnessNil sets the value for Brightness to be an explicit nil

### UnsetBrightness
`func (o *ListingImagesResultsInner) UnsetBrightness()`

UnsetBrightness ensures that no value is present for Brightness, not even an explicit nil
### GetIsBlackAndWhite

`func (o *ListingImagesResultsInner) GetIsBlackAndWhite() bool`

GetIsBlackAndWhite returns the IsBlackAndWhite field if non-nil, zero value otherwise.

### GetIsBlackAndWhiteOk

`func (o *ListingImagesResultsInner) GetIsBlackAndWhiteOk() (*bool, bool)`

GetIsBlackAndWhiteOk returns a tuple with the IsBlackAndWhite field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsBlackAndWhite

`func (o *ListingImagesResultsInner) SetIsBlackAndWhite(v bool)`

SetIsBlackAndWhite sets IsBlackAndWhite field to given value.

### HasIsBlackAndWhite

`func (o *ListingImagesResultsInner) HasIsBlackAndWhite() bool`

HasIsBlackAndWhite returns a boolean if a field has been set.

### SetIsBlackAndWhiteNil

`func (o *ListingImagesResultsInner) SetIsBlackAndWhiteNil(b bool)`

 SetIsBlackAndWhiteNil sets the value for IsBlackAndWhite to be an explicit nil

### UnsetIsBlackAndWhite
`func (o *ListingImagesResultsInner) UnsetIsBlackAndWhite()`

UnsetIsBlackAndWhite ensures that no value is present for IsBlackAndWhite, not even an explicit nil
### GetCreationTsz

`func (o *ListingImagesResultsInner) GetCreationTsz() int32`

GetCreationTsz returns the CreationTsz field if non-nil, zero value otherwise.

### GetCreationTszOk

`func (o *ListingImagesResultsInner) GetCreationTszOk() (*int32, bool)`

GetCreationTszOk returns a tuple with the CreationTsz field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreationTsz

`func (o *ListingImagesResultsInner) SetCreationTsz(v int32)`

SetCreationTsz sets CreationTsz field to given value.

### HasCreationTsz

`func (o *ListingImagesResultsInner) HasCreationTsz() bool`

HasCreationTsz returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ListingImagesResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ListingImagesResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ListingImagesResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ListingImagesResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetRank

`func (o *ListingImagesResultsInner) GetRank() int32`

GetRank returns the Rank field if non-nil, zero value otherwise.

### GetRankOk

`func (o *ListingImagesResultsInner) GetRankOk() (*int32, bool)`

GetRankOk returns a tuple with the Rank field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRank

`func (o *ListingImagesResultsInner) SetRank(v int32)`

SetRank sets Rank field to given value.

### HasRank

`func (o *ListingImagesResultsInner) HasRank() bool`

HasRank returns a boolean if a field has been set.

### GetUrl75x75

`func (o *ListingImagesResultsInner) GetUrl75x75() string`

GetUrl75x75 returns the Url75x75 field if non-nil, zero value otherwise.

### GetUrl75x75Ok

`func (o *ListingImagesResultsInner) GetUrl75x75Ok() (*string, bool)`

GetUrl75x75Ok returns a tuple with the Url75x75 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl75x75

`func (o *ListingImagesResultsInner) SetUrl75x75(v string)`

SetUrl75x75 sets Url75x75 field to given value.

### HasUrl75x75

`func (o *ListingImagesResultsInner) HasUrl75x75() bool`

HasUrl75x75 returns a boolean if a field has been set.

### GetUrl170x135

`func (o *ListingImagesResultsInner) GetUrl170x135() string`

GetUrl170x135 returns the Url170x135 field if non-nil, zero value otherwise.

### GetUrl170x135Ok

`func (o *ListingImagesResultsInner) GetUrl170x135Ok() (*string, bool)`

GetUrl170x135Ok returns a tuple with the Url170x135 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl170x135

`func (o *ListingImagesResultsInner) SetUrl170x135(v string)`

SetUrl170x135 sets Url170x135 field to given value.

### HasUrl170x135

`func (o *ListingImagesResultsInner) HasUrl170x135() bool`

HasUrl170x135 returns a boolean if a field has been set.

### GetUrl570xN

`func (o *ListingImagesResultsInner) GetUrl570xN() string`

GetUrl570xN returns the Url570xN field if non-nil, zero value otherwise.

### GetUrl570xNOk

`func (o *ListingImagesResultsInner) GetUrl570xNOk() (*string, bool)`

GetUrl570xNOk returns a tuple with the Url570xN field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl570xN

`func (o *ListingImagesResultsInner) SetUrl570xN(v string)`

SetUrl570xN sets Url570xN field to given value.

### HasUrl570xN

`func (o *ListingImagesResultsInner) HasUrl570xN() bool`

HasUrl570xN returns a boolean if a field has been set.

### GetUrlFullxfull

`func (o *ListingImagesResultsInner) GetUrlFullxfull() string`

GetUrlFullxfull returns the UrlFullxfull field if non-nil, zero value otherwise.

### GetUrlFullxfullOk

`func (o *ListingImagesResultsInner) GetUrlFullxfullOk() (*string, bool)`

GetUrlFullxfullOk returns a tuple with the UrlFullxfull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrlFullxfull

`func (o *ListingImagesResultsInner) SetUrlFullxfull(v string)`

SetUrlFullxfull sets UrlFullxfull field to given value.

### HasUrlFullxfull

`func (o *ListingImagesResultsInner) HasUrlFullxfull() bool`

HasUrlFullxfull returns a boolean if a field has been set.

### GetFullHeight

`func (o *ListingImagesResultsInner) GetFullHeight() int32`

GetFullHeight returns the FullHeight field if non-nil, zero value otherwise.

### GetFullHeightOk

`func (o *ListingImagesResultsInner) GetFullHeightOk() (*int32, bool)`

GetFullHeightOk returns a tuple with the FullHeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullHeight

`func (o *ListingImagesResultsInner) SetFullHeight(v int32)`

SetFullHeight sets FullHeight field to given value.

### HasFullHeight

`func (o *ListingImagesResultsInner) HasFullHeight() bool`

HasFullHeight returns a boolean if a field has been set.

### SetFullHeightNil

`func (o *ListingImagesResultsInner) SetFullHeightNil(b bool)`

 SetFullHeightNil sets the value for FullHeight to be an explicit nil

### UnsetFullHeight
`func (o *ListingImagesResultsInner) UnsetFullHeight()`

UnsetFullHeight ensures that no value is present for FullHeight, not even an explicit nil
### GetFullWidth

`func (o *ListingImagesResultsInner) GetFullWidth() int32`

GetFullWidth returns the FullWidth field if non-nil, zero value otherwise.

### GetFullWidthOk

`func (o *ListingImagesResultsInner) GetFullWidthOk() (*int32, bool)`

GetFullWidthOk returns a tuple with the FullWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullWidth

`func (o *ListingImagesResultsInner) SetFullWidth(v int32)`

SetFullWidth sets FullWidth field to given value.

### HasFullWidth

`func (o *ListingImagesResultsInner) HasFullWidth() bool`

HasFullWidth returns a boolean if a field has been set.

### SetFullWidthNil

`func (o *ListingImagesResultsInner) SetFullWidthNil(b bool)`

 SetFullWidthNil sets the value for FullWidth to be an explicit nil

### UnsetFullWidth
`func (o *ListingImagesResultsInner) UnsetFullWidth()`

UnsetFullWidth ensures that no value is present for FullWidth, not even an explicit nil
### GetAltText

`func (o *ListingImagesResultsInner) GetAltText() string`

GetAltText returns the AltText field if non-nil, zero value otherwise.

### GetAltTextOk

`func (o *ListingImagesResultsInner) GetAltTextOk() (*string, bool)`

GetAltTextOk returns a tuple with the AltText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAltText

`func (o *ListingImagesResultsInner) SetAltText(v string)`

SetAltText sets AltText field to given value.

### HasAltText

`func (o *ListingImagesResultsInner) HasAltText() bool`

HasAltText returns a boolean if a field has been set.

### SetAltTextNil

`func (o *ListingImagesResultsInner) SetAltTextNil(b bool)`

 SetAltTextNil sets the value for AltText to be an explicit nil

### UnsetAltText
`func (o *ListingImagesResultsInner) UnsetAltText()`

UnsetAltText ensures that no value is present for AltText, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


