# UpdateUserPreferencesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DefaultScanGroup** | Pointer to **string** | Default Scan Group ID (selected by default when creating a new scan) | [optional] 

## Methods

### NewUpdateUserPreferencesRequest

`func NewUpdateUserPreferencesRequest() *UpdateUserPreferencesRequest`

NewUpdateUserPreferencesRequest instantiates a new UpdateUserPreferencesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateUserPreferencesRequestWithDefaults

`func NewUpdateUserPreferencesRequestWithDefaults() *UpdateUserPreferencesRequest`

NewUpdateUserPreferencesRequestWithDefaults instantiates a new UpdateUserPreferencesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDefaultScanGroup

`func (o *UpdateUserPreferencesRequest) GetDefaultScanGroup() string`

GetDefaultScanGroup returns the DefaultScanGroup field if non-nil, zero value otherwise.

### GetDefaultScanGroupOk

`func (o *UpdateUserPreferencesRequest) GetDefaultScanGroupOk() (*string, bool)`

GetDefaultScanGroupOk returns a tuple with the DefaultScanGroup field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultScanGroup

`func (o *UpdateUserPreferencesRequest) SetDefaultScanGroup(v string)`

SetDefaultScanGroup sets DefaultScanGroup field to given value.

### HasDefaultScanGroup

`func (o *UpdateUserPreferencesRequest) HasDefaultScanGroup() bool`

HasDefaultScanGroup returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


