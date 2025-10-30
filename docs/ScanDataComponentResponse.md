# ScanDataComponentResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Component ID | 
**Name** | **string** | Component name | 
**Urn** | **string** | Component URN | 
**Cpe23** | Pointer to **string** | Component CPE23 | [optional] 
**Vendor** | Pointer to **string** | Component vendor | [optional] 
**Version** | Pointer to **string** | Component version | [optional] 
**Services** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Services | 
**RiskCounts** | Pointer to [**ScanDataRiskCountsResponse**](ScanDataRiskCountsResponse.md) |  | [optional] 
**Risks** | Pointer to [**[]ScanDataRiskResponse**](ScanDataRiskResponse.md) |  | [optional] 
**Created** | **time.Time** | Component creation date | 
**LastSeen** | **time.Time** | Component last seen date | 

## Methods

### NewScanDataComponentResponse

`func NewScanDataComponentResponse(id string, name string, urn string, services []ScanDataNodeResponse, created time.Time, lastSeen time.Time, ) *ScanDataComponentResponse`

NewScanDataComponentResponse instantiates a new ScanDataComponentResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataComponentResponseWithDefaults

`func NewScanDataComponentResponseWithDefaults() *ScanDataComponentResponse`

NewScanDataComponentResponseWithDefaults instantiates a new ScanDataComponentResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataComponentResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataComponentResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataComponentResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ScanDataComponentResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanDataComponentResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanDataComponentResponse) SetName(v string)`

SetName sets Name field to given value.


### GetUrn

`func (o *ScanDataComponentResponse) GetUrn() string`

GetUrn returns the Urn field if non-nil, zero value otherwise.

### GetUrnOk

`func (o *ScanDataComponentResponse) GetUrnOk() (*string, bool)`

GetUrnOk returns a tuple with the Urn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrn

`func (o *ScanDataComponentResponse) SetUrn(v string)`

SetUrn sets Urn field to given value.


### GetCpe23

`func (o *ScanDataComponentResponse) GetCpe23() string`

GetCpe23 returns the Cpe23 field if non-nil, zero value otherwise.

### GetCpe23Ok

`func (o *ScanDataComponentResponse) GetCpe23Ok() (*string, bool)`

GetCpe23Ok returns a tuple with the Cpe23 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCpe23

`func (o *ScanDataComponentResponse) SetCpe23(v string)`

SetCpe23 sets Cpe23 field to given value.

### HasCpe23

`func (o *ScanDataComponentResponse) HasCpe23() bool`

HasCpe23 returns a boolean if a field has been set.

### GetVendor

`func (o *ScanDataComponentResponse) GetVendor() string`

GetVendor returns the Vendor field if non-nil, zero value otherwise.

### GetVendorOk

`func (o *ScanDataComponentResponse) GetVendorOk() (*string, bool)`

GetVendorOk returns a tuple with the Vendor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVendor

`func (o *ScanDataComponentResponse) SetVendor(v string)`

SetVendor sets Vendor field to given value.

### HasVendor

`func (o *ScanDataComponentResponse) HasVendor() bool`

HasVendor returns a boolean if a field has been set.

### GetVersion

`func (o *ScanDataComponentResponse) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ScanDataComponentResponse) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ScanDataComponentResponse) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *ScanDataComponentResponse) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### GetServices

`func (o *ScanDataComponentResponse) GetServices() []ScanDataNodeResponse`

GetServices returns the Services field if non-nil, zero value otherwise.

### GetServicesOk

`func (o *ScanDataComponentResponse) GetServicesOk() (*[]ScanDataNodeResponse, bool)`

GetServicesOk returns a tuple with the Services field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServices

`func (o *ScanDataComponentResponse) SetServices(v []ScanDataNodeResponse)`

SetServices sets Services field to given value.


### GetRiskCounts

`func (o *ScanDataComponentResponse) GetRiskCounts() ScanDataRiskCountsResponse`

GetRiskCounts returns the RiskCounts field if non-nil, zero value otherwise.

### GetRiskCountsOk

`func (o *ScanDataComponentResponse) GetRiskCountsOk() (*ScanDataRiskCountsResponse, bool)`

GetRiskCountsOk returns a tuple with the RiskCounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskCounts

`func (o *ScanDataComponentResponse) SetRiskCounts(v ScanDataRiskCountsResponse)`

SetRiskCounts sets RiskCounts field to given value.

### HasRiskCounts

`func (o *ScanDataComponentResponse) HasRiskCounts() bool`

HasRiskCounts returns a boolean if a field has been set.

### GetRisks

`func (o *ScanDataComponentResponse) GetRisks() []ScanDataRiskResponse`

GetRisks returns the Risks field if non-nil, zero value otherwise.

### GetRisksOk

`func (o *ScanDataComponentResponse) GetRisksOk() (*[]ScanDataRiskResponse, bool)`

GetRisksOk returns a tuple with the Risks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRisks

`func (o *ScanDataComponentResponse) SetRisks(v []ScanDataRiskResponse)`

SetRisks sets Risks field to given value.

### HasRisks

`func (o *ScanDataComponentResponse) HasRisks() bool`

HasRisks returns a boolean if a field has been set.

### GetCreated

`func (o *ScanDataComponentResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataComponentResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataComponentResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataComponentResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataComponentResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataComponentResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


