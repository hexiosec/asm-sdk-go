# DomainGraphNode

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
**Ignored** | **bool** |  | 
**IpsIgnored** | **bool** |  | 

## Methods

### NewDomainGraphNode

`func NewDomainGraphNode(id string, scanId string, label string, name string, created time.Time, updated time.Time, lastSeen time.Time, ignored bool, ipsIgnored bool, ) *DomainGraphNode`

NewDomainGraphNode instantiates a new DomainGraphNode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDomainGraphNodeWithDefaults

`func NewDomainGraphNodeWithDefaults() *DomainGraphNode`

NewDomainGraphNodeWithDefaults instantiates a new DomainGraphNode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *DomainGraphNode) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DomainGraphNode) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DomainGraphNode) SetId(v string)`

SetId sets Id field to given value.


### GetScanId

`func (o *DomainGraphNode) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *DomainGraphNode) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *DomainGraphNode) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetLabel

`func (o *DomainGraphNode) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *DomainGraphNode) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *DomainGraphNode) SetLabel(v string)`

SetLabel sets Label field to given value.


### GetName

`func (o *DomainGraphNode) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DomainGraphNode) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DomainGraphNode) SetName(v string)`

SetName sets Name field to given value.


### GetCreated

`func (o *DomainGraphNode) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *DomainGraphNode) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *DomainGraphNode) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *DomainGraphNode) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *DomainGraphNode) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *DomainGraphNode) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetLastSeen

`func (o *DomainGraphNode) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *DomainGraphNode) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *DomainGraphNode) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.


### GetIgnored

`func (o *DomainGraphNode) GetIgnored() bool`

GetIgnored returns the Ignored field if non-nil, zero value otherwise.

### GetIgnoredOk

`func (o *DomainGraphNode) GetIgnoredOk() (*bool, bool)`

GetIgnoredOk returns a tuple with the Ignored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnored

`func (o *DomainGraphNode) SetIgnored(v bool)`

SetIgnored sets Ignored field to given value.


### GetIpsIgnored

`func (o *DomainGraphNode) GetIpsIgnored() bool`

GetIpsIgnored returns the IpsIgnored field if non-nil, zero value otherwise.

### GetIpsIgnoredOk

`func (o *DomainGraphNode) GetIpsIgnoredOk() (*bool, bool)`

GetIpsIgnoredOk returns a tuple with the IpsIgnored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpsIgnored

`func (o *DomainGraphNode) SetIpsIgnored(v bool)`

SetIpsIgnored sets IpsIgnored field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


