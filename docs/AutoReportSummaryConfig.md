# AutoReportSummaryConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**SendEmail** | Pointer to **bool** |  | [optional] 
**ExecutiveSummary** | Pointer to **string** |  | [optional] 
**TimeZone** | Pointer to **string** |  | [optional] 
**TimeSelection** | Pointer to [**ReportTimeSelection**](ReportTimeSelection.md) |  | [optional] 
**Branded** | Pointer to **bool** |  | [optional] 

## Methods

### NewAutoReportSummaryConfig

`func NewAutoReportSummaryConfig() *AutoReportSummaryConfig`

NewAutoReportSummaryConfig instantiates a new AutoReportSummaryConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutoReportSummaryConfigWithDefaults

`func NewAutoReportSummaryConfigWithDefaults() *AutoReportSummaryConfig`

NewAutoReportSummaryConfigWithDefaults instantiates a new AutoReportSummaryConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *AutoReportSummaryConfig) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *AutoReportSummaryConfig) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *AutoReportSummaryConfig) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *AutoReportSummaryConfig) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetSendEmail

`func (o *AutoReportSummaryConfig) GetSendEmail() bool`

GetSendEmail returns the SendEmail field if non-nil, zero value otherwise.

### GetSendEmailOk

`func (o *AutoReportSummaryConfig) GetSendEmailOk() (*bool, bool)`

GetSendEmailOk returns a tuple with the SendEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendEmail

`func (o *AutoReportSummaryConfig) SetSendEmail(v bool)`

SetSendEmail sets SendEmail field to given value.

### HasSendEmail

`func (o *AutoReportSummaryConfig) HasSendEmail() bool`

HasSendEmail returns a boolean if a field has been set.

### GetExecutiveSummary

`func (o *AutoReportSummaryConfig) GetExecutiveSummary() string`

GetExecutiveSummary returns the ExecutiveSummary field if non-nil, zero value otherwise.

### GetExecutiveSummaryOk

`func (o *AutoReportSummaryConfig) GetExecutiveSummaryOk() (*string, bool)`

GetExecutiveSummaryOk returns a tuple with the ExecutiveSummary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutiveSummary

`func (o *AutoReportSummaryConfig) SetExecutiveSummary(v string)`

SetExecutiveSummary sets ExecutiveSummary field to given value.

### HasExecutiveSummary

`func (o *AutoReportSummaryConfig) HasExecutiveSummary() bool`

HasExecutiveSummary returns a boolean if a field has been set.

### GetTimeZone

`func (o *AutoReportSummaryConfig) GetTimeZone() string`

GetTimeZone returns the TimeZone field if non-nil, zero value otherwise.

### GetTimeZoneOk

`func (o *AutoReportSummaryConfig) GetTimeZoneOk() (*string, bool)`

GetTimeZoneOk returns a tuple with the TimeZone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeZone

`func (o *AutoReportSummaryConfig) SetTimeZone(v string)`

SetTimeZone sets TimeZone field to given value.

### HasTimeZone

`func (o *AutoReportSummaryConfig) HasTimeZone() bool`

HasTimeZone returns a boolean if a field has been set.

### GetTimeSelection

`func (o *AutoReportSummaryConfig) GetTimeSelection() ReportTimeSelection`

GetTimeSelection returns the TimeSelection field if non-nil, zero value otherwise.

### GetTimeSelectionOk

`func (o *AutoReportSummaryConfig) GetTimeSelectionOk() (*ReportTimeSelection, bool)`

GetTimeSelectionOk returns a tuple with the TimeSelection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeSelection

`func (o *AutoReportSummaryConfig) SetTimeSelection(v ReportTimeSelection)`

SetTimeSelection sets TimeSelection field to given value.

### HasTimeSelection

`func (o *AutoReportSummaryConfig) HasTimeSelection() bool`

HasTimeSelection returns a boolean if a field has been set.

### GetBranded

`func (o *AutoReportSummaryConfig) GetBranded() bool`

GetBranded returns the Branded field if non-nil, zero value otherwise.

### GetBrandedOk

`func (o *AutoReportSummaryConfig) GetBrandedOk() (*bool, bool)`

GetBrandedOk returns a tuple with the Branded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranded

`func (o *AutoReportSummaryConfig) SetBranded(v bool)`

SetBranded sets Branded field to given value.

### HasBranded

`func (o *AutoReportSummaryConfig) HasBranded() bool`

HasBranded returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


