# PaymentAdjustedFees

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amount** | Pointer to **int32** | The amount of represented by this data. | [optional] 
**Divisor** | Pointer to **int32** | The divisor to render the amount. | [optional] 
**CurrencyCode** | Pointer to **string** | The ISO currency code for this data. | [optional] 

## Methods

### NewPaymentAdjustedFees

`func NewPaymentAdjustedFees() *PaymentAdjustedFees`

NewPaymentAdjustedFees instantiates a new PaymentAdjustedFees object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentAdjustedFeesWithDefaults

`func NewPaymentAdjustedFeesWithDefaults() *PaymentAdjustedFees`

NewPaymentAdjustedFeesWithDefaults instantiates a new PaymentAdjustedFees object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmount

`func (o *PaymentAdjustedFees) GetAmount() int32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentAdjustedFees) GetAmountOk() (*int32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentAdjustedFees) SetAmount(v int32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *PaymentAdjustedFees) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetDivisor

`func (o *PaymentAdjustedFees) GetDivisor() int32`

GetDivisor returns the Divisor field if non-nil, zero value otherwise.

### GetDivisorOk

`func (o *PaymentAdjustedFees) GetDivisorOk() (*int32, bool)`

GetDivisorOk returns a tuple with the Divisor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDivisor

`func (o *PaymentAdjustedFees) SetDivisor(v int32)`

SetDivisor sets Divisor field to given value.

### HasDivisor

`func (o *PaymentAdjustedFees) HasDivisor() bool`

HasDivisor returns a boolean if a field has been set.

### GetCurrencyCode

`func (o *PaymentAdjustedFees) GetCurrencyCode() string`

GetCurrencyCode returns the CurrencyCode field if non-nil, zero value otherwise.

### GetCurrencyCodeOk

`func (o *PaymentAdjustedFees) GetCurrencyCodeOk() (*string, bool)`

GetCurrencyCodeOk returns a tuple with the CurrencyCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyCode

`func (o *PaymentAdjustedFees) SetCurrencyCode(v string)`

SetCurrencyCode sets CurrencyCode field to given value.

### HasCurrencyCode

`func (o *PaymentAdjustedFees) HasCurrencyCode() bool`

HasCurrencyCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


