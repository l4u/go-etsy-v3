# ShopReceiptsResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReceiptId** | Pointer to **int32** | The numeric ID for the [receipt](/documentation/reference#tag/Shop-Receipt) associated to this transaction. | [optional] 
**ReceiptType** | Pointer to **int32** | The numeric value for the Etsy channel that serviced the purchase: 0 for Etsy.com, 1 for a Pattern shop. | [optional] 
**SellerUserId** | Pointer to **int32** | The numeric ID for the [user](/documentation/reference#tag/User) (seller) fulfilling the purchase. | [optional] 
**SellerEmail** | Pointer to **NullableString** | The email address string for the seller of the listing. | [optional] 
**BuyerUserId** | Pointer to **int32** | The numeric ID for the [user](/documentation/reference#tag/User) making the purchase. | [optional] 
**BuyerEmail** | Pointer to **NullableString** | The email address string for the buyer of the listing. | [optional] 
**Name** | Pointer to **string** | The name string for the recipient in the shipping address. | [optional] 
**FirstLine** | Pointer to **string** | The first address line string for the recipient in the shipping address. | [optional] 
**SecondLine** | Pointer to **NullableString** | The optional second address line string for the recipient in the shipping address. | [optional] 
**City** | Pointer to **string** | The city string for the recipient in the shipping address. | [optional] 
**State** | Pointer to **NullableString** | The state string for the recipient in the shipping address. | [optional] 
**Zip** | Pointer to **string** | The zip code string (not necessarily a number) for the recipient in the shipping address. | [optional] 
**Status** | Pointer to **string** | The current order status string. One of: &#x60;paid&#x60;, &#x60;completed&#x60;, &#x60;open&#x60;, &#x60;payment processing&#x60; or &#x60;canceled&#x60;. | [optional] 
**FormattedAddress** | Pointer to **string** | The formatted shipping address string for the recipient in the shipping address. | [optional] 
**CountryIso** | Pointer to **string** | The ISO-3166 alpha-2 country code string for the recipient in the shipping address. | [optional] 
**PaymentMethod** | Pointer to **string** | The payment method string identifying purchaser&#39;s payment method, which must be one of: \\&#39;cc\\&#39; (credit card), \\&#39;paypal\\&#39;, \\&#39;check\\&#39;, \\&#39;mo\\&#39; (money order), \\&#39;bt\\&#39; (bank transfer), \\&#39;other\\&#39;, \\&#39;ideal\\&#39;, \\&#39;sofort\\&#39;, \\&#39;apple_pay\\&#39;, \\&#39;google\\&#39;, \\&#39;android_pay\\&#39;, \\&#39;google_pay\\&#39;, \\&#39;klarna\\&#39;, \\&#39;k_pay_in_4\\&#39; (klarna), \\&#39;k_pay_in_3\\&#39; (klarna), or \\&#39;k_financing\\&#39; (klarna). | [optional] 
**PaymentEmail** | Pointer to **string** | The email address string for the email address to which to send payment confirmation | [optional] 
**MessageFromSeller** | Pointer to **NullableString** | An optional message string from the seller. | [optional] 
**MessageFromBuyer** | Pointer to **NullableString** | An optional message string from the buyer. | [optional] 
**MessageFromPayment** | Pointer to **NullableString** | The machine-generated acknowledgement string from the payment system. | [optional] 
**IsPaid** | Pointer to **bool** | When true, buyer paid for this purchase. | [optional] 
**IsShipped** | Pointer to **bool** | When true, seller shipped the products. | [optional] 
**CreateTimestamp** | Pointer to **int32** | The receipt\\&#39;s creation time, in epoch seconds. | [optional] 
**CreatedTimestamp** | Pointer to **int32** | The receipt\\&#39;s creation time, in epoch seconds. | [optional] 
**UpdateTimestamp** | Pointer to **int32** | The time of the last update to the receipt, in epoch seconds. | [optional] 
**UpdatedTimestamp** | Pointer to **int32** | The time of the last update to the receipt, in epoch seconds. | [optional] 
**IsGift** | Pointer to **bool** | When true, the buyer indicated this purchase is a gift. | [optional] 
**GiftMessage** | Pointer to **string** | A gift message string the buyer requests delivered with the product. | [optional] 
**Grandtotal** | Pointer to [**ShopReceiptGrandtotal**](ShopReceiptGrandtotal.md) |  | [optional] 
**Subtotal** | Pointer to [**ShopReceiptSubtotal**](ShopReceiptSubtotal.md) |  | [optional] 
**TotalPrice** | Pointer to [**ShopReceiptTotalPrice**](ShopReceiptTotalPrice.md) |  | [optional] 
**TotalShippingCost** | Pointer to [**ShopReceiptTotalShippingCost**](ShopReceiptTotalShippingCost.md) |  | [optional] 
**TotalTaxCost** | Pointer to [**ShopReceiptTotalTaxCost**](ShopReceiptTotalTaxCost.md) |  | [optional] 
**TotalVatCost** | Pointer to [**ShopReceiptTotalVatCost**](ShopReceiptTotalVatCost.md) |  | [optional] 
**DiscountAmt** | Pointer to [**ShopReceiptDiscountAmt**](ShopReceiptDiscountAmt.md) |  | [optional] 
**GiftWrapPrice** | Pointer to [**ShopReceiptGiftWrapPrice**](ShopReceiptGiftWrapPrice.md) |  | [optional] 
**Shipments** | Pointer to [**[]ShopReceiptShipmentsInner**](ShopReceiptShipmentsInner.md) | A list of shipment statements for this receipt. | [optional] 
**Transactions** | Pointer to [**[]ShopReceiptTransactionsInner**](ShopReceiptTransactionsInner.md) | Array of transactions for the receipt. | [optional] 
**Refunds** | Pointer to [**[]ShopReceiptRefundsInner**](ShopReceiptRefundsInner.md) | Refunds for a given receipt. | [optional] 

## Methods

### NewShopReceiptsResultsInner

`func NewShopReceiptsResultsInner() *ShopReceiptsResultsInner`

NewShopReceiptsResultsInner instantiates a new ShopReceiptsResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReceiptsResultsInnerWithDefaults

`func NewShopReceiptsResultsInnerWithDefaults() *ShopReceiptsResultsInner`

NewShopReceiptsResultsInnerWithDefaults instantiates a new ShopReceiptsResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReceiptId

`func (o *ShopReceiptsResultsInner) GetReceiptId() int32`

GetReceiptId returns the ReceiptId field if non-nil, zero value otherwise.

### GetReceiptIdOk

`func (o *ShopReceiptsResultsInner) GetReceiptIdOk() (*int32, bool)`

GetReceiptIdOk returns a tuple with the ReceiptId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptId

`func (o *ShopReceiptsResultsInner) SetReceiptId(v int32)`

SetReceiptId sets ReceiptId field to given value.

### HasReceiptId

`func (o *ShopReceiptsResultsInner) HasReceiptId() bool`

HasReceiptId returns a boolean if a field has been set.

### GetReceiptType

`func (o *ShopReceiptsResultsInner) GetReceiptType() int32`

GetReceiptType returns the ReceiptType field if non-nil, zero value otherwise.

### GetReceiptTypeOk

`func (o *ShopReceiptsResultsInner) GetReceiptTypeOk() (*int32, bool)`

GetReceiptTypeOk returns a tuple with the ReceiptType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptType

`func (o *ShopReceiptsResultsInner) SetReceiptType(v int32)`

SetReceiptType sets ReceiptType field to given value.

### HasReceiptType

`func (o *ShopReceiptsResultsInner) HasReceiptType() bool`

HasReceiptType returns a boolean if a field has been set.

### GetSellerUserId

`func (o *ShopReceiptsResultsInner) GetSellerUserId() int32`

GetSellerUserId returns the SellerUserId field if non-nil, zero value otherwise.

### GetSellerUserIdOk

`func (o *ShopReceiptsResultsInner) GetSellerUserIdOk() (*int32, bool)`

GetSellerUserIdOk returns a tuple with the SellerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerUserId

`func (o *ShopReceiptsResultsInner) SetSellerUserId(v int32)`

SetSellerUserId sets SellerUserId field to given value.

### HasSellerUserId

`func (o *ShopReceiptsResultsInner) HasSellerUserId() bool`

HasSellerUserId returns a boolean if a field has been set.

### GetSellerEmail

`func (o *ShopReceiptsResultsInner) GetSellerEmail() string`

GetSellerEmail returns the SellerEmail field if non-nil, zero value otherwise.

### GetSellerEmailOk

`func (o *ShopReceiptsResultsInner) GetSellerEmailOk() (*string, bool)`

GetSellerEmailOk returns a tuple with the SellerEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerEmail

`func (o *ShopReceiptsResultsInner) SetSellerEmail(v string)`

SetSellerEmail sets SellerEmail field to given value.

### HasSellerEmail

`func (o *ShopReceiptsResultsInner) HasSellerEmail() bool`

HasSellerEmail returns a boolean if a field has been set.

### SetSellerEmailNil

`func (o *ShopReceiptsResultsInner) SetSellerEmailNil(b bool)`

 SetSellerEmailNil sets the value for SellerEmail to be an explicit nil

### UnsetSellerEmail
`func (o *ShopReceiptsResultsInner) UnsetSellerEmail()`

UnsetSellerEmail ensures that no value is present for SellerEmail, not even an explicit nil
### GetBuyerUserId

`func (o *ShopReceiptsResultsInner) GetBuyerUserId() int32`

GetBuyerUserId returns the BuyerUserId field if non-nil, zero value otherwise.

### GetBuyerUserIdOk

`func (o *ShopReceiptsResultsInner) GetBuyerUserIdOk() (*int32, bool)`

GetBuyerUserIdOk returns a tuple with the BuyerUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerUserId

`func (o *ShopReceiptsResultsInner) SetBuyerUserId(v int32)`

SetBuyerUserId sets BuyerUserId field to given value.

### HasBuyerUserId

`func (o *ShopReceiptsResultsInner) HasBuyerUserId() bool`

HasBuyerUserId returns a boolean if a field has been set.

### GetBuyerEmail

`func (o *ShopReceiptsResultsInner) GetBuyerEmail() string`

GetBuyerEmail returns the BuyerEmail field if non-nil, zero value otherwise.

### GetBuyerEmailOk

`func (o *ShopReceiptsResultsInner) GetBuyerEmailOk() (*string, bool)`

GetBuyerEmailOk returns a tuple with the BuyerEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuyerEmail

`func (o *ShopReceiptsResultsInner) SetBuyerEmail(v string)`

SetBuyerEmail sets BuyerEmail field to given value.

### HasBuyerEmail

`func (o *ShopReceiptsResultsInner) HasBuyerEmail() bool`

HasBuyerEmail returns a boolean if a field has been set.

### SetBuyerEmailNil

`func (o *ShopReceiptsResultsInner) SetBuyerEmailNil(b bool)`

 SetBuyerEmailNil sets the value for BuyerEmail to be an explicit nil

### UnsetBuyerEmail
`func (o *ShopReceiptsResultsInner) UnsetBuyerEmail()`

UnsetBuyerEmail ensures that no value is present for BuyerEmail, not even an explicit nil
### GetName

`func (o *ShopReceiptsResultsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ShopReceiptsResultsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ShopReceiptsResultsInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ShopReceiptsResultsInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetFirstLine

`func (o *ShopReceiptsResultsInner) GetFirstLine() string`

GetFirstLine returns the FirstLine field if non-nil, zero value otherwise.

### GetFirstLineOk

`func (o *ShopReceiptsResultsInner) GetFirstLineOk() (*string, bool)`

GetFirstLineOk returns a tuple with the FirstLine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstLine

`func (o *ShopReceiptsResultsInner) SetFirstLine(v string)`

SetFirstLine sets FirstLine field to given value.

### HasFirstLine

`func (o *ShopReceiptsResultsInner) HasFirstLine() bool`

HasFirstLine returns a boolean if a field has been set.

### GetSecondLine

`func (o *ShopReceiptsResultsInner) GetSecondLine() string`

GetSecondLine returns the SecondLine field if non-nil, zero value otherwise.

### GetSecondLineOk

`func (o *ShopReceiptsResultsInner) GetSecondLineOk() (*string, bool)`

GetSecondLineOk returns a tuple with the SecondLine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondLine

`func (o *ShopReceiptsResultsInner) SetSecondLine(v string)`

SetSecondLine sets SecondLine field to given value.

### HasSecondLine

`func (o *ShopReceiptsResultsInner) HasSecondLine() bool`

HasSecondLine returns a boolean if a field has been set.

### SetSecondLineNil

`func (o *ShopReceiptsResultsInner) SetSecondLineNil(b bool)`

 SetSecondLineNil sets the value for SecondLine to be an explicit nil

### UnsetSecondLine
`func (o *ShopReceiptsResultsInner) UnsetSecondLine()`

UnsetSecondLine ensures that no value is present for SecondLine, not even an explicit nil
### GetCity

`func (o *ShopReceiptsResultsInner) GetCity() string`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *ShopReceiptsResultsInner) GetCityOk() (*string, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *ShopReceiptsResultsInner) SetCity(v string)`

SetCity sets City field to given value.

### HasCity

`func (o *ShopReceiptsResultsInner) HasCity() bool`

HasCity returns a boolean if a field has been set.

### GetState

`func (o *ShopReceiptsResultsInner) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ShopReceiptsResultsInner) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ShopReceiptsResultsInner) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *ShopReceiptsResultsInner) HasState() bool`

HasState returns a boolean if a field has been set.

### SetStateNil

`func (o *ShopReceiptsResultsInner) SetStateNil(b bool)`

 SetStateNil sets the value for State to be an explicit nil

### UnsetState
`func (o *ShopReceiptsResultsInner) UnsetState()`

UnsetState ensures that no value is present for State, not even an explicit nil
### GetZip

`func (o *ShopReceiptsResultsInner) GetZip() string`

GetZip returns the Zip field if non-nil, zero value otherwise.

### GetZipOk

`func (o *ShopReceiptsResultsInner) GetZipOk() (*string, bool)`

GetZipOk returns a tuple with the Zip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZip

`func (o *ShopReceiptsResultsInner) SetZip(v string)`

SetZip sets Zip field to given value.

### HasZip

`func (o *ShopReceiptsResultsInner) HasZip() bool`

HasZip returns a boolean if a field has been set.

### GetStatus

`func (o *ShopReceiptsResultsInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ShopReceiptsResultsInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ShopReceiptsResultsInner) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ShopReceiptsResultsInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetFormattedAddress

`func (o *ShopReceiptsResultsInner) GetFormattedAddress() string`

GetFormattedAddress returns the FormattedAddress field if non-nil, zero value otherwise.

### GetFormattedAddressOk

`func (o *ShopReceiptsResultsInner) GetFormattedAddressOk() (*string, bool)`

GetFormattedAddressOk returns a tuple with the FormattedAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormattedAddress

`func (o *ShopReceiptsResultsInner) SetFormattedAddress(v string)`

SetFormattedAddress sets FormattedAddress field to given value.

### HasFormattedAddress

`func (o *ShopReceiptsResultsInner) HasFormattedAddress() bool`

HasFormattedAddress returns a boolean if a field has been set.

### GetCountryIso

`func (o *ShopReceiptsResultsInner) GetCountryIso() string`

GetCountryIso returns the CountryIso field if non-nil, zero value otherwise.

### GetCountryIsoOk

`func (o *ShopReceiptsResultsInner) GetCountryIsoOk() (*string, bool)`

GetCountryIsoOk returns a tuple with the CountryIso field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryIso

`func (o *ShopReceiptsResultsInner) SetCountryIso(v string)`

SetCountryIso sets CountryIso field to given value.

### HasCountryIso

`func (o *ShopReceiptsResultsInner) HasCountryIso() bool`

HasCountryIso returns a boolean if a field has been set.

### GetPaymentMethod

`func (o *ShopReceiptsResultsInner) GetPaymentMethod() string`

GetPaymentMethod returns the PaymentMethod field if non-nil, zero value otherwise.

### GetPaymentMethodOk

`func (o *ShopReceiptsResultsInner) GetPaymentMethodOk() (*string, bool)`

GetPaymentMethodOk returns a tuple with the PaymentMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentMethod

`func (o *ShopReceiptsResultsInner) SetPaymentMethod(v string)`

SetPaymentMethod sets PaymentMethod field to given value.

### HasPaymentMethod

`func (o *ShopReceiptsResultsInner) HasPaymentMethod() bool`

HasPaymentMethod returns a boolean if a field has been set.

### GetPaymentEmail

`func (o *ShopReceiptsResultsInner) GetPaymentEmail() string`

GetPaymentEmail returns the PaymentEmail field if non-nil, zero value otherwise.

### GetPaymentEmailOk

`func (o *ShopReceiptsResultsInner) GetPaymentEmailOk() (*string, bool)`

GetPaymentEmailOk returns a tuple with the PaymentEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaymentEmail

`func (o *ShopReceiptsResultsInner) SetPaymentEmail(v string)`

SetPaymentEmail sets PaymentEmail field to given value.

### HasPaymentEmail

`func (o *ShopReceiptsResultsInner) HasPaymentEmail() bool`

HasPaymentEmail returns a boolean if a field has been set.

### GetMessageFromSeller

`func (o *ShopReceiptsResultsInner) GetMessageFromSeller() string`

GetMessageFromSeller returns the MessageFromSeller field if non-nil, zero value otherwise.

### GetMessageFromSellerOk

`func (o *ShopReceiptsResultsInner) GetMessageFromSellerOk() (*string, bool)`

GetMessageFromSellerOk returns a tuple with the MessageFromSeller field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageFromSeller

`func (o *ShopReceiptsResultsInner) SetMessageFromSeller(v string)`

SetMessageFromSeller sets MessageFromSeller field to given value.

### HasMessageFromSeller

`func (o *ShopReceiptsResultsInner) HasMessageFromSeller() bool`

HasMessageFromSeller returns a boolean if a field has been set.

### SetMessageFromSellerNil

`func (o *ShopReceiptsResultsInner) SetMessageFromSellerNil(b bool)`

 SetMessageFromSellerNil sets the value for MessageFromSeller to be an explicit nil

### UnsetMessageFromSeller
`func (o *ShopReceiptsResultsInner) UnsetMessageFromSeller()`

UnsetMessageFromSeller ensures that no value is present for MessageFromSeller, not even an explicit nil
### GetMessageFromBuyer

`func (o *ShopReceiptsResultsInner) GetMessageFromBuyer() string`

GetMessageFromBuyer returns the MessageFromBuyer field if non-nil, zero value otherwise.

### GetMessageFromBuyerOk

`func (o *ShopReceiptsResultsInner) GetMessageFromBuyerOk() (*string, bool)`

GetMessageFromBuyerOk returns a tuple with the MessageFromBuyer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageFromBuyer

`func (o *ShopReceiptsResultsInner) SetMessageFromBuyer(v string)`

SetMessageFromBuyer sets MessageFromBuyer field to given value.

### HasMessageFromBuyer

`func (o *ShopReceiptsResultsInner) HasMessageFromBuyer() bool`

HasMessageFromBuyer returns a boolean if a field has been set.

### SetMessageFromBuyerNil

`func (o *ShopReceiptsResultsInner) SetMessageFromBuyerNil(b bool)`

 SetMessageFromBuyerNil sets the value for MessageFromBuyer to be an explicit nil

### UnsetMessageFromBuyer
`func (o *ShopReceiptsResultsInner) UnsetMessageFromBuyer()`

UnsetMessageFromBuyer ensures that no value is present for MessageFromBuyer, not even an explicit nil
### GetMessageFromPayment

`func (o *ShopReceiptsResultsInner) GetMessageFromPayment() string`

GetMessageFromPayment returns the MessageFromPayment field if non-nil, zero value otherwise.

### GetMessageFromPaymentOk

`func (o *ShopReceiptsResultsInner) GetMessageFromPaymentOk() (*string, bool)`

GetMessageFromPaymentOk returns a tuple with the MessageFromPayment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageFromPayment

`func (o *ShopReceiptsResultsInner) SetMessageFromPayment(v string)`

SetMessageFromPayment sets MessageFromPayment field to given value.

### HasMessageFromPayment

`func (o *ShopReceiptsResultsInner) HasMessageFromPayment() bool`

HasMessageFromPayment returns a boolean if a field has been set.

### SetMessageFromPaymentNil

`func (o *ShopReceiptsResultsInner) SetMessageFromPaymentNil(b bool)`

 SetMessageFromPaymentNil sets the value for MessageFromPayment to be an explicit nil

### UnsetMessageFromPayment
`func (o *ShopReceiptsResultsInner) UnsetMessageFromPayment()`

UnsetMessageFromPayment ensures that no value is present for MessageFromPayment, not even an explicit nil
### GetIsPaid

`func (o *ShopReceiptsResultsInner) GetIsPaid() bool`

GetIsPaid returns the IsPaid field if non-nil, zero value otherwise.

### GetIsPaidOk

`func (o *ShopReceiptsResultsInner) GetIsPaidOk() (*bool, bool)`

GetIsPaidOk returns a tuple with the IsPaid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPaid

`func (o *ShopReceiptsResultsInner) SetIsPaid(v bool)`

SetIsPaid sets IsPaid field to given value.

### HasIsPaid

`func (o *ShopReceiptsResultsInner) HasIsPaid() bool`

HasIsPaid returns a boolean if a field has been set.

### GetIsShipped

`func (o *ShopReceiptsResultsInner) GetIsShipped() bool`

GetIsShipped returns the IsShipped field if non-nil, zero value otherwise.

### GetIsShippedOk

`func (o *ShopReceiptsResultsInner) GetIsShippedOk() (*bool, bool)`

GetIsShippedOk returns a tuple with the IsShipped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsShipped

`func (o *ShopReceiptsResultsInner) SetIsShipped(v bool)`

SetIsShipped sets IsShipped field to given value.

### HasIsShipped

`func (o *ShopReceiptsResultsInner) HasIsShipped() bool`

HasIsShipped returns a boolean if a field has been set.

### GetCreateTimestamp

`func (o *ShopReceiptsResultsInner) GetCreateTimestamp() int32`

GetCreateTimestamp returns the CreateTimestamp field if non-nil, zero value otherwise.

### GetCreateTimestampOk

`func (o *ShopReceiptsResultsInner) GetCreateTimestampOk() (*int32, bool)`

GetCreateTimestampOk returns a tuple with the CreateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreateTimestamp

`func (o *ShopReceiptsResultsInner) SetCreateTimestamp(v int32)`

SetCreateTimestamp sets CreateTimestamp field to given value.

### HasCreateTimestamp

`func (o *ShopReceiptsResultsInner) HasCreateTimestamp() bool`

HasCreateTimestamp returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *ShopReceiptsResultsInner) GetCreatedTimestamp() int32`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *ShopReceiptsResultsInner) GetCreatedTimestampOk() (*int32, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *ShopReceiptsResultsInner) SetCreatedTimestamp(v int32)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *ShopReceiptsResultsInner) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdateTimestamp

`func (o *ShopReceiptsResultsInner) GetUpdateTimestamp() int32`

GetUpdateTimestamp returns the UpdateTimestamp field if non-nil, zero value otherwise.

### GetUpdateTimestampOk

`func (o *ShopReceiptsResultsInner) GetUpdateTimestampOk() (*int32, bool)`

GetUpdateTimestampOk returns a tuple with the UpdateTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateTimestamp

`func (o *ShopReceiptsResultsInner) SetUpdateTimestamp(v int32)`

SetUpdateTimestamp sets UpdateTimestamp field to given value.

### HasUpdateTimestamp

`func (o *ShopReceiptsResultsInner) HasUpdateTimestamp() bool`

HasUpdateTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *ShopReceiptsResultsInner) GetUpdatedTimestamp() int32`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *ShopReceiptsResultsInner) GetUpdatedTimestampOk() (*int32, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *ShopReceiptsResultsInner) SetUpdatedTimestamp(v int32)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *ShopReceiptsResultsInner) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.

### GetIsGift

`func (o *ShopReceiptsResultsInner) GetIsGift() bool`

GetIsGift returns the IsGift field if non-nil, zero value otherwise.

### GetIsGiftOk

`func (o *ShopReceiptsResultsInner) GetIsGiftOk() (*bool, bool)`

GetIsGiftOk returns a tuple with the IsGift field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsGift

`func (o *ShopReceiptsResultsInner) SetIsGift(v bool)`

SetIsGift sets IsGift field to given value.

### HasIsGift

`func (o *ShopReceiptsResultsInner) HasIsGift() bool`

HasIsGift returns a boolean if a field has been set.

### GetGiftMessage

`func (o *ShopReceiptsResultsInner) GetGiftMessage() string`

GetGiftMessage returns the GiftMessage field if non-nil, zero value otherwise.

### GetGiftMessageOk

`func (o *ShopReceiptsResultsInner) GetGiftMessageOk() (*string, bool)`

GetGiftMessageOk returns a tuple with the GiftMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGiftMessage

`func (o *ShopReceiptsResultsInner) SetGiftMessage(v string)`

SetGiftMessage sets GiftMessage field to given value.

### HasGiftMessage

`func (o *ShopReceiptsResultsInner) HasGiftMessage() bool`

HasGiftMessage returns a boolean if a field has been set.

### GetGrandtotal

`func (o *ShopReceiptsResultsInner) GetGrandtotal() ShopReceiptGrandtotal`

GetGrandtotal returns the Grandtotal field if non-nil, zero value otherwise.

### GetGrandtotalOk

`func (o *ShopReceiptsResultsInner) GetGrandtotalOk() (*ShopReceiptGrandtotal, bool)`

GetGrandtotalOk returns a tuple with the Grandtotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrandtotal

`func (o *ShopReceiptsResultsInner) SetGrandtotal(v ShopReceiptGrandtotal)`

SetGrandtotal sets Grandtotal field to given value.

### HasGrandtotal

`func (o *ShopReceiptsResultsInner) HasGrandtotal() bool`

HasGrandtotal returns a boolean if a field has been set.

### GetSubtotal

`func (o *ShopReceiptsResultsInner) GetSubtotal() ShopReceiptSubtotal`

GetSubtotal returns the Subtotal field if non-nil, zero value otherwise.

### GetSubtotalOk

`func (o *ShopReceiptsResultsInner) GetSubtotalOk() (*ShopReceiptSubtotal, bool)`

GetSubtotalOk returns a tuple with the Subtotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubtotal

`func (o *ShopReceiptsResultsInner) SetSubtotal(v ShopReceiptSubtotal)`

SetSubtotal sets Subtotal field to given value.

### HasSubtotal

`func (o *ShopReceiptsResultsInner) HasSubtotal() bool`

HasSubtotal returns a boolean if a field has been set.

### GetTotalPrice

`func (o *ShopReceiptsResultsInner) GetTotalPrice() ShopReceiptTotalPrice`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *ShopReceiptsResultsInner) GetTotalPriceOk() (*ShopReceiptTotalPrice, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *ShopReceiptsResultsInner) SetTotalPrice(v ShopReceiptTotalPrice)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *ShopReceiptsResultsInner) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalShippingCost

`func (o *ShopReceiptsResultsInner) GetTotalShippingCost() ShopReceiptTotalShippingCost`

GetTotalShippingCost returns the TotalShippingCost field if non-nil, zero value otherwise.

### GetTotalShippingCostOk

`func (o *ShopReceiptsResultsInner) GetTotalShippingCostOk() (*ShopReceiptTotalShippingCost, bool)`

GetTotalShippingCostOk returns a tuple with the TotalShippingCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalShippingCost

`func (o *ShopReceiptsResultsInner) SetTotalShippingCost(v ShopReceiptTotalShippingCost)`

SetTotalShippingCost sets TotalShippingCost field to given value.

### HasTotalShippingCost

`func (o *ShopReceiptsResultsInner) HasTotalShippingCost() bool`

HasTotalShippingCost returns a boolean if a field has been set.

### GetTotalTaxCost

`func (o *ShopReceiptsResultsInner) GetTotalTaxCost() ShopReceiptTotalTaxCost`

GetTotalTaxCost returns the TotalTaxCost field if non-nil, zero value otherwise.

### GetTotalTaxCostOk

`func (o *ShopReceiptsResultsInner) GetTotalTaxCostOk() (*ShopReceiptTotalTaxCost, bool)`

GetTotalTaxCostOk returns a tuple with the TotalTaxCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalTaxCost

`func (o *ShopReceiptsResultsInner) SetTotalTaxCost(v ShopReceiptTotalTaxCost)`

SetTotalTaxCost sets TotalTaxCost field to given value.

### HasTotalTaxCost

`func (o *ShopReceiptsResultsInner) HasTotalTaxCost() bool`

HasTotalTaxCost returns a boolean if a field has been set.

### GetTotalVatCost

`func (o *ShopReceiptsResultsInner) GetTotalVatCost() ShopReceiptTotalVatCost`

GetTotalVatCost returns the TotalVatCost field if non-nil, zero value otherwise.

### GetTotalVatCostOk

`func (o *ShopReceiptsResultsInner) GetTotalVatCostOk() (*ShopReceiptTotalVatCost, bool)`

GetTotalVatCostOk returns a tuple with the TotalVatCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalVatCost

`func (o *ShopReceiptsResultsInner) SetTotalVatCost(v ShopReceiptTotalVatCost)`

SetTotalVatCost sets TotalVatCost field to given value.

### HasTotalVatCost

`func (o *ShopReceiptsResultsInner) HasTotalVatCost() bool`

HasTotalVatCost returns a boolean if a field has been set.

### GetDiscountAmt

`func (o *ShopReceiptsResultsInner) GetDiscountAmt() ShopReceiptDiscountAmt`

GetDiscountAmt returns the DiscountAmt field if non-nil, zero value otherwise.

### GetDiscountAmtOk

`func (o *ShopReceiptsResultsInner) GetDiscountAmtOk() (*ShopReceiptDiscountAmt, bool)`

GetDiscountAmtOk returns a tuple with the DiscountAmt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscountAmt

`func (o *ShopReceiptsResultsInner) SetDiscountAmt(v ShopReceiptDiscountAmt)`

SetDiscountAmt sets DiscountAmt field to given value.

### HasDiscountAmt

`func (o *ShopReceiptsResultsInner) HasDiscountAmt() bool`

HasDiscountAmt returns a boolean if a field has been set.

### GetGiftWrapPrice

`func (o *ShopReceiptsResultsInner) GetGiftWrapPrice() ShopReceiptGiftWrapPrice`

GetGiftWrapPrice returns the GiftWrapPrice field if non-nil, zero value otherwise.

### GetGiftWrapPriceOk

`func (o *ShopReceiptsResultsInner) GetGiftWrapPriceOk() (*ShopReceiptGiftWrapPrice, bool)`

GetGiftWrapPriceOk returns a tuple with the GiftWrapPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGiftWrapPrice

`func (o *ShopReceiptsResultsInner) SetGiftWrapPrice(v ShopReceiptGiftWrapPrice)`

SetGiftWrapPrice sets GiftWrapPrice field to given value.

### HasGiftWrapPrice

`func (o *ShopReceiptsResultsInner) HasGiftWrapPrice() bool`

HasGiftWrapPrice returns a boolean if a field has been set.

### GetShipments

`func (o *ShopReceiptsResultsInner) GetShipments() []ShopReceiptShipmentsInner`

GetShipments returns the Shipments field if non-nil, zero value otherwise.

### GetShipmentsOk

`func (o *ShopReceiptsResultsInner) GetShipmentsOk() (*[]ShopReceiptShipmentsInner, bool)`

GetShipmentsOk returns a tuple with the Shipments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipments

`func (o *ShopReceiptsResultsInner) SetShipments(v []ShopReceiptShipmentsInner)`

SetShipments sets Shipments field to given value.

### HasShipments

`func (o *ShopReceiptsResultsInner) HasShipments() bool`

HasShipments returns a boolean if a field has been set.

### GetTransactions

`func (o *ShopReceiptsResultsInner) GetTransactions() []ShopReceiptTransactionsInner`

GetTransactions returns the Transactions field if non-nil, zero value otherwise.

### GetTransactionsOk

`func (o *ShopReceiptsResultsInner) GetTransactionsOk() (*[]ShopReceiptTransactionsInner, bool)`

GetTransactionsOk returns a tuple with the Transactions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactions

`func (o *ShopReceiptsResultsInner) SetTransactions(v []ShopReceiptTransactionsInner)`

SetTransactions sets Transactions field to given value.

### HasTransactions

`func (o *ShopReceiptsResultsInner) HasTransactions() bool`

HasTransactions returns a boolean if a field has been set.

### GetRefunds

`func (o *ShopReceiptsResultsInner) GetRefunds() []ShopReceiptRefundsInner`

GetRefunds returns the Refunds field if non-nil, zero value otherwise.

### GetRefundsOk

`func (o *ShopReceiptsResultsInner) GetRefundsOk() (*[]ShopReceiptRefundsInner, bool)`

GetRefundsOk returns a tuple with the Refunds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefunds

`func (o *ShopReceiptsResultsInner) SetRefunds(v []ShopReceiptRefundsInner)`

SetRefunds sets Refunds field to given value.

### HasRefunds

`func (o *ShopReceiptsResultsInner) HasRefunds() bool`

HasRefunds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


