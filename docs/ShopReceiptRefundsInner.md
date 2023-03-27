# ShopReceiptRefundsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amount** | Pointer to [**ShopRefundAmount**](ShopRefundAmount.md) |  | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The date &amp; time of the refund, in epoch seconds. | [optional] 
**Reason** | Pointer to **NullableString** | The reason string given for the refund. | [optional] 
**NoteFromIssuer** | Pointer to **NullableString** | The note string created by the refund issuer. | [optional] 
**Status** | Pointer to **NullableString** | The status indication string for the refund. | [optional] 

## Methods

### NewShopReceiptRefundsInner

`func NewShopReceiptRefundsInner() *ShopReceiptRefundsInner`

NewShopReceiptRefundsInner instantiates a new ShopReceiptRefundsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReceiptRefundsInnerWithDefaults

`func NewShopReceiptRefundsInnerWithDefaults() *ShopReceiptRefundsInner`

NewShopReceiptRefundsInnerWithDefaults instantiates a new ShopReceiptRefundsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmount

`func (o *ShopReceiptRefundsInner) GetAmount() ShopRefundAmount`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *ShopReceiptRefundsInner) GetAmountOk() (*ShopRefundAmount, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *ShopReceiptRefundsInner) SetAmount(v ShopRefundAmount)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *ShopReceiptRefundsInner) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopReceiptRefundsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopReceiptRefundsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopReceiptRefundsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopReceiptRefundsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetReason

`func (o *ShopReceiptRefundsInner) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *ShopReceiptRefundsInner) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *ShopReceiptRefundsInner) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *ShopReceiptRefundsInner) HasReason() bool`

HasReason returns a boolean if a field has been set.

### SetReasonNil

`func (o *ShopReceiptRefundsInner) SetReasonNil(b bool)`

 SetReasonNil sets the value for Reason to be an explicit nil

### UnsetReason
`func (o *ShopReceiptRefundsInner) UnsetReason()`

UnsetReason ensures that no value is present for Reason, not even an explicit nil
### GetNoteFromIssuer

`func (o *ShopReceiptRefundsInner) GetNoteFromIssuer() string`

GetNoteFromIssuer returns the NoteFromIssuer field if non-nil, zero value otherwise.

### GetNoteFromIssuerOk

`func (o *ShopReceiptRefundsInner) GetNoteFromIssuerOk() (*string, bool)`

GetNoteFromIssuerOk returns a tuple with the NoteFromIssuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNoteFromIssuer

`func (o *ShopReceiptRefundsInner) SetNoteFromIssuer(v string)`

SetNoteFromIssuer sets NoteFromIssuer field to given value.

### HasNoteFromIssuer

`func (o *ShopReceiptRefundsInner) HasNoteFromIssuer() bool`

HasNoteFromIssuer returns a boolean if a field has been set.

### SetNoteFromIssuerNil

`func (o *ShopReceiptRefundsInner) SetNoteFromIssuerNil(b bool)`

 SetNoteFromIssuerNil sets the value for NoteFromIssuer to be an explicit nil

### UnsetNoteFromIssuer
`func (o *ShopReceiptRefundsInner) UnsetNoteFromIssuer()`

UnsetNoteFromIssuer ensures that no value is present for NoteFromIssuer, not even an explicit nil
### GetStatus

`func (o *ShopReceiptRefundsInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ShopReceiptRefundsInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ShopReceiptRefundsInner) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ShopReceiptRefundsInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *ShopReceiptRefundsInner) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *ShopReceiptRefundsInner) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


