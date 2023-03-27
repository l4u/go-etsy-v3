# UserAddressesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserAddressId** | Pointer to **int32** | The numeric ID of the user&#39;s address. | [optional] 
**UserId** | Pointer to **int32** | The user&#39;s numeric ID. | [optional] 
**Name** | Pointer to **string** | The user&#39;s name for this address. | [optional] 
**FirstLine** | Pointer to **string** | The first line of the user&#39;s address. | [optional] 
**SecondLine** | Pointer to **NullableString** | The second line of the user&#39;s address. | [optional] 
**City** | Pointer to **string** | The city field of the user&#39;s address. | [optional] 
**State** | Pointer to **NullableString** | The state field of the user&#39;s address. | [optional] 
**Zip** | Pointer to **string** | The zip code field of the user&#39;s address. | [optional] 
**IsoCountryCode** | Pointer to **NullableString** | The ISO code of the country in this address. | [optional] 
**CountryName** | Pointer to **NullableString** | The name of the user&#39;s country. | [optional] 
**IsDefaultShippingAddress** | Pointer to **bool** | Is this the user&#39;s default shipping address. | [optional] 

## Methods

### NewUserAddressesResultsInner

`func NewUserAddressesResultsInner() *UserAddressesResultsInner`

NewUserAddressesResultsInner instantiates a new UserAddressesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserAddressesResultsInnerWithDefaults

`func NewUserAddressesResultsInnerWithDefaults() *UserAddressesResultsInner`

NewUserAddressesResultsInnerWithDefaults instantiates a new UserAddressesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserAddressId

`func (o *UserAddressesResultsInner) GetUserAddressId() int32`

GetUserAddressId returns the UserAddressId field if non-nil, zero value otherwise.

### GetUserAddressIdOk

`func (o *UserAddressesResultsInner) GetUserAddressIdOk() (*int32, bool)`

GetUserAddressIdOk returns a tuple with the UserAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserAddressId

`func (o *UserAddressesResultsInner) SetUserAddressId(v int32)`

SetUserAddressId sets UserAddressId field to given value.

### HasUserAddressId

`func (o *UserAddressesResultsInner) HasUserAddressId() bool`

HasUserAddressId returns a boolean if a field has been set.

### GetUserId

`func (o *UserAddressesResultsInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *UserAddressesResultsInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *UserAddressesResultsInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *UserAddressesResultsInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetName

`func (o *UserAddressesResultsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UserAddressesResultsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UserAddressesResultsInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UserAddressesResultsInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetFirstLine

`func (o *UserAddressesResultsInner) GetFirstLine() string`

GetFirstLine returns the FirstLine field if non-nil, zero value otherwise.

### GetFirstLineOk

`func (o *UserAddressesResultsInner) GetFirstLineOk() (*string, bool)`

GetFirstLineOk returns a tuple with the FirstLine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstLine

`func (o *UserAddressesResultsInner) SetFirstLine(v string)`

SetFirstLine sets FirstLine field to given value.

### HasFirstLine

`func (o *UserAddressesResultsInner) HasFirstLine() bool`

HasFirstLine returns a boolean if a field has been set.

### GetSecondLine

`func (o *UserAddressesResultsInner) GetSecondLine() string`

GetSecondLine returns the SecondLine field if non-nil, zero value otherwise.

### GetSecondLineOk

`func (o *UserAddressesResultsInner) GetSecondLineOk() (*string, bool)`

GetSecondLineOk returns a tuple with the SecondLine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondLine

`func (o *UserAddressesResultsInner) SetSecondLine(v string)`

SetSecondLine sets SecondLine field to given value.

### HasSecondLine

`func (o *UserAddressesResultsInner) HasSecondLine() bool`

HasSecondLine returns a boolean if a field has been set.

### SetSecondLineNil

`func (o *UserAddressesResultsInner) SetSecondLineNil(b bool)`

 SetSecondLineNil sets the value for SecondLine to be an explicit nil

### UnsetSecondLine
`func (o *UserAddressesResultsInner) UnsetSecondLine()`

UnsetSecondLine ensures that no value is present for SecondLine, not even an explicit nil
### GetCity

`func (o *UserAddressesResultsInner) GetCity() string`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *UserAddressesResultsInner) GetCityOk() (*string, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *UserAddressesResultsInner) SetCity(v string)`

SetCity sets City field to given value.

### HasCity

`func (o *UserAddressesResultsInner) HasCity() bool`

HasCity returns a boolean if a field has been set.

### GetState

`func (o *UserAddressesResultsInner) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *UserAddressesResultsInner) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *UserAddressesResultsInner) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *UserAddressesResultsInner) HasState() bool`

HasState returns a boolean if a field has been set.

### SetStateNil

`func (o *UserAddressesResultsInner) SetStateNil(b bool)`

 SetStateNil sets the value for State to be an explicit nil

### UnsetState
`func (o *UserAddressesResultsInner) UnsetState()`

UnsetState ensures that no value is present for State, not even an explicit nil
### GetZip

`func (o *UserAddressesResultsInner) GetZip() string`

GetZip returns the Zip field if non-nil, zero value otherwise.

### GetZipOk

`func (o *UserAddressesResultsInner) GetZipOk() (*string, bool)`

GetZipOk returns a tuple with the Zip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZip

`func (o *UserAddressesResultsInner) SetZip(v string)`

SetZip sets Zip field to given value.

### HasZip

`func (o *UserAddressesResultsInner) HasZip() bool`

HasZip returns a boolean if a field has been set.

### GetIsoCountryCode

`func (o *UserAddressesResultsInner) GetIsoCountryCode() string`

GetIsoCountryCode returns the IsoCountryCode field if non-nil, zero value otherwise.

### GetIsoCountryCodeOk

`func (o *UserAddressesResultsInner) GetIsoCountryCodeOk() (*string, bool)`

GetIsoCountryCodeOk returns a tuple with the IsoCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsoCountryCode

`func (o *UserAddressesResultsInner) SetIsoCountryCode(v string)`

SetIsoCountryCode sets IsoCountryCode field to given value.

### HasIsoCountryCode

`func (o *UserAddressesResultsInner) HasIsoCountryCode() bool`

HasIsoCountryCode returns a boolean if a field has been set.

### SetIsoCountryCodeNil

`func (o *UserAddressesResultsInner) SetIsoCountryCodeNil(b bool)`

 SetIsoCountryCodeNil sets the value for IsoCountryCode to be an explicit nil

### UnsetIsoCountryCode
`func (o *UserAddressesResultsInner) UnsetIsoCountryCode()`

UnsetIsoCountryCode ensures that no value is present for IsoCountryCode, not even an explicit nil
### GetCountryName

`func (o *UserAddressesResultsInner) GetCountryName() string`

GetCountryName returns the CountryName field if non-nil, zero value otherwise.

### GetCountryNameOk

`func (o *UserAddressesResultsInner) GetCountryNameOk() (*string, bool)`

GetCountryNameOk returns a tuple with the CountryName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryName

`func (o *UserAddressesResultsInner) SetCountryName(v string)`

SetCountryName sets CountryName field to given value.

### HasCountryName

`func (o *UserAddressesResultsInner) HasCountryName() bool`

HasCountryName returns a boolean if a field has been set.

### SetCountryNameNil

`func (o *UserAddressesResultsInner) SetCountryNameNil(b bool)`

 SetCountryNameNil sets the value for CountryName to be an explicit nil

### UnsetCountryName
`func (o *UserAddressesResultsInner) UnsetCountryName()`

UnsetCountryName ensures that no value is present for CountryName, not even an explicit nil
### GetIsDefaultShippingAddress

`func (o *UserAddressesResultsInner) GetIsDefaultShippingAddress() bool`

GetIsDefaultShippingAddress returns the IsDefaultShippingAddress field if non-nil, zero value otherwise.

### GetIsDefaultShippingAddressOk

`func (o *UserAddressesResultsInner) GetIsDefaultShippingAddressOk() (*bool, bool)`

GetIsDefaultShippingAddressOk returns a tuple with the IsDefaultShippingAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefaultShippingAddress

`func (o *UserAddressesResultsInner) SetIsDefaultShippingAddress(v bool)`

SetIsDefaultShippingAddress sets IsDefaultShippingAddress field to given value.

### HasIsDefaultShippingAddress

`func (o *UserAddressesResultsInner) HasIsDefaultShippingAddress() bool`

HasIsDefaultShippingAddress returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


