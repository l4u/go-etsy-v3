# PaymentAccountLedgerEntriesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EntryId** | Pointer to **int32** | The ledger entry&#39;s numeric ID. | [optional] 
**LedgerId** | Pointer to **int32** | The ledger&#39;s numeric ID. | [optional] 
**SequenceNumber** | Pointer to **int32** | The sequence allows ledger entries to be sorted chronologically. The higher the sequence, the more recent the entry. | [optional] 
**Amount** | Pointer to **int32** | The amount of money credited to the ledger. | [optional] 
**Currency** | Pointer to **string** | The currency of the entry on the ledger. | [optional] 
**Description** | Pointer to **string** | Details what kind of ledger entry this is: a payment, refund, reversal of a failed refund, disbursement, returned disbursement, recoupment, miscellaneous credit, miscellaneous debit, or bill payment. | [optional] 
**Balance** | Pointer to **int32** | The amount of money in the shop&#39;s ledger the moment after this entry was applied. | [optional] 
**CreateDate** | Pointer to **int32** | The date and time the ledger entry was created in Epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The date and time the ledger entry was created in Epoch seconds. | [optional] 
**LedgerType** | Pointer to **string** | The original reference type for the ledger entry. | [optional] 
**ReferenceType** | Pointer to **string** | The object type the ledger entry refers to. | [optional] 
**ReferenceId** | Pointer to **NullableString** | The object id the ledger entry refers to. | [optional] 
**PaymentAdjustments** | Pointer to [**[]PaymentAccountLedgerEntryPaymentAdjustmentsInner**](PaymentAccountLedgerEntryPaymentAdjustmentsInner.md) | List of refund objects on an Etsy Payments transaction. All monetary amounts are in USD pennies unless otherwise specified. | [optional] 

## Methods

### NewPaymentAccountLedgerEntriesResultsInner

`func NewPaymentAccountLedgerEntriesResultsInner() *PaymentAccountLedgerEntriesResultsInner`

NewPaymentAccountLedgerEntriesResultsInner instantiates a new PaymentAccountLedgerEntriesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentAccountLedgerEntriesResultsInnerWithDefaults

`func NewPaymentAccountLedgerEntriesResultsInnerWithDefaults() *PaymentAccountLedgerEntriesResultsInner`

NewPaymentAccountLedgerEntriesResultsInnerWithDefaults instantiates a new PaymentAccountLedgerEntriesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEntryId

`func (o *PaymentAccountLedgerEntriesResultsInner) GetEntryId() int32`

GetEntryId returns the EntryId field if non-nil, zero value otherwise.

### GetEntryIdOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetEntryIdOk() (*int32, bool)`

GetEntryIdOk returns a tuple with the EntryId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntryId

`func (o *PaymentAccountLedgerEntriesResultsInner) SetEntryId(v int32)`

SetEntryId sets EntryId field to given value.

### HasEntryId

`func (o *PaymentAccountLedgerEntriesResultsInner) HasEntryId() bool`

HasEntryId returns a boolean if a field has been set.

### GetLedgerId

`func (o *PaymentAccountLedgerEntriesResultsInner) GetLedgerId() int32`

GetLedgerId returns the LedgerId field if non-nil, zero value otherwise.

### GetLedgerIdOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetLedgerIdOk() (*int32, bool)`

GetLedgerIdOk returns a tuple with the LedgerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLedgerId

`func (o *PaymentAccountLedgerEntriesResultsInner) SetLedgerId(v int32)`

SetLedgerId sets LedgerId field to given value.

### HasLedgerId

`func (o *PaymentAccountLedgerEntriesResultsInner) HasLedgerId() bool`

HasLedgerId returns a boolean if a field has been set.

### GetSequenceNumber

`func (o *PaymentAccountLedgerEntriesResultsInner) GetSequenceNumber() int32`

GetSequenceNumber returns the SequenceNumber field if non-nil, zero value otherwise.

### GetSequenceNumberOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetSequenceNumberOk() (*int32, bool)`

GetSequenceNumberOk returns a tuple with the SequenceNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSequenceNumber

`func (o *PaymentAccountLedgerEntriesResultsInner) SetSequenceNumber(v int32)`

SetSequenceNumber sets SequenceNumber field to given value.

### HasSequenceNumber

`func (o *PaymentAccountLedgerEntriesResultsInner) HasSequenceNumber() bool`

HasSequenceNumber returns a boolean if a field has been set.

### GetAmount

`func (o *PaymentAccountLedgerEntriesResultsInner) GetAmount() int32`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetAmountOk() (*int32, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *PaymentAccountLedgerEntriesResultsInner) SetAmount(v int32)`

SetAmount sets Amount field to given value.

### HasAmount

`func (o *PaymentAccountLedgerEntriesResultsInner) HasAmount() bool`

HasAmount returns a boolean if a field has been set.

### GetCurrency

`func (o *PaymentAccountLedgerEntriesResultsInner) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *PaymentAccountLedgerEntriesResultsInner) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *PaymentAccountLedgerEntriesResultsInner) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetDescription

`func (o *PaymentAccountLedgerEntriesResultsInner) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PaymentAccountLedgerEntriesResultsInner) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PaymentAccountLedgerEntriesResultsInner) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBalance

`func (o *PaymentAccountLedgerEntriesResultsInner) GetBalance() int32`

GetBalance returns the Balance field if non-nil, zero value otherwise.

### GetBalanceOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetBalanceOk() (*int32, bool)`

GetBalanceOk returns a tuple with the Balance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalance

`func (o *PaymentAccountLedgerEntriesResultsInner) SetBalance(v int32)`

SetBalance sets Balance field to given value.

### HasBalance

`func (o *PaymentAccountLedgerEntriesResultsInner) HasBalance() bool`

HasBalance returns a boolean if a field has been set.

### GetCreateDate

`func (o *PaymentAccountLedgerEntriesResultsInner) GetCreateDate() int32`

GetCreateDate returns the CreateDate field if non-nil, zero value otherwise.

### GetCreateDateOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetCreateDateOk() (*int32, bool)`

GetCreateDateOk returns a tuple with the CreateDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateDate

`func (o *PaymentAccountLedgerEntriesResultsInner) SetCreateDate(v int32)`

SetCreateDate sets CreateDate field to given value.

### HasCreateDate

`func (o *PaymentAccountLedgerEntriesResultsInner) HasCreateDate() bool`

HasCreateDate returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *PaymentAccountLedgerEntriesResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *PaymentAccountLedgerEntriesResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *PaymentAccountLedgerEntriesResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetLedgerType

`func (o *PaymentAccountLedgerEntriesResultsInner) GetLedgerType() string`

GetLedgerType returns the LedgerType field if non-nil, zero value otherwise.

### GetLedgerTypeOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetLedgerTypeOk() (*string, bool)`

GetLedgerTypeOk returns a tuple with the LedgerType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLedgerType

`func (o *PaymentAccountLedgerEntriesResultsInner) SetLedgerType(v string)`

SetLedgerType sets LedgerType field to given value.

### HasLedgerType

`func (o *PaymentAccountLedgerEntriesResultsInner) HasLedgerType() bool`

HasLedgerType returns a boolean if a field has been set.

### GetReferenceType

`func (o *PaymentAccountLedgerEntriesResultsInner) GetReferenceType() string`

GetReferenceType returns the ReferenceType field if non-nil, zero value otherwise.

### GetReferenceTypeOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetReferenceTypeOk() (*string, bool)`

GetReferenceTypeOk returns a tuple with the ReferenceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceType

`func (o *PaymentAccountLedgerEntriesResultsInner) SetReferenceType(v string)`

SetReferenceType sets ReferenceType field to given value.

### HasReferenceType

`func (o *PaymentAccountLedgerEntriesResultsInner) HasReferenceType() bool`

HasReferenceType returns a boolean if a field has been set.

### GetReferenceId

`func (o *PaymentAccountLedgerEntriesResultsInner) GetReferenceId() string`

GetReferenceId returns the ReferenceId field if non-nil, zero value otherwise.

### GetReferenceIdOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetReferenceIdOk() (*string, bool)`

GetReferenceIdOk returns a tuple with the ReferenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceId

`func (o *PaymentAccountLedgerEntriesResultsInner) SetReferenceId(v string)`

SetReferenceId sets ReferenceId field to given value.

### HasReferenceId

`func (o *PaymentAccountLedgerEntriesResultsInner) HasReferenceId() bool`

HasReferenceId returns a boolean if a field has been set.

### SetReferenceIdNil

`func (o *PaymentAccountLedgerEntriesResultsInner) SetReferenceIdNil(b bool)`

 SetReferenceIdNil sets the value for ReferenceId to be an explicit nil

### UnsetReferenceId
`func (o *PaymentAccountLedgerEntriesResultsInner) UnsetReferenceId()`

UnsetReferenceId ensures that no value is present for ReferenceId, not even an explicit nil
### GetPaymentAdjustments

`func (o *PaymentAccountLedgerEntriesResultsInner) GetPaymentAdjustments() []PaymentAccountLedgerEntryPaymentAdjustmentsInner`

GetPaymentAdjustments returns the PaymentAdjustments field if non-nil, zero value otherwise.

### GetPaymentAdjustmentsOk

`func (o *PaymentAccountLedgerEntriesResultsInner) GetPaymentAdjustmentsOk() (*[]PaymentAccountLedgerEntryPaymentAdjustmentsInner, bool)`

GetPaymentAdjustmentsOk returns a tuple with the PaymentAdjustments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAdjustments

`func (o *PaymentAccountLedgerEntriesResultsInner) SetPaymentAdjustments(v []PaymentAccountLedgerEntryPaymentAdjustmentsInner)`

SetPaymentAdjustments sets PaymentAdjustments field to given value.

### HasPaymentAdjustments

`func (o *PaymentAccountLedgerEntriesResultsInner) HasPaymentAdjustments() bool`

HasPaymentAdjustments returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


