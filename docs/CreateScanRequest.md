# CreateScanRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Scan name | 
**ScanGroupId** | **string** | Scan Group ID | 
**Type** | [**ScanType**](ScanType.md) |  | 
**DnsNamelist** | Pointer to **bool** | Check for commonly used seed domains (true if not set) | [optional] 
**IgnoreIpNodes** | Pointer to **bool** | Only show IP risks if they relate to seed IP nodes (false if not set) | [optional] 
**CalendarSchedule** | Pointer to **string** | The frequency of scan iteration  i.e. \&quot;daily\&quot;, \&quot;weekly\&quot;, \&quot;monthly\&quot;, \&quot;quarterly\&quot;, \&quot;yearly\&quot;  | [optional] 
**IncludeBrRisks** | Pointer to [**CreateScanRequestIncludeBrRisks**](CreateScanRequestIncludeBrRisks.md) |  | [optional] 

## Methods

### NewCreateScanRequest

`func NewCreateScanRequest(name string, scanGroupId string, type_ ScanType, ) *CreateScanRequest`

NewCreateScanRequest instantiates a new CreateScanRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateScanRequestWithDefaults

`func NewCreateScanRequestWithDefaults() *CreateScanRequest`

NewCreateScanRequestWithDefaults instantiates a new CreateScanRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateScanRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateScanRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateScanRequest) SetName(v string)`

SetName sets Name field to given value.


### GetScanGroupId

`func (o *CreateScanRequest) GetScanGroupId() string`

GetScanGroupId returns the ScanGroupId field if non-nil, zero value otherwise.

### GetScanGroupIdOk

`func (o *CreateScanRequest) GetScanGroupIdOk() (*string, bool)`

GetScanGroupIdOk returns a tuple with the ScanGroupId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanGroupId

`func (o *CreateScanRequest) SetScanGroupId(v string)`

SetScanGroupId sets ScanGroupId field to given value.


### GetType

`func (o *CreateScanRequest) GetType() ScanType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateScanRequest) GetTypeOk() (*ScanType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateScanRequest) SetType(v ScanType)`

SetType sets Type field to given value.


### GetDnsNamelist

`func (o *CreateScanRequest) GetDnsNamelist() bool`

GetDnsNamelist returns the DnsNamelist field if non-nil, zero value otherwise.

### GetDnsNamelistOk

`func (o *CreateScanRequest) GetDnsNamelistOk() (*bool, bool)`

GetDnsNamelistOk returns a tuple with the DnsNamelist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDnsNamelist

`func (o *CreateScanRequest) SetDnsNamelist(v bool)`

SetDnsNamelist sets DnsNamelist field to given value.

### HasDnsNamelist

`func (o *CreateScanRequest) HasDnsNamelist() bool`

HasDnsNamelist returns a boolean if a field has been set.

### GetIgnoreIpNodes

`func (o *CreateScanRequest) GetIgnoreIpNodes() bool`

GetIgnoreIpNodes returns the IgnoreIpNodes field if non-nil, zero value otherwise.

### GetIgnoreIpNodesOk

`func (o *CreateScanRequest) GetIgnoreIpNodesOk() (*bool, bool)`

GetIgnoreIpNodesOk returns a tuple with the IgnoreIpNodes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnoreIpNodes

`func (o *CreateScanRequest) SetIgnoreIpNodes(v bool)`

SetIgnoreIpNodes sets IgnoreIpNodes field to given value.

### HasIgnoreIpNodes

`func (o *CreateScanRequest) HasIgnoreIpNodes() bool`

HasIgnoreIpNodes returns a boolean if a field has been set.

### GetCalendarSchedule

`func (o *CreateScanRequest) GetCalendarSchedule() string`

GetCalendarSchedule returns the CalendarSchedule field if non-nil, zero value otherwise.

### GetCalendarScheduleOk

`func (o *CreateScanRequest) GetCalendarScheduleOk() (*string, bool)`

GetCalendarScheduleOk returns a tuple with the CalendarSchedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalendarSchedule

`func (o *CreateScanRequest) SetCalendarSchedule(v string)`

SetCalendarSchedule sets CalendarSchedule field to given value.

### HasCalendarSchedule

`func (o *CreateScanRequest) HasCalendarSchedule() bool`

HasCalendarSchedule returns a boolean if a field has been set.

### GetIncludeBrRisks

`func (o *CreateScanRequest) GetIncludeBrRisks() CreateScanRequestIncludeBrRisks`

GetIncludeBrRisks returns the IncludeBrRisks field if non-nil, zero value otherwise.

### GetIncludeBrRisksOk

`func (o *CreateScanRequest) GetIncludeBrRisksOk() (*CreateScanRequestIncludeBrRisks, bool)`

GetIncludeBrRisksOk returns a tuple with the IncludeBrRisks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeBrRisks

`func (o *CreateScanRequest) SetIncludeBrRisks(v CreateScanRequestIncludeBrRisks)`

SetIncludeBrRisks sets IncludeBrRisks field to given value.

### HasIncludeBrRisks

`func (o *CreateScanRequest) HasIncludeBrRisks() bool`

HasIncludeBrRisks returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


