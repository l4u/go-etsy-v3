# SellerTaxonomyNodesResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** | The unique numeric ID of an Etsy taxonomy node, which is a metadata category for listings organized into the seller taxonomy hierarchy tree. For example, the \\\&quot;shoes\\\&quot; taxonomy node (ID: 1429, level: 1) is higher in the hierarchy than \\\&quot;girls&#39; shoes\\\&quot; (ID: 1440, level: 2). The taxonomy nodes assigned to a listing support access to specific standardized product scales and properties. For example, listings assigned the taxonomy nodes \\\&quot;shoes\\\&quot; or \\\&quot;girls&#39; shoes\\\&quot; support access to the \\\&quot;EU\\\&quot; shoe size scale with its associated property names and IDs for EU shoe sizes, such as property &#x60;value_id&#x60;:\\\&quot;1394\\\&quot;, and &#x60;name&#x60;:\\\&quot;38\\\&quot;. | [optional] 
**Level** | Pointer to **int32** | The integer depth of this taxonomy node in the seller taxonomy tree, with roots at level 0. | [optional] 
**Name** | Pointer to **string** | The name string for this taxonomy node. | [optional] 
**ParentId** | Pointer to **NullableInt32** | The numeric taxonomy ID of the parent of this node. | [optional] 
**Children** | Pointer to [**[]SellerTaxonomyNodeChildrenInner**](SellerTaxonomyNodeChildrenInner.md) | An array of taxonomy nodes for all the direct children of this taxonomy node in the seller taxonomy tree. | [optional] 
**FullPathTaxonomyIds** | Pointer to **[]int32** | An array of &#x60;taxonomy_id&#x60;s including this node and all of its direct parents in the seller taxonomy tree up to a root node. They are listed in order from root to leaf. | [optional] 

## Methods

### NewSellerTaxonomyNodesResultsInner

`func NewSellerTaxonomyNodesResultsInner() *SellerTaxonomyNodesResultsInner`

NewSellerTaxonomyNodesResultsInner instantiates a new SellerTaxonomyNodesResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSellerTaxonomyNodesResultsInnerWithDefaults

`func NewSellerTaxonomyNodesResultsInnerWithDefaults() *SellerTaxonomyNodesResultsInner`

NewSellerTaxonomyNodesResultsInnerWithDefaults instantiates a new SellerTaxonomyNodesResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SellerTaxonomyNodesResultsInner) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SellerTaxonomyNodesResultsInner) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SellerTaxonomyNodesResultsInner) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *SellerTaxonomyNodesResultsInner) HasId() bool`

HasId returns a boolean if a field has been set.

### GetLevel

`func (o *SellerTaxonomyNodesResultsInner) GetLevel() int32`

GetLevel returns the Level field if non-nil, zero value otherwise.

### GetLevelOk

`func (o *SellerTaxonomyNodesResultsInner) GetLevelOk() (*int32, bool)`

GetLevelOk returns a tuple with the Level field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLevel

`func (o *SellerTaxonomyNodesResultsInner) SetLevel(v int32)`

SetLevel sets Level field to given value.

### HasLevel

`func (o *SellerTaxonomyNodesResultsInner) HasLevel() bool`

HasLevel returns a boolean if a field has been set.

### GetName

`func (o *SellerTaxonomyNodesResultsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SellerTaxonomyNodesResultsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SellerTaxonomyNodesResultsInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *SellerTaxonomyNodesResultsInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetParentId

`func (o *SellerTaxonomyNodesResultsInner) GetParentId() int32`

GetParentId returns the ParentId field if non-nil, zero value otherwise.

### GetParentIdOk

`func (o *SellerTaxonomyNodesResultsInner) GetParentIdOk() (*int32, bool)`

GetParentIdOk returns a tuple with the ParentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentId

`func (o *SellerTaxonomyNodesResultsInner) SetParentId(v int32)`

SetParentId sets ParentId field to given value.

### HasParentId

`func (o *SellerTaxonomyNodesResultsInner) HasParentId() bool`

HasParentId returns a boolean if a field has been set.

### SetParentIdNil

`func (o *SellerTaxonomyNodesResultsInner) SetParentIdNil(b bool)`

 SetParentIdNil sets the value for ParentId to be an explicit nil

### UnsetParentId
`func (o *SellerTaxonomyNodesResultsInner) UnsetParentId()`

UnsetParentId ensures that no value is present for ParentId, not even an explicit nil
### GetChildren

`func (o *SellerTaxonomyNodesResultsInner) GetChildren() []SellerTaxonomyNodeChildrenInner`

GetChildren returns the Children field if non-nil, zero value otherwise.

### GetChildrenOk

`func (o *SellerTaxonomyNodesResultsInner) GetChildrenOk() (*[]SellerTaxonomyNodeChildrenInner, bool)`

GetChildrenOk returns a tuple with the Children field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChildren

`func (o *SellerTaxonomyNodesResultsInner) SetChildren(v []SellerTaxonomyNodeChildrenInner)`

SetChildren sets Children field to given value.

### HasChildren

`func (o *SellerTaxonomyNodesResultsInner) HasChildren() bool`

HasChildren returns a boolean if a field has been set.

### GetFullPathTaxonomyIds

`func (o *SellerTaxonomyNodesResultsInner) GetFullPathTaxonomyIds() []int32`

GetFullPathTaxonomyIds returns the FullPathTaxonomyIds field if non-nil, zero value otherwise.

### GetFullPathTaxonomyIdsOk

`func (o *SellerTaxonomyNodesResultsInner) GetFullPathTaxonomyIdsOk() (*[]int32, bool)`

GetFullPathTaxonomyIdsOk returns a tuple with the FullPathTaxonomyIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullPathTaxonomyIds

`func (o *SellerTaxonomyNodesResultsInner) SetFullPathTaxonomyIds(v []int32)`

SetFullPathTaxonomyIds sets FullPathTaxonomyIds field to given value.

### HasFullPathTaxonomyIds

`func (o *SellerTaxonomyNodesResultsInner) HasFullPathTaxonomyIds() bool`

HasFullPathTaxonomyIds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


