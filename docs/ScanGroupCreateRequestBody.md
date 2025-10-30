# ScanGroupCreateRequestBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Scan Group Name | 
**OrganisationId** | **string** | Organisation ID | 

## Methods

### NewScanGroupCreateRequestBody

`func NewScanGroupCreateRequestBody(name string, organisationId string, ) *ScanGroupCreateRequestBody`

NewScanGroupCreateRequestBody instantiates a new ScanGroupCreateRequestBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanGroupCreateRequestBodyWithDefaults

`func NewScanGroupCreateRequestBodyWithDefaults() *ScanGroupCreateRequestBody`

NewScanGroupCreateRequestBodyWithDefaults instantiates a new ScanGroupCreateRequestBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *ScanGroupCreateRequestBody) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ScanGroupCreateRequestBody) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ScanGroupCreateRequestBody) SetName(v string)`

SetName sets Name field to given value.


### GetOrganisationId

`func (o *ScanGroupCreateRequestBody) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *ScanGroupCreateRequestBody) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *ScanGroupCreateRequestBody) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


