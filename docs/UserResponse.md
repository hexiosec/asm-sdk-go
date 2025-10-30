# UserResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Email** | **string** |  | 
**Enabled** | **bool** |  | 
**LastSessionUpdated** | Pointer to **time.Time** | Most recent session activity of user | [optional] 
**TotpEnabled** | **bool** | User has enabled Time-based one-time passwords (TOTP) | 
**SsoUser** | Pointer to **bool** | User is an SSO user | [optional] 
**Groups** | **[]string** | Groups the user is a apart of in the organisation / scan group | 
**Roles** | **[]string** | Roles the user has in the organisation / scan group | 
**ScanGroups** | Pointer to [**[]UserResponseScanGroupsInner**](UserResponseScanGroupsInner.md) | Scan Groups the user is apart of in the organisation (if the organisation is requested) | [optional] 

## Methods

### NewUserResponse

`func NewUserResponse(id string, name string, email string, enabled bool, totpEnabled bool, groups []string, roles []string, ) *UserResponse`

NewUserResponse instantiates a new UserResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserResponseWithDefaults

`func NewUserResponseWithDefaults() *UserResponse`

NewUserResponseWithDefaults instantiates a new UserResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *UserResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *UserResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *UserResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *UserResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UserResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UserResponse) SetName(v string)`

SetName sets Name field to given value.


### GetEmail

`func (o *UserResponse) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *UserResponse) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *UserResponse) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetEnabled

`func (o *UserResponse) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *UserResponse) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *UserResponse) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetLastSessionUpdated

`func (o *UserResponse) GetLastSessionUpdated() time.Time`

GetLastSessionUpdated returns the LastSessionUpdated field if non-nil, zero value otherwise.

### GetLastSessionUpdatedOk

`func (o *UserResponse) GetLastSessionUpdatedOk() (*time.Time, bool)`

GetLastSessionUpdatedOk returns a tuple with the LastSessionUpdated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSessionUpdated

`func (o *UserResponse) SetLastSessionUpdated(v time.Time)`

SetLastSessionUpdated sets LastSessionUpdated field to given value.

### HasLastSessionUpdated

`func (o *UserResponse) HasLastSessionUpdated() bool`

HasLastSessionUpdated returns a boolean if a field has been set.

### GetTotpEnabled

`func (o *UserResponse) GetTotpEnabled() bool`

GetTotpEnabled returns the TotpEnabled field if non-nil, zero value otherwise.

### GetTotpEnabledOk

`func (o *UserResponse) GetTotpEnabledOk() (*bool, bool)`

GetTotpEnabledOk returns a tuple with the TotpEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotpEnabled

`func (o *UserResponse) SetTotpEnabled(v bool)`

SetTotpEnabled sets TotpEnabled field to given value.


### GetSsoUser

`func (o *UserResponse) GetSsoUser() bool`

GetSsoUser returns the SsoUser field if non-nil, zero value otherwise.

### GetSsoUserOk

`func (o *UserResponse) GetSsoUserOk() (*bool, bool)`

GetSsoUserOk returns a tuple with the SsoUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSsoUser

`func (o *UserResponse) SetSsoUser(v bool)`

SetSsoUser sets SsoUser field to given value.

### HasSsoUser

`func (o *UserResponse) HasSsoUser() bool`

HasSsoUser returns a boolean if a field has been set.

### GetGroups

`func (o *UserResponse) GetGroups() []string`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *UserResponse) GetGroupsOk() (*[]string, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *UserResponse) SetGroups(v []string)`

SetGroups sets Groups field to given value.


### GetRoles

`func (o *UserResponse) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *UserResponse) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *UserResponse) SetRoles(v []string)`

SetRoles sets Roles field to given value.


### GetScanGroups

`func (o *UserResponse) GetScanGroups() []UserResponseScanGroupsInner`

GetScanGroups returns the ScanGroups field if non-nil, zero value otherwise.

### GetScanGroupsOk

`func (o *UserResponse) GetScanGroupsOk() (*[]UserResponseScanGroupsInner, bool)`

GetScanGroupsOk returns a tuple with the ScanGroups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanGroups

`func (o *UserResponse) SetScanGroups(v []UserResponseScanGroupsInner)`

SetScanGroups sets ScanGroups field to given value.

### HasScanGroups

`func (o *UserResponse) HasScanGroups() bool`

HasScanGroups returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


