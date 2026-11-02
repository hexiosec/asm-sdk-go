# CreateExcelSummaryReportBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | [**ReportType**](ReportType.md) |  | 
**ScanId** | **string** | Scan ID | 
**Name** | **string** | Report display name | 
**SendEmail** | Pointer to **bool** | Send email notification when report is ready | [optional] 
**ExecutiveSummary** | Pointer to **string** | Executive summary displayed on the initial tab | [optional] 
**Branded** | Pointer to **bool** | Display organisation logo on the initial tab. Requires feature to be enabled for the organisation. | [optional] 

## Methods

### NewCreateExcelSummaryReportBody

`func NewCreateExcelSummaryReportBody(type_ ReportType, scanId string, name string, ) *CreateExcelSummaryReportBody`

NewCreateExcelSummaryReportBody instantiates a new CreateExcelSummaryReportBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateExcelSummaryReportBodyWithDefaults

`func NewCreateExcelSummaryReportBodyWithDefaults() *CreateExcelSummaryReportBody`

NewCreateExcelSummaryReportBodyWithDefaults instantiates a new CreateExcelSummaryReportBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateExcelSummaryReportBody) GetType() ReportType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateExcelSummaryReportBody) GetTypeOk() (*ReportType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateExcelSummaryReportBody) SetType(v ReportType)`

SetType sets Type field to given value.


### GetScanId

`func (o *CreateExcelSummaryReportBody) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *CreateExcelSummaryReportBody) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *CreateExcelSummaryReportBody) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetName

`func (o *CreateExcelSummaryReportBody) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateExcelSummaryReportBody) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateExcelSummaryReportBody) SetName(v string)`

SetName sets Name field to given value.


### GetSendEmail

`func (o *CreateExcelSummaryReportBody) GetSendEmail() bool`

GetSendEmail returns the SendEmail field if non-nil, zero value otherwise.

### GetSendEmailOk

`func (o *CreateExcelSummaryReportBody) GetSendEmailOk() (*bool, bool)`

GetSendEmailOk returns a tuple with the SendEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendEmail

`func (o *CreateExcelSummaryReportBody) SetSendEmail(v bool)`

SetSendEmail sets SendEmail field to given value.

### HasSendEmail

`func (o *CreateExcelSummaryReportBody) HasSendEmail() bool`

HasSendEmail returns a boolean if a field has been set.

### GetExecutiveSummary

`func (o *CreateExcelSummaryReportBody) GetExecutiveSummary() string`

GetExecutiveSummary returns the ExecutiveSummary field if non-nil, zero value otherwise.

### GetExecutiveSummaryOk

`func (o *CreateExcelSummaryReportBody) GetExecutiveSummaryOk() (*string, bool)`

GetExecutiveSummaryOk returns a tuple with the ExecutiveSummary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutiveSummary

`func (o *CreateExcelSummaryReportBody) SetExecutiveSummary(v string)`

SetExecutiveSummary sets ExecutiveSummary field to given value.

### HasExecutiveSummary

`func (o *CreateExcelSummaryReportBody) HasExecutiveSummary() bool`

HasExecutiveSummary returns a boolean if a field has been set.

### GetBranded

`func (o *CreateExcelSummaryReportBody) GetBranded() bool`

GetBranded returns the Branded field if non-nil, zero value otherwise.

### GetBrandedOk

`func (o *CreateExcelSummaryReportBody) GetBrandedOk() (*bool, bool)`

GetBrandedOk returns a tuple with the Branded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranded

`func (o *CreateExcelSummaryReportBody) SetBranded(v bool)`

SetBranded sets Branded field to given value.

### HasBranded

`func (o *CreateExcelSummaryReportBody) HasBranded() bool`

HasBranded returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


