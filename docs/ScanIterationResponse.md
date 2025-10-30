# ScanIterationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Scan Iteration ID | 
**ScanId** | **string** | Scan ID | 
**State** | **string** | Scan Iteration state | 
**Created** | **time.Time** | Timestamp at which the entry was created | 
**Updated** | **time.Time** | Timestamp at which the entry was last updated | 
**Started** | **time.Time** | Timestamp at which the Scan Iteration started running | 
**Completed** | Pointer to **time.Time** | Timestamp at which the Scan Iteration completed running | [optional] 
**CompletedTime** | Pointer to **time.Time** | Deprecated - Timestamp at which the Scan Iteration completed running - Use **completed** | [optional] 
**Limited** | Pointer to **bool** | Scan Iteration reached the scan&#39;s organisation limit | [optional] 
**SummaryGenerated** | Pointer to **time.Time** | Timestamp at which the scores, issues and stats were generated | [optional] 
**Scores** | Pointer to **map[string]interface{}** | Health scores for Scan Iteration | [optional] 
**Issues** | Pointer to **map[string]interface{}** | Summary of issues found in Scan Iteration | [optional] 
**Stats** | Pointer to **map[string]interface{}** | Breakdown of the number of items discovered in Scan Iteration | [optional] 
**InsightsGenerated** | Pointer to **time.Time** | Timestamp at which the insights were generated | [optional] 
**Insights** | Pointer to **map[string]interface{}** | Insights for Scan Iteration | [optional] 
**Merged** | Pointer to **string** | Scan Iteration has been consolidated in accordance with scan&#39;s organisation history settings | [optional] 

## Methods

### NewScanIterationResponse

`func NewScanIterationResponse(id string, scanId string, state string, created time.Time, updated time.Time, started time.Time, ) *ScanIterationResponse`

NewScanIterationResponse instantiates a new ScanIterationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanIterationResponseWithDefaults

`func NewScanIterationResponseWithDefaults() *ScanIterationResponse`

NewScanIterationResponseWithDefaults instantiates a new ScanIterationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanIterationResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanIterationResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanIterationResponse) SetId(v string)`

SetId sets Id field to given value.


### GetScanId

`func (o *ScanIterationResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ScanIterationResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ScanIterationResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetState

`func (o *ScanIterationResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ScanIterationResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ScanIterationResponse) SetState(v string)`

SetState sets State field to given value.


### GetCreated

`func (o *ScanIterationResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanIterationResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanIterationResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetUpdated

`func (o *ScanIterationResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ScanIterationResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ScanIterationResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.


### GetStarted

`func (o *ScanIterationResponse) GetStarted() time.Time`

GetStarted returns the Started field if non-nil, zero value otherwise.

### GetStartedOk

`func (o *ScanIterationResponse) GetStartedOk() (*time.Time, bool)`

GetStartedOk returns a tuple with the Started field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarted

`func (o *ScanIterationResponse) SetStarted(v time.Time)`

SetStarted sets Started field to given value.


### GetCompleted

`func (o *ScanIterationResponse) GetCompleted() time.Time`

GetCompleted returns the Completed field if non-nil, zero value otherwise.

### GetCompletedOk

`func (o *ScanIterationResponse) GetCompletedOk() (*time.Time, bool)`

GetCompletedOk returns a tuple with the Completed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompleted

`func (o *ScanIterationResponse) SetCompleted(v time.Time)`

SetCompleted sets Completed field to given value.

### HasCompleted

`func (o *ScanIterationResponse) HasCompleted() bool`

HasCompleted returns a boolean if a field has been set.

### GetCompletedTime

`func (o *ScanIterationResponse) GetCompletedTime() time.Time`

GetCompletedTime returns the CompletedTime field if non-nil, zero value otherwise.

### GetCompletedTimeOk

`func (o *ScanIterationResponse) GetCompletedTimeOk() (*time.Time, bool)`

GetCompletedTimeOk returns a tuple with the CompletedTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedTime

`func (o *ScanIterationResponse) SetCompletedTime(v time.Time)`

SetCompletedTime sets CompletedTime field to given value.

### HasCompletedTime

`func (o *ScanIterationResponse) HasCompletedTime() bool`

HasCompletedTime returns a boolean if a field has been set.

### GetLimited

`func (o *ScanIterationResponse) GetLimited() bool`

GetLimited returns the Limited field if non-nil, zero value otherwise.

### GetLimitedOk

`func (o *ScanIterationResponse) GetLimitedOk() (*bool, bool)`

GetLimitedOk returns a tuple with the Limited field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimited

`func (o *ScanIterationResponse) SetLimited(v bool)`

SetLimited sets Limited field to given value.

### HasLimited

`func (o *ScanIterationResponse) HasLimited() bool`

HasLimited returns a boolean if a field has been set.

### GetSummaryGenerated

`func (o *ScanIterationResponse) GetSummaryGenerated() time.Time`

GetSummaryGenerated returns the SummaryGenerated field if non-nil, zero value otherwise.

### GetSummaryGeneratedOk

`func (o *ScanIterationResponse) GetSummaryGeneratedOk() (*time.Time, bool)`

GetSummaryGeneratedOk returns a tuple with the SummaryGenerated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSummaryGenerated

`func (o *ScanIterationResponse) SetSummaryGenerated(v time.Time)`

SetSummaryGenerated sets SummaryGenerated field to given value.

### HasSummaryGenerated

`func (o *ScanIterationResponse) HasSummaryGenerated() bool`

HasSummaryGenerated returns a boolean if a field has been set.

### GetScores

`func (o *ScanIterationResponse) GetScores() map[string]interface{}`

GetScores returns the Scores field if non-nil, zero value otherwise.

### GetScoresOk

`func (o *ScanIterationResponse) GetScoresOk() (*map[string]interface{}, bool)`

GetScoresOk returns a tuple with the Scores field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScores

`func (o *ScanIterationResponse) SetScores(v map[string]interface{})`

SetScores sets Scores field to given value.

### HasScores

`func (o *ScanIterationResponse) HasScores() bool`

HasScores returns a boolean if a field has been set.

### GetIssues

`func (o *ScanIterationResponse) GetIssues() map[string]interface{}`

GetIssues returns the Issues field if non-nil, zero value otherwise.

### GetIssuesOk

`func (o *ScanIterationResponse) GetIssuesOk() (*map[string]interface{}, bool)`

GetIssuesOk returns a tuple with the Issues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssues

`func (o *ScanIterationResponse) SetIssues(v map[string]interface{})`

SetIssues sets Issues field to given value.

### HasIssues

`func (o *ScanIterationResponse) HasIssues() bool`

HasIssues returns a boolean if a field has been set.

### GetStats

`func (o *ScanIterationResponse) GetStats() map[string]interface{}`

GetStats returns the Stats field if non-nil, zero value otherwise.

### GetStatsOk

`func (o *ScanIterationResponse) GetStatsOk() (*map[string]interface{}, bool)`

GetStatsOk returns a tuple with the Stats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStats

`func (o *ScanIterationResponse) SetStats(v map[string]interface{})`

SetStats sets Stats field to given value.

### HasStats

`func (o *ScanIterationResponse) HasStats() bool`

HasStats returns a boolean if a field has been set.

### GetInsightsGenerated

`func (o *ScanIterationResponse) GetInsightsGenerated() time.Time`

GetInsightsGenerated returns the InsightsGenerated field if non-nil, zero value otherwise.

### GetInsightsGeneratedOk

`func (o *ScanIterationResponse) GetInsightsGeneratedOk() (*time.Time, bool)`

GetInsightsGeneratedOk returns a tuple with the InsightsGenerated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInsightsGenerated

`func (o *ScanIterationResponse) SetInsightsGenerated(v time.Time)`

SetInsightsGenerated sets InsightsGenerated field to given value.

### HasInsightsGenerated

`func (o *ScanIterationResponse) HasInsightsGenerated() bool`

HasInsightsGenerated returns a boolean if a field has been set.

### GetInsights

`func (o *ScanIterationResponse) GetInsights() map[string]interface{}`

GetInsights returns the Insights field if non-nil, zero value otherwise.

### GetInsightsOk

`func (o *ScanIterationResponse) GetInsightsOk() (*map[string]interface{}, bool)`

GetInsightsOk returns a tuple with the Insights field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInsights

`func (o *ScanIterationResponse) SetInsights(v map[string]interface{})`

SetInsights sets Insights field to given value.

### HasInsights

`func (o *ScanIterationResponse) HasInsights() bool`

HasInsights returns a boolean if a field has been set.

### GetMerged

`func (o *ScanIterationResponse) GetMerged() string`

GetMerged returns the Merged field if non-nil, zero value otherwise.

### GetMergedOk

`func (o *ScanIterationResponse) GetMergedOk() (*string, bool)`

GetMergedOk returns a tuple with the Merged field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMerged

`func (o *ScanIterationResponse) SetMerged(v string)`

SetMerged sets Merged field to given value.

### HasMerged

`func (o *ScanIterationResponse) HasMerged() bool`

HasMerged returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


