# ScanDataServiceResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Service ID | 
**Name** | **string** | Service name | 
**Host** | [**ScanDataServiceResponseHost**](ScanDataServiceResponseHost.md) |  | 
**Port** | Pointer to **int32** | Service port | [optional] 
**Protocol** | Pointer to **string** | Service protocol | [optional] 
**IanaName** | Pointer to **string** | Service IANA name | [optional] 
**IanaDescription** | Pointer to **string** | Service IANA description | [optional] 
**SocketEncrypted** | Pointer to **bool** | Whether the service used SSL | [optional] 
**SocketAuthorized** | Pointer to **bool** | Whether the SSL certificate is valid | [optional] 
**RiskCounts** | Pointer to [**ScanDataRiskCountsResponse**](ScanDataRiskCountsResponse.md) |  | [optional] 
**Risks** | Pointer to [**[]ScanDataRiskResponse**](ScanDataRiskResponse.md) |  | [optional] 
**ShodanLastUpdate** | Pointer to **time.Time** | Last time Shodan data was updated for the host IP. Has been replaced by source_last_updated | [optional] 
**SourceLastUpdated** | Pointer to **time.Time** | Last time IP data source was updated for the host IP. | [optional] 
**Created** | **time.Time** | Service creation date | 
**LastSeen** | **time.Time** | Service last seen date | 

## Methods

### NewScanDataServiceResponse

`func NewScanDataServiceResponse(id string, name string, host ScanDataServiceResponseHost, created time.Time, lastSeen time.Time, ) *ScanDataServiceResponse`

NewScanDataServiceResponse instantiates a new ScanDataServiceResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataServiceResponseWithDefaults

`func NewScanDataServiceResponseWithDefaults() *ScanDataServiceResponse`

NewScanDataServiceResponseWithDefaults instantiates a new ScanDataServiceResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataServiceResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataServiceResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataServiceResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ScanDataServiceResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanDataServiceResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanDataServiceResponse) SetName(v string)`

SetName sets Name field to given value.


### GetHost

`func (o *ScanDataServiceResponse) GetHost() ScanDataServiceResponseHost`

GetHost returns the Host field if non-nil, zero value otherwise.

### GetHostOk

`func (o *ScanDataServiceResponse) GetHostOk() (*ScanDataServiceResponseHost, bool)`

GetHostOk returns a tuple with the Host field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHost

`func (o *ScanDataServiceResponse) SetHost(v ScanDataServiceResponseHost)`

SetHost sets Host field to given value.


### GetPort

`func (o *ScanDataServiceResponse) GetPort() int32`

GetPort returns the Port field if non-nil, zero value otherwise.

### GetPortOk

`func (o *ScanDataServiceResponse) GetPortOk() (*int32, bool)`

GetPortOk returns a tuple with the Port field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPort

`func (o *ScanDataServiceResponse) SetPort(v int32)`

SetPort sets Port field to given value.

### HasPort

`func (o *ScanDataServiceResponse) HasPort() bool`

HasPort returns a boolean if a field has been set.

### GetProtocol

`func (o *ScanDataServiceResponse) GetProtocol() string`

GetProtocol returns the Protocol field if non-nil, zero value otherwise.

### GetProtocolOk

`func (o *ScanDataServiceResponse) GetProtocolOk() (*string, bool)`

GetProtocolOk returns a tuple with the Protocol field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtocol

`func (o *ScanDataServiceResponse) SetProtocol(v string)`

SetProtocol sets Protocol field to given value.

### HasProtocol

`func (o *ScanDataServiceResponse) HasProtocol() bool`

HasProtocol returns a boolean if a field has been set.

### GetIanaName

`func (o *ScanDataServiceResponse) GetIanaName() string`

GetIanaName returns the IanaName field if non-nil, zero value otherwise.

### GetIanaNameOk

`func (o *ScanDataServiceResponse) GetIanaNameOk() (*string, bool)`

GetIanaNameOk returns a tuple with the IanaName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIanaName

`func (o *ScanDataServiceResponse) SetIanaName(v string)`

SetIanaName sets IanaName field to given value.

### HasIanaName

`func (o *ScanDataServiceResponse) HasIanaName() bool`

HasIanaName returns a boolean if a field has been set.

### GetIanaDescription

`func (o *ScanDataServiceResponse) GetIanaDescription() string`

GetIanaDescription returns the IanaDescription field if non-nil, zero value otherwise.

### GetIanaDescriptionOk

`func (o *ScanDataServiceResponse) GetIanaDescriptionOk() (*string, bool)`

GetIanaDescriptionOk returns a tuple with the IanaDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIanaDescription

`func (o *ScanDataServiceResponse) SetIanaDescription(v string)`

SetIanaDescription sets IanaDescription field to given value.

### HasIanaDescription

`func (o *ScanDataServiceResponse) HasIanaDescription() bool`

HasIanaDescription returns a boolean if a field has been set.

### GetSocketEncrypted

`func (o *ScanDataServiceResponse) GetSocketEncrypted() bool`

GetSocketEncrypted returns the SocketEncrypted field if non-nil, zero value otherwise.

### GetSocketEncryptedOk

`func (o *ScanDataServiceResponse) GetSocketEncryptedOk() (*bool, bool)`

GetSocketEncryptedOk returns a tuple with the SocketEncrypted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSocketEncrypted

`func (o *ScanDataServiceResponse) SetSocketEncrypted(v bool)`

SetSocketEncrypted sets SocketEncrypted field to given value.

### HasSocketEncrypted

`func (o *ScanDataServiceResponse) HasSocketEncrypted() bool`

HasSocketEncrypted returns a boolean if a field has been set.

### GetSocketAuthorized

`func (o *ScanDataServiceResponse) GetSocketAuthorized() bool`

GetSocketAuthorized returns the SocketAuthorized field if non-nil, zero value otherwise.

### GetSocketAuthorizedOk

`func (o *ScanDataServiceResponse) GetSocketAuthorizedOk() (*bool, bool)`

GetSocketAuthorizedOk returns a tuple with the SocketAuthorized field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSocketAuthorized

`func (o *ScanDataServiceResponse) SetSocketAuthorized(v bool)`

SetSocketAuthorized sets SocketAuthorized field to given value.

### HasSocketAuthorized

`func (o *ScanDataServiceResponse) HasSocketAuthorized() bool`

HasSocketAuthorized returns a boolean if a field has been set.

### GetRiskCounts

`func (o *ScanDataServiceResponse) GetRiskCounts() ScanDataRiskCountsResponse`

GetRiskCounts returns the RiskCounts field if non-nil, zero value otherwise.

### GetRiskCountsOk

`func (o *ScanDataServiceResponse) GetRiskCountsOk() (*ScanDataRiskCountsResponse, bool)`

GetRiskCountsOk returns a tuple with the RiskCounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskCounts

`func (o *ScanDataServiceResponse) SetRiskCounts(v ScanDataRiskCountsResponse)`

SetRiskCounts sets RiskCounts field to given value.

### HasRiskCounts

`func (o *ScanDataServiceResponse) HasRiskCounts() bool`

HasRiskCounts returns a boolean if a field has been set.

### GetRisks

`func (o *ScanDataServiceResponse) GetRisks() []ScanDataRiskResponse`

GetRisks returns the Risks field if non-nil, zero value otherwise.

### GetRisksOk

`func (o *ScanDataServiceResponse) GetRisksOk() (*[]ScanDataRiskResponse, bool)`

GetRisksOk returns a tuple with the Risks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRisks

`func (o *ScanDataServiceResponse) SetRisks(v []ScanDataRiskResponse)`

SetRisks sets Risks field to given value.

### HasRisks

`func (o *ScanDataServiceResponse) HasRisks() bool`

HasRisks returns a boolean if a field has been set.

### GetShodanLastUpdate

`func (o *ScanDataServiceResponse) GetShodanLastUpdate() time.Time`

GetShodanLastUpdate returns the ShodanLastUpdate field if non-nil, zero value otherwise.

### GetShodanLastUpdateOk

`func (o *ScanDataServiceResponse) GetShodanLastUpdateOk() (*time.Time, bool)`

GetShodanLastUpdateOk returns a tuple with the ShodanLastUpdate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShodanLastUpdate

`func (o *ScanDataServiceResponse) SetShodanLastUpdate(v time.Time)`

SetShodanLastUpdate sets ShodanLastUpdate field to given value.

### HasShodanLastUpdate

`func (o *ScanDataServiceResponse) HasShodanLastUpdate() bool`

HasShodanLastUpdate returns a boolean if a field has been set.

### GetSourceLastUpdated

`func (o *ScanDataServiceResponse) GetSourceLastUpdated() time.Time`

GetSourceLastUpdated returns the SourceLastUpdated field if non-nil, zero value otherwise.

### GetSourceLastUpdatedOk

`func (o *ScanDataServiceResponse) GetSourceLastUpdatedOk() (*time.Time, bool)`

GetSourceLastUpdatedOk returns a tuple with the SourceLastUpdated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceLastUpdated

`func (o *ScanDataServiceResponse) SetSourceLastUpdated(v time.Time)`

SetSourceLastUpdated sets SourceLastUpdated field to given value.

### HasSourceLastUpdated

`func (o *ScanDataServiceResponse) HasSourceLastUpdated() bool`

HasSourceLastUpdated returns a boolean if a field has been set.

### GetCreated

`func (o *ScanDataServiceResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataServiceResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataServiceResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataServiceResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataServiceResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataServiceResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


