# UserResponseScanGroupsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**OrganisationId** | **string** |  | 
**Name** | **string** |  | 
**IsDefault** | **bool** | Scan Group is the user&#39;s default | 
**Groups** | **[]string** | Groups the user is a apart of in the organisation | 
**Roles** | **[]string** | Roles the user has in the organisation | 

## Methods

### NewUserResponseScanGroupsInner

`func NewUserResponseScanGroupsInner(id string, organisationId string, name string, isDefault bool, groups []string, roles []string, ) *UserResponseScanGroupsInner`

NewUserResponseScanGroupsInner instantiates a new UserResponseScanGroupsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserResponseScanGroupsInnerWithDefaults

`func NewUserResponseScanGroupsInnerWithDefaults() *UserResponseScanGroupsInner`

NewUserResponseScanGroupsInnerWithDefaults instantiates a new UserResponseScanGroupsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *UserResponseScanGroupsInner) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *UserResponseScanGroupsInner) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *UserResponseScanGroupsInner) SetId(v string)`

SetId sets Id field to given value.


### GetOrganisationId

`func (o *UserResponseScanGroupsInner) GetOrganisationId() string`

GetOrganisationId returns the OrganisationId field if non-nil, zero value otherwise.

### GetOrganisationIdOk

`func (o *UserResponseScanGroupsInner) GetOrganisationIdOk() (*string, bool)`

GetOrganisationIdOk returns a tuple with the OrganisationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganisationId

`func (o *UserResponseScanGroupsInner) SetOrganisationId(v string)`

SetOrganisationId sets OrganisationId field to given value.


### GetName

`func (o *UserResponseScanGroupsInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UserResponseScanGroupsInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UserResponseScanGroupsInner) SetName(v string)`

SetName sets Name field to given value.


### GetIsDefault

`func (o *UserResponseScanGroupsInner) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *UserResponseScanGroupsInner) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *UserResponseScanGroupsInner) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.


### GetGroups

`func (o *UserResponseScanGroupsInner) GetGroups() []string`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *UserResponseScanGroupsInner) GetGroupsOk() (*[]string, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *UserResponseScanGroupsInner) SetGroups(v []string)`

SetGroups sets Groups field to given value.


### GetRoles

`func (o *UserResponseScanGroupsInner) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *UserResponseScanGroupsInner) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *UserResponseScanGroupsInner) SetRoles(v []string)`

SetRoles sets Roles field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


