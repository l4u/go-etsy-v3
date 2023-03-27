# ShopReturnPoliciesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnPolicyId** | Pointer to **int32** | The numeric ID of the [Return Policy](/documentation/reference#operation/getShopReturnPolicies). | [optional] 
**ShopId** | Pointer to **int32** | The unique positive non-zero numeric ID for an Etsy Shop. | [optional] 
**AcceptsReturns** | Pointer to **bool** | return_policy_accepts_returns | [optional] 
**AcceptsExchanges** | Pointer to **bool** | return_policy_accepts_exchanges | [optional] 
**ReturnDeadline** | Pointer to **NullableInt32** | The deadline for the Return Policy, measured in days. The value must be one of the following: [7, 14, 21, 30, 45, 60, 90]. | [optional] 

## Methods

### NewShopReturnPoliciesResultsInner

`func NewShopReturnPoliciesResultsInner() *ShopReturnPoliciesResultsInner`

NewShopReturnPoliciesResultsInner instantiates a new ShopReturnPoliciesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShopReturnPoliciesResultsInnerWithDefaults

`func NewShopReturnPoliciesResultsInnerWithDefaults() *ShopReturnPoliciesResultsInner`

NewShopReturnPoliciesResultsInnerWithDefaults instantiates a new ShopReturnPoliciesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReturnPolicyId

`func (o *ShopReturnPoliciesResultsInner) GetReturnPolicyId() int32`

GetReturnPolicyId returns the ReturnPolicyId field if non-nil, zero value otherwise.

### GetReturnPolicyIdOk

`func (o *ShopReturnPoliciesResultsInner) GetReturnPolicyIdOk() (*int32, bool)`

GetReturnPolicyIdOk returns a tuple with the ReturnPolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnPolicyId

`func (o *ShopReturnPoliciesResultsInner) SetReturnPolicyId(v int32)`

SetReturnPolicyId sets ReturnPolicyId field to given value.

### HasReturnPolicyId

`func (o *ShopReturnPoliciesResultsInner) HasReturnPolicyId() bool`

HasReturnPolicyId returns a boolean if a field has been set.

### GetShopId

`func (o *ShopReturnPoliciesResultsInner) GetShopId() int32`

GetShopId returns the ShopId field if non-nil, zero value otherwise.

### GetShopIdOk

`func (o *ShopReturnPoliciesResultsInner) GetShopIdOk() (*int32, bool)`

GetShopIdOk returns a tuple with the ShopId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShopId

`func (o *ShopReturnPoliciesResultsInner) SetShopId(v int32)`

SetShopId sets ShopId field to given value.

### HasShopId

`func (o *ShopReturnPoliciesResultsInner) HasShopId() bool`

HasShopId returns a boolean if a field has been set.

### GetAcceptsReturns

`func (o *ShopReturnPoliciesResultsInner) GetAcceptsReturns() bool`

GetAcceptsReturns returns the AcceptsReturns field if non-nil, zero value otherwise.

### GetAcceptsReturnsOk

`func (o *ShopReturnPoliciesResultsInner) GetAcceptsReturnsOk() (*bool, bool)`

GetAcceptsReturnsOk returns a tuple with the AcceptsReturns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAcceptsReturns

`func (o *ShopReturnPoliciesResultsInner) SetAcceptsReturns(v bool)`

SetAcceptsReturns sets AcceptsReturns field to given value.

### HasAcceptsReturns

`func (o *ShopReturnPoliciesResultsInner) HasAcceptsReturns() bool`

HasAcceptsReturns returns a boolean if a field has been set.

### GetAcceptsExchanges

`func (o *ShopReturnPoliciesResultsInner) GetAcceptsExchanges() bool`

GetAcceptsExchanges returns the AcceptsExchanges field if non-nil, zero value otherwise.

### GetAcceptsExchangesOk

`func (o *ShopReturnPoliciesResultsInner) GetAcceptsExchangesOk() (*bool, bool)`

GetAcceptsExchangesOk returns a tuple with the AcceptsExchanges field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAcceptsExchanges

`func (o *ShopReturnPoliciesResultsInner) SetAcceptsExchanges(v bool)`

SetAcceptsExchanges sets AcceptsExchanges field to given value.

### HasAcceptsExchanges

`func (o *ShopReturnPoliciesResultsInner) HasAcceptsExchanges() bool`

HasAcceptsExchanges returns a boolean if a field has been set.

### GetReturnDeadline

`func (o *ShopReturnPoliciesResultsInner) GetReturnDeadline() int32`

GetReturnDeadline returns the ReturnDeadline field if non-nil, zero value otherwise.

### GetReturnDeadlineOk

`func (o *ShopReturnPoliciesResultsInner) GetReturnDeadlineOk() (*int32, bool)`

GetReturnDeadlineOk returns a tuple with the ReturnDeadline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnDeadline

`func (o *ShopReturnPoliciesResultsInner) SetReturnDeadline(v int32)`

SetReturnDeadline sets ReturnDeadline field to given value.

### HasReturnDeadline

`func (o *ShopReturnPoliciesResultsInner) HasReturnDeadline() bool`

HasReturnDeadline returns a boolean if a field has been set.

### SetReturnDeadlineNil

`func (o *ShopReturnPoliciesResultsInner) SetReturnDeadlineNil(b bool)`

 SetReturnDeadlineNil sets the value for ReturnDeadline to be an explicit nil

### UnsetReturnDeadline
`func (o *ShopReturnPoliciesResultsInner) UnsetReturnDeadline()`

UnsetReturnDeadline ensures that no value is present for ReturnDeadline, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


