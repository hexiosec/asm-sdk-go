# ScanDataLinkChangesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Comparison** | [**ScanDataLinkChangesResponseComparison**](ScanDataLinkChangesResponseComparison.md) |  | 
**Added** | [**[]ScanDataLinkChangeResponse**](ScanDataLinkChangeResponse.md) | List of added links | 
**Removed** | [**[]ScanDataLinkChangeResponse**](ScanDataLinkChangeResponse.md) | List of removed links | 

## Methods

### NewScanDataLinkChangesResponse

`func NewScanDataLinkChangesResponse(comparison ScanDataLinkChangesResponseComparison, added []ScanDataLinkChangeResponse, removed []ScanDataLinkChangeResponse, ) *ScanDataLinkChangesResponse`

NewScanDataLinkChangesResponse instantiates a new ScanDataLinkChangesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataLinkChangesResponseWithDefaults

`func NewScanDataLinkChangesResponseWithDefaults() *ScanDataLinkChangesResponse`

NewScanDataLinkChangesResponseWithDefaults instantiates a new ScanDataLinkChangesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetComparison

`func (o *ScanDataLinkChangesResponse) GetComparison() ScanDataLinkChangesResponseComparison`

GetComparison returns the Comparison field if non-nil, zero value otherwise.

### GetComparisonOk

`func (o *ScanDataLinkChangesResponse) GetComparisonOk() (*ScanDataLinkChangesResponseComparison, bool)`

GetComparisonOk returns a tuple with the Comparison field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComparison

`func (o *ScanDataLinkChangesResponse) SetComparison(v ScanDataLinkChangesResponseComparison)`

SetComparison sets Comparison field to given value.


### GetAdded

`func (o *ScanDataLinkChangesResponse) GetAdded() []ScanDataLinkChangeResponse`

GetAdded returns the Added field if non-nil, zero value otherwise.

### GetAddedOk

`func (o *ScanDataLinkChangesResponse) GetAddedOk() (*[]ScanDataLinkChangeResponse, bool)`

GetAddedOk returns a tuple with the Added field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdded

`func (o *ScanDataLinkChangesResponse) SetAdded(v []ScanDataLinkChangeResponse)`

SetAdded sets Added field to given value.


### GetRemoved

`func (o *ScanDataLinkChangesResponse) GetRemoved() []ScanDataLinkChangeResponse`

GetRemoved returns the Removed field if non-nil, zero value otherwise.

### GetRemovedOk

`func (o *ScanDataLinkChangesResponse) GetRemovedOk() (*[]ScanDataLinkChangeResponse, bool)`

GetRemovedOk returns a tuple with the Removed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoved

`func (o *ScanDataLinkChangesResponse) SetRemoved(v []ScanDataLinkChangeResponse)`

SetRemoved sets Removed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


