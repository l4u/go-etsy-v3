# Payment

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

### NewPayment

`func NewPayment() *Payment`

NewPayment instantiates a new Payment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaymentWithDefaults

`func NewPaymentWithDefaults() *Payment`

NewPaymentWithDefaults instantiates a new Payment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaymentId

`func (o *Payment) GetPaymentId() int32`

GetPaymentId returns the PaymentId field if non-nil, zero value otherwise.

### GetPaymentIdOk

`func (o *Payment) GetPaymentIdOk() (*int32, bool)`

GetPaymentIdOk returns a tuple with the PaymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentId

`func (o *Payment) SetPaymentId(v int32)`

SetPaymentId sets PaymentId field to given value.

### HasPaymentId

`func (o *Payment) HasPaymentId() bool`

HasPaymentId returns a boolean if a field has been set.

### GetBuyerUserId

`func (o *Payment) GetBuyerUserId() int32`

GetBuyerUserId returns the BuyerUserId field if non-nil, zero value otherwise.

### GetBuyerUserIdOk

`func (o *Payment) GetBuyerUserIdOk() (*int32, bool)`

GetBuyerUserIdOk returns a tuple with the BuyerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerUserId

`func (o *Payment) SetBuyerUserId(v int32)`

SetBuyerUserId sets BuyerUserId field to given value.

### HasBuyerUserId

`func (o *Payment) HasBuyerUserId() bool`

HasBuyerUserId returns a boolean if a field has been set.

### GetShopId

`func (o *Payment) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *Payment) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *Payment) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *Payment) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetReceiptId

`func (o *Payment) GetReceiptId() int32`

GetReceiptId returns the ReceiptId field if non-nil, zero value otherwise.

### GetReceiptIdOk

`func (o *Payment) GetReceiptIdOk() (*int32, bool)`

GetReceiptIdOk returns a tuple with the ReceiptId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptId

`func (o *Payment) SetReceiptId(v int32)`

SetReceiptId sets ReceiptId field to given value.

### HasReceiptId

`func (o *Payment) HasReceiptId() bool`

HasReceiptId returns a boolean if a field has been set.

### GetAmountGross

`func (o *Payment) GetAmountGross() PaymentAmountGross`

GetAmountGross returns the AmountGross field if non-nil, zero value otherwise.

### GetAmountGrossOk

`func (o *Payment) GetAmountGrossOk() (*PaymentAmountGross, bool)`

GetAmountGrossOk returns a tuple with the AmountGross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmountGross

`func (o *Payment) SetAmountGross(v PaymentAmountGross)`

SetAmountGross sets AmountGross field to given value.

### HasAmountGross

`func (o *Payment) HasAmountGross() bool`

HasAmountGross returns a boolean if a field has been set.

### GetAmountFees

`func (o *Payment) GetAmountFees() PaymentAmountFees`

GetAmountFees returns the AmountFees field if non-nil, zero value otherwise.

### GetAmountFeesOk

`func (o *Payment) GetAmountFeesOk() (*PaymentAmountFees, bool)`

GetAmountFeesOk returns a tuple with the AmountFees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmountFees

`func (o *Payment) SetAmountFees(v PaymentAmountFees)`

SetAmountFees sets AmountFees field to given value.

### HasAmountFees

`func (o *Payment) HasAmountFees() bool`

HasAmountFees returns a boolean if a field has been set.

### GetAmountNet

`func (o *Payment) GetAmountNet() PaymentAmountNet`

GetAmountNet returns the AmountNet field if non-nil, zero value otherwise.

### GetAmountNetOk

`func (o *Payment) GetAmountNetOk() (*PaymentAmountNet, bool)`

GetAmountNetOk returns a tuple with the AmountNet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmountNet

`func (o *Payment) SetAmountNet(v PaymentAmountNet)`

SetAmountNet sets AmountNet field to given value.

### HasAmountNet

`func (o *Payment) HasAmountNet() bool`

HasAmountNet returns a boolean if a field has been set.

### GetPostedGross

`func (o *Payment) GetPostedGross() PaymentPostedGross`

GetPostedGross returns the PostedGross field if non-nil, zero value otherwise.

### GetPostedGrossOk

`func (o *Payment) GetPostedGrossOk() (*PaymentPostedGross, bool)`

GetPostedGrossOk returns a tuple with the PostedGross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostedGross

`func (o *Payment) SetPostedGross(v PaymentPostedGross)`

SetPostedGross sets PostedGross field to given value.

### HasPostedGross

`func (o *Payment) HasPostedGross() bool`

HasPostedGross returns a boolean if a field has been set.

### GetPostedFees

`func (o *Payment) GetPostedFees() PaymentPostedFees`

GetPostedFees returns the PostedFees field if non-nil, zero value otherwise.

### GetPostedFeesOk

`func (o *Payment) GetPostedFeesOk() (*PaymentPostedFees, bool)`

GetPostedFeesOk returns a tuple with the PostedFees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostedFees

`func (o *Payment) SetPostedFees(v PaymentPostedFees)`

SetPostedFees sets PostedFees field to given value.

### HasPostedFees

`func (o *Payment) HasPostedFees() bool`

HasPostedFees returns a boolean if a field has been set.

### GetPostedNet

`func (o *Payment) GetPostedNet() PaymentPostedNet`

GetPostedNet returns the PostedNet field if non-nil, zero value otherwise.

### GetPostedNetOk

`func (o *Payment) GetPostedNetOk() (*PaymentPostedNet, bool)`

GetPostedNetOk returns a tuple with the PostedNet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostedNet

`func (o *Payment) SetPostedNet(v PaymentPostedNet)`

SetPostedNet sets PostedNet field to given value.

### HasPostedNet

`func (o *Payment) HasPostedNet() bool`

HasPostedNet returns a boolean if a field has been set.

### GetAdjustedGross

`func (o *Payment) GetAdjustedGross() PaymentAdjustedGross`

GetAdjustedGross returns the AdjustedGross field if non-nil, zero value otherwise.

### GetAdjustedGrossOk

`func (o *Payment) GetAdjustedGrossOk() (*PaymentAdjustedGross, bool)`

GetAdjustedGrossOk returns a tuple with the AdjustedGross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustedGross

`func (o *Payment) SetAdjustedGross(v PaymentAdjustedGross)`

SetAdjustedGross sets AdjustedGross field to given value.

### HasAdjustedGross

`func (o *Payment) HasAdjustedGross() bool`

HasAdjustedGross returns a boolean if a field has been set.

### GetAdjustedFees

`func (o *Payment) GetAdjustedFees() PaymentAdjustedFees`

GetAdjustedFees returns the AdjustedFees field if non-nil, zero value otherwise.

### GetAdjustedFeesOk

`func (o *Payment) GetAdjustedFeesOk() (*PaymentAdjustedFees, bool)`

GetAdjustedFeesOk returns a tuple with the AdjustedFees field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustedFees

`func (o *Payment) SetAdjustedFees(v PaymentAdjustedFees)`

SetAdjustedFees sets AdjustedFees field to given value.

### HasAdjustedFees

`func (o *Payment) HasAdjustedFees() bool`

HasAdjustedFees returns a boolean if a field has been set.

### GetAdjustedNet

`func (o *Payment) GetAdjustedNet() PaymentAdjustedNet`

GetAdjustedNet returns the AdjustedNet field if non-nil, zero value otherwise.

### GetAdjustedNetOk

`func (o *Payment) GetAdjustedNetOk() (*PaymentAdjustedNet, bool)`

GetAdjustedNetOk returns a tuple with the AdjustedNet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustedNet

`func (o *Payment) SetAdjustedNet(v PaymentAdjustedNet)`

SetAdjustedNet sets AdjustedNet field to given value.

### HasAdjustedNet

`func (o *Payment) HasAdjustedNet() bool`

HasAdjustedNet returns a boolean if a field has been set.

### GetCurrency

`func (o *Payment) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *Payment) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *Payment) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *Payment) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetShopCurrency

`func (o *Payment) GetShopCurrency() string`

GetShopCurrency returns the ShopCurrency field if non-nil, zero value otherwise.

### GetShopCurrencyOk

`func (o *Payment) GetShopCurrencyOk() (*string, bool)`

GetShopCurrencyOk returns a tuple with the ShopCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopCurrency

`func (o *Payment) SetShopCurrency(v string)`

SetShopCurrency sets ShopCurrency field to given value.

### HasShopCurrency

`func (o *Payment) HasShopCurrency() bool`

HasShopCurrency returns a boolean if a field has been set.

### SetShopCurrencyNil

`func (o *Payment) SetShopCurrencyNil(b bool)`

 SetShopCurrencyNil sets the value for ShopCurrency to be an explicit nil

### UnsetShopCurrency
`func (o *Payment) UnsetShopCurrency()`

UnsetShopCurrency ensures that no value is present for ShopCurrency, not even an explicit nil
### GetBuyerCurrency

`func (o *Payment) GetBuyerCurrency() string`

GetBuyerCurrency returns the BuyerCurrency field if non-nil, zero value otherwise.

### GetBuyerCurrencyOk

`func (o *Payment) GetBuyerCurrencyOk() (*string, bool)`

GetBuyerCurrencyOk returns a tuple with the BuyerCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerCurrency

`func (o *Payment) SetBuyerCurrency(v string)`

SetBuyerCurrency sets BuyerCurrency field to given value.

### HasBuyerCurrency

`func (o *Payment) HasBuyerCurrency() bool`

HasBuyerCurrency returns a boolean if a field has been set.

### SetBuyerCurrencyNil

`func (o *Payment) SetBuyerCurrencyNil(b bool)`

 SetBuyerCurrencyNil sets the value for BuyerCurrency to be an explicit nil

### UnsetBuyerCurrency
`func (o *Payment) UnsetBuyerCurrency()`

UnsetBuyerCurrency ensures that no value is present for BuyerCurrency, not even an explicit nil
### GetShippingUserId

`func (o *Payment) GetShippingUserId() int32`

GetShippingUserId returns the ShippingUserId field if non-nil, zero value otherwise.

### GetShippingUserIdOk

`func (o *Payment) GetShippingUserIdOk() (*int32, bool)`

GetShippingUserIdOk returns a tuple with the ShippingUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingUserId

`func (o *Payment) SetShippingUserId(v int32)`

SetShippingUserId sets ShippingUserId field to given value.

### HasShippingUserId

`func (o *Payment) HasShippingUserId() bool`

HasShippingUserId returns a boolean if a field has been set.

### SetShippingUserIdNil

`func (o *Payment) SetShippingUserIdNil(b bool)`

 SetShippingUserIdNil sets the value for ShippingUserId to be an explicit nil

### UnsetShippingUserId
`func (o *Payment) UnsetShippingUserId()`

UnsetShippingUserId ensures that no value is present for ShippingUserId, not even an explicit nil
### GetShippingAddressId

`func (o *Payment) GetShippingAddressId() int32`

GetShippingAddressId returns the ShippingAddressId field if non-nil, zero value otherwise.

### GetShippingAddressIdOk

`func (o *Payment) GetShippingAddressIdOk() (*int32, bool)`

GetShippingAddressIdOk returns a tuple with the ShippingAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippingAddressId

`func (o *Payment) SetShippingAddressId(v int32)`

SetShippingAddressId sets ShippingAddressId field to given value.

### HasShippingAddressId

`func (o *Payment) HasShippingAddressId() bool`

HasShippingAddressId returns a boolean if a field has been set.

### GetBillingAddressId

`func (o *Payment) GetBillingAddressId() int32`

GetBillingAddressId returns the BillingAddressId field if non-nil, zero value otherwise.

### GetBillingAddressIdOk

`func (o *Payment) GetBillingAddressIdOk() (*int32, bool)`

GetBillingAddressIdOk returns a tuple with the BillingAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBillingAddressId

`func (o *Payment) SetBillingAddressId(v int32)`

SetBillingAddressId sets BillingAddressId field to given value.

### HasBillingAddressId

`func (o *Payment) HasBillingAddressId() bool`

HasBillingAddressId returns a boolean if a field has been set.

### GetStatus

`func (o *Payment) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Payment) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Payment) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *Payment) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetShippedTimestamp

`func (o *Payment) GetShippedTimestamp() int32`

GetShippedTimestamp returns the ShippedTimestamp field if non-nil, zero value otherwise.

### GetShippedTimestampOk

`func (o *Payment) GetShippedTimestampOk() (*int32, bool)`

GetShippedTimestampOk returns a tuple with the ShippedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShippedTimestamp

`func (o *Payment) SetShippedTimestamp(v int32)`

SetShippedTimestamp sets ShippedTimestamp field to given value.

### HasShippedTimestamp

`func (o *Payment) HasShippedTimestamp() bool`

HasShippedTimestamp returns a boolean if a field has been set.

### SetShippedTimestampNil

`func (o *Payment) SetShippedTimestampNil(b bool)`

 SetShippedTimestampNil sets the value for ShippedTimestamp to be an explicit nil

### UnsetShippedTimestamp
`func (o *Payment) UnsetShippedTimestamp()`

UnsetShippedTimestamp ensures that no value is present for ShippedTimestamp, not even an explicit nil
### GetCreateTimestamp

`func (o *Payment) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *Payment) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *Payment) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *Payment) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *Payment) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *Payment) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *Payment) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *Payment) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdateTimestamp

`func (o *Payment) GetUpdateTimestamp() int32`

GetUpdateTimestamp returns the UpdateTimestamp field if non-nil, zero value otherwise.

### GetUpdateTimestampOk

`func (o *Payment) GetUpdateTimestampOk() (*int32, bool)`

GetUpdateTimestampOk returns a tuple with the UpdateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateTimestamp

`func (o *Payment) SetUpdateTimestamp(v int32)`

SetUpdateTimestamp sets UpdateTimestamp field to given value.

### HasUpdateTimestamp

`func (o *Payment) HasUpdateTimestamp() bool`

HasUpdateTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *Payment) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *Payment) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *Payment) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *Payment) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetPaymentAdjustments

`func (o *Payment) GetPaymentAdjustments() []PaymentAccountLedgerEntryPaymentAdjustmentsInner`

GetPaymentAdjustments returns the PaymentAdjustments field if non-nil, zero value otherwise.

### GetPaymentAdjustmentsOk

`func (o *Payment) GetPaymentAdjustmentsOk() (*[]PaymentAccountLedgerEntryPaymentAdjustmentsInner, bool)`

GetPaymentAdjustmentsOk returns a tuple with the PaymentAdjustments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentAdjustments

`func (o *Payment) SetPaymentAdjustments(v []PaymentAccountLedgerEntryPaymentAdjustmentsInner)`

SetPaymentAdjustments sets PaymentAdjustments field to given value.

### HasPaymentAdjustments

`func (o *Payment) HasPaymentAdjustments() bool`

HasPaymentAdjustments returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


