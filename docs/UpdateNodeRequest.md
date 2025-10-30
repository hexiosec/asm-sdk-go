# UpdateNodeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RemoveFromScope** | Pointer to **bool** | Deprecated - remove the node from scope, if it is in scope. Or undo this action, if it has been previously removed from scope - Use **mark_as_secondary** | [optional] 
**MarkAsSecondary** | Pointer to **bool** | Mark node as secondary asset if the node is a primary asset. Or undo this action, if it has been previously marked as secondary. | [optional] 
**IgnoreIps** | Pointer to **bool** | Ignore IPs for the node | [optional] 

## Methods

### NewUpdateNodeRequest

`func NewUpdateNodeRequest() *UpdateNodeRequest`

NewUpdateNodeRequest instantiates a new UpdateNodeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateNodeRequestWithDefaults

`func NewUpdateNodeRequestWithDefaults() *UpdateNodeRequest`

NewUpdateNodeRequestWithDefaults instantiates a new UpdateNodeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRemoveFromScope

`func (o *UpdateNodeRequest) GetRemoveFromScope() bool`

GetRemoveFromScope returns the RemoveFromScope field if non-nil, zero value otherwise.

### GetRemoveFromScopeOk

`func (o *UpdateNodeRequest) GetRemoveFromScopeOk() (*bool, bool)`

GetRemoveFromScopeOk returns a tuple with the RemoveFromScope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoveFromScope

`func (o *UpdateNodeRequest) SetRemoveFromScope(v bool)`

SetRemoveFromScope sets RemoveFromScope field to given value.

### HasRemoveFromScope

`func (o *UpdateNodeRequest) HasRemoveFromScope() bool`

HasRemoveFromScope returns a boolean if a field has been set.

### GetMarkAsSecondary

`func (o *UpdateNodeRequest) GetMarkAsSecondary() bool`

GetMarkAsSecondary returns the MarkAsSecondary field if non-nil, zero value otherwise.

### GetMarkAsSecondaryOk

`func (o *UpdateNodeRequest) GetMarkAsSecondaryOk() (*bool, bool)`

GetMarkAsSecondaryOk returns a tuple with the MarkAsSecondary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarkAsSecondary

`func (o *UpdateNodeRequest) SetMarkAsSecondary(v bool)`

SetMarkAsSecondary sets MarkAsSecondary field to given value.

### HasMarkAsSecondary

`func (o *UpdateNodeRequest) HasMarkAsSecondary() bool`

HasMarkAsSecondary returns a boolean if a field has been set.

### GetIgnoreIps

`func (o *UpdateNodeRequest) GetIgnoreIps() bool`

GetIgnoreIps returns the IgnoreIps field if non-nil, zero value otherwise.

### GetIgnoreIpsOk

`func (o *UpdateNodeRequest) GetIgnoreIpsOk() (*bool, bool)`

GetIgnoreIpsOk returns a tuple with the IgnoreIps field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnoreIps

`func (o *UpdateNodeRequest) SetIgnoreIps(v bool)`

SetIgnoreIps sets IgnoreIps field to given value.

### HasIgnoreIps

`func (o *UpdateNodeRequest) HasIgnoreIps() bool`

HasIgnoreIps returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


