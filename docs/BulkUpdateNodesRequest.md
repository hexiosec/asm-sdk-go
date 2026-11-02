# BulkUpdateNodesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NodeIds** | **[]string** |  | 
**MarkAsSecondary** | Pointer to **bool** | Mark nodes as secondary assets if they are primary assets. Or undo this action if they have previously been marked as secondary. | [optional] 
**AddTags** | Pointer to **[]string** | Tag IDs to add to each node in this request. | [optional] 
**RemoveTags** | Pointer to **[]string** | Tag IDs to remove from each node in this request. | [optional] 

## Methods

### NewBulkUpdateNodesRequest

`func NewBulkUpdateNodesRequest(nodeIds []string, ) *BulkUpdateNodesRequest`

NewBulkUpdateNodesRequest instantiates a new BulkUpdateNodesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBulkUpdateNodesRequestWithDefaults

`func NewBulkUpdateNodesRequestWithDefaults() *BulkUpdateNodesRequest`

NewBulkUpdateNodesRequestWithDefaults instantiates a new BulkUpdateNodesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNodeIds

`func (o *BulkUpdateNodesRequest) GetNodeIds() []string`

GetNodeIds returns the NodeIds field if non-nil, zero value otherwise.

### GetNodeIdsOk

`func (o *BulkUpdateNodesRequest) GetNodeIdsOk() (*[]string, bool)`

GetNodeIdsOk returns a tuple with the NodeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeIds

`func (o *BulkUpdateNodesRequest) SetNodeIds(v []string)`

SetNodeIds sets NodeIds field to given value.


### GetMarkAsSecondary

`func (o *BulkUpdateNodesRequest) GetMarkAsSecondary() bool`

GetMarkAsSecondary returns the MarkAsSecondary field if non-nil, zero value otherwise.

### GetMarkAsSecondaryOk

`func (o *BulkUpdateNodesRequest) GetMarkAsSecondaryOk() (*bool, bool)`

GetMarkAsSecondaryOk returns a tuple with the MarkAsSecondary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarkAsSecondary

`func (o *BulkUpdateNodesRequest) SetMarkAsSecondary(v bool)`

SetMarkAsSecondary sets MarkAsSecondary field to given value.

### HasMarkAsSecondary

`func (o *BulkUpdateNodesRequest) HasMarkAsSecondary() bool`

HasMarkAsSecondary returns a boolean if a field has been set.

### GetAddTags

`func (o *BulkUpdateNodesRequest) GetAddTags() []string`

GetAddTags returns the AddTags field if non-nil, zero value otherwise.

### GetAddTagsOk

`func (o *BulkUpdateNodesRequest) GetAddTagsOk() (*[]string, bool)`

GetAddTagsOk returns a tuple with the AddTags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddTags

`func (o *BulkUpdateNodesRequest) SetAddTags(v []string)`

SetAddTags sets AddTags field to given value.

### HasAddTags

`func (o *BulkUpdateNodesRequest) HasAddTags() bool`

HasAddTags returns a boolean if a field has been set.

### GetRemoveTags

`func (o *BulkUpdateNodesRequest) GetRemoveTags() []string`

GetRemoveTags returns the RemoveTags field if non-nil, zero value otherwise.

### GetRemoveTagsOk

`func (o *BulkUpdateNodesRequest) GetRemoveTagsOk() (*[]string, bool)`

GetRemoveTagsOk returns a tuple with the RemoveTags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoveTags

`func (o *BulkUpdateNodesRequest) SetRemoveTags(v []string)`

SetRemoveTags sets RemoveTags field to given value.

### HasRemoveTags

`func (o *BulkUpdateNodesRequest) HasRemoveTags() bool`

HasRemoveTags returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


