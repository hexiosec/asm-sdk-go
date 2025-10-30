# AuthResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Authenticated** | **bool** | True if the chosen authentication scheme has passed. | 
**Scheme** | Pointer to **string** | Name of the authentication scheme used. | [optional] 
**Groups** | Pointer to **[]string** | List of groups for which the current user is a member. | [optional] 
**Roles** | Pointer to **[]string** | List of roles granted to the current user | [optional] 
**Csrf** | Pointer to **string** | CSRF token to use with POST/PUT/PATCH/DELETE requests which use session authentication. | [optional] 
**Attributes** | Pointer to **map[string]interface{}** | Combined attributes for the current user. | [optional] 
**User** | Pointer to [**UserRowResponse**](UserRowResponse.md) |  | [optional] 

## Methods

### NewAuthResponse

`func NewAuthResponse(authenticated bool, ) *AuthResponse`

NewAuthResponse instantiates a new AuthResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthResponseWithDefaults

`func NewAuthResponseWithDefaults() *AuthResponse`

NewAuthResponseWithDefaults instantiates a new AuthResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAuthenticated

`func (o *AuthResponse) GetAuthenticated() bool`

GetAuthenticated returns the Authenticated field if non-nil, zero value otherwise.

### GetAuthenticatedOk

`func (o *AuthResponse) GetAuthenticatedOk() (*bool, bool)`

GetAuthenticatedOk returns a tuple with the Authenticated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthenticated

`func (o *AuthResponse) SetAuthenticated(v bool)`

SetAuthenticated sets Authenticated field to given value.


### GetScheme

`func (o *AuthResponse) GetScheme() string`

GetScheme returns the Scheme field if non-nil, zero value otherwise.

### GetSchemeOk

`func (o *AuthResponse) GetSchemeOk() (*string, bool)`

GetSchemeOk returns a tuple with the Scheme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheme

`func (o *AuthResponse) SetScheme(v string)`

SetScheme sets Scheme field to given value.

### HasScheme

`func (o *AuthResponse) HasScheme() bool`

HasScheme returns a boolean if a field has been set.

### GetGroups

`func (o *AuthResponse) GetGroups() []string`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *AuthResponse) GetGroupsOk() (*[]string, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *AuthResponse) SetGroups(v []string)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *AuthResponse) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### GetRoles

`func (o *AuthResponse) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *AuthResponse) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *AuthResponse) SetRoles(v []string)`

SetRoles sets Roles field to given value.

### HasRoles

`func (o *AuthResponse) HasRoles() bool`

HasRoles returns a boolean if a field has been set.

### GetCsrf

`func (o *AuthResponse) GetCsrf() string`

GetCsrf returns the Csrf field if non-nil, zero value otherwise.

### GetCsrfOk

`func (o *AuthResponse) GetCsrfOk() (*string, bool)`

GetCsrfOk returns a tuple with the Csrf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCsrf

`func (o *AuthResponse) SetCsrf(v string)`

SetCsrf sets Csrf field to given value.

### HasCsrf

`func (o *AuthResponse) HasCsrf() bool`

HasCsrf returns a boolean if a field has been set.

### GetAttributes

`func (o *AuthResponse) GetAttributes() map[string]interface{}`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *AuthResponse) GetAttributesOk() (*map[string]interface{}, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *AuthResponse) SetAttributes(v map[string]interface{})`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *AuthResponse) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetUser

`func (o *AuthResponse) GetUser() UserRowResponse`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *AuthResponse) GetUserOk() (*UserRowResponse, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *AuthResponse) SetUser(v UserRowResponse)`

SetUser sets User field to given value.

### HasUser

`func (o *AuthResponse) HasUser() bool`

HasUser returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


