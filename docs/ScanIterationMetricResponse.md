# ScanIterationMetricResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Scan iteration metric row ID | 
**ScanId** | **string** | Scan ID | 
**IterationId** | **string** | Scan iteration ID | 
**Started** | **time.Time** | Timestamp at which the scan iteration started | 
**MetricKey** | [**DashboardMetricKey**](DashboardMetricKey.md) |  | 
**Values** | [**ScanIterationMetricValuesResponse**](ScanIterationMetricValuesResponse.md) |  | 
**Components** | Pointer to [**ScanIterationMetricComponentsResponse**](ScanIterationMetricComponentsResponse.md) |  | [optional] 
**Created** | **time.Time** | Timestamp at which the metric row was created | 

## Methods

### NewScanIterationMetricResponse

`func NewScanIterationMetricResponse(id string, scanId string, iterationId string, started time.Time, metricKey DashboardMetricKey, values ScanIterationMetricValuesResponse, created time.Time, ) *ScanIterationMetricResponse`

NewScanIterationMetricResponse instantiates a new ScanIterationMetricResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanIterationMetricResponseWithDefaults

`func NewScanIterationMetricResponseWithDefaults() *ScanIterationMetricResponse`

NewScanIterationMetricResponseWithDefaults instantiates a new ScanIterationMetricResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanIterationMetricResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanIterationMetricResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanIterationMetricResponse) SetId(v string)`

SetId sets Id field to given value.


### GetScanId

`func (o *ScanIterationMetricResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ScanIterationMetricResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ScanIterationMetricResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetIterationId

`func (o *ScanIterationMetricResponse) GetIterationId() string`

GetIterationId returns the IterationId field if non-nil, zero value otherwise.

### GetIterationIdOk

`func (o *ScanIterationMetricResponse) GetIterationIdOk() (*string, bool)`

GetIterationIdOk returns a tuple with the IterationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIterationId

`func (o *ScanIterationMetricResponse) SetIterationId(v string)`

SetIterationId sets IterationId field to given value.


### GetStarted

`func (o *ScanIterationMetricResponse) GetStarted() time.Time`

GetStarted returns the Started field if non-nil, zero value otherwise.

### GetStartedOk

`func (o *ScanIterationMetricResponse) GetStartedOk() (*time.Time, bool)`

GetStartedOk returns a tuple with the Started field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarted

`func (o *ScanIterationMetricResponse) SetStarted(v time.Time)`

SetStarted sets Started field to given value.


### GetMetricKey

`func (o *ScanIterationMetricResponse) GetMetricKey() DashboardMetricKey`

GetMetricKey returns the MetricKey field if non-nil, zero value otherwise.

### GetMetricKeyOk

`func (o *ScanIterationMetricResponse) GetMetricKeyOk() (*DashboardMetricKey, bool)`

GetMetricKeyOk returns a tuple with the MetricKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetricKey

`func (o *ScanIterationMetricResponse) SetMetricKey(v DashboardMetricKey)`

SetMetricKey sets MetricKey field to given value.


### GetValues

`func (o *ScanIterationMetricResponse) GetValues() ScanIterationMetricValuesResponse`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *ScanIterationMetricResponse) GetValuesOk() (*ScanIterationMetricValuesResponse, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *ScanIterationMetricResponse) SetValues(v ScanIterationMetricValuesResponse)`

SetValues sets Values field to given value.


### GetComponents

`func (o *ScanIterationMetricResponse) GetComponents() ScanIterationMetricComponentsResponse`

GetComponents returns the Components field if non-nil, zero value otherwise.

### GetComponentsOk

`func (o *ScanIterationMetricResponse) GetComponentsOk() (*ScanIterationMetricComponentsResponse, bool)`

GetComponentsOk returns a tuple with the Components field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComponents

`func (o *ScanIterationMetricResponse) SetComponents(v ScanIterationMetricComponentsResponse)`

SetComponents sets Components field to given value.

### HasComponents

`func (o *ScanIterationMetricResponse) HasComponents() bool`

HasComponents returns a boolean if a field has been set.

### GetCreated

`func (o *ScanIterationMetricResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanIterationMetricResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanIterationMetricResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


