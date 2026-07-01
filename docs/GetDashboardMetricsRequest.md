# GetDashboardMetricsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ScanIds** | **[]string** | Scan IDs to fetch dashboard metrics for | 
**MetricKey** | [**DashboardMetricKey**](DashboardMetricKey.md) |  | 
**StartedMin** | Pointer to **time.Time** | Inclusive lower bound for iteration started time | [optional] 
**StartedMax** | Pointer to **time.Time** | Inclusive upper bound for iteration started time | [optional] 
**Limit** | **float32** | Maximum number of entries to return | 
**Offset** | Pointer to **float32** | Offset into the list of entries to return | [optional] [default to 0]

## Methods

### NewGetDashboardMetricsRequest

`func NewGetDashboardMetricsRequest(scanIds []string, metricKey DashboardMetricKey, limit float32, ) *GetDashboardMetricsRequest`

NewGetDashboardMetricsRequest instantiates a new GetDashboardMetricsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetDashboardMetricsRequestWithDefaults

`func NewGetDashboardMetricsRequestWithDefaults() *GetDashboardMetricsRequest`

NewGetDashboardMetricsRequestWithDefaults instantiates a new GetDashboardMetricsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScanIds

`func (o *GetDashboardMetricsRequest) GetScanIds() []string`

GetScanIds returns the ScanIds field if non-nil, zero value otherwise.

### GetScanIdsOk

`func (o *GetDashboardMetricsRequest) GetScanIdsOk() (*[]string, bool)`

GetScanIdsOk returns a tuple with the ScanIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanIds

`func (o *GetDashboardMetricsRequest) SetScanIds(v []string)`

SetScanIds sets ScanIds field to given value.


### GetMetricKey

`func (o *GetDashboardMetricsRequest) GetMetricKey() DashboardMetricKey`

GetMetricKey returns the MetricKey field if non-nil, zero value otherwise.

### GetMetricKeyOk

`func (o *GetDashboardMetricsRequest) GetMetricKeyOk() (*DashboardMetricKey, bool)`

GetMetricKeyOk returns a tuple with the MetricKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetricKey

`func (o *GetDashboardMetricsRequest) SetMetricKey(v DashboardMetricKey)`

SetMetricKey sets MetricKey field to given value.


### GetStartedMin

`func (o *GetDashboardMetricsRequest) GetStartedMin() time.Time`

GetStartedMin returns the StartedMin field if non-nil, zero value otherwise.

### GetStartedMinOk

`func (o *GetDashboardMetricsRequest) GetStartedMinOk() (*time.Time, bool)`

GetStartedMinOk returns a tuple with the StartedMin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartedMin

`func (o *GetDashboardMetricsRequest) SetStartedMin(v time.Time)`

SetStartedMin sets StartedMin field to given value.

### HasStartedMin

`func (o *GetDashboardMetricsRequest) HasStartedMin() bool`

HasStartedMin returns a boolean if a field has been set.

### GetStartedMax

`func (o *GetDashboardMetricsRequest) GetStartedMax() time.Time`

GetStartedMax returns the StartedMax field if non-nil, zero value otherwise.

### GetStartedMaxOk

`func (o *GetDashboardMetricsRequest) GetStartedMaxOk() (*time.Time, bool)`

GetStartedMaxOk returns a tuple with the StartedMax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartedMax

`func (o *GetDashboardMetricsRequest) SetStartedMax(v time.Time)`

SetStartedMax sets StartedMax field to given value.

### HasStartedMax

`func (o *GetDashboardMetricsRequest) HasStartedMax() bool`

HasStartedMax returns a boolean if a field has been set.

### GetLimit

`func (o *GetDashboardMetricsRequest) GetLimit() float32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *GetDashboardMetricsRequest) GetLimitOk() (*float32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *GetDashboardMetricsRequest) SetLimit(v float32)`

SetLimit sets Limit field to given value.


### GetOffset

`func (o *GetDashboardMetricsRequest) GetOffset() float32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *GetDashboardMetricsRequest) GetOffsetOk() (*float32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *GetDashboardMetricsRequest) SetOffset(v float32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *GetDashboardMetricsRequest) HasOffset() bool`

HasOffset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


