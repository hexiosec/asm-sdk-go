# CreateReportRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | [**ReportType**](ReportType.md) |  | 
**ScanId** | **string** | Scan ID | 
**Name** | **string** | Report display name | 
**SendEmail** | Pointer to **bool** | Send email notification when report is ready | [optional] 
**TimeZone** | **string** | IANA Time zone | 
**ExecutiveSummary** | Pointer to **string** | Executive summary displayed on the initial tab | [optional] 
**TimeSelection** | Pointer to [**ReportTimeSelection**](ReportTimeSelection.md) |  | [optional] 
**Branded** | Pointer to **bool** | Display organisation logo on the initial tab. Requires feature to be enabled for the organisation. | [optional] 

## Methods

### NewCreateReportRequest

`func NewCreateReportRequest(type_ ReportType, scanId string, name string, timeZone string, ) *CreateReportRequest`

NewCreateReportRequest instantiates a new CreateReportRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateReportRequestWithDefaults

`func NewCreateReportRequestWithDefaults() *CreateReportRequest`

NewCreateReportRequestWithDefaults instantiates a new CreateReportRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateReportRequest) GetType() ReportType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateReportRequest) GetTypeOk() (*ReportType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateReportRequest) SetType(v ReportType)`

SetType sets Type field to given value.


### GetScanId

`func (o *CreateReportRequest) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *CreateReportRequest) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *CreateReportRequest) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetName

`func (o *CreateReportRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateReportRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateReportRequest) SetName(v string)`

SetName sets Name field to given value.


### GetSendEmail

`func (o *CreateReportRequest) GetSendEmail() bool`

GetSendEmail returns the SendEmail field if non-nil, zero value otherwise.

### GetSendEmailOk

`func (o *CreateReportRequest) GetSendEmailOk() (*bool, bool)`

GetSendEmailOk returns a tuple with the SendEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendEmail

`func (o *CreateReportRequest) SetSendEmail(v bool)`

SetSendEmail sets SendEmail field to given value.

### HasSendEmail

`func (o *CreateReportRequest) HasSendEmail() bool`

HasSendEmail returns a boolean if a field has been set.

### GetTimeZone

`func (o *CreateReportRequest) GetTimeZone() string`

GetTimeZone returns the TimeZone field if non-nil, zero value otherwise.

### GetTimeZoneOk

`func (o *CreateReportRequest) GetTimeZoneOk() (*string, bool)`

GetTimeZoneOk returns a tuple with the TimeZone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeZone

`func (o *CreateReportRequest) SetTimeZone(v string)`

SetTimeZone sets TimeZone field to given value.


### GetExecutiveSummary

`func (o *CreateReportRequest) GetExecutiveSummary() string`

GetExecutiveSummary returns the ExecutiveSummary field if non-nil, zero value otherwise.

### GetExecutiveSummaryOk

`func (o *CreateReportRequest) GetExecutiveSummaryOk() (*string, bool)`

GetExecutiveSummaryOk returns a tuple with the ExecutiveSummary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutiveSummary

`func (o *CreateReportRequest) SetExecutiveSummary(v string)`

SetExecutiveSummary sets ExecutiveSummary field to given value.

### HasExecutiveSummary

`func (o *CreateReportRequest) HasExecutiveSummary() bool`

HasExecutiveSummary returns a boolean if a field has been set.

### GetTimeSelection

`func (o *CreateReportRequest) GetTimeSelection() ReportTimeSelection`

GetTimeSelection returns the TimeSelection field if non-nil, zero value otherwise.

### GetTimeSelectionOk

`func (o *CreateReportRequest) GetTimeSelectionOk() (*ReportTimeSelection, bool)`

GetTimeSelectionOk returns a tuple with the TimeSelection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeSelection

`func (o *CreateReportRequest) SetTimeSelection(v ReportTimeSelection)`

SetTimeSelection sets TimeSelection field to given value.

### HasTimeSelection

`func (o *CreateReportRequest) HasTimeSelection() bool`

HasTimeSelection returns a boolean if a field has been set.

### GetBranded

`func (o *CreateReportRequest) GetBranded() bool`

GetBranded returns the Branded field if non-nil, zero value otherwise.

### GetBrandedOk

`func (o *CreateReportRequest) GetBrandedOk() (*bool, bool)`

GetBrandedOk returns a tuple with the Branded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranded

`func (o *CreateReportRequest) SetBranded(v bool)`

SetBranded sets Branded field to given value.

### HasBranded

`func (o *CreateReportRequest) HasBranded() bool`

HasBranded returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


