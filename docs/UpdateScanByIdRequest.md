# UpdateScanByIdRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** | Name of the scan | [optional] 
**Enabled** | Pointer to **bool** | Whether the scan is enabled (&#x60;false&#x60; on new scans, enable to start the scan) | [optional] 
**ScanGroupId** | Pointer to **string** | Scan Group ID | [optional] 
**IgnoreIpNodes** | Pointer to **bool** | Whether to hide IP risks | [optional] 
**CalendarSchedule** | Pointer to **string** | The frequency of scan iteration  i.e. \&quot;daily\&quot;, \&quot;weekly\&quot;, \&quot;monthly\&quot;, \&quot;quarterly\&quot;, \&quot;yearly\&quot;  | [optional] 
**IncludeBrRisks** | Pointer to [**UpdateScanByIdRequestIncludeBrRisks**](UpdateScanByIdRequestIncludeBrRisks.md) |  | [optional] 
**AutoReports** | Pointer to [**AutoReports**](AutoReports.md) |  | [optional] 

## Methods

### NewUpdateScanByIdRequest

`func NewUpdateScanByIdRequest() *UpdateScanByIdRequest`

NewUpdateScanByIdRequest instantiates a new UpdateScanByIdRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateScanByIdRequestWithDefaults

`func NewUpdateScanByIdRequestWithDefaults() *UpdateScanByIdRequest`

NewUpdateScanByIdRequestWithDefaults instantiates a new UpdateScanByIdRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateScanByIdRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateScanByIdRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateScanByIdRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateScanByIdRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetEnabled

`func (o *UpdateScanByIdRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *UpdateScanByIdRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *UpdateScanByIdRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *UpdateScanByIdRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetScanGroupId

`func (o *UpdateScanByIdRequest) GetScanGroupId() string`

GetScanGroupId returns the ScanGroupId field if non-nil, zero value otherwise.

### GetScanGroupIdOk

`func (o *UpdateScanByIdRequest) GetScanGroupIdOk() (*string, bool)`

GetScanGroupIdOk returns a tuple with the ScanGroupId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanGroupId

`func (o *UpdateScanByIdRequest) SetScanGroupId(v string)`

SetScanGroupId sets ScanGroupId field to given value.

### HasScanGroupId

`func (o *UpdateScanByIdRequest) HasScanGroupId() bool`

HasScanGroupId returns a boolean if a field has been set.

### GetIgnoreIpNodes

`func (o *UpdateScanByIdRequest) GetIgnoreIpNodes() bool`

GetIgnoreIpNodes returns the IgnoreIpNodes field if non-nil, zero value otherwise.

### GetIgnoreIpNodesOk

`func (o *UpdateScanByIdRequest) GetIgnoreIpNodesOk() (*bool, bool)`

GetIgnoreIpNodesOk returns a tuple with the IgnoreIpNodes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnoreIpNodes

`func (o *UpdateScanByIdRequest) SetIgnoreIpNodes(v bool)`

SetIgnoreIpNodes sets IgnoreIpNodes field to given value.

### HasIgnoreIpNodes

`func (o *UpdateScanByIdRequest) HasIgnoreIpNodes() bool`

HasIgnoreIpNodes returns a boolean if a field has been set.

### GetCalendarSchedule

`func (o *UpdateScanByIdRequest) GetCalendarSchedule() string`

GetCalendarSchedule returns the CalendarSchedule field if non-nil, zero value otherwise.

### GetCalendarScheduleOk

`func (o *UpdateScanByIdRequest) GetCalendarScheduleOk() (*string, bool)`

GetCalendarScheduleOk returns a tuple with the CalendarSchedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalendarSchedule

`func (o *UpdateScanByIdRequest) SetCalendarSchedule(v string)`

SetCalendarSchedule sets CalendarSchedule field to given value.

### HasCalendarSchedule

`func (o *UpdateScanByIdRequest) HasCalendarSchedule() bool`

HasCalendarSchedule returns a boolean if a field has been set.

### GetIncludeBrRisks

`func (o *UpdateScanByIdRequest) GetIncludeBrRisks() UpdateScanByIdRequestIncludeBrRisks`

GetIncludeBrRisks returns the IncludeBrRisks field if non-nil, zero value otherwise.

### GetIncludeBrRisksOk

`func (o *UpdateScanByIdRequest) GetIncludeBrRisksOk() (*UpdateScanByIdRequestIncludeBrRisks, bool)`

GetIncludeBrRisksOk returns a tuple with the IncludeBrRisks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeBrRisks

`func (o *UpdateScanByIdRequest) SetIncludeBrRisks(v UpdateScanByIdRequestIncludeBrRisks)`

SetIncludeBrRisks sets IncludeBrRisks field to given value.

### HasIncludeBrRisks

`func (o *UpdateScanByIdRequest) HasIncludeBrRisks() bool`

HasIncludeBrRisks returns a boolean if a field has been set.

### GetAutoReports

`func (o *UpdateScanByIdRequest) GetAutoReports() AutoReports`

GetAutoReports returns the AutoReports field if non-nil, zero value otherwise.

### GetAutoReportsOk

`func (o *UpdateScanByIdRequest) GetAutoReportsOk() (*AutoReports, bool)`

GetAutoReportsOk returns a tuple with the AutoReports field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoReports

`func (o *UpdateScanByIdRequest) SetAutoReports(v AutoReports)`

SetAutoReports sets AutoReports field to given value.

### HasAutoReports

`func (o *UpdateScanByIdRequest) HasAutoReports() bool`

HasAutoReports returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


