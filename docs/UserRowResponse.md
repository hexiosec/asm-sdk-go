# UserRowResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Email** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**FamilyName** | Pointer to **string** |  | [optional] 
**GivenName** | Pointer to **string** |  | [optional] 
**LastIp** | Pointer to **string** |  | [optional] 
**Created** | Pointer to **time.Time** |  | [optional] 
**Updated** | Pointer to **time.Time** |  | [optional] 
**SsoSubject** | Pointer to **string** |  | [optional] 
**Attributes** | Pointer to **map[string]interface{}** |  | [optional] 
**Enabled** | Pointer to **bool** |  | [optional] 
**DefaultOrganisationId** | Pointer to **string** |  | [optional] 
**TotpEnabled** | Pointer to **bool** | User has enabled Time-based one-time passwords (TOTP) | [optional] 

## Methods

### NewUserRowResponse

`func NewUserRowResponse() *UserRowResponse`

NewUserRowResponse instantiates a new UserRowResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserRowResponseWithDefaults

`func NewUserRowResponseWithDefaults() *UserRowResponse`

NewUserRowResponseWithDefaults instantiates a new UserRowResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *UserRowResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *UserRowResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *UserRowResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *UserRowResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetEmail

`func (o *UserRowResponse) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *UserRowResponse) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *UserRowResponse) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *UserRowResponse) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetName

`func (o *UserRowResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UserRowResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UserRowResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UserRowResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetFamilyName

`func (o *UserRowResponse) GetFamilyName() string`

GetFamilyName returns the FamilyName field if non-nil, zero value otherwise.

### GetFamilyNameOk

`func (o *UserRowResponse) GetFamilyNameOk() (*string, bool)`

GetFamilyNameOk returns a tuple with the FamilyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFamilyName

`func (o *UserRowResponse) SetFamilyName(v string)`

SetFamilyName sets FamilyName field to given value.

### HasFamilyName

`func (o *UserRowResponse) HasFamilyName() bool`

HasFamilyName returns a boolean if a field has been set.

### GetGivenName

`func (o *UserRowResponse) GetGivenName() string`

GetGivenName returns the GivenName field if non-nil, zero value otherwise.

### GetGivenNameOk

`func (o *UserRowResponse) GetGivenNameOk() (*string, bool)`

GetGivenNameOk returns a tuple with the GivenName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGivenName

`func (o *UserRowResponse) SetGivenName(v string)`

SetGivenName sets GivenName field to given value.

### HasGivenName

`func (o *UserRowResponse) HasGivenName() bool`

HasGivenName returns a boolean if a field has been set.

### GetLastIp

`func (o *UserRowResponse) GetLastIp() string`

GetLastIp returns the LastIp field if non-nil, zero value otherwise.

### GetLastIpOk

`func (o *UserRowResponse) GetLastIpOk() (*string, bool)`

GetLastIpOk returns a tuple with the LastIp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastIp

`func (o *UserRowResponse) SetLastIp(v string)`

SetLastIp sets LastIp field to given value.

### HasLastIp

`func (o *UserRowResponse) HasLastIp() bool`

HasLastIp returns a boolean if a field has been set.

### GetCreated

`func (o *UserRowResponse) GetCreated() time.Time`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *UserRowResponse) GetCreatedOk() (*time.Time, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *UserRowResponse) SetCreated(v time.Time)`

SetCreated sets Created field to given value.

### HasCreated

`func (o *UserRowResponse) HasCreated() bool`

HasCreated returns a boolean if a field has been set.

### GetUpdated

`func (o *UserRowResponse) GetUpdated() time.Time`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *UserRowResponse) GetUpdatedOk() (*time.Time, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *UserRowResponse) SetUpdated(v time.Time)`

SetUpdated sets Updated field to given value.

### HasUpdated

`func (o *UserRowResponse) HasUpdated() bool`

HasUpdated returns a boolean if a field has been set.

### GetSsoSubject

`func (o *UserRowResponse) GetSsoSubject() string`

GetSsoSubject returns the SsoSubject field if non-nil, zero value otherwise.

### GetSsoSubjectOk

`func (o *UserRowResponse) GetSsoSubjectOk() (*string, bool)`

GetSsoSubjectOk returns a tuple with the SsoSubject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSsoSubject

`func (o *UserRowResponse) SetSsoSubject(v string)`

SetSsoSubject sets SsoSubject field to given value.

### HasSsoSubject

`func (o *UserRowResponse) HasSsoSubject() bool`

HasSsoSubject returns a boolean if a field has been set.

### GetAttributes

`func (o *UserRowResponse) GetAttributes() map[string]interface{}`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *UserRowResponse) GetAttributesOk() (*map[string]interface{}, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *UserRowResponse) SetAttributes(v map[string]interface{})`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *UserRowResponse) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetEnabled

`func (o *UserRowResponse) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *UserRowResponse) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *UserRowResponse) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *UserRowResponse) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetDefaultOrganisationId

`func (o *UserRowResponse) GetDefaultOrganisationId() string`

GetDefaultOrganisationId returns the DefaultOrganisationId field if non-nil, zero value otherwise.

### GetDefaultOrganisationIdOk

`func (o *UserRowResponse) GetDefaultOrganisationIdOk() (*string, bool)`

GetDefaultOrganisationIdOk returns a tuple with the DefaultOrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultOrganisationId

`func (o *UserRowResponse) SetDefaultOrganisationId(v string)`

SetDefaultOrganisationId sets DefaultOrganisationId field to given value.

### HasDefaultOrganisationId

`func (o *UserRowResponse) HasDefaultOrganisationId() bool`

HasDefaultOrganisationId returns a boolean if a field has been set.

### GetTotpEnabled

`func (o *UserRowResponse) GetTotpEnabled() bool`

GetTotpEnabled returns the TotpEnabled field if non-nil, zero value otherwise.

### GetTotpEnabledOk

`func (o *UserRowResponse) GetTotpEnabledOk() (*bool, bool)`

GetTotpEnabledOk returns a tuple with the TotpEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotpEnabled

`func (o *UserRowResponse) SetTotpEnabled(v bool)`

SetTotpEnabled sets TotpEnabled field to given value.

### HasTotpEnabled

`func (o *UserRowResponse) HasTotpEnabled() bool`

HasTotpEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


