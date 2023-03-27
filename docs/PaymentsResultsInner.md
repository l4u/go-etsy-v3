# PaymentsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PaymentId** | Pointer to **int32** | A unique numeric ID for a payment to a specific Etsy [shop](/documentation/reference#tag/Shop). | [optional] 
**BuyerUserId** | Pointer to **int32** | The numeric ID for the [user](/documentation/reference#tag/User) who paid the purchase. | [optional] 
**ShopId** | Pointer to **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | [optional] 
**ReceiptId** | Pointer to **int32** | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction. | [optional] 
**AmountGross** | Pointer to [**PaymentAmountGross**](PaymentAmountGross.md) |  | [optional] 
**AmountFees** | Pointer to [**PaymentAmountFees**](PaymentAmountFees.md) |  | [optional] 
**AmountNet** | Pointer to [**PaymentAmountNet**](PaymentAmountNet.md) |  | [optional] 
**PostedGross** | Pointer to [**PaymentPostedGross**](PaymentPostedGross.md) |  | [optional] 
**PostedFees** | Pointer to [**PaymentPostedFees**](PaymentPostedFees.md) |  | [optional] 
**PostedNet** | Pointer to [**PaymentPostedNet**](PaymentPostedNet.md) |  | [optional] 
**AdjustedGross** | Pointer to [**PaymentAdjustedGross**](PaymentAdjustedGross.md) |  | [optional] 
**AdjustedFees** | Pointer to [**PaymentAdjustedFees**](PaymentAdjustedFees.md) |  | [optional] 
**AdjustedNet** | Pointer to [**PaymentAdjustedNet**](PaymentAdjustedNet.md) |  | [optional] 
**Currency** | Pointer to **string** | The ISO (alphabetic) code string for the payment&#39;s currency. | [optional] 
**ShopCurrency** | Pointer to **NullableString** | The ISO (alphabetic) code for the shop&#39;s currency. The shop displays all prices in this currency by default. | [optional] 
**BuyerCurrency** | Pointer to **NullableString** | The currency string of the buyer. | [optional] 
**ShippingUserId** | Pointer to **NullableInt32** | The numeric ID of the user to which the seller ships the order. | [optional] 
**ShippingAddressId** | Pointer to **int32** | The numeric id identifying the shipping address. | [optional] 
**BillingAddressId** | Pointer to **int32** | The numeric ID identifying the billing address of the buyer. | [optional] 
**Status** | Pointer to **string** | A string indicating the current status of the payment, most commonly \&quot;settled\&quot; or \&quot;authed\&quot;. | [optional] 
**ShippedTimestamp** | Pointer to **NullableInt32** | The transaction\\&#39;s shipping date and time, in epoch seconds. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The transaction\\&#39;s creation date and time, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The transaction\\&#39;s creation date and time, in epoch seconds. | [optional] 
**UpdateTimestamp** | Pointer to **int32** | The date and time of the last change to the payment adjustment in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The date and time of the last change to the payment adjustment in epoch seconds. | [optional] 
**PaymentAdjustments** | Pointer to [**[]PaymentAccountLedgerEntryPaymentAdjustmentsInner**](PaymentAccountLedgerEntryPaymentAdjustmentsInner.md) | List of refund objects on an Etsy Payments transaction. All monetary amounts are in USD pennies unless otherwise specified. | [optional] 

## Methods

### NewPaymentsResultsInner

`func NewPaymentsResultsInner() *PaymentsResultsInner`

NewPaymentsResultsInner instantiates a new PaymentsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentsResultsInnerWithDefaults

`func NewPaymentsResultsInnerWithDefaults() *PaymentsResultsInner`

NewPaymentsResultsInnerWithDefaults instantiates a new PaymentsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaymentId

`func (o *PaymentsResultsInner) GetPaymentId() int32`

GetPaymentId returns the PaymentId field if non-nil, zero value otherwise.

### GetPaymentIdOk

`func (o *PaymentsResultsInner) GetPaymentIdOk() (*int32, bool)`

GetPaymentIdOk returns a tuple with the PaymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentId

`func (o *PaymentsResultsInner) SetPaymentId(v int32)`

SetPaymentId sets PaymentId field to given value.

### HasPaymentId

`func (o *PaymentsResultsInner) HasPaymentId() bool`

HasPaymentId returns a boolean if a field has been set.

### GetBuyerUserId

`func (o *PaymentsResultsInner) GetBuyerUserId() int32`

GetBuyerUserId returns the BuyerUserId field if non-nil, zero value otherwise.

### GetBuyerUserIdOk

`func (o *PaymentsResultsInner) GetBuyerUserIdOk() (*int32, bool)`

GetBuyerUserIdOk returns a tuple with the BuyerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerUserId

`func (o *PaymentsResultsInner) SetBuyerUserId(v int32)`

SetBuyerUserId sets BuyerUserId field to given value.

### HasBuyerUserId

`func (o *PaymentsResultsInner) HasBuyerUserId() bool`

HasBuyerUserId returns a boolean if a field has been set.

### GetShopId

`func (o *PaymentsResultsInner) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *PaymentsResultsInner) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *PaymentsResultsInner) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *PaymentsResultsInner) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetReceiptId

`func (o *PaymentsResultsInner) GetReceiptId() int32`

GetReceiptId returns the ReceiptId field if non-nil, zero value otherwise.

### GetReceiptIdOk

`func (o *PaymentsResultsInner) GetReceiptIdOk() (*int32, bool)`

GetReceiptIdOk returns a tuple with the ReceiptId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptId

`func (o *PaymentsResultsInner) SetReceiptId(v int32)`

SetReceiptId sets ReceiptId field to given value.

### HasReceiptId

`func (o *PaymentsResultsInner) HasReceiptId() bool`

HasReceiptId returns a boolean if a field has been set.

### GetAmountGross

`func (o *PaymentsResultsInner) GetAmountGross() PaymentAmountGross`

GetAmountGross returns the AmountGross field if non-nil, zero value otherwise.

### GetAmountGrossOk

`func (o *PaymentsResultsInner) GetAmountGrossOk() (*PaymentAmountGross, bool)`

GetAmountGrossOk returns a tuple with the AmountGross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmountGross

`func (o *PaymentsResultsInner) SetAmountGross(v PaymentAmountGross)`

SetAmountGross sets AmountGross field to given value.

### HasAmountGross

`func (o *PaymentsResultsInner) HasAmountGross() bool`

HasAmountGross returns a boolean if a field has been set.

### GetAmountFees

`func (o *PaymentsResultsInner) GetAmountFees() PaymentAmountFees`

GetAmountFees returns the AmountFees field if non-nil, zero value otherwise.

### GetAmountFeesOk

`func (o *PaymentsResultsInner) GetAmountFeesOk() (*PaymentAmountFees, bool)`

GetAmountFeesOk returns a tuple with the AmountFees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmountFees

`func (o *PaymentsResultsInner) SetAmountFees(v PaymentAmountFees)`

SetAmountFees sets AmountFees field to given value.

### HasAmountFees

`func (o *PaymentsResultsInner) HasAmountFees() bool`

HasAmountFees returns a boolean if a field has been set.

### GetAmountNet

`func (o *PaymentsResultsInner) GetAmountNet() PaymentAmountNet`

GetAmountNet returns the AmountNet field if non-nil, zero value otherwise.

### GetAmountNetOk

`func (o *PaymentsResultsInner) GetAmountNetOk() (*PaymentAmountNet, bool)`

GetAmountNetOk returns a tuple with the AmountNet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmountNet

`func (o *PaymentsResultsInner) SetAmountNet(v PaymentAmountNet)`

SetAmountNet sets AmountNet field to given value.

### HasAmountNet

`func (o *PaymentsResultsInner) HasAmountNet() bool`

HasAmountNet returns a boolean if a field has been set.

### GetPostedGross

`func (o *PaymentsResultsInner) GetPostedGross() PaymentPostedGross`

GetPostedGross returns the PostedGross field if non-nil, zero value otherwise.

### GetPostedGrossOk

`func (o *PaymentsResultsInner) GetPostedGrossOk() (*PaymentPostedGross, bool)`

GetPostedGrossOk returns a tuple with the PostedGross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostedGross

`func (o *PaymentsResultsInner) SetPostedGross(v PaymentPostedGross)`

SetPostedGross sets PostedGross field to given value.

### HasPostedGross

`func (o *PaymentsResultsInner) HasPostedGross() bool`

HasPostedGross returns a boolean if a field has been set.

### GetPostedFees

`func (o *PaymentsResultsInner) GetPostedFees() PaymentPostedFees`

GetPostedFees returns the PostedFees field if non-nil, zero value otherwise.

### GetPostedFeesOk

`func (o *PaymentsResultsInner) GetPostedFeesOk() (*PaymentPostedFees, bool)`

GetPostedFeesOk returns a tuple with the PostedFees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostedFees

`func (o *PaymentsResultsInner) SetPostedFees(v PaymentPostedFees)`

SetPostedFees sets PostedFees field to given value.

### HasPostedFees

`func (o *PaymentsResultsInner) HasPostedFees() bool`

HasPostedFees returns a boolean if a field has been set.

### GetPostedNet

`func (o *PaymentsResultsInner) GetPostedNet() PaymentPostedNet`

GetPostedNet returns the PostedNet field if non-nil, zero value otherwise.

### GetPostedNetOk

`func (o *PaymentsResultsInner) GetPostedNetOk() (*PaymentPostedNet, bool)`

GetPostedNetOk returns a tuple with the PostedNet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostedNet

`func (o *PaymentsResultsInner) SetPostedNet(v PaymentPostedNet)`

SetPostedNet sets PostedNet field to given value.

### HasPostedNet

`func (o *PaymentsResultsInner) HasPostedNet() bool`

HasPostedNet returns a boolean if a field has been set.

### GetAdjustedGross

`func (o *PaymentsResultsInner) GetAdjustedGross() PaymentAdjustedGross`

GetAdjustedGross returns the AdjustedGross field if non-nil, zero value otherwise.

### GetAdjustedGrossOk

`func (o *PaymentsResultsInner) GetAdjustedGrossOk() (*PaymentAdjustedGross, bool)`

GetAdjustedGrossOk returns a tuple with the AdjustedGross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustedGross

`func (o *PaymentsResultsInner) SetAdjustedGross(v PaymentAdjustedGross)`

SetAdjustedGross sets AdjustedGross field to given value.

### HasAdjustedGross

`func (o *PaymentsResultsInner) HasAdjustedGross() bool`

HasAdjustedGross returns a boolean if a field has been set.

### GetAdjustedFees

`func (o *PaymentsResultsInner) GetAdjustedFees() PaymentAdjustedFees`

GetAdjustedFees returns the AdjustedFees field if non-nil, zero value otherwise.

### GetAdjustedFeesOk

`func (o *PaymentsResultsInner) GetAdjustedFeesOk() (*PaymentAdjustedFees, bool)`

GetAdjustedFeesOk returns a tuple with the AdjustedFees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustedFees

`func (o *PaymentsResultsInner) SetAdjustedFees(v PaymentAdjustedFees)`

SetAdjustedFees sets AdjustedFees field to given value.

### HasAdjustedFees

`func (o *PaymentsResultsInner) HasAdjustedFees() bool`

HasAdjustedFees returns a boolean if a field has been set.

### GetAdjustedNet

`func (o *PaymentsResultsInner) GetAdjustedNet() PaymentAdjustedNet`

GetAdjustedNet returns the AdjustedNet field if non-nil, zero value otherwise.

### GetAdjustedNetOk

`func (o *PaymentsResultsInner) GetAdjustedNetOk() (*PaymentAdjustedNet, bool)`

GetAdjustedNetOk returns a tuple with the AdjustedNet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustedNet

`func (o *PaymentsResultsInner) SetAdjustedNet(v PaymentAdjustedNet)`

SetAdjustedNet sets AdjustedNet field to given value.

### HasAdjustedNet

`func (o *PaymentsResultsInner) HasAdjustedNet() bool`

HasAdjustedNet returns a boolean if a field has been set.

### GetCurrency

`func (o *PaymentsResultsInner) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *PaymentsResultsInner) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *PaymentsResultsInner) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *PaymentsResultsInner) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetShopCurrency

`func (o *PaymentsResultsInner) GetShopCurrency() string`

GetShopCurrency returns the ShopCurrency field if non-nil, zero value otherwise.

### GetShopCurrencyOk

`func (o *PaymentsResultsInner) GetShopCurrencyOk() (*string, bool)`

GetShopCurrencyOk returns a tuple with the ShopCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopCurrency

`func (o *PaymentsResultsInner) SetShopCurrency(v string)`

SetShopCurrency sets ShopCurrency field to given value.

### HasShopCurrency

`func (o *PaymentsResultsInner) HasShopCurrency() bool`

HasShopCurrency returns a boolean if a field has been set.

### SetShopCurrencyNil

`func (o *PaymentsResultsInner) SetShopCurrencyNil(b bool)`

 SetShopCurrencyNil sets the value for ShopCurrency to be an explicit nil

### UnsetShopCurrency
`func (o *PaymentsResultsInner) UnsetShopCurrency()`

UnsetShopCurrency ensures that no value is present for ShopCurrency, not even an explicit nil
### GetBuyerCurrency

`func (o *PaymentsResultsInner) GetBuyerCurrency() string`

GetBuyerCurrency returns the BuyerCurrency field if non-nil, zero value otherwise.

### GetBuyerCurrencyOk

`func (o *PaymentsResultsInner) GetBuyerCurrencyOk() (*string, bool)`

GetBuyerCurrencyOk returns a tuple with the BuyerCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerCurrency

`func (o *PaymentsResultsInner) SetBuyerCurrency(v string)`

SetBuyerCurrency sets BuyerCurrency field to given value.

### HasBuyerCurrency

`func (o *PaymentsResultsInner) HasBuyerCurrency() bool`

HasBuyerCurrency returns a boolean if a field has been set.

### SetBuyerCurrencyNil

`func (o *PaymentsResultsInner) SetBuyerCurrencyNil(b bool)`

 SetBuyerCurrencyNil sets the value for BuyerCurrency to be an explicit nil

### UnsetBuyerCurrency
`func (o *PaymentsResultsInner) UnsetBuyerCurrency()`

UnsetBuyerCurrency ensures that no value is present for BuyerCurrency, not even an explicit nil
### GetShippingUserId

`func (o *PaymentsResultsInner) GetShippingUserId() int32`

GetShippingUserId returns the ShippingUserId field if non-nil, zero value otherwise.

### GetShippingUserIdOk

`func (o *PaymentsResultsInner) GetShippingUserIdOk() (*int32, bool)`

GetShippingUserIdOk returns a tuple with the ShippingUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingUserId

`func (o *PaymentsResultsInner) SetShippingUserId(v int32)`

SetShippingUserId sets ShippingUserId field to given value.

### HasShippingUserId

`func (o *PaymentsResultsInner) HasShippingUserId() bool`

HasShippingUserId returns a boolean if a field has been set.

### SetShippingUserIdNil

`func (o *PaymentsResultsInner) SetShippingUserIdNil(b bool)`

 SetShippingUserIdNil sets the value for ShippingUserId to be an explicit nil

### UnsetShippingUserId
`func (o *PaymentsResultsInner) UnsetShippingUserId()`

UnsetShippingUserId ensures that no value is present for ShippingUserId, not even an explicit nil
### GetShippingAddressId

`func (o *PaymentsResultsInner) GetShippingAddressId() int32`

GetShippingAddressId returns the ShippingAddressId field if non-nil, zero value otherwise.

### GetShippingAddressIdOk

`func (o *PaymentsResultsInner) GetShippingAddressIdOk() (*int32, bool)`

GetShippingAddressIdOk returns a tuple with the ShippingAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingAddressId

`func (o *PaymentsResultsInner) SetShippingAddressId(v int32)`

SetShippingAddressId sets ShippingAddressId field to given value.

### HasShippingAddressId

`func (o *PaymentsResultsInner) HasShippingAddressId() bool`

HasShippingAddressId returns a boolean if a field has been set.

### GetBillingAddressId

`func (o *PaymentsResultsInner) GetBillingAddressId() int32`

GetBillingAddressId returns the BillingAddressId field if non-nil, zero value otherwise.

### GetBillingAddressIdOk

`func (o *PaymentsResultsInner) GetBillingAddressIdOk() (*int32, bool)`

GetBillingAddressIdOk returns a tuple with the BillingAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBillingAddressId

`func (o *PaymentsResultsInner) SetBillingAddressId(v int32)`

SetBillingAddressId sets BillingAddressId field to given value.

### HasBillingAddressId

`func (o *PaymentsResultsInner) HasBillingAddressId() bool`

HasBillingAddressId returns a boolean if a field has been set.

### GetStatus

`func (o *PaymentsResultsInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PaymentsResultsInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PaymentsResultsInner) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *PaymentsResultsInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetShippedTimestamp

`func (o *PaymentsResultsInner) GetShippedTimestamp() int32`

GetShippedTimestamp returns the ShippedTimestamp field if non-nil, zero value otherwise.

### GetShippedTimestampOk

`func (o *PaymentsResultsInner) GetShippedTimestampOk() (*int32, bool)`

GetShippedTimestampOk returns a tuple with the ShippedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippedTimestamp

`func (o *PaymentsResultsInner) SetShippedTimestamp(v int32)`

SetShippedTimestamp sets ShippedTimestamp field to given value.

### HasShippedTimestamp

`func (o *PaymentsResultsInner) HasShippedTimestamp() bool`

HasShippedTimestamp returns a boolean if a field has been set.

### SetShippedTimestampNil

`func (o *PaymentsResultsInner) SetShippedTimestampNil(b bool)`

 SetShippedTimestampNil sets the value for ShippedTimestamp to be an explicit nil

### UnsetShippedTimestamp
`func (o *PaymentsResultsInner) UnsetShippedTimestamp()`

UnsetShippedTimestamp ensures that no value is present for ShippedTimestamp, not even an explicit nil
### GetCreateTimestamp

`func (o *PaymentsResultsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *PaymentsResultsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *PaymentsResultsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *PaymentsResultsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *PaymentsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *PaymentsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *PaymentsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *PaymentsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdateTimestamp

`func (o *PaymentsResultsInner) GetUpdateTimestamp() int32`

GetUpdateTimestamp returns the UpdateTimestamp field if non-nil, zero value otherwise.

### GetUpdateTimestampOk

`func (o *PaymentsResultsInner) GetUpdateTimestampOk() (*int32, bool)`

GetUpdateTimestampOk returns a tuple with the UpdateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateTimestamp

`func (o *PaymentsResultsInner) SetUpdateTimestamp(v int32)`

SetUpdateTimestamp sets UpdateTimestamp field to given value.

### HasUpdateTimestamp

`func (o *PaymentsResultsInner) HasUpdateTimestamp() bool`

HasUpdateTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *PaymentsResultsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *PaymentsResultsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *PaymentsResultsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *PaymentsResultsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetPaymentAdjustments

`func (o *PaymentsResultsInner) GetPaymentAdjustments() []PaymentAccountLedgerEntryPaymentAdjustmentsInner`

GetPaymentAdjustments returns the PaymentAdjustments field if non-nil, zero value otherwise.

### GetPaymentAdjustmentsOk

`func (o *PaymentsResultsInner) GetPaymentAdjustmentsOk() (*[]PaymentAccountLedgerEntryPaymentAdjustmentsInner, bool)`

GetPaymentAdjustmentsOk returns a tuple with the PaymentAdjustments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAdjustments

`func (o *PaymentsResultsInner) SetPaymentAdjustments(v []PaymentAccountLedgerEntryPaymentAdjustmentsInner)`

SetPaymentAdjustments sets PaymentAdjustments field to given value.

### HasPaymentAdjustments

`func (o *PaymentsResultsInner) HasPaymentAdjustments() bool`

HasPaymentAdjustments returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


