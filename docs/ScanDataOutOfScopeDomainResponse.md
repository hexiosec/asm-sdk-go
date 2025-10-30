# ScanDataOutOfScopeDomainResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Domain ID | 
**Name** | **string** | Domain name | 
**Created** | **time.Time** | Domain creation date | 
**LastSeen** | **time.Time** | Domain last seen date | 

## Methods

### NewScanDataOutOfScopeDomainResponse

`func NewScanDataOutOfScopeDomainResponse(id string, name string, created time.Time, lastSeen time.Time, ) *ScanDataOutOfScopeDomainResponse`

NewScanDataOutOfScopeDomainResponse instantiates a new ScanDataOutOfScopeDomainResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanDataOutOfScopeDomainResponseWithDefaults

`func NewScanDataOutOfScopeDomainResponseWithDefaults() *ScanDataOutOfScopeDomainResponse`

NewScanDataOutOfScopeDomainResponseWithDefaults instantiates a new ScanDataOutOfScopeDomainResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ScanDataOutOfScopeDomainResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ScanDataOutOfScopeDomainResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ScanDataOutOfScopeDomainResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ScanDataOutOfScopeDomainResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanDataOutOfScopeDomainResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanDataOutOfScopeDomainResponse) SetName(v string)`

SetName sets Name field to given value.


### GetCreated

`func (o *ScanDataOutOfScopeDomainResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ScanDataOutOfScopeDomainResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ScanDataOutOfScopeDomainResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetLastSeen

`func (o *ScanDataOutOfScopeDomainResponse) GetLastSeen() time.Time`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *ScanDataOutOfScopeDomainResponse) GetLastSeenOk() (*time.Time, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *ScanDataOutOfScopeDomainResponse) SetLastSeen(v time.Time)`

SetLastSeen sets LastSeen field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


