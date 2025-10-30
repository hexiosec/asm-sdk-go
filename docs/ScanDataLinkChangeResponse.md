# ScanDataLinkChangeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Link ID | 
**LinkType** | **string** | Type of the link | 
**AddedIn** | **string** | Iteration ID link was added in | 
**RemovedIn** | Pointer to **string** | Iteration ID link was removed in | [optional] 
**From** | [**ScanDataLinkChangeResponseFrom**](ScanDataLinkChangeResponseFrom.md) |  | 
**To** | [**ScanDataLinkChangeResponseTo**](ScanDataLinkChangeResponseTo.md) |  | 
**RiskSeverity** | Pointer to **string** | Set if the link type is RISK | [optional] 
**RiskSeverityNumber** | Pointer to **int32** |  | [optional] 

## Methods

### NewScanDataLinkChangeResponse

`func NewScanDataLinkChangeResponse(id string, linkType string, addedIn string, from ScanDataLinkChangeResponseFrom, to ScanDataLinkChangeResponseTo, ) *ScanDataLinkChangeResponse`

NewScanDataLinkChangeResponse instantiates a new ScanDataLinkChangeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataLinkChangeResponseWithDefaults

`func NewScanDataLinkChangeResponseWithDefaults() *ScanDataLinkChangeResponse`

NewScanDataLinkChangeResponseWithDefaults instantiates a new ScanDataLinkChangeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataLinkChangeResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataLinkChangeResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataLinkChangeResponse) SetId(v string)`

SetId sets Id field to given value.


### GetLinkType

`func (o *ScanDataLinkChangeResponse) GetLinkType() string`

GetLinkType returns the LinkType field if non-nil, zero value otherwise.

### GetLinkTypeOk

`func (o *ScanDataLinkChangeResponse) GetLinkTypeOk() (*string, bool)`

GetLinkTypeOk returns a tuple with the LinkType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinkType

`func (o *ScanDataLinkChangeResponse) SetLinkType(v string)`

SetLinkType sets LinkType field to given value.


### GetAddedIn

`func (o *ScanDataLinkChangeResponse) GetAddedIn() string`

GetAddedIn returns the AddedIn field if non-nil, zero value otherwise.

### GetAddedInOk

`func (o *ScanDataLinkChangeResponse) GetAddedInOk() (*string, bool)`

GetAddedInOk returns a tuple with the AddedIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddedIn

`func (o *ScanDataLinkChangeResponse) SetAddedIn(v string)`

SetAddedIn sets AddedIn field to given value.


### GetRemovedIn

`func (o *ScanDataLinkChangeResponse) GetRemovedIn() string`

GetRemovedIn returns the RemovedIn field if non-nil, zero value otherwise.

### GetRemovedInOk

`func (o *ScanDataLinkChangeResponse) GetRemovedInOk() (*string, bool)`

GetRemovedInOk returns a tuple with the RemovedIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemovedIn

`func (o *ScanDataLinkChangeResponse) SetRemovedIn(v string)`

SetRemovedIn sets RemovedIn field to given value.

### HasRemovedIn

`func (o *ScanDataLinkChangeResponse) HasRemovedIn() bool`

HasRemovedIn returns a boolean if a field has been set.

### GetFrom

`func (o *ScanDataLinkChangeResponse) GetFrom() ScanDataLinkChangeResponseFrom`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ScanDataLinkChangeResponse) GetFromOk() (*ScanDataLinkChangeResponseFrom, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ScanDataLinkChangeResponse) SetFrom(v ScanDataLinkChangeResponseFrom)`

SetFrom sets From field to given value.


### GetTo

`func (o *ScanDataLinkChangeResponse) GetTo() ScanDataLinkChangeResponseTo`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ScanDataLinkChangeResponse) GetToOk() (*ScanDataLinkChangeResponseTo, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ScanDataLinkChangeResponse) SetTo(v ScanDataLinkChangeResponseTo)`

SetTo sets To field to given value.


### GetRiskSeverity

`func (o *ScanDataLinkChangeResponse) GetRiskSeverity() string`

GetRiskSeverity returns the RiskSeverity field if non-nil, zero value otherwise.

### GetRiskSeverityOk

`func (o *ScanDataLinkChangeResponse) GetRiskSeverityOk() (*string, bool)`

GetRiskSeverityOk returns a tuple with the RiskSeverity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskSeverity

`func (o *ScanDataLinkChangeResponse) SetRiskSeverity(v string)`

SetRiskSeverity sets RiskSeverity field to given value.

### HasRiskSeverity

`func (o *ScanDataLinkChangeResponse) HasRiskSeverity() bool`

HasRiskSeverity returns a boolean if a field has been set.

### GetRiskSeverityNumber

`func (o *ScanDataLinkChangeResponse) GetRiskSeverityNumber() int32`

GetRiskSeverityNumber returns the RiskSeverityNumber field if non-nil, zero value otherwise.

### GetRiskSeverityNumberOk

`func (o *ScanDataLinkChangeResponse) GetRiskSeverityNumberOk() (*int32, bool)`

GetRiskSeverityNumberOk returns a tuple with the RiskSeverityNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskSeverityNumber

`func (o *ScanDataLinkChangeResponse) SetRiskSeverityNumber(v int32)`

SetRiskSeverityNumber sets RiskSeverityNumber field to given value.

### HasRiskSeverityNumber

`func (o *ScanDataLinkChangeResponse) HasRiskSeverityNumber() bool`

HasRiskSeverityNumber returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


