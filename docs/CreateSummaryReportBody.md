# CreateSummaryReportBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | [**ReportType**](ReportType.md) |  | 
**ScanId** | **string** | Scan ID | 
**Name** | **string** | Report display name | 
**SendEmail** | Pointer to **bool** | Send email notification when report is ready | [optional] 
**TimeZone** | **string** | IANA Time zone | 
**ExecutiveSummary** | Pointer to **string** | Executive summary | [optional] 
**TimeSelection** | Pointer to [**ReportTimeSelection**](ReportTimeSelection.md) |  | [optional] 
**Branded** | Pointer to **bool** | Display organisation logo in report header. Requires feature to be enabled for the organisation. | [optional] 

## Methods

### NewCreateSummaryReportBody

`func NewCreateSummaryReportBody(type_ ReportType, scanId string, name string, timeZone string, ) *CreateSummaryReportBody`

NewCreateSummaryReportBody instantiates a new CreateSummaryReportBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateSummaryReportBodyWithDefaults

`func NewCreateSummaryReportBodyWithDefaults() *CreateSummaryReportBody`

NewCreateSummaryReportBodyWithDefaults instantiates a new CreateSummaryReportBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateSummaryReportBody) GetType() ReportType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateSummaryReportBody) GetTypeOk() (*ReportType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateSummaryReportBody) SetType(v ReportType)`

SetType sets Type field to given value.


### GetScanId

`func (o *CreateSummaryReportBody) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *CreateSummaryReportBody) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *CreateSummaryReportBody) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetName

`func (o *CreateSummaryReportBody) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateSummaryReportBody) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateSummaryReportBody) SetName(v string)`

SetName sets Name field to given value.


### GetSendEmail

`func (o *CreateSummaryReportBody) GetSendEmail() bool`

GetSendEmail returns the SendEmail field if non-nil, zero value otherwise.

### GetSendEmailOk

`func (o *CreateSummaryReportBody) GetSendEmailOk() (*bool, bool)`

GetSendEmailOk returns a tuple with the SendEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendEmail

`func (o *CreateSummaryReportBody) SetSendEmail(v bool)`

SetSendEmail sets SendEmail field to given value.

### HasSendEmail

`func (o *CreateSummaryReportBody) HasSendEmail() bool`

HasSendEmail returns a boolean if a field has been set.

### GetTimeZone

`func (o *CreateSummaryReportBody) GetTimeZone() string`

GetTimeZone returns the TimeZone field if non-nil, zero value otherwise.

### GetTimeZoneOk

`func (o *CreateSummaryReportBody) GetTimeZoneOk() (*string, bool)`

GetTimeZoneOk returns a tuple with the TimeZone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeZone

`func (o *CreateSummaryReportBody) SetTimeZone(v string)`

SetTimeZone sets TimeZone field to given value.


### GetExecutiveSummary

`func (o *CreateSummaryReportBody) GetExecutiveSummary() string`

GetExecutiveSummary returns the ExecutiveSummary field if non-nil, zero value otherwise.

### GetExecutiveSummaryOk

`func (o *CreateSummaryReportBody) GetExecutiveSummaryOk() (*string, bool)`

GetExecutiveSummaryOk returns a tuple with the ExecutiveSummary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutiveSummary

`func (o *CreateSummaryReportBody) SetExecutiveSummary(v string)`

SetExecutiveSummary sets ExecutiveSummary field to given value.

### HasExecutiveSummary

`func (o *CreateSummaryReportBody) HasExecutiveSummary() bool`

HasExecutiveSummary returns a boolean if a field has been set.

### GetTimeSelection

`func (o *CreateSummaryReportBody) GetTimeSelection() ReportTimeSelection`

GetTimeSelection returns the TimeSelection field if non-nil, zero value otherwise.

### GetTimeSelectionOk

`func (o *CreateSummaryReportBody) GetTimeSelectionOk() (*ReportTimeSelection, bool)`

GetTimeSelectionOk returns a tuple with the TimeSelection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeSelection

`func (o *CreateSummaryReportBody) SetTimeSelection(v ReportTimeSelection)`

SetTimeSelection sets TimeSelection field to given value.

### HasTimeSelection

`func (o *CreateSummaryReportBody) HasTimeSelection() bool`

HasTimeSelection returns a boolean if a field has been set.

### GetBranded

`func (o *CreateSummaryReportBody) GetBranded() bool`

GetBranded returns the Branded field if non-nil, zero value otherwise.

### GetBrandedOk

`func (o *CreateSummaryReportBody) GetBrandedOk() (*bool, bool)`

GetBrandedOk returns a tuple with the Branded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranded

`func (o *CreateSummaryReportBody) SetBranded(v bool)`

SetBranded sets Branded field to given value.

### HasBranded

`func (o *CreateSummaryReportBody) HasBranded() bool`

HasBranded returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


