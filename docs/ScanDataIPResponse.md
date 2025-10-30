# ScanDataIPResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | IP ID | 
**Ip** | **string** | IP Address | 
**DnsSources** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | DNS sources | 
**DnsPtrs** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | DNS pointers | 
**Services** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Services | 
**Certificates** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Certificates | 
**CloudRegions** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Cloud regions | 
**Asns** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | ASNs | 
**Entities** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Entities | 
**RiskCounts** | [**ScanDataRiskCountsResponse**](ScanDataRiskCountsResponse.md) |  | 
**Risks** | Pointer to [**[]ScanDataRiskResponse**](ScanDataRiskResponse.md) |  | [optional] 
**Limited** | **bool** | Whether the IP is limited or not | 
**Country** | Pointer to **string** | Country | [optional] 
**City** | Pointer to **string** | City | [optional] 
**Latitude** | Pointer to **float32** | Latitude | [optional] 
**Longitude** | Pointer to **float32** | Longitude | [optional] 
**Seed** | **bool** | Whether the IP is a seed or not | 
**Created** | **time.Time** | IP creation date | 
**LastSeen** | **time.Time** | IP last seen date | 

## Methods

### NewScanDataIPResponse

`func NewScanDataIPResponse(id string, ip string, dnsSources []ScanDataNodeResponse, dnsPtrs []ScanDataNodeResponse, services []ScanDataNodeResponse, certificates []ScanDataNodeResponse, cloudRegions []ScanDataNodeResponse, asns []ScanDataNodeResponse, entities []ScanDataNodeResponse, riskCounts ScanDataRiskCountsResponse, limited bool, seed bool, created time.Time, lastSeen time.Time, ) *ScanDataIPResponse`

NewScanDataIPResponse instantiates a new ScanDataIPResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataIPResponseWithDefaults

`func NewScanDataIPResponseWithDefaults() *ScanDataIPResponse`

NewScanDataIPResponseWithDefaults instantiates a new ScanDataIPResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataIPResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataIPResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataIPResponse) SetId(v string)`

SetId sets Id field to given value.


### GetIp

`func (o *ScanDataIPResponse) GetIp() string`

GetIp returns the Ip field if non-nil, zero value otherwise.

### GetIpOk

`func (o *ScanDataIPResponse) GetIpOk() (*string, bool)`

GetIpOk returns a tuple with the Ip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIp

`func (o *ScanDataIPResponse) SetIp(v string)`

SetIp sets Ip field to given value.


### GetDnsSources

`func (o *ScanDataIPResponse) GetDnsSources() []ScanDataNodeResponse`

GetDnsSources returns the DnsSources field if non-nil, zero value otherwise.

### GetDnsSourcesOk

`func (o *ScanDataIPResponse) GetDnsSourcesOk() (*[]ScanDataNodeResponse, bool)`

GetDnsSourcesOk returns a tuple with the DnsSources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDnsSources

`func (o *ScanDataIPResponse) SetDnsSources(v []ScanDataNodeResponse)`

SetDnsSources sets DnsSources field to given value.


### GetDnsPtrs

`func (o *ScanDataIPResponse) GetDnsPtrs() []ScanDataNodeResponse`

GetDnsPtrs returns the DnsPtrs field if non-nil, zero value otherwise.

### GetDnsPtrsOk

`func (o *ScanDataIPResponse) GetDnsPtrsOk() (*[]ScanDataNodeResponse, bool)`

GetDnsPtrsOk returns a tuple with the DnsPtrs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDnsPtrs

`func (o *ScanDataIPResponse) SetDnsPtrs(v []ScanDataNodeResponse)`

SetDnsPtrs sets DnsPtrs field to given value.


### GetServices

`func (o *ScanDataIPResponse) GetServices() []ScanDataNodeResponse`

GetServices returns the Services field if non-nil, zero value otherwise.

### GetServicesOk

`func (o *ScanDataIPResponse) GetServicesOk() (*[]ScanDataNodeResponse, bool)`

GetServicesOk returns a tuple with the Services field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServices

`func (o *ScanDataIPResponse) SetServices(v []ScanDataNodeResponse)`

SetServices sets Services field to given value.


### GetCertificates

`func (o *ScanDataIPResponse) GetCertificates() []ScanDataNodeResponse`

GetCertificates returns the Certificates field if non-nil, zero value otherwise.

### GetCertificatesOk

`func (o *ScanDataIPResponse) GetCertificatesOk() (*[]ScanDataNodeResponse, bool)`

GetCertificatesOk returns a tuple with the Certificates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertificates

`func (o *ScanDataIPResponse) SetCertificates(v []ScanDataNodeResponse)`

SetCertificates sets Certificates field to given value.


### GetCloudRegions

`func (o *ScanDataIPResponse) GetCloudRegions() []ScanDataNodeResponse`

GetCloudRegions returns the CloudRegions field if non-nil, zero value otherwise.

### GetCloudRegionsOk

`func (o *ScanDataIPResponse) GetCloudRegionsOk() (*[]ScanDataNodeResponse, bool)`

GetCloudRegionsOk returns a tuple with the CloudRegions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCloudRegions

`func (o *ScanDataIPResponse) SetCloudRegions(v []ScanDataNodeResponse)`

SetCloudRegions sets CloudRegions field to given value.


### GetAsns

`func (o *ScanDataIPResponse) GetAsns() []ScanDataNodeResponse`

GetAsns returns the Asns field if non-nil, zero value otherwise.

### GetAsnsOk

`func (o *ScanDataIPResponse) GetAsnsOk() (*[]ScanDataNodeResponse, bool)`

GetAsnsOk returns a tuple with the Asns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsns

`func (o *ScanDataIPResponse) SetAsns(v []ScanDataNodeResponse)`

SetAsns sets Asns field to given value.


### GetEntities

`func (o *ScanDataIPResponse) GetEntities() []ScanDataNodeResponse`

GetEntities returns the Entities field if non-nil, zero value otherwise.

### GetEntitiesOk

`func (o *ScanDataIPResponse) GetEntitiesOk() (*[]ScanDataNodeResponse, bool)`

GetEntitiesOk returns a tuple with the Entities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntities

`func (o *ScanDataIPResponse) SetEntities(v []ScanDataNodeResponse)`

SetEntities sets Entities field to given value.


### GetRiskCounts

`func (o *ScanDataIPResponse) GetRiskCounts() ScanDataRiskCountsResponse`

GetRiskCounts returns the RiskCounts field if non-nil, zero value otherwise.

### GetRiskCountsOk

`func (o *ScanDataIPResponse) GetRiskCountsOk() (*ScanDataRiskCountsResponse, bool)`

GetRiskCountsOk returns a tuple with the RiskCounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskCounts

`func (o *ScanDataIPResponse) SetRiskCounts(v ScanDataRiskCountsResponse)`

SetRiskCounts sets RiskCounts field to given value.


### GetRisks

`func (o *ScanDataIPResponse) GetRisks() []ScanDataRiskResponse`

GetRisks returns the Risks field if non-nil, zero value otherwise.

### GetRisksOk

`func (o *ScanDataIPResponse) GetRisksOk() (*[]ScanDataRiskResponse, bool)`

GetRisksOk returns a tuple with the Risks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRisks

`func (o *ScanDataIPResponse) SetRisks(v []ScanDataRiskResponse)`

SetRisks sets Risks field to given value.

### HasRisks

`func (o *ScanDataIPResponse) HasRisks() bool`

HasRisks returns a boolean if a field has been set.

### GetLimited

`func (o *ScanDataIPResponse) GetLimited() bool`

GetLimited returns the Limited field if non-nil, zero value otherwise.

### GetLimitedOk

`func (o *ScanDataIPResponse) GetLimitedOk() (*bool, bool)`

GetLimitedOk returns a tuple with the Limited field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimited

`func (o *ScanDataIPResponse) SetLimited(v bool)`

SetLimited sets Limited field to given value.


### GetCountry

`func (o *ScanDataIPResponse) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ScanDataIPResponse) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ScanDataIPResponse) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ScanDataIPResponse) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCity

`func (o *ScanDataIPResponse) GetCity() string`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *ScanDataIPResponse) GetCityOk() (*string, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *ScanDataIPResponse) SetCity(v string)`

SetCity sets City field to given value.

### HasCity

`func (o *ScanDataIPResponse) HasCity() bool`

HasCity returns a boolean if a field has been set.

### GetLatitude

`func (o *ScanDataIPResponse) GetLatitude() float32`

GetLatitude returns the Latitude field if non-nil, zero value otherwise.

### GetLatitudeOk

`func (o *ScanDataIPResponse) GetLatitudeOk() (*float32, bool)`

GetLatitudeOk returns a tuple with the Latitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatitude

`func (o *ScanDataIPResponse) SetLatitude(v float32)`

SetLatitude sets Latitude field to given value.

### HasLatitude

`func (o *ScanDataIPResponse) HasLatitude() bool`

HasLatitude returns a boolean if a field has been set.

### GetLongitude

`func (o *ScanDataIPResponse) GetLongitude() float32`

GetLongitude returns the Longitude field if non-nil, zero value otherwise.

### GetLongitudeOk

`func (o *ScanDataIPResponse) GetLongitudeOk() (*float32, bool)`

GetLongitudeOk returns a tuple with the Longitude field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongitude

`func (o *ScanDataIPResponse) SetLongitude(v float32)`

SetLongitude sets Longitude field to given value.

### HasLongitude

`func (o *ScanDataIPResponse) HasLongitude() bool`

HasLongitude returns a boolean if a field has been set.

### GetSeed

`func (o *ScanDataIPResponse) GetSeed() bool`

GetSeed returns the Seed field if non-nil, zero value otherwise.

### GetSeedOk

`func (o *ScanDataIPResponse) GetSeedOk() (*bool, bool)`

GetSeedOk returns a tuple with the Seed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeed

`func (o *ScanDataIPResponse) SetSeed(v bool)`

SetSeed sets Seed field to given value.


### GetCreated

`func (o *ScanDataIPResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataIPResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataIPResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataIPResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataIPResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataIPResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


