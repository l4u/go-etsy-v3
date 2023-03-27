# ShopReceiptTransactionPrice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amount** | Pointer to **int32** | The amount of represented by this data. | [optional] 
**Divisor** | Pointer to **int32** | The divisor to render the amount. | [optional] 
**CurrencyCode** | Pointer to **string** | The ISO currency code for this data. | [optional] 

## Methods

### NewShopReceiptTransactionPrice

`func NewShopReceiptTransactionPrice() *ShopReceiptTransactionPrice`

NewShopReceiptTransactionPrice instantiates a new ShopReceiptTransactionPrice object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReceiptTransactionPriceWithDefaults

`func NewShopReceiptTransactionPriceWithDefaults() *ShopReceiptTransactionPrice`

NewShopReceiptTransactionPriceWithDefaults instantiates a new ShopReceiptTransactionPrice object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmount

`func (o *ShopReceiptTransactionPrice) GetAmount() int32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *ShopReceiptTransactionPrice) GetAmountOk() (*int32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *ShopReceiptTransactionPrice) SetAmount(v int32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *ShopReceiptTransactionPrice) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetDivisor

`func (o *ShopReceiptTransactionPrice) GetDivisor() int32`

GetDivisor returns the Divisor field if non-nil, zero value otherwise.

### GetDivisorOk

`func (o *ShopReceiptTransactionPrice) GetDivisorOk() (*int32, bool)`

GetDivisorOk returns a tuple with the Divisor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDivisor

`func (o *ShopReceiptTransactionPrice) SetDivisor(v int32)`

SetDivisor sets Divisor field to given value.

### HasDivisor

`func (o *ShopReceiptTransactionPrice) HasDivisor() bool`

HasDivisor returns a boolean if a field has been set.

### GetCurrencyCode

`func (o *ShopReceiptTransactionPrice) GetCurrencyCode() string`

GetCurrencyCode returns the CurrencyCode field if non-nil, zero value otherwise.

### GetCurrencyCodeOk

`func (o *ShopReceiptTransactionPrice) GetCurrencyCodeOk() (*string, bool)`

GetCurrencyCodeOk returns a tuple with the CurrencyCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyCode

`func (o *ShopReceiptTransactionPrice) SetCurrencyCode(v string)`

SetCurrencyCode sets CurrencyCode field to given value.

### HasCurrencyCode

`func (o *ShopReceiptTransactionPrice) HasCurrencyCode() bool`

HasCurrencyCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


