# ReportTimeSelection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | Pointer to **time.Time** | From time (ISO 8601) | [optional] 
**To** | Pointer to **time.Time** | To time (ISO 8601) | [optional] 
**AllTime** | Pointer to **bool** | Include data from the first scan iteration through to report generation time. | [optional] 
**RelativeDuration** | Pointer to [**ReportTimeSelectionRelativeDuration**](ReportTimeSelectionRelativeDuration.md) |  | [optional] 

## Methods

### NewReportTimeSelection

`func NewReportTimeSelection() *ReportTimeSelection`

NewReportTimeSelection instantiates a new ReportTimeSelection object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReportTimeSelectionWithDefaults

`func NewReportTimeSelectionWithDefaults() *ReportTimeSelection`

NewReportTimeSelectionWithDefaults instantiates a new ReportTimeSelection object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *ReportTimeSelection) GetFrom() time.Time`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ReportTimeSelection) GetFromOk() (*time.Time, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ReportTimeSelection) SetFrom(v time.Time)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ReportTimeSelection) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *ReportTimeSelection) GetTo() time.Time`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ReportTimeSelection) GetToOk() (*time.Time, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ReportTimeSelection) SetTo(v time.Time)`

SetTo sets To field to given value.

### HasTo

`func (o *ReportTimeSelection) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetAllTime

`func (o *ReportTimeSelection) GetAllTime() bool`

GetAllTime returns the AllTime field if non-nil, zero value otherwise.

### GetAllTimeOk

`func (o *ReportTimeSelection) GetAllTimeOk() (*bool, bool)`

GetAllTimeOk returns a tuple with the AllTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllTime

`func (o *ReportTimeSelection) SetAllTime(v bool)`

SetAllTime sets AllTime field to given value.

### HasAllTime

`func (o *ReportTimeSelection) HasAllTime() bool`

HasAllTime returns a boolean if a field has been set.

### GetRelativeDuration

`func (o *ReportTimeSelection) GetRelativeDuration() ReportTimeSelectionRelativeDuration`

GetRelativeDuration returns the RelativeDuration field if non-nil, zero value otherwise.

### GetRelativeDurationOk

`func (o *ReportTimeSelection) GetRelativeDurationOk() (*ReportTimeSelectionRelativeDuration, bool)`

GetRelativeDurationOk returns a tuple with the RelativeDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRelativeDuration

`func (o *ReportTimeSelection) SetRelativeDuration(v ReportTimeSelectionRelativeDuration)`

SetRelativeDuration sets RelativeDuration field to given value.

### HasRelativeDuration

`func (o *ReportTimeSelection) HasRelativeDuration() bool`

HasRelativeDuration returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


