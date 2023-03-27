# PaymentAccountLedgerEntryPaymentAdjustmentsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PaymentAdjustmentId** | Pointer to **int32** | The numeric ID for a payment adjustment. | [optional] 
**PaymentId** | Pointer to **int32** | A unique numeric ID for a payment to a specific Etsy [shop](/documentation/reference#tag/Shop). | [optional] 
**Status** | Pointer to **string** | The status string of the payment adjustment. | [optional] 
**IsSuccess** | Pointer to **bool** | When true, the payment adjustment was or is likely to complete successfully. | [optional] 
**UserId** | Pointer to **int32** | The numeric ID for the [user](/documentation/reference#tag/User) (seller) fulfilling the purchase. | [optional] 
**ReasonCode** | Pointer to **string** | A human-readable string describing the reason for the refund. | [optional] 
**TotalAdjustmentAmount** | Pointer to **NullableInt32** | The total numeric amount of the refund in the payment currency. | [optional] 
**ShopTotalAdjustmentAmount** | Pointer to **NullableInt32** | The numeric amount of the refund in the shop currency. | [optional] 
**BuyerTotalAdjustmentAmount** | Pointer to **NullableInt32** | The numeric amount of the refund in the buyer currency. | [optional] 
**TotalFeeAdjustmentAmount** | Pointer to **NullableInt32** | The numeric amount of card processing fees associated with a payment adjustment. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The transaction\\&#39;s creation date and time, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The transaction\\&#39;s creation date and time, in epoch seconds. | [optional] 
**UpdateTimestamp** | Pointer to **int32** | The date and time of the last change to the payment adjustment in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The date and time of the last change to the payment adjustment in epoch seconds. | [optional] 
**PaymentAdjustmentItems** | Pointer to [**[]PaymentAdjustmentPaymentAdjustmentItemsInner**](PaymentAdjustmentPaymentAdjustmentItemsInner.md) | List of payment adjustment line items. | [optional] 

## Methods

### NewPaymentAccountLedgerEntryPaymentAdjustmentsInner

`func NewPaymentAccountLedgerEntryPaymentAdjustmentsInner() *PaymentAccountLedgerEntryPaymentAdjustmentsInner`

NewPaymentAccountLedgerEntryPaymentAdjustmentsInner instantiates a new PaymentAccountLedgerEntryPaymentAdjustmentsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentAccountLedgerEntryPaymentAdjustmentsInnerWithDefaults

`func NewPaymentAccountLedgerEntryPaymentAdjustmentsInnerWithDefaults() *PaymentAccountLedgerEntryPaymentAdjustmentsInner`

NewPaymentAccountLedgerEntryPaymentAdjustmentsInnerWithDefaults instantiates a new PaymentAccountLedgerEntryPaymentAdjustmentsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaymentAdjustmentId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetPaymentAdjustmentId() int32`

GetPaymentAdjustmentId returns the PaymentAdjustmentId field if non-nil, zero value otherwise.

### GetPaymentAdjustmentIdOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetPaymentAdjustmentIdOk() (*int32, bool)`

GetPaymentAdjustmentIdOk returns a tuple with the PaymentAdjustmentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAdjustmentId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetPaymentAdjustmentId(v int32)`

SetPaymentAdjustmentId sets PaymentAdjustmentId field to given value.

### HasPaymentAdjustmentId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasPaymentAdjustmentId() bool`

HasPaymentAdjustmentId returns a boolean if a field has been set.

### GetPaymentId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetPaymentId() int32`

GetPaymentId returns the PaymentId field if non-nil, zero value otherwise.

### GetPaymentIdOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetPaymentIdOk() (*int32, bool)`

GetPaymentIdOk returns a tuple with the PaymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetPaymentId(v int32)`

SetPaymentId sets PaymentId field to given value.

### HasPaymentId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasPaymentId() bool`

HasPaymentId returns a boolean if a field has been set.

### GetStatus

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetIsSuccess

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetIsSuccess() bool`

GetIsSuccess returns the IsSuccess field if non-nil, zero value otherwise.

### GetIsSuccessOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetIsSuccessOk() (*bool, bool)`

GetIsSuccessOk returns a tuple with the IsSuccess field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSuccess

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetIsSuccess(v bool)`

SetIsSuccess sets IsSuccess field to given value.

### HasIsSuccess

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasIsSuccess() bool`

HasIsSuccess returns a boolean if a field has been set.

### GetUserId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetReasonCode

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetReasonCode() string`

GetReasonCode returns the ReasonCode field if non-nil, zero value otherwise.

### GetReasonCodeOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetReasonCodeOk() (*string, bool)`

GetReasonCodeOk returns a tuple with the ReasonCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReasonCode

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetReasonCode(v string)`

SetReasonCode sets ReasonCode field to given value.

### HasReasonCode

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasReasonCode() bool`

HasReasonCode returns a boolean if a field has been set.

### GetTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetTotalAdjustmentAmount() int32`

GetTotalAdjustmentAmount returns the TotalAdjustmentAmount field if non-nil, zero value otherwise.

### GetTotalAdjustmentAmountOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetTotalAdjustmentAmountOk() (*int32, bool)`

GetTotalAdjustmentAmountOk returns a tuple with the TotalAdjustmentAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetTotalAdjustmentAmount(v int32)`

SetTotalAdjustmentAmount sets TotalAdjustmentAmount field to given value.

### HasTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasTotalAdjustmentAmount() bool`

HasTotalAdjustmentAmount returns a boolean if a field has been set.

### SetTotalAdjustmentAmountNil

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetTotalAdjustmentAmountNil(b bool)`

 SetTotalAdjustmentAmountNil sets the value for TotalAdjustmentAmount to be an explicit nil

### UnsetTotalAdjustmentAmount
`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) UnsetTotalAdjustmentAmount()`

UnsetTotalAdjustmentAmount ensures that no value is present for TotalAdjustmentAmount, not even an explicit nil
### GetShopTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetShopTotalAdjustmentAmount() int32`

GetShopTotalAdjustmentAmount returns the ShopTotalAdjustmentAmount field if non-nil, zero value otherwise.

### GetShopTotalAdjustmentAmountOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetShopTotalAdjustmentAmountOk() (*int32, bool)`

GetShopTotalAdjustmentAmountOk returns a tuple with the ShopTotalAdjustmentAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetShopTotalAdjustmentAmount(v int32)`

SetShopTotalAdjustmentAmount sets ShopTotalAdjustmentAmount field to given value.

### HasShopTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasShopTotalAdjustmentAmount() bool`

HasShopTotalAdjustmentAmount returns a boolean if a field has been set.

### SetShopTotalAdjustmentAmountNil

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetShopTotalAdjustmentAmountNil(b bool)`

 SetShopTotalAdjustmentAmountNil sets the value for ShopTotalAdjustmentAmount to be an explicit nil

### UnsetShopTotalAdjustmentAmount
`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) UnsetShopTotalAdjustmentAmount()`

UnsetShopTotalAdjustmentAmount ensures that no value is present for ShopTotalAdjustmentAmount, not even an explicit nil
### GetBuyerTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetBuyerTotalAdjustmentAmount() int32`

GetBuyerTotalAdjustmentAmount returns the BuyerTotalAdjustmentAmount field if non-nil, zero value otherwise.

### GetBuyerTotalAdjustmentAmountOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetBuyerTotalAdjustmentAmountOk() (*int32, bool)`

GetBuyerTotalAdjustmentAmountOk returns a tuple with the BuyerTotalAdjustmentAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetBuyerTotalAdjustmentAmount(v int32)`

SetBuyerTotalAdjustmentAmount sets BuyerTotalAdjustmentAmount field to given value.

### HasBuyerTotalAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasBuyerTotalAdjustmentAmount() bool`

HasBuyerTotalAdjustmentAmount returns a boolean if a field has been set.

### SetBuyerTotalAdjustmentAmountNil

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetBuyerTotalAdjustmentAmountNil(b bool)`

 SetBuyerTotalAdjustmentAmountNil sets the value for BuyerTotalAdjustmentAmount to be an explicit nil

### UnsetBuyerTotalAdjustmentAmount
`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) UnsetBuyerTotalAdjustmentAmount()`

UnsetBuyerTotalAdjustmentAmount ensures that no value is present for BuyerTotalAdjustmentAmount, not even an explicit nil
### GetTotalFeeAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetTotalFeeAdjustmentAmount() int32`

GetTotalFeeAdjustmentAmount returns the TotalFeeAdjustmentAmount field if non-nil, zero value otherwise.

### GetTotalFeeAdjustmentAmountOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetTotalFeeAdjustmentAmountOk() (*int32, bool)`

GetTotalFeeAdjustmentAmountOk returns a tuple with the TotalFeeAdjustmentAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalFeeAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetTotalFeeAdjustmentAmount(v int32)`

SetTotalFeeAdjustmentAmount sets TotalFeeAdjustmentAmount field to given value.

### HasTotalFeeAdjustmentAmount

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasTotalFeeAdjustmentAmount() bool`

HasTotalFeeAdjustmentAmount returns a boolean if a field has been set.

### SetTotalFeeAdjustmentAmountNil

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetTotalFeeAdjustmentAmountNil(b bool)`

 SetTotalFeeAdjustmentAmountNil sets the value for TotalFeeAdjustmentAmount to be an explicit nil

### UnsetTotalFeeAdjustmentAmount
`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) UnsetTotalFeeAdjustmentAmount()`

UnsetTotalFeeAdjustmentAmount ensures that no value is present for TotalFeeAdjustmentAmount, not even an explicit nil
### GetCreateTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdateTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetUpdateTimestamp() int32`

GetUpdateTimestamp returns the UpdateTimestamp field if non-nil, zero value otherwise.

### GetUpdateTimestampOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetUpdateTimestampOk() (*int32, bool)`

GetUpdateTimestampOk returns a tuple with the UpdateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetUpdateTimestamp(v int32)`

SetUpdateTimestamp sets UpdateTimestamp field to given value.

### HasUpdateTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasUpdateTimestamp() bool`

HasUpdateTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetPaymentAdjustmentItems

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetPaymentAdjustmentItems() []PaymentAdjustmentPaymentAdjustmentItemsInner`

GetPaymentAdjustmentItems returns the PaymentAdjustmentItems field if non-nil, zero value otherwise.

### GetPaymentAdjustmentItemsOk

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) GetPaymentAdjustmentItemsOk() (*[]PaymentAdjustmentPaymentAdjustmentItemsInner, bool)`

GetPaymentAdjustmentItemsOk returns a tuple with the PaymentAdjustmentItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAdjustmentItems

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) SetPaymentAdjustmentItems(v []PaymentAdjustmentPaymentAdjustmentItemsInner)`

SetPaymentAdjustmentItems sets PaymentAdjustmentItems field to given value.

### HasPaymentAdjustmentItems

`func (o *PaymentAccountLedgerEntryPaymentAdjustmentsInner) HasPaymentAdjustmentItems() bool`

HasPaymentAdjustmentItems returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


