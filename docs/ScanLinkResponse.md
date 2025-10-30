# ScanLinkResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Link ID | 
**FromId** | **string** | From Node ID | 
**ToId** | **string** | To Node ID | 
**ScanId** | **string** | Scan ID | 
**Label** | **string** | Link label | 
**Hash** | **string** | Hash of metadata | 
**Created** | **time.Time** | Timestamp at which the link was created | 
**Updated** | **time.Time** | Timestamp at which the link was last updated | 
**LastSeen** | **time.Time** | Timestamp at which the link was last seen in an iteration | 
**ValidFrom** | **time.Time** | Timestamp at which the link is valid from | 
**ValidTo** | **time.Time** | Timestamp at which the link is valid to. When valid to &lt; valid from the link is considered open. | 
**Metadata** | **map[string]interface{}** | Link metadata | 
**Deleted** | **bool** | Link is deleted | 

## Methods

### NewScanLinkResponse

`func NewScanLinkResponse(id string, fromId string, toId string, scanId string, label string, hash string, created time.Time, updated time.Time, lastSeen time.Time, validFrom time.Time, validTo time.Time, metadata map[string]interface{}, deleted bool, ) *ScanLinkResponse`

NewScanLinkResponse instantiates a new ScanLinkResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanLinkResponseWithDefaults

`func NewScanLinkResponseWithDefaults() *ScanLinkResponse`

NewScanLinkResponseWithDefaults instantiates a new ScanLinkResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanLinkResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanLinkResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanLinkResponse) SetId(v string)`

SetId sets Id field to given value.


### GetFromId

`func (o *ScanLinkResponse) GetFromId() string`

GetFromId returns the FromId field if non-nil, zero value otherwise.

### GetFromIdOk

`func (o *ScanLinkResponse) GetFromIdOk() (*string, bool)`

GetFromIdOk returns a tuple with the FromId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromId

`func (o *ScanLinkResponse) SetFromId(v string)`

SetFromId sets FromId field to given value.


### GetToId

`func (o *ScanLinkResponse) GetToId() string`

GetToId returns the ToId field if non-nil, zero value otherwise.

### GetToIdOk

`func (o *ScanLinkResponse) GetToIdOk() (*string, bool)`

GetToIdOk returns a tuple with the ToId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToId

`func (o *ScanLinkResponse) SetToId(v string)`

SetToId sets ToId field to given value.


### GetScanId

`func (o *ScanLinkResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ScanLinkResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ScanLinkResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetLabel

`func (o *ScanLinkResponse) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *ScanLinkResponse) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *ScanLinkResponse) SetLabel(v string)`

SetLabel sets Label field to given value.


### GetHash

`func (o *ScanLinkResponse) GetHash() string`

GetHash returns the Hash field if non-nil, zero value otherwise.

### GetHashOk

`func (o *ScanLinkResponse) GetHashOk() (*string, bool)`

GetHashOk returns a tuple with the Hash field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHash

`func (o *ScanLinkResponse) SetHash(v string)`

SetHash sets Hash field to given value.


### GetCreated

`func (o *ScanLinkResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanLinkResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanLinkResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *ScanLinkResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ScanLinkResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ScanLinkResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetLastSeen

`func (o *ScanLinkResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanLinkResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanLinkResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.


### GetValidFrom

`func (o *ScanLinkResponse) GetValidFrom() time.Time`

GetValidFrom returns the ValidFrom field if non-nil, zero value otherwise.

### GetValidFromOk

`func (o *ScanLinkResponse) GetValidFromOk() (*time.Time, bool)`

GetValidFromOk returns a tuple with the ValidFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidFrom

`func (o *ScanLinkResponse) SetValidFrom(v time.Time)`

SetValidFrom sets ValidFrom field to given value.


### GetValidTo

`func (o *ScanLinkResponse) GetValidTo() time.Time`

GetValidTo returns the ValidTo field if non-nil, zero value otherwise.

### GetValidToOk

`func (o *ScanLinkResponse) GetValidToOk() (*time.Time, bool)`

GetValidToOk returns a tuple with the ValidTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidTo

`func (o *ScanLinkResponse) SetValidTo(v time.Time)`

SetValidTo sets ValidTo field to given value.


### GetMetadata

`func (o *ScanLinkResponse) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *ScanLinkResponse) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *ScanLinkResponse) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.


### GetDeleted

`func (o *ScanLinkResponse) GetDeleted() bool`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *ScanLinkResponse) GetDeletedOk() (*bool, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *ScanLinkResponse) SetDeleted(v bool)`

SetDeleted sets Deleted field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


