# ShopListingWithAssociationsImagesInner

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

### NewShopListingWithAssociationsImagesInner

`func NewShopListingWithAssociationsImagesInner() *ShopListingWithAssociationsImagesInner`

NewShopListingWithAssociationsImagesInner instantiates a new ShopListingWithAssociationsImagesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopListingWithAssociationsImagesInnerWithDefaults

`func NewShopListingWithAssociationsImagesInnerWithDefaults() *ShopListingWithAssociationsImagesInner`

NewShopListingWithAssociationsImagesInnerWithDefaults instantiates a new ShopListingWithAssociationsImagesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListingId

`func (o *ShopListingWithAssociationsImagesInner) GetListingId() int32`

GetListingId returns the ListingId field if non-nil, zero value otherwise.

### GetListingIdOk

`func (o *ShopListingWithAssociationsImagesInner) GetListingIdOk() (*int32, bool)`

GetListingIdOk returns a tuple with the ListingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingId

`func (o *ShopListingWithAssociationsImagesInner) SetListingId(v int32)`

SetListingId sets ListingId field to given value.

### HasListingId

`func (o *ShopListingWithAssociationsImagesInner) HasListingId() bool`

HasListingId returns a boolean if a field has been set.

### GetListingImageId

`func (o *ShopListingWithAssociationsImagesInner) GetListingImageId() int32`

GetListingImageId returns the ListingImageId field if non-nil, zero value otherwise.

### GetListingImageIdOk

`func (o *ShopListingWithAssociationsImagesInner) GetListingImageIdOk() (*int32, bool)`

GetListingImageIdOk returns a tuple with the ListingImageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListingImageId

`func (o *ShopListingWithAssociationsImagesInner) SetListingImageId(v int32)`

SetListingImageId sets ListingImageId field to given value.

### HasListingImageId

`func (o *ShopListingWithAssociationsImagesInner) HasListingImageId() bool`

HasListingImageId returns a boolean if a field has been set.

### GetHexCode

`func (o *ShopListingWithAssociationsImagesInner) GetHexCode() string`

GetHexCode returns the HexCode field if non-nil, zero value otherwise.

### GetHexCodeOk

`func (o *ShopListingWithAssociationsImagesInner) GetHexCodeOk() (*string, bool)`

GetHexCodeOk returns a tuple with the HexCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHexCode

`func (o *ShopListingWithAssociationsImagesInner) SetHexCode(v string)`

SetHexCode sets HexCode field to given value.

### HasHexCode

`func (o *ShopListingWithAssociationsImagesInner) HasHexCode() bool`

HasHexCode returns a boolean if a field has been set.

### SetHexCodeNil

`func (o *ShopListingWithAssociationsImagesInner) SetHexCodeNil(b bool)`

 SetHexCodeNil sets the value for HexCode to be an explicit nil

### UnsetHexCode
`func (o *ShopListingWithAssociationsImagesInner) UnsetHexCode()`

UnsetHexCode ensures that no value is present for HexCode, not even an explicit nil
### GetRed

`func (o *ShopListingWithAssociationsImagesInner) GetRed() int32`

GetRed returns the Red field if non-nil, zero value otherwise.

### GetRedOk

`func (o *ShopListingWithAssociationsImagesInner) GetRedOk() (*int32, bool)`

GetRedOk returns a tuple with the Red field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRed

`func (o *ShopListingWithAssociationsImagesInner) SetRed(v int32)`

SetRed sets Red field to given value.

### HasRed

`func (o *ShopListingWithAssociationsImagesInner) HasRed() bool`

HasRed returns a boolean if a field has been set.

### SetRedNil

`func (o *ShopListingWithAssociationsImagesInner) SetRedNil(b bool)`

 SetRedNil sets the value for Red to be an explicit nil

### UnsetRed
`func (o *ShopListingWithAssociationsImagesInner) UnsetRed()`

UnsetRed ensures that no value is present for Red, not even an explicit nil
### GetGreen

`func (o *ShopListingWithAssociationsImagesInner) GetGreen() int32`

GetGreen returns the Green field if non-nil, zero value otherwise.

### GetGreenOk

`func (o *ShopListingWithAssociationsImagesInner) GetGreenOk() (*int32, bool)`

GetGreenOk returns a tuple with the Green field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGreen

`func (o *ShopListingWithAssociationsImagesInner) SetGreen(v int32)`

SetGreen sets Green field to given value.

### HasGreen

`func (o *ShopListingWithAssociationsImagesInner) HasGreen() bool`

HasGreen returns a boolean if a field has been set.

### SetGreenNil

`func (o *ShopListingWithAssociationsImagesInner) SetGreenNil(b bool)`

 SetGreenNil sets the value for Green to be an explicit nil

### UnsetGreen
`func (o *ShopListingWithAssociationsImagesInner) UnsetGreen()`

UnsetGreen ensures that no value is present for Green, not even an explicit nil
### GetBlue

`func (o *ShopListingWithAssociationsImagesInner) GetBlue() int32`

GetBlue returns the Blue field if non-nil, zero value otherwise.

### GetBlueOk

`func (o *ShopListingWithAssociationsImagesInner) GetBlueOk() (*int32, bool)`

GetBlueOk returns a tuple with the Blue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlue

`func (o *ShopListingWithAssociationsImagesInner) SetBlue(v int32)`

SetBlue sets Blue field to given value.

### HasBlue

`func (o *ShopListingWithAssociationsImagesInner) HasBlue() bool`

HasBlue returns a boolean if a field has been set.

### SetBlueNil

`func (o *ShopListingWithAssociationsImagesInner) SetBlueNil(b bool)`

 SetBlueNil sets the value for Blue to be an explicit nil

### UnsetBlue
`func (o *ShopListingWithAssociationsImagesInner) UnsetBlue()`

UnsetBlue ensures that no value is present for Blue, not even an explicit nil
### GetHue

`func (o *ShopListingWithAssociationsImagesInner) GetHue() int32`

GetHue returns the Hue field if non-nil, zero value otherwise.

### GetHueOk

`func (o *ShopListingWithAssociationsImagesInner) GetHueOk() (*int32, bool)`

GetHueOk returns a tuple with the Hue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHue

`func (o *ShopListingWithAssociationsImagesInner) SetHue(v int32)`

SetHue sets Hue field to given value.

### HasHue

`func (o *ShopListingWithAssociationsImagesInner) HasHue() bool`

HasHue returns a boolean if a field has been set.

### SetHueNil

`func (o *ShopListingWithAssociationsImagesInner) SetHueNil(b bool)`

 SetHueNil sets the value for Hue to be an explicit nil

### UnsetHue
`func (o *ShopListingWithAssociationsImagesInner) UnsetHue()`

UnsetHue ensures that no value is present for Hue, not even an explicit nil
### GetSaturation

`func (o *ShopListingWithAssociationsImagesInner) GetSaturation() int32`

GetSaturation returns the Saturation field if non-nil, zero value otherwise.

### GetSaturationOk

`func (o *ShopListingWithAssociationsImagesInner) GetSaturationOk() (*int32, bool)`

GetSaturationOk returns a tuple with the Saturation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSaturation

`func (o *ShopListingWithAssociationsImagesInner) SetSaturation(v int32)`

SetSaturation sets Saturation field to given value.

### HasSaturation

`func (o *ShopListingWithAssociationsImagesInner) HasSaturation() bool`

HasSaturation returns a boolean if a field has been set.

### SetSaturationNil

`func (o *ShopListingWithAssociationsImagesInner) SetSaturationNil(b bool)`

 SetSaturationNil sets the value for Saturation to be an explicit nil

### UnsetSaturation
`func (o *ShopListingWithAssociationsImagesInner) UnsetSaturation()`

UnsetSaturation ensures that no value is present for Saturation, not even an explicit nil
### GetBrightness

`func (o *ShopListingWithAssociationsImagesInner) GetBrightness() int32`

GetBrightness returns the Brightness field if non-nil, zero value otherwise.

### GetBrightnessOk

`func (o *ShopListingWithAssociationsImagesInner) GetBrightnessOk() (*int32, bool)`

GetBrightnessOk returns a tuple with the Brightness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrightness

`func (o *ShopListingWithAssociationsImagesInner) SetBrightness(v int32)`

SetBrightness sets Brightness field to given value.

### HasBrightness

`func (o *ShopListingWithAssociationsImagesInner) HasBrightness() bool`

HasBrightness returns a boolean if a field has been set.

### SetBrightnessNil

`func (o *ShopListingWithAssociationsImagesInner) SetBrightnessNil(b bool)`

 SetBrightnessNil sets the value for Brightness to be an explicit nil

### UnsetBrightness
`func (o *ShopListingWithAssociationsImagesInner) UnsetBrightness()`

UnsetBrightness ensures that no value is present for Brightness, not even an explicit nil
### GetIsBlackAndWhite

`func (o *ShopListingWithAssociationsImagesInner) GetIsBlackAndWhite() bool`

GetIsBlackAndWhite returns the IsBlackAndWhite field if non-nil, zero value otherwise.

### GetIsBlackAndWhiteOk

`func (o *ShopListingWithAssociationsImagesInner) GetIsBlackAndWhiteOk() (*bool, bool)`

GetIsBlackAndWhiteOk returns a tuple with the IsBlackAndWhite field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsBlackAndWhite

`func (o *ShopListingWithAssociationsImagesInner) SetIsBlackAndWhite(v bool)`

SetIsBlackAndWhite sets IsBlackAndWhite field to given value.

### HasIsBlackAndWhite

`func (o *ShopListingWithAssociationsImagesInner) HasIsBlackAndWhite() bool`

HasIsBlackAndWhite returns a boolean if a field has been set.

### SetIsBlackAndWhiteNil

`func (o *ShopListingWithAssociationsImagesInner) SetIsBlackAndWhiteNil(b bool)`

 SetIsBlackAndWhiteNil sets the value for IsBlackAndWhite to be an explicit nil

### UnsetIsBlackAndWhite
`func (o *ShopListingWithAssociationsImagesInner) UnsetIsBlackAndWhite()`

UnsetIsBlackAndWhite ensures that no value is present for IsBlackAndWhite, not even an explicit nil
### GetCreationTsz

`func (o *ShopListingWithAssociationsImagesInner) GetCreationTsz() int32`

GetCreationTsz returns the CreationTsz field if non-nil, zero value otherwise.

### GetCreationTszOk

`func (o *ShopListingWithAssociationsImagesInner) GetCreationTszOk() (*int32, bool)`

GetCreationTszOk returns a tuple with the CreationTsz field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreationTsz

`func (o *ShopListingWithAssociationsImagesInner) SetCreationTsz(v int32)`

SetCreationTsz sets CreationTsz field to given value.

### HasCreationTsz

`func (o *ShopListingWithAssociationsImagesInner) HasCreationTsz() bool`

HasCreationTsz returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopListingWithAssociationsImagesInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopListingWithAssociationsImagesInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopListingWithAssociationsImagesInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopListingWithAssociationsImagesInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetRank

`func (o *ShopListingWithAssociationsImagesInner) GetRank() int32`

GetRank returns the Rank field if non-nil, zero value otherwise.

### GetRankOk

`func (o *ShopListingWithAssociationsImagesInner) GetRankOk() (*int32, bool)`

GetRankOk returns a tuple with the Rank field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRank

`func (o *ShopListingWithAssociationsImagesInner) SetRank(v int32)`

SetRank sets Rank field to given value.

### HasRank

`func (o *ShopListingWithAssociationsImagesInner) HasRank() bool`

HasRank returns a boolean if a field has been set.

### GetUrl75x75

`func (o *ShopListingWithAssociationsImagesInner) GetUrl75x75() string`

GetUrl75x75 returns the Url75x75 field if non-nil, zero value otherwise.

### GetUrl75x75Ok

`func (o *ShopListingWithAssociationsImagesInner) GetUrl75x75Ok() (*string, bool)`

GetUrl75x75Ok returns a tuple with the Url75x75 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl75x75

`func (o *ShopListingWithAssociationsImagesInner) SetUrl75x75(v string)`

SetUrl75x75 sets Url75x75 field to given value.

### HasUrl75x75

`func (o *ShopListingWithAssociationsImagesInner) HasUrl75x75() bool`

HasUrl75x75 returns a boolean if a field has been set.

### GetUrl170x135

`func (o *ShopListingWithAssociationsImagesInner) GetUrl170x135() string`

GetUrl170x135 returns the Url170x135 field if non-nil, zero value otherwise.

### GetUrl170x135Ok

`func (o *ShopListingWithAssociationsImagesInner) GetUrl170x135Ok() (*string, bool)`

GetUrl170x135Ok returns a tuple with the Url170x135 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl170x135

`func (o *ShopListingWithAssociationsImagesInner) SetUrl170x135(v string)`

SetUrl170x135 sets Url170x135 field to given value.

### HasUrl170x135

`func (o *ShopListingWithAssociationsImagesInner) HasUrl170x135() bool`

HasUrl170x135 returns a boolean if a field has been set.

### GetUrl570xN

`func (o *ShopListingWithAssociationsImagesInner) GetUrl570xN() string`

GetUrl570xN returns the Url570xN field if non-nil, zero value otherwise.

### GetUrl570xNOk

`func (o *ShopListingWithAssociationsImagesInner) GetUrl570xNOk() (*string, bool)`

GetUrl570xNOk returns a tuple with the Url570xN field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl570xN

`func (o *ShopListingWithAssociationsImagesInner) SetUrl570xN(v string)`

SetUrl570xN sets Url570xN field to given value.

### HasUrl570xN

`func (o *ShopListingWithAssociationsImagesInner) HasUrl570xN() bool`

HasUrl570xN returns a boolean if a field has been set.

### GetUrlFullxfull

`func (o *ShopListingWithAssociationsImagesInner) GetUrlFullxfull() string`

GetUrlFullxfull returns the UrlFullxfull field if non-nil, zero value otherwise.

### GetUrlFullxfullOk

`func (o *ShopListingWithAssociationsImagesInner) GetUrlFullxfullOk() (*string, bool)`

GetUrlFullxfullOk returns a tuple with the UrlFullxfull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrlFullxfull

`func (o *ShopListingWithAssociationsImagesInner) SetUrlFullxfull(v string)`

SetUrlFullxfull sets UrlFullxfull field to given value.

### HasUrlFullxfull

`func (o *ShopListingWithAssociationsImagesInner) HasUrlFullxfull() bool`

HasUrlFullxfull returns a boolean if a field has been set.

### GetFullHeight

`func (o *ShopListingWithAssociationsImagesInner) GetFullHeight() int32`

GetFullHeight returns the FullHeight field if non-nil, zero value otherwise.

### GetFullHeightOk

`func (o *ShopListingWithAssociationsImagesInner) GetFullHeightOk() (*int32, bool)`

GetFullHeightOk returns a tuple with the FullHeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullHeight

`func (o *ShopListingWithAssociationsImagesInner) SetFullHeight(v int32)`

SetFullHeight sets FullHeight field to given value.

### HasFullHeight

`func (o *ShopListingWithAssociationsImagesInner) HasFullHeight() bool`

HasFullHeight returns a boolean if a field has been set.

### SetFullHeightNil

`func (o *ShopListingWithAssociationsImagesInner) SetFullHeightNil(b bool)`

 SetFullHeightNil sets the value for FullHeight to be an explicit nil

### UnsetFullHeight
`func (o *ShopListingWithAssociationsImagesInner) UnsetFullHeight()`

UnsetFullHeight ensures that no value is present for FullHeight, not even an explicit nil
### GetFullWidth

`func (o *ShopListingWithAssociationsImagesInner) GetFullWidth() int32`

GetFullWidth returns the FullWidth field if non-nil, zero value otherwise.

### GetFullWidthOk

`func (o *ShopListingWithAssociationsImagesInner) GetFullWidthOk() (*int32, bool)`

GetFullWidthOk returns a tuple with the FullWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullWidth

`func (o *ShopListingWithAssociationsImagesInner) SetFullWidth(v int32)`

SetFullWidth sets FullWidth field to given value.

### HasFullWidth

`func (o *ShopListingWithAssociationsImagesInner) HasFullWidth() bool`

HasFullWidth returns a boolean if a field has been set.

### SetFullWidthNil

`func (o *ShopListingWithAssociationsImagesInner) SetFullWidthNil(b bool)`

 SetFullWidthNil sets the value for FullWidth to be an explicit nil

### UnsetFullWidth
`func (o *ShopListingWithAssociationsImagesInner) UnsetFullWidth()`

UnsetFullWidth ensures that no value is present for FullWidth, not even an explicit nil
### GetAltText

`func (o *ShopListingWithAssociationsImagesInner) GetAltText() string`

GetAltText returns the AltText field if non-nil, zero value otherwise.

### GetAltTextOk

`func (o *ShopListingWithAssociationsImagesInner) GetAltTextOk() (*string, bool)`

GetAltTextOk returns a tuple with the AltText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAltText

`func (o *ShopListingWithAssociationsImagesInner) SetAltText(v string)`

SetAltText sets AltText field to given value.

### HasAltText

`func (o *ShopListingWithAssociationsImagesInner) HasAltText() bool`

HasAltText returns a boolean if a field has been set.

### SetAltTextNil

`func (o *ShopListingWithAssociationsImagesInner) SetAltTextNil(b bool)`

 SetAltTextNil sets the value for AltText to be an explicit nil

### UnsetAltText
`func (o *ShopListingWithAssociationsImagesInner) UnsetAltText()`

UnsetAltText ensures that no value is present for AltText, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


