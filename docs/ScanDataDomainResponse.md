# ScanDataDomainResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Domain ID | 
**Name** | **string** | Domain name | 
**DnsDestinations** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | [DEPRECATED] use &#x60;ips&#x60; and &#x60;alias&#x60; instead, they contain the same data. | 
**Alias** | Pointer to [**ScanDataNodeResponse**](ScanDataNodeResponse.md) | CNAME Domain | [optional] 
**Ips** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | IPs | 
**Services** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Services | 
**Certificates** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Certificates | 
**CloudRegions** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Cloud regions | 
**Asns** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | ASNs | 
**Entities** | [**[]ScanDataNodeResponse**](ScanDataNodeResponse.md) | Entities | 
**RiskCounts** | [**ScanDataRiskCountsResponse**](ScanDataRiskCountsResponse.md) |  | 
**Risks** | Pointer to [**[]ScanDataRiskResponse**](ScanDataRiskResponse.md) |  | [optional] 
**Limited** | **bool** | Whether the domain is limited or not | 
**Stale** | **bool** | Whether the domain is stale or not | 
**NameServer** | **bool** | Whether the domain is a name server or not | 
**Seed** | **bool** | Whether the domain is a seed or not | 
**Created** | **time.Time** | Domain creation date | 
**LastSeen** | **time.Time** | Domain last seen date | 

## Methods

### NewScanDataDomainResponse

`func NewScanDataDomainResponse(id string, name string, dnsDestinations []ScanDataNodeResponse, ips []ScanDataNodeResponse, services []ScanDataNodeResponse, certificates []ScanDataNodeResponse, cloudRegions []ScanDataNodeResponse, asns []ScanDataNodeResponse, entities []ScanDataNodeResponse, riskCounts ScanDataRiskCountsResponse, limited bool, stale bool, nameServer bool, seed bool, created time.Time, lastSeen time.Time, ) *ScanDataDomainResponse`

NewScanDataDomainResponse instantiates a new ScanDataDomainResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataDomainResponseWithDefaults

`func NewScanDataDomainResponseWithDefaults() *ScanDataDomainResponse`

NewScanDataDomainResponseWithDefaults instantiates a new ScanDataDomainResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataDomainResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataDomainResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataDomainResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ScanDataDomainResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanDataDomainResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanDataDomainResponse) SetName(v string)`

SetName sets Name field to given value.


### GetDnsDestinations

`func (o *ScanDataDomainResponse) GetDnsDestinations() []ScanDataNodeResponse`

GetDnsDestinations returns the DnsDestinations field if non-nil, zero value otherwise.

### GetDnsDestinationsOk

`func (o *ScanDataDomainResponse) GetDnsDestinationsOk() (*[]ScanDataNodeResponse, bool)`

GetDnsDestinationsOk returns a tuple with the DnsDestinations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDnsDestinations

`func (o *ScanDataDomainResponse) SetDnsDestinations(v []ScanDataNodeResponse)`

SetDnsDestinations sets DnsDestinations field to given value.


### GetAlias

`func (o *ScanDataDomainResponse) GetAlias() ScanDataNodeResponse`

GetAlias returns the Alias field if non-nil, zero value otherwise.

### GetAliasOk

`func (o *ScanDataDomainResponse) GetAliasOk() (*ScanDataNodeResponse, bool)`

GetAliasOk returns a tuple with the Alias field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlias

`func (o *ScanDataDomainResponse) SetAlias(v ScanDataNodeResponse)`

SetAlias sets Alias field to given value.

### HasAlias

`func (o *ScanDataDomainResponse) HasAlias() bool`

HasAlias returns a boolean if a field has been set.

### GetIps

`func (o *ScanDataDomainResponse) GetIps() []ScanDataNodeResponse`

GetIps returns the Ips field if non-nil, zero value otherwise.

### GetIpsOk

`func (o *ScanDataDomainResponse) GetIpsOk() (*[]ScanDataNodeResponse, bool)`

GetIpsOk returns a tuple with the Ips field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIps

`func (o *ScanDataDomainResponse) SetIps(v []ScanDataNodeResponse)`

SetIps sets Ips field to given value.


### GetServices

`func (o *ScanDataDomainResponse) GetServices() []ScanDataNodeResponse`

GetServices returns the Services field if non-nil, zero value otherwise.

### GetServicesOk

`func (o *ScanDataDomainResponse) GetServicesOk() (*[]ScanDataNodeResponse, bool)`

GetServicesOk returns a tuple with the Services field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServices

`func (o *ScanDataDomainResponse) SetServices(v []ScanDataNodeResponse)`

SetServices sets Services field to given value.


### GetCertificates

`func (o *ScanDataDomainResponse) GetCertificates() []ScanDataNodeResponse`

GetCertificates returns the Certificates field if non-nil, zero value otherwise.

### GetCertificatesOk

`func (o *ScanDataDomainResponse) GetCertificatesOk() (*[]ScanDataNodeResponse, bool)`

GetCertificatesOk returns a tuple with the Certificates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertificates

`func (o *ScanDataDomainResponse) SetCertificates(v []ScanDataNodeResponse)`

SetCertificates sets Certificates field to given value.


### GetCloudRegions

`func (o *ScanDataDomainResponse) GetCloudRegions() []ScanDataNodeResponse`

GetCloudRegions returns the CloudRegions field if non-nil, zero value otherwise.

### GetCloudRegionsOk

`func (o *ScanDataDomainResponse) GetCloudRegionsOk() (*[]ScanDataNodeResponse, bool)`

GetCloudRegionsOk returns a tuple with the CloudRegions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCloudRegions

`func (o *ScanDataDomainResponse) SetCloudRegions(v []ScanDataNodeResponse)`

SetCloudRegions sets CloudRegions field to given value.


### GetAsns

`func (o *ScanDataDomainResponse) GetAsns() []ScanDataNodeResponse`

GetAsns returns the Asns field if non-nil, zero value otherwise.

### GetAsnsOk

`func (o *ScanDataDomainResponse) GetAsnsOk() (*[]ScanDataNodeResponse, bool)`

GetAsnsOk returns a tuple with the Asns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsns

`func (o *ScanDataDomainResponse) SetAsns(v []ScanDataNodeResponse)`

SetAsns sets Asns field to given value.


### GetEntities

`func (o *ScanDataDomainResponse) GetEntities() []ScanDataNodeResponse`

GetEntities returns the Entities field if non-nil, zero value otherwise.

### GetEntitiesOk

`func (o *ScanDataDomainResponse) GetEntitiesOk() (*[]ScanDataNodeResponse, bool)`

GetEntitiesOk returns a tuple with the Entities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntities

`func (o *ScanDataDomainResponse) SetEntities(v []ScanDataNodeResponse)`

SetEntities sets Entities field to given value.


### GetRiskCounts

`func (o *ScanDataDomainResponse) GetRiskCounts() ScanDataRiskCountsResponse`

GetRiskCounts returns the RiskCounts field if non-nil, zero value otherwise.

### GetRiskCountsOk

`func (o *ScanDataDomainResponse) GetRiskCountsOk() (*ScanDataRiskCountsResponse, bool)`

GetRiskCountsOk returns a tuple with the RiskCounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskCounts

`func (o *ScanDataDomainResponse) SetRiskCounts(v ScanDataRiskCountsResponse)`

SetRiskCounts sets RiskCounts field to given value.


### GetRisks

`func (o *ScanDataDomainResponse) GetRisks() []ScanDataRiskResponse`

GetRisks returns the Risks field if non-nil, zero value otherwise.

### GetRisksOk

`func (o *ScanDataDomainResponse) GetRisksOk() (*[]ScanDataRiskResponse, bool)`

GetRisksOk returns a tuple with the Risks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRisks

`func (o *ScanDataDomainResponse) SetRisks(v []ScanDataRiskResponse)`

SetRisks sets Risks field to given value.

### HasRisks

`func (o *ScanDataDomainResponse) HasRisks() bool`

HasRisks returns a boolean if a field has been set.

### GetLimited

`func (o *ScanDataDomainResponse) GetLimited() bool`

GetLimited returns the Limited field if non-nil, zero value otherwise.

### GetLimitedOk

`func (o *ScanDataDomainResponse) GetLimitedOk() (*bool, bool)`

GetLimitedOk returns a tuple with the Limited field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimited

`func (o *ScanDataDomainResponse) SetLimited(v bool)`

SetLimited sets Limited field to given value.


### GetStale

`func (o *ScanDataDomainResponse) GetStale() bool`

GetStale returns the Stale field if non-nil, zero value otherwise.

### GetStaleOk

`func (o *ScanDataDomainResponse) GetStaleOk() (*bool, bool)`

GetStaleOk returns a tuple with the Stale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStale

`func (o *ScanDataDomainResponse) SetStale(v bool)`

SetStale sets Stale field to given value.


### GetNameServer

`func (o *ScanDataDomainResponse) GetNameServer() bool`

GetNameServer returns the NameServer field if non-nil, zero value otherwise.

### GetNameServerOk

`func (o *ScanDataDomainResponse) GetNameServerOk() (*bool, bool)`

GetNameServerOk returns a tuple with the NameServer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNameServer

`func (o *ScanDataDomainResponse) SetNameServer(v bool)`

SetNameServer sets NameServer field to given value.


### GetSeed

`func (o *ScanDataDomainResponse) GetSeed() bool`

GetSeed returns the Seed field if non-nil, zero value otherwise.

### GetSeedOk

`func (o *ScanDataDomainResponse) GetSeedOk() (*bool, bool)`

GetSeedOk returns a tuple with the Seed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeed

`func (o *ScanDataDomainResponse) SetSeed(v bool)`

SetSeed sets Seed field to given value.


### GetCreated

`func (o *ScanDataDomainResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataDomainResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataDomainResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataDomainResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataDomainResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataDomainResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


