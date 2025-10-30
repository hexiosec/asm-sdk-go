# UsersCreateAPIKeyResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ApiKey** | **string** | API Key | 
**Description** | **string** | API Key description | 
**Lifetime** | Pointer to **string** | Validity duration | [optional] 

## Methods

### NewUsersCreateAPIKeyResponse

`func NewUsersCreateAPIKeyResponse(apiKey string, description string, ) *UsersCreateAPIKeyResponse`

NewUsersCreateAPIKeyResponse instantiates a new UsersCreateAPIKeyResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsersCreateAPIKeyResponseWithDefaults

`func NewUsersCreateAPIKeyResponseWithDefaults() *UsersCreateAPIKeyResponse`

NewUsersCreateAPIKeyResponseWithDefaults instantiates a new UsersCreateAPIKeyResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetApiKey

`func (o *UsersCreateAPIKeyResponse) GetApiKey() string`

GetApiKey returns the ApiKey field if non-nil, zero value otherwise.

### GetApiKeyOk

`func (o *UsersCreateAPIKeyResponse) GetApiKeyOk() (*string, bool)`

GetApiKeyOk returns a tuple with the ApiKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiKey

`func (o *UsersCreateAPIKeyResponse) SetApiKey(v string)`

SetApiKey sets ApiKey field to given value.


### GetDescription

`func (o *UsersCreateAPIKeyResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UsersCreateAPIKeyResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UsersCreateAPIKeyResponse) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetLifetime

`func (o *UsersCreateAPIKeyResponse) GetLifetime() string`

GetLifetime returns the Lifetime field if non-nil, zero value otherwise.

### GetLifetimeOk

`func (o *UsersCreateAPIKeyResponse) GetLifetimeOk() (*string, bool)`

GetLifetimeOk returns a tuple with the Lifetime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLifetime

`func (o *UsersCreateAPIKeyResponse) SetLifetime(v string)`

SetLifetime sets Lifetime field to given value.

### HasLifetime

`func (o *UsersCreateAPIKeyResponse) HasLifetime() bool`

HasLifetime returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


