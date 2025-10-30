# NodeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ScanId** | **string** |  | 
**Label** | **string** |  | 
**Deleted** | **bool** |  | 
**Hash** | **string** |  | 
**Metadata** | **map[string]interface{}** |  | 
**Created** | **time.Time** |  | 
**Updated** | **time.Time** |  | 
**LastSeen** | **time.Time** |  | 

## Methods

### NewNodeResponse

`func NewNodeResponse(id string, scanId string, label string, deleted bool, hash string, metadata map[string]interface{}, created time.Time, updated time.Time, lastSeen time.Time, ) *NodeResponse`

NewNodeResponse instantiates a new NodeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNodeResponseWithDefaults

`func NewNodeResponseWithDefaults() *NodeResponse`

NewNodeResponseWithDefaults instantiates a new NodeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *NodeResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *NodeResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *NodeResponse) SetId(v string)`

SetId sets Id field to given value.


### GetScanId

`func (o *NodeResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *NodeResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *NodeResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetLabel

`func (o *NodeResponse) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *NodeResponse) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *NodeResponse) SetLabel(v string)`

SetLabel sets Label field to given value.


### GetDeleted

`func (o *NodeResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *NodeResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *NodeResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.


### GetHash

`func (o *NodeResponse) GetHash() string`

GetHash returns the Hash field if non-nil, zero value otherwise.

### GetHashOk

`func (o *NodeResponse) GetHashOk() (*string, bool)`

GetHashOk returns a tuple with the Hash field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHash

`func (o *NodeResponse) SetHash(v string)`

SetHash sets Hash field to given value.


### GetMetadata

`func (o *NodeResponse) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *NodeResponse) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *NodeResponse) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.


### GetCreated

`func (o *NodeResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *NodeResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *NodeResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *NodeResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *NodeResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *NodeResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetLastSeen

`func (o *NodeResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *NodeResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *NodeResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


