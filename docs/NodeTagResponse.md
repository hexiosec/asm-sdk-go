# NodeTagResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NodeId** | **string** | Node ID | 
**TagId** | **string** | Tag ID | 
**Deleted** | **bool** | Whether the node tag has been soft deleted | 
**CreatedAt** | **time.Time** | Timestamp at which the tag was added to the node | 
**CreatedBy** | **string** | User ID of the creator | 
**UpdatedAt** | **time.Time** | Timestamp at which the node tag was last updated | 
**UpdatedBy** | **string** | User ID of the last updater | 
**TagName** | Pointer to **string** | Tag Name | [optional] 
**Colour** | Pointer to **string** | Optional tag colour as a hex value | [optional] 

## Methods

### NewNodeTagResponse

`func NewNodeTagResponse(nodeId string, tagId string, deleted bool, createdAt time.Time, createdBy string, updatedAt time.Time, updatedBy string, ) *NodeTagResponse`

NewNodeTagResponse instantiates a new NodeTagResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNodeTagResponseWithDefaults

`func NewNodeTagResponseWithDefaults() *NodeTagResponse`

NewNodeTagResponseWithDefaults instantiates a new NodeTagResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNodeId

`func (o *NodeTagResponse) GetNodeId() string`

GetNodeId returns the NodeId field if non-nil, zero value otherwise.

### GetNodeIdOk

`func (o *NodeTagResponse) GetNodeIdOk() (*string, bool)`

GetNodeIdOk returns a tuple with the NodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeId

`func (o *NodeTagResponse) SetNodeId(v string)`

SetNodeId sets NodeId field to given value.


### GetTagId

`func (o *NodeTagResponse) GetTagId() string`

GetTagId returns the TagId field if non-nil, zero value otherwise.

### GetTagIdOk

`func (o *NodeTagResponse) GetTagIdOk() (*string, bool)`

GetTagIdOk returns a tuple with the TagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagId

`func (o *NodeTagResponse) SetTagId(v string)`

SetTagId sets TagId field to given value.


### GetDeleted

`func (o *NodeTagResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *NodeTagResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *NodeTagResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.


### GetCreatedAt

`func (o *NodeTagResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *NodeTagResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *NodeTagResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetCreatedBy

`func (o *NodeTagResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *NodeTagResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *NodeTagResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetUpdatedAt

`func (o *NodeTagResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *NodeTagResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *NodeTagResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetUpdatedBy

`func (o *NodeTagResponse) GetUpdatedBy() string`

GetUpdatedBy returns the UpdatedBy field if non-nil, zero value otherwise.

### GetUpdatedByOk

`func (o *NodeTagResponse) GetUpdatedByOk() (*string, bool)`

GetUpdatedByOk returns a tuple with the UpdatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedBy

`func (o *NodeTagResponse) SetUpdatedBy(v string)`

SetUpdatedBy sets UpdatedBy field to given value.


### GetTagName

`func (o *NodeTagResponse) GetTagName() string`

GetTagName returns the TagName field if non-nil, zero value otherwise.

### GetTagNameOk

`func (o *NodeTagResponse) GetTagNameOk() (*string, bool)`

GetTagNameOk returns a tuple with the TagName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagName

`func (o *NodeTagResponse) SetTagName(v string)`

SetTagName sets TagName field to given value.

### HasTagName

`func (o *NodeTagResponse) HasTagName() bool`

HasTagName returns a boolean if a field has been set.

### GetColour

`func (o *NodeTagResponse) GetColour() string`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *NodeTagResponse) GetColourOk() (*string, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *NodeTagResponse) SetColour(v string)`

SetColour sets Colour field to given value.

### HasColour

`func (o *NodeTagResponse) HasColour() bool`

HasColour returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


