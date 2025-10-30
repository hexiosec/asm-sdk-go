# GenericGraphNode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ScanId** | **string** |  | 
**Label** | **string** |  | 
**Name** | **string** |  | 
**Created** | **time.Time** |  | 
**Updated** | **time.Time** |  | 
**LastSeen** | **time.Time** |  | 

## Methods

### NewGenericGraphNode

`func NewGenericGraphNode(id string, scanId string, label string, name string, created time.Time, updated time.Time, lastSeen time.Time, ) *GenericGraphNode`

NewGenericGraphNode instantiates a new GenericGraphNode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGenericGraphNodeWithDefaults

`func NewGenericGraphNodeWithDefaults() *GenericGraphNode`

NewGenericGraphNodeWithDefaults instantiates a new GenericGraphNode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *GenericGraphNode) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GenericGraphNode) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GenericGraphNode) SetId(v string)`

SetId sets Id field to given value.


### GetScanId

`func (o *GenericGraphNode) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *GenericGraphNode) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *GenericGraphNode) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetLabel

`func (o *GenericGraphNode) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *GenericGraphNode) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *GenericGraphNode) SetLabel(v string)`

SetLabel sets Label field to given value.


### GetName

`func (o *GenericGraphNode) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GenericGraphNode) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GenericGraphNode) SetName(v string)`

SetName sets Name field to given value.


### GetCreated

`func (o *GenericGraphNode) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *GenericGraphNode) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *GenericGraphNode) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *GenericGraphNode) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *GenericGraphNode) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *GenericGraphNode) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetLastSeen

`func (o *GenericGraphNode) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *GenericGraphNode) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *GenericGraphNode) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


