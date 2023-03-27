# ShopReceiptShipmentsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReceiptShippingId** | Pointer to **NullableInt32** | The unique numeric ID of a Shop Receipt Shipment record. | [optional] 
**ShipmentNotificationTimestamp** | Pointer to **int32** | The time at which Etsy notified the buyer of the shipment event, in epoch seconds. | [optional] 
**CarrierName** | Pointer to **string** | The name string for the carrier/company responsible for delivering the shipment. | [optional] 
**TrackingCode** | Pointer to **string** | The tracking code string provided by the carrier/company for the shipment. | [optional] 

## Methods

### NewShopReceiptShipmentsInner

`func NewShopReceiptShipmentsInner() *ShopReceiptShipmentsInner`

NewShopReceiptShipmentsInner instantiates a new ShopReceiptShipmentsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReceiptShipmentsInnerWithDefaults

`func NewShopReceiptShipmentsInnerWithDefaults() *ShopReceiptShipmentsInner`

NewShopReceiptShipmentsInnerWithDefaults instantiates a new ShopReceiptShipmentsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReceiptShippingId

`func (o *ShopReceiptShipmentsInner) GetReceiptShippingId() int32`

GetReceiptShippingId returns the ReceiptShippingId field if non-nil, zero value otherwise.

### GetReceiptShippingIdOk

`func (o *ShopReceiptShipmentsInner) GetReceiptShippingIdOk() (*int32, bool)`

GetReceiptShippingIdOk returns a tuple with the ReceiptShippingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptShippingId

`func (o *ShopReceiptShipmentsInner) SetReceiptShippingId(v int32)`

SetReceiptShippingId sets ReceiptShippingId field to given value.

### HasReceiptShippingId

`func (o *ShopReceiptShipmentsInner) HasReceiptShippingId() bool`

HasReceiptShippingId returns a boolean if a field has been set.

### SetReceiptShippingIdNil

`func (o *ShopReceiptShipmentsInner) SetReceiptShippingIdNil(b bool)`

 SetReceiptShippingIdNil sets the value for ReceiptShippingId to be an explicit nil

### UnsetReceiptShippingId
`func (o *ShopReceiptShipmentsInner) UnsetReceiptShippingId()`

UnsetReceiptShippingId ensures that no value is present for ReceiptShippingId, not even an explicit nil
### GetShipmentNotificationTimestamp

`func (o *ShopReceiptShipmentsInner) GetShipmentNotificationTimestamp() int32`

GetShipmentNotificationTimestamp returns the ShipmentNotificationTimestamp field if non-nil, zero value otherwise.

### GetShipmentNotificationTimestampOk

`func (o *ShopReceiptShipmentsInner) GetShipmentNotificationTimestampOk() (*int32, bool)`

GetShipmentNotificationTimestampOk returns a tuple with the ShipmentNotificationTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShipmentNotificationTimestamp

`func (o *ShopReceiptShipmentsInner) SetShipmentNotificationTimestamp(v int32)`

SetShipmentNotificationTimestamp sets ShipmentNotificationTimestamp field to given value.

### HasShipmentNotificationTimestamp

`func (o *ShopReceiptShipmentsInner) HasShipmentNotificationTimestamp() bool`

HasShipmentNotificationTimestamp returns a boolean if a field has been set.

### GetCarrierName

`func (o *ShopReceiptShipmentsInner) GetCarrierName() string`

GetCarrierName returns the CarrierName field if non-nil, zero value otherwise.

### GetCarrierNameOk

`func (o *ShopReceiptShipmentsInner) GetCarrierNameOk() (*string, bool)`

GetCarrierNameOk returns a tuple with the CarrierName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCarrierName

`func (o *ShopReceiptShipmentsInner) SetCarrierName(v string)`

SetCarrierName sets CarrierName field to given value.

### HasCarrierName

`func (o *ShopReceiptShipmentsInner) HasCarrierName() bool`

HasCarrierName returns a boolean if a field has been set.

### GetTrackingCode

`func (o *ShopReceiptShipmentsInner) GetTrackingCode() string`

GetTrackingCode returns the TrackingCode field if non-nil, zero value otherwise.

### GetTrackingCodeOk

`func (o *ShopReceiptShipmentsInner) GetTrackingCodeOk() (*string, bool)`

GetTrackingCodeOk returns a tuple with the TrackingCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrackingCode

`func (o *ShopReceiptShipmentsInner) SetTrackingCode(v string)`

SetTrackingCode sets TrackingCode field to given value.

### HasTrackingCode

`func (o *ShopReceiptShipmentsInner) HasTrackingCode() bool`

HasTrackingCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


