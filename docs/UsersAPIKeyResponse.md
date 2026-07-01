# UsersAPIKeyResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | API Key ID | 
**Description** | **string** | API Key description | 
**Created** | **time.Time** | Timestamp at which the API key was created | 
**Expires** | Pointer to **time.Time** | Timestamp at which the API key expires | [optional] 
**LastUsed** | Pointer to **time.Time** | Timestamp at which the API key was used most recently | [optional] 
**UsageCount** | **int32** | Number of times the API key has been used | 

## Methods

### NewUsersAPIKeyResponse

`func NewUsersAPIKeyResponse(id string, description string, created time.Time, usageCount int32, ) *UsersAPIKeyResponse`

NewUsersAPIKeyResponse instantiates a new UsersAPIKeyResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsersAPIKeyResponseWithDefaults

`func NewUsersAPIKeyResponseWithDefaults() *UsersAPIKeyResponse`

NewUsersAPIKeyResponseWithDefaults instantiates a new UsersAPIKeyResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *UsersAPIKeyResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *UsersAPIKeyResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *UsersAPIKeyResponse) SetId(v string)`

SetId sets Id field to given value.


### GetDescription

`func (o *UsersAPIKeyResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UsersAPIKeyResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UsersAPIKeyResponse) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetCreated

`func (o *UsersAPIKeyResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *UsersAPIKeyResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *UsersAPIKeyResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.


### GetExpires

`func (o *UsersAPIKeyResponse) GetExpires() time.Time`

GetExpires returns the Expires field if non-nil, zero value otherwise.

### GetExpiresOk

`func (o *UsersAPIKeyResponse) GetExpiresOk() (*time.Time, bool)`

GetExpiresOk returns a tuple with the Expires field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpires

`func (o *UsersAPIKeyResponse) SetExpires(v time.Time)`

SetExpires sets Expires field to given value.

### HasExpires

`func (o *UsersAPIKeyResponse) HasExpires() bool`

HasExpires returns a boolean if a field has been set.

### GetLastUsed

`func (o *UsersAPIKeyResponse) GetLastUsed() time.Time`

GetLastUsed returns the LastUsed field if non-nil, zero value otherwise.

### GetLastUsedOk

`func (o *UsersAPIKeyResponse) GetLastUsedOk() (*time.Time, bool)`

GetLastUsedOk returns a tuple with the LastUsed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsed

`func (o *UsersAPIKeyResponse) SetLastUsed(v time.Time)`

SetLastUsed sets LastUsed field to given value.

### HasLastUsed

`func (o *UsersAPIKeyResponse) HasLastUsed() bool`

HasLastUsed returns a boolean if a field has been set.

### GetUsageCount

`func (o *UsersAPIKeyResponse) GetUsageCount() int32`

GetUsageCount returns the UsageCount field if non-nil, zero value otherwise.

### GetUsageCountOk

`func (o *UsersAPIKeyResponse) GetUsageCountOk() (*int32, bool)`

GetUsageCountOk returns a tuple with the UsageCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsageCount

`func (o *UsersAPIKeyResponse) SetUsageCount(v int32)`

SetUsageCount sets UsageCount field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


